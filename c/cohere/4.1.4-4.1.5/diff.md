# Comparing `tmp/cohere-4.1.4.tar.gz` & `tmp/cohere-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.1.4.tar", max compression
+gzip compressed data, was "cohere-4.1.5.tar", max compression
```

## Comparing `cohere-4.1.4.tar` & `cohere-4.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-04-06 00:30:29.520457 cohere-4.1.4/LICENSE
--rw-r--r--   0        0        0     4271 2023-04-06 00:30:29.520457 cohere-4.1.4/README.md
--rw-r--r--   0        0        0      638 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/__init__.py
--rw-r--r--   0        0        0    29257 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/client.py
--rw-r--r--   0        0        0    21762 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/error.py
--rw-r--r--   0        0        0      529 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/logging.py
--rw-r--r--   0        0        0      721 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/responses/base.py
--rw-r--r--   0        0        0     3142 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/responses/classify.py
--rw-r--r--   0        0        0     4711 2023-04-06 00:30:29.520457 cohere-4.1.4/cohere/responses/cluster.py
--rw-r--r--   0        0        0      552 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      442 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      771 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     1453 2023-04-06 00:30:29.524457 cohere-4.1.4/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-04-06 00:30:29.524457 cohere-4.1.4/pyproject.toml
--rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 cohere-4.1.4/setup.py
--rw-r--r--   0        0        0     4825 1970-01-01 00:00:00.000000 cohere-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-18 12:20:48.510770 cohere-4.1.5/LICENSE
+-rw-r--r--   0        0        0     4480 2023-04-18 12:20:48.510770 cohere-4.1.5/README.md
+-rw-r--r--   0        0        0      739 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/__init__.py
+-rw-r--r--   0        0        0    35046 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/client.py
+-rw-r--r--   0        0        0    26373 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/client_async.py
+-rw-r--r--   0        0        0     1187 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/logging.py
+-rw-r--r--   0        0        0      792 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     3142 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-04-18 12:20:48.510770 cohere-4.1.5/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      552 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      442 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     2614 2023-04-18 12:20:48.514771 cohere-4.1.5/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-04-18 12:20:48.514771 cohere-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.1.5/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.1.5/PKG-INFO
```

### Comparing `cohere-4.1.4/LICENSE` & `cohere-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/README.md` & `cohere-4.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -99,8 +99,15 @@
 ```
 
 You can run tests locally using:
 ```
 python -m pytest
 ```
 
-
+You can configure a different base url with:
+```bash
+CO_API_URL="https://localhost:8050" python3 foo.py
+```
+or
+```python
+cohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization
+```
```

### Comparing `cohere-4.1.4/cohere/__init__.py` & `cohere-4.1.5/cohere/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 API_VERSION = "1"
 COHERE_EMBED_BATCH_SIZE = 96
 CHAT_URL = "chat"
 CLASSIFY_URL = "classify"
 DETECT_LANG_URL = "detect-language"
 EMBED_URL = "embed"
 GENERATE_FEEDBACK_URL = "feedback/generate"
+GENERATE_PREFERENCE_FEEDBACK_URL = "feedback/generate/preference"
 GENERATE_URL = "generate"
 SUMMARIZE_URL = "summarize"
 RERANK_URL = "rerank"
 
 CHECK_API_KEY_URL = "check-api-key"
 TOKENIZE_URL = "tokenize"
 DETOKENIZE_URL = "detokenize"
 
 CLUSTER_JOBS_URL = "cluster-jobs"
+BULK_EMBED_JOBS_URL = "embed-jobs"
```

### Comparing `cohere-4.1.4/cohere/client.py` & `cohere-4.1.5/cohere/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import json as jsonlib
 import os
-import time
 from concurrent import futures
 from concurrent.futures import ThreadPoolExecutor
+from dataclasses import asdict
+from functools import partial
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 import cohere
-from cohere.error import CohereAPIError, CohereError
+from cohere.error import CohereAPIError, CohereConnectionError, CohereError
 from cohere.logging import logger
 from cohere.responses import (
     Classification,
     Classifications,
     Detokenization,
     Generations,
     StreamingGenerations,
     Tokens,
 )
+from cohere.responses.bulk_embed import BulkEmbedJob, CreateBulkEmbedJobResponse
 from cohere.responses.chat import Chat, StreamingChat
 from cohere.responses.classify import Example as ClassifyExample
 from cohere.responses.classify import LabelPrediction
 from cohere.responses.cluster import ClusterJobResult, CreateClusterJobResponse
 from cohere.responses.detectlang import DetectLanguageResponse, Language
 from cohere.responses.embeddings import Embeddings
-from cohere.responses.feedback import GenerateFeedbackResponse
+from cohere.responses.feedback import (
+    GenerateFeedbackResponse,
+    GeneratePreferenceFeedbackResponse,
+    PreferenceRating,
+)
 from cohere.responses.rerank import Reranking
 from cohere.responses.summarize import SummarizeResponse
-from cohere.utils import is_api_key_valid
+from cohere.utils import is_api_key_valid, wait_for_job
 
 
 class Client:
     """Cohere Client
 
     Args:
         api_key (str): Your API key.
@@ -52,15 +58,15 @@
         request_dict: dict = {},
         check_api_key: bool = True,
         client_name: Optional[str] = None,
         max_retries: int = 3,
         timeout: int = 120,
     ) -> None:
         self.api_key = api_key or os.getenv("CO_API_KEY")
-        self.api_url = cohere.COHERE_API_URL
+        self.api_url = os.getenv("CO_API_URL", cohere.COHERE_API_URL)
         self.batch_size = cohere.COHERE_EMBED_BATCH_SIZE
         self._executor = ThreadPoolExecutor(num_workers)
         self.num_workers = num_workers
         self.request_dict = request_dict
         self.request_source = "python-sdk"
         self.max_retries = max_retries
         self.timeout = timeout
@@ -493,14 +499,55 @@
             "prompt": prompt,
             "annotator_id": annotator_id,
             "model": model,
         }
         response = self._request(cohere.GENERATE_FEEDBACK_URL, json_body)
         return GenerateFeedbackResponse(id=response["id"])
 
+    def generate_preference_feedback(
+        self,
+        ratings: List[PreferenceRating],
+        model=None,
+        prompt: str = None,
+        annotator_id: str = None,
+    ) -> GeneratePreferenceFeedbackResponse:
+        """Give preference feedback on a response from the Cohere Generate API to improve the model.
+
+        Args:
+            ratings (List[PreferenceRating]): A list of PreferenceRating objects.
+            model (str): (Optional) ID of the model.
+            prompt (str): (Optional) The prompt used to generate the response.
+            annotator_id (str): (Optional) The ID of the annotator.
+
+        Examples:
+            A user accepts a model's suggestion in an assisted writing setting, and prefers it to a second suggestion:
+            >>> generations = co.generate(f"Write me a polite email responding to the one below: {email}. Response:", num_generations=2)
+            >>> if user_accepted_idx: // prompt user for which generation they prefer
+            >>>    ratings = []
+            >>>    if user_accepted_idx == 0:
+            >>>        ratings.append(PreferenceRating(request_id=0, rating=1))
+            >>>        ratings.append(PreferenceRating(request_id=1, rating=0))
+            >>>    else:
+            >>>        ratings.append(PreferenceRating(request_id=0, rating=0))
+            >>>        ratings.append(PreferenceRating(request_id=1, rating=1))
+            >>>    co.generate_preference_feedback(ratings=ratings)
+        """
+        ratings_dicts = []
+        for rating in ratings:
+            ratings_dicts.append(asdict(rating))
+
+        json_body = {
+            "ratings": ratings_dicts,
+            "prompt": prompt,
+            "annotator_id": annotator_id,
+            "model": model,
+        }
+        response = self._request(cohere.GENERATE_PREFERENCE_FEEDBACK_URL, json_body)
+        return GenerateFeedbackResponse(id=response["id"])
+
     def rerank(
         self,
         query: str,
         documents: Union[List[str], List[Dict[str, Any]]],
         model: str = None,
         top_n: Optional[int] = None,
     ) -> Reranking:
@@ -673,18 +720,125 @@
         Raises:
             TimeoutError: wait timed out
 
         Returns:
             ClusterJobResult: Clustering job result.
         """
 
-        start_time = time.time()
-        job = self.get_cluster_job(job_id)
+        return wait_for_job(
+            get_job=partial(self.get_cluster_job, job_id),
+            timeout=timeout,
+            interval=interval,
+        )
+
+    def create_bulk_embed_job(
+        self,
+        input_file_url: str,
+        model: Optional[str] = None,
+        truncate: Optional[str] = None,
+        compress: Optional[bool] = None,
+        compression_codebook: Optional[str] = None,
+        text_field: Optional[str] = None,
+        output_format: Optional[str] = None,
+    ) -> CreateBulkEmbedJobResponse:
+        """Create bulk embed job.
+
+        Args:
+            input_file_url (str): File with texts to embed.
+            model (Optional[str], optional): The model ID to use for embedding the text. Defaults to None.
+            truncate (Optional[str], optional): How the API handles text longer than the maximum token length. Defaults to None.
+            compress (Optional[bool], optional): Use embedding compression. Defaults to None.
+            compression_codebook (Optional[str], optional): Embedding compression codebook. Defaults to None.
+            text_field (Optional[str], optional): Name of the column containing text to embed. Defaults to None.
+            output_format (Optional[str], optional): Output format and file extension. Defaults to None.
+
+        Returns:
+            CreateBulkEmbedJobResponse: Created bulk embed job handler
+        """
+
+        json_body = {
+            "input_file_url": input_file_url,
+            "model": model,
+            "truncate": truncate,
+            "compress": compress,
+            "compression_codebook": compression_codebook,
+            "text_field": text_field,
+            "output_format": output_format,
+        }
+
+        response = self._request(cohere.BULK_EMBED_JOBS_URL, json=json_body)
+
+        return CreateBulkEmbedJobResponse.from_dict(
+            response,
+            wait_fn=self.wait_for_bulk_embed_job,
+        )
+
+    def list_bulk_embed_jobs(self) -> List[BulkEmbedJob]:
+        """List bulk embed jobs.
 
-        while not job.is_final_state:
-            if timeout is not None and time.time() - start_time > timeout:
-                raise TimeoutError(f"wait_for_cluster_job timed out after {timeout} seconds")
+        Returns:
+            List[BulkEmbedJob]: Bulk embed jobs.
+        """
 
-            time.sleep(interval)
-            job = self.get_cluster_job(job_id)
+        response = self._request(f"{cohere.BULK_EMBED_JOBS_URL}/list", method="GET")
+        return [BulkEmbedJob.from_dict({"meta": response.get("meta"), **r}) for r in response["bulk_embed_jobs"]]
 
-        return job
+    def get_bulk_embed_job(self, job_id: str) -> BulkEmbedJob:
+        """Get bulk embed job.
+
+        Args:
+            job_id (str): Bulk embed job id.
+
+        Raises:
+            ValueError: "job_id" is empty
+
+        Returns:
+            BulkEmbedJob: Bulk embed job.
+        """
+
+        if not job_id.strip():
+            raise ValueError('"job_id" is empty')
+
+        response = self._request(f"{cohere.BULK_EMBED_JOBS_URL}/{job_id}", method="GET")
+        return BulkEmbedJob.from_dict(response)
+
+    def cancel_bulk_embed_job(self, job_id: str) -> None:
+        """Cancel bulk embed job.
+
+        Args:
+            job_id (str): Bulk embed job id.
+
+        Raises:
+            ValueError: "job_id" is empty
+        """
+
+        if not job_id.strip():
+            raise ValueError('"job_id" is empty')
+
+        self._request(f"{cohere.BULK_EMBED_JOBS_URL}/{job_id}/cancel", method="POST", json={})
+
+    def wait_for_bulk_embed_job(
+        self,
+        job_id: str,
+        timeout: Optional[float] = None,
+        interval: float = 10,
+    ) -> BulkEmbedJob:
+        """Wait for bulk embed job completion.
+
+        Args:
+            job_id (str): Bulk embed job id.
+            timeout (Optional[float], optional): Wait timeout in seconds, if None - there is no limit to the wait time.
+                Defaults to None.
+            interval (float, optional): Wait poll interval in seconds. Defaults to 10.
+
+        Raises:
+            TimeoutError: wait timed out
+
+        Returns:
+            BulkEmbedJob: Bulk embed job.
+        """
+
+        return wait_for_job(
+            get_job=partial(self.get_bulk_embed_job, job_id),
+            timeout=timeout,
+            interval=interval,
+        )
```

### Comparing `cohere-4.1.4/cohere/client_async.py` & `cohere-4.1.5/cohere/client_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import json as jsonlib
 import os
 import posixpath
 import time
 from collections import defaultdict
+from dataclasses import asdict
+from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import aiohttp
 import backoff
 
 import cohere
 from cohere.client import Client
@@ -18,25 +20,28 @@
     Classification,
     Classifications,
     ClusterJobResult,
     DetectLanguageResponse,
     Detokenization,
     Embeddings,
     GenerateFeedbackResponse,
+    GeneratePreferenceFeedbackResponse,
     Generations,
     LabelPrediction,
     Language,
+    PreferenceRating,
     Reranking,
     StreamingGenerations,
     SummarizeResponse,
     Tokens,
 )
+from cohere.responses.bulk_embed import AsyncCreateBulkEmbedJobResponse, BulkEmbedJob
 from cohere.responses.chat import AsyncChat, StreamingChat
 from cohere.responses.classify import Example as ClassifyExample
-from cohere.utils import is_api_key_valid, np_json_dumps
+from cohere.utils import async_wait_for_job, is_api_key_valid, np_json_dumps
 
 JSON = Union[Dict, List]
 
 
 class AsyncClient(Client):
     """AsyncClient
 
@@ -54,15 +59,15 @@
         request_dict: dict = {},
         check_api_key: bool = True,
         client_name: Optional[str] = None,
         max_retries: int = 3,
         timeout=120,
     ) -> None:
         self.api_key = api_key or os.getenv("CO_API_KEY")
-        self.api_url = cohere.COHERE_API_URL
+        self.api_url = os.getenv("CO_API_URL", cohere.COHERE_API_URL)
         self.batch_size = cohere.COHERE_EMBED_BATCH_SIZE
         self.num_workers = num_workers
         self.request_dict = request_dict
         self.request_source = "python-sdk"
         self.max_retries = max_retries
         if client_name:
             self.request_source += ":" + client_name
@@ -334,14 +339,33 @@
             "prompt": prompt,
             "annotator_id": annotator_id,
             "model": model,
         }
         response = await self._request(cohere.GENERATE_FEEDBACK_URL, json_body)
         return GenerateFeedbackResponse(id=response["id"])
 
+    async def generate_preference_feedback(
+        self,
+        ratings: List[PreferenceRating],
+        model=None,
+        prompt: str = None,
+        annotator_id: str = None,
+    ) -> GeneratePreferenceFeedbackResponse:
+        ratings_dicts = []
+        for rating in ratings:
+            ratings_dicts.append(asdict(rating))
+        json_body = {
+            "ratings": ratings_dicts,
+            "prompt": prompt,
+            "annotator_id": annotator_id,
+            "model": model,
+        }
+        response = await self._request(cohere.GENERATE_PREFERENCE_FEEDBACK_URL, json_body)
+        return GeneratePreferenceFeedbackResponse(id=response["id"])
+
     async def rerank(
         self,
         query: str,
         documents: Union[List[str], List[Dict[str, Any]]],
         model: str = None,
         top_n: Optional[int] = None,
     ) -> Reranking:
@@ -454,25 +478,132 @@
         Raises:
             TimeoutError: wait timed out
 
         Returns:
             ClusterJobResult: Clustering job result.
         """
 
-        start_time = time.time()
-        job = await self.get_cluster_job(job_id)
+        return await async_wait_for_job(
+            get_job=partial(self.get_cluster_job, job_id),
+            timeout=timeout,
+            interval=interval,
+        )
 
-        while not job.is_final_state:
-            if timeout is not None and time.time() - start_time > timeout:
-                raise TimeoutError(f"wait_for_cluster_job timed out after {timeout} seconds")
+    async def create_bulk_embed_job(
+        self,
+        input_file_url: str,
+        model: Optional[str] = None,
+        truncate: Optional[str] = None,
+        compress: Optional[bool] = None,
+        compression_codebook: Optional[str] = None,
+        text_field: Optional[str] = None,
+        output_format: Optional[str] = None,
+    ) -> AsyncCreateBulkEmbedJobResponse:
+        """Create bulk embed job.
 
-            await asyncio.sleep(interval)
-            job = await self.get_cluster_job(job_id)
+        Args:
+            input_file_url (str): File with texts to embed.
+            model (Optional[str], optional): The model ID to use for embedding the text. Defaults to None.
+            truncate (Optional[str], optional): How the API handles text longer than the maximum token length. Defaults to None.
+            compress (Optional[bool], optional): Use embedding compression. Defaults to None.
+            compression_codebook (Optional[str], optional): Embedding compression codebook. Defaults to None.
+            text_field (Optional[str], optional): Name of the column containing text to embed. Defaults to None.
+            output_format (Optional[str], optional): Output format and file extension. Defaults to None.
 
-        return job
+        Returns:
+            AsyncCreateBulkEmbedJobResponse: Created bulk embed job handler
+        """
+
+        json_body = {
+            "input_file_url": input_file_url,
+            "model": model,
+            "truncate": truncate,
+            "compress": compress,
+            "compression_codebook": compression_codebook,
+            "text_field": text_field,
+            "output_format": output_format,
+        }
+
+        response = await self._request(cohere.BULK_EMBED_JOBS_URL, json=json_body)
+
+        return AsyncCreateBulkEmbedJobResponse.from_dict(
+            response,
+            wait_fn=self.wait_for_bulk_embed_job,
+        )
+
+    async def list_bulk_embed_jobs(self) -> List[BulkEmbedJob]:
+        """List bulk embed jobs.
+
+        Returns:
+            List[BulkEmbedJob]: Bulk embed jobs.
+        """
+
+        response = await self._request(f"{cohere.BULK_EMBED_JOBS_URL}/list", method="GET")
+        return [BulkEmbedJob.from_dict({"meta": response.get("meta"), **r}) for r in response["bulk_embed_jobs"]]
+
+    async def get_bulk_embed_job(self, job_id: str) -> BulkEmbedJob:
+        """Get bulk embed job.
+
+        Args:
+            job_id (str): Bulk embed job id.
+
+        Raises:
+            ValueError: "job_id" is empty
+
+        Returns:
+            BulkEmbedJob: Bulk embed job.
+        """
+
+        if not job_id.strip():
+            raise ValueError('"job_id" is empty')
+
+        response = await self._request(f"{cohere.BULK_EMBED_JOBS_URL}/{job_id}", method="GET")
+        return BulkEmbedJob.from_dict(response)
+
+    async def cancel_bulk_embed_job(self, job_id: str) -> None:
+        """Cancel bulk embed job.
+
+        Args:
+            job_id (str): Bulk embed job id.
+
+        Raises:
+            ValueError: "job_id" is empty
+        """
+
+        if not job_id.strip():
+            raise ValueError('"job_id" is empty')
+
+        await self._request(f"{cohere.BULK_EMBED_JOBS_URL}/{job_id}/cancel", method="POST", json={})
+
+    async def wait_for_bulk_embed_job(
+        self,
+        job_id: str,
+        timeout: Optional[float] = None,
+        interval: float = 10,
+    ) -> BulkEmbedJob:
+        """Wait for bulk embed job completion.
+
+        Args:
+            job_id (str): Bulk embed job id.
+            timeout (Optional[float], optional): Wait timeout in seconds, if None - there is no limit to the wait time.
+                Defaults to None.
+            interval (float, optional): Wait poll interval in seconds. Defaults to 10.
+
+        Raises:
+            TimeoutError: wait timed out
+
+        Returns:
+            BulkEmbedJob: Bulk embed job.
+        """
+
+        return await async_wait_for_job(
+            get_job=partial(self.get_bulk_embed_job, job_id),
+            timeout=timeout,
+            interval=interval,
+        )
 
 
 class AIOHTTPBackend:
     """HTTP backend which handles retries, concurrency limiting and logging"""
 
     SLEEP_AFTER_FAILURE = defaultdict(lambda: 0.25, {429: 5})
```

### Comparing `cohere-4.1.4/cohere/error.py` & `cohere-4.1.5/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/logging.py` & `cohere-4.1.5/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/__init__.py` & `cohere-4.1.5/cohere/responses/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,12 +3,16 @@
 from cohere.responses.cluster import (
     AsyncCreateClusterJobResponse,
     ClusterJobResult,
     CreateClusterJobResponse,
 )
 from cohere.responses.detectlang import DetectLanguageResponse, Language
 from cohere.responses.embeddings import Embeddings
-from cohere.responses.feedback import GenerateFeedbackResponse
+from cohere.responses.feedback import (
+    GenerateFeedbackResponse,
+    GeneratePreferenceFeedbackResponse,
+    PreferenceRating,
+)
 from cohere.responses.generation import Generation, Generations, StreamingGenerations
 from cohere.responses.rerank import RerankDocument, Reranking, RerankResult
 from cohere.responses.summarize import SummarizeResponse
 from cohere.responses.tokenize import Detokenization, Tokens
```

### Comparing `cohere-4.1.4/cohere/responses/base.py` & `cohere-4.1.5/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/chat.py` & `cohere-4.1.5/cohere/responses/chat.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/classify.py` & `cohere-4.1.5/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/cluster.py` & `cohere-4.1.5/cohere/responses/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List, Optional
 
 from cohere.responses.base import CohereObject
+from cohere.utils import JobWithStatus
 
 
 class Cluster(CohereObject):
     id: str
     keywords: List[str]
     description: str
     size: int
@@ -31,15 +32,15 @@
             keywords=data["keywords"],
             description=data["description"],
             size=data["size"],
             sample_elements=data["sample_elements"],
         )
 
 
-class ClusterJobResult(CohereObject):
+class ClusterJobResult(CohereObject, JobWithStatus):
     job_id: str
     status: str
     is_final_state: bool
     output_clusters_url: Optional[str]
     output_outliers_url: Optional[str]
     clusters: Optional[List[Cluster]]
     error: Optional[str]
@@ -49,15 +50,15 @@
         self,
         job_id: str,
         status: str,
         output_clusters_url: Optional[str],
         output_outliers_url: Optional[str],
         clusters: Optional[List[Cluster]],
         error: Optional[str],
-        is_final_state: Optional[bool] = None,
+        is_final_state: bool,
         meta: Optional[Dict[str, Any]] = None,
     ):
         # convert empty string to `None`
         if not output_clusters_url:
             output_clusters_url = None
         if not output_outliers_url:
             output_outliers_url = None
@@ -78,36 +79,39 @@
         else:
             clusters = [Cluster.from_dict(c) for c in data["clusters"]]
 
         is_final_state = data.get("is_final_state")
         status = data["status"]
         # TODO: remove this. temp for backward compatibility until the `is_final_state` field is added to the API
         if is_final_state is None:
-            is_final_state = status in ["completed", "failed"]
+            is_final_state = status in ["complete", "failed"]
 
         return ClusterJobResult(
             job_id=data["job_id"],
             status=status,
             is_final_state=is_final_state,
             output_clusters_url=data["output_clusters_url"],
             output_outliers_url=data["output_outliers_url"],
             clusters=clusters,
             error=data.get("error"),
             meta=data.get("meta"),
         )
 
+    def has_terminal_status(self) -> bool:
+        return self.is_final_state
+
 
 class CreateClusterJobResponse(CohereObject):
     job_id: str
     meta: Optional[Dict[str, Any]]
 
     def __init__(self, job_id: str, meta: Optional[Dict[str, Any]], wait_fn):
         self.job_id = job_id
-        self._wait_fn = wait_fn
         self.meta = meta
+        self._wait_fn = wait_fn
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any], wait_fn) -> "CreateClusterJobResponse":
         return cls(job_id=data["job_id"], wait_fn=wait_fn, meta=data.get("meta"))
 
     def wait(
         self,
```

### Comparing `cohere-4.1.4/cohere/responses/detectlang.py` & `cohere-4.1.5/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/generation.py` & `cohere-4.1.5/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/rerank.py` & `cohere-4.1.5/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/summarize.py` & `cohere-4.1.5/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/cohere/responses/tokenize.py` & `cohere-4.1.5/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.1.4/pyproject.toml` & `cohere-4.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.1.4"
+version = "4.1.5"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.1.4/setup.py` & `cohere-4.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.1.4',
+    'version': '4.1.5',
     'description': '',
-    'long_description': "![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client('YOUR_API_KEY')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model='large',\n            prompt='co:here',\n            max_tokens=10)\n\n# print the predicted text\nprint('prediction: {}'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere's APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation's page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\n\n",
+    'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cohere-4.1.4/PKG-INFO` & `cohere-4.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.1.4
+Version: 4.1.5
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -116,9 +116,16 @@
 ```
 
 You can run tests locally using:
 ```
 python -m pytest
 ```
 
-
+You can configure a different base url with:
+```bash
+CO_API_URL="https://localhost:8050" python3 foo.py
+```
+or
+```python
+cohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization
+```
```

