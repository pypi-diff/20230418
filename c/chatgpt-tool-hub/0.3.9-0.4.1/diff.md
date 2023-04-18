# Comparing `tmp/chatgpt-tool-hub-0.3.9.tar.gz` & `tmp/chatgpt-tool-hub-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.3.9.tar", last modified: Tue Apr 11 18:05:34 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.4.1.tar", last modified: Tue Apr 18 17:25:16 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.3.9.tar` & `chatgpt-tool-hub-0.4.1.tar`

### file list

```diff
@@ -1,141 +1,155 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.750461 chatgpt-tool-hub-0.3.9/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.3.9/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    12322 2023-04-11 18:05:34.750254 chatgpt-tool-hub-0.3.9/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    11527 2023-04-11 17:18:33.000000 chatgpt-tool-hub-0.3.9/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.723220 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)      287 2023-04-11 14:39:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.725372 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       52 2023-04-08 09:10:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      215 2023-03-27 18:16:41.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/all_app_list.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1546 2023-04-03 00:57:23.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1733 2023-04-08 18:43:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1943 2023-04-08 19:02:47.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1641 2023-04-08 18:42:45.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/load_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4390 2023-04-09 04:03:14.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.726482 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      236 2023-03-27 18:17:19.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/all_bot_list.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12507 2023-04-11 16:27:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11530 2023-04-08 02:32:23.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot_executor.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.727074 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5338 2023-04-11 14:56:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      915 2023-04-11 14:00:29.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-02 11:55:16.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/initialize.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.727666 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4475 2023-03-27 18:25:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      635 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.728514 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.729324 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4243 2023-04-09 16:23:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1229 2023-04-09 16:24:47.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10688 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7544 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.733257 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1646 2023-04-10 16:23:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    25561 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)      262 2023-04-11 14:28:26.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1262 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      981 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1092 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)      601 2023-04-09 14:00:24.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8579 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6714 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      693 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.734155 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1684 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2395 2023-04-02 13:29:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.735202 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)     1381 2023-04-11 15:05:57.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13016 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.736057 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15182 2023-04-07 16:11:18.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/chatgpt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/model_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)    28454 2023-04-08 08:51:59.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/openai.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.737062 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6421 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.738112 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)      535 2023-04-11 17:10:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      737 2023-04-08 18:52:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/all_tool_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.738772 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      143 2023-04-05 16:49:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1660 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/arxiv_search.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1672 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4023 2023-04-02 11:48:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.739452 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      146 2023-04-01 00:56:58.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1219 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/bing_search.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3449 2023-04-09 04:35:45.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.739929 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/
--rw-r--r--   0 goldfish   (502) staff       (20)       57 2023-04-03 14:50:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1101 2023-04-08 19:06:04.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.740588 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      174 2023-03-30 14:10:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1804 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/google_search.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3571 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2001 2023-04-09 04:04:32.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.741300 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)       71 2023-04-08 18:45:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4625 2023-04-11 17:08:37.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1679 2023-04-11 17:15:41.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/meteo_weather.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.741933 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       77 2023-04-11 16:16:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2321 2023-04-11 16:12:06.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/morning_news.py
--rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/summary_prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.742622 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      121 2023-03-28 16:36:30.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2437 2023-04-03 14:18:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/api_docs_prompts.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1664 2023-04-08 18:30:12.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/news.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.743105 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)       68 2023-04-08 18:36:10.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2153 2023-04-08 19:22:38.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/python_repl.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.743780 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      172 2023-04-03 16:21:48.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1887 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/searxng.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15595 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.744309 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)       57 2023-04-08 18:44:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4229 2023-04-09 03:07:36.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3673 2023-04-09 15:20:49.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.744754 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/
--rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2229 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/text2image.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.746981 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     1919 2023-04-11 15:50:56.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1338 2023-04-05 05:14:36.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      749 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1821 2023-04-08 19:06:57.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2058 2023-03-30 15:44:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6307 2023-04-11 15:03:14.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.748568 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1058 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2370 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.749389 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1177 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1902 2023-03-30 15:40:12.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-11 18:05:22.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.723811 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    12322 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     4358 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      213 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-11 18:05:34.750501 chatgpt-tool-hub-0.3.9/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1897 2023-04-11 17:57:20.000000 chatgpt-tool-hub-0.3.9/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.644944 chatgpt-tool-hub-0.4.1/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.1/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    12339 2023-04-18 17:25:16.644718 chatgpt-tool-hub-0.4.1/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    11544 2023-04-17 13:50:36.000000 chatgpt-tool-hub-0.4.1/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.612497 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)      144 2023-04-18 14:50:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.615568 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-17 13:52:51.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1546 2023-04-03 00:57:23.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2259 2023-04-18 16:14:53.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3542 2023-04-18 16:19:53.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/auto_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1947 2023-04-17 13:52:51.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4487 2023-04-18 17:07:45.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.616691 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)      232 2023-04-16 13:47:06.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-16 10:53:41.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/all_bot_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.617286 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5230 2023-04-18 15:11:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1096 2023-04-18 15:50:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-16 13:47:07.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/initialize.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.618004 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5064 2023-04-18 15:54:05.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      860 2023-04-18 15:54:05.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.619051 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.620103 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4243 2023-04-09 16:23:42.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1229 2023-04-09 16:24:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10688 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7544 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.624019 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    25561 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-17 13:38:40.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/config.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      168 2023-04-16 00:10:23.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1262 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      981 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1092 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      601 2023-04-09 14:00:24.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8579 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6714 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.625170 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1684 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2395 2023-04-02 13:29:17.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.626016 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/
+-rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-16 11:07:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12527 2023-04-18 16:55:30.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11922 2023-04-18 16:27:57.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/tool_engine.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.627215 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2142 2023-04-18 16:55:30.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13016 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.628361 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15184 2023-04-18 14:30:05.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/model_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    28455 2023-04-18 14:30:05.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/openai.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.629363 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6421 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.630972 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)      921 2023-04-17 15:09:40.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 13:37:31.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.632094 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      135 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1861 2023-04-17 15:13:14.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1672 2023-04-18 13:52:01.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4022 2023-04-17 14:40:26.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.632839 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1287 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3467 2023-04-18 14:34:32.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.633509 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/debug/
+-rw-r--r--   0 goldfish   (502) staff       (20)       56 2023-04-17 14:03:49.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/debug/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1125 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/debug/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.634112 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1828 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3572 2023-04-18 13:52:01.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2547 2023-04-18 14:44:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.634794 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4894 2023-04-11 18:27:51.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1699 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.635283 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      581 2023-04-18 14:44:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.635796 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/finance_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/finance_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1281 2023-04-18 15:20:18.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/finance_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.636542 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2272 2023-04-18 14:38:46.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.637254 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/
+-rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2594 2023-04-18 15:33:01.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/docs_prompts.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1693 2023-04-18 15:20:18.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-18 15:50:55.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.637582 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2177 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/python/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.639008 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1911 2023-04-18 13:56:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15595 2023-04-18 13:56:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.640078 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/summary/
+-rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/summary/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 16:44:58.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/summary/map_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 16:58:39.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/summary/reduce_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6823 2023-04-18 14:58:22.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/summary/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.640502 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-16 10:42:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4261 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3673 2023-04-17 14:20:38.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      788 2023-04-17 14:40:26.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/tool_register.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.641003 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2254 2023-04-17 14:36:10.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.642945 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2208 2023-04-18 13:56:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5121 2023-04-18 16:36:50.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-17 15:29:00.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1835 2023-04-18 14:22:11.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2058 2023-03-30 15:44:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4429 2023-04-18 17:23:59.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.643720 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1082 2023-04-17 15:29:00.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2370 2023-04-18 13:56:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.644376 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1202 2023-04-17 14:40:26.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1902 2023-04-18 13:56:29.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-18 17:02:47.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-18 17:25:16.613391 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    12339 2023-04-18 17:25:16.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     4759 2023-04-18 17:25:16.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-18 17:25:16.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      240 2023-04-18 17:25:16.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-18 17:25:16.000000 chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-18 17:25:16.644989 chatgpt-tool-hub-0.4.1/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1946 2023-04-18 17:21:40.000000 chatgpt-tool-hub-0.4.1/setup.py
```

### Comparing `chatgpt-tool-hub-0.3.9/LICENSE` & `chatgpt-tool-hub-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/PKG-INFO` & `chatgpt-tool-hub-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.3.9
+Version: 0.4.1
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -95,15 +95,15 @@
       "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
       "no_default": false,  // 控制是否加载默认工具
       "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
   }
 }
 ```
 
-#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+#### (4). `python3 test.py 你的问题1 [你的问题2 ......]`
 
 > chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
 
 #### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
 
 --- 
 
@@ -119,19 +119,19 @@
 
 `pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
 
 #### (2). 示例代码：
 
 ```python
 import os
-from chatgpt_tool_hub.apps import load_app
-os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
-os.environ["PROXY"] = "http://192.168.7.1:7890"
-app = load_app()
-reply = app.ask(YOUR_QUESTION_TO_HERE)
+from chatgpt_tool_hub.apps import AppFactory
+os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"
+app = AppFactory().create_app()
+reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
   
 > 如果有需求，我会更新接入的文档，欢迎提issue
 
 ---
```

### Comparing `chatgpt-tool-hub-0.3.9/README.md` & `chatgpt-tool-hub-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
       "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
       "no_default": false,  // 控制是否加载默认工具
       "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
   }
 }
 ```
 
-#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+#### (4). `python3 test.py 你的问题1 [你的问题2 ......]`
 
 > chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
 
 #### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
 
 --- 
 
@@ -100,19 +100,19 @@
 
 `pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
 
 #### (2). 示例代码：
 
 ```python
 import os
-from chatgpt_tool_hub.apps import load_app
-os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
-os.environ["PROXY"] = "http://192.168.7.1:7890"
-app = load_app()
-reply = app.ask(YOUR_QUESTION_TO_HERE)
+from chatgpt_tool_hub.apps import AppFactory
+os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"
+app = AppFactory().create_app()
+reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
   
 > 如果有需求，我会更新接入的文档，欢迎提issue
 
 ---
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app_factory.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/app_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
-from chatgpt_tool_hub.apps.app import App
-from chatgpt_tool_hub.common.utils import get_from_dict_or_env
+from chatgpt_tool_hub.apps import App
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.models import build_model_params
+from chatgpt_tool_hub.tools import dynamic_tool_loader
 
 
 class AppFactory:
     def __init__(self):
         self.default_tools_list = []
         pass
 
@@ -21,15 +22,18 @@
             LOG.setLevel(logging.INFO)
 
         # default tools
         no_default_flag = get_from_dict_or_env(kwargs, "no_default", "NO_DEFAULT", "")
         if no_default_flag:
             self.default_tools_list = []
         else:
-            self.default_tools_list = ["python", "url-get", "terminal", "meteo-weather"]
+            self.default_tools_list = ["python", "terminal", "url-get", "meteo-weather", "news"]
+
+        # dynamic loading tool
+        dynamic_tool_loader()
 
     def create_app(self, app_type: str = 'victorinox', tools_list: list = None, **kwargs) -> App:
         tools_list = [] if not tools_list else tools_list
 
         self.init_env(**kwargs)
 
         if app_type == 'lite':
@@ -40,14 +44,24 @@
 
         elif app_type == 'victorinox':
             from chatgpt_tool_hub.apps.victorinox import Victorinox
 
             for default_tool in self.default_tools_list:
                 if default_tool not in tools_list:
                     tools_list.append(default_tool)
+            # todo refactor
+            if "browser" in tools_list:
+                tools_list = list(filter(lambda tool: tool != "url-get", tools_list))
 
             app = Victorinox(**build_model_params(kwargs))
             app.create(tools_list, **kwargs)
             return app
+        elif app_type == 'auto':
+            from chatgpt_tool_hub.apps.auto_app import AutoApp
 
+            # todo no default
+
+            app = AutoApp(**build_model_params(kwargs))
+            app.create(tools_list, **kwargs)
+            return app
         else:
             raise NotImplementedError
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/lite_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from chatgpt_tool_hub.apps.app import App
-from chatgpt_tool_hub.apps.load_app import load_app
+from chatgpt_tool_hub.apps import App
+from chatgpt_tool_hub.apps import AppFactory
 from chatgpt_tool_hub.chains import LLMChain
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.models.model_factory import ModelFactory
 from chatgpt_tool_hub.prompts import PromptTemplate
 
 
 class LiteApp(App):
@@ -47,10 +47,10 @@
                 return self.ask(query, chat_history, retry_num + 1)
             else:
                 LOG.error("exceed retry_num")
                 raise TimeoutError("超过重试次数")
 
 
 if __name__ == "__main__":
-    bot = load_app('lite', tools_list=["wikipedia"])
+    bot = AppFactory().create_app('lite', tools_list=["wikipedia"])
     response = bot.ask("")
     print(response)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/apps/victorinox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from chatgpt_tool_hub.apps.app import App
-from chatgpt_tool_hub.apps.load_app import load_app
-from chatgpt_tool_hub.bots.initialize import initialize_bot
-from chatgpt_tool_hub.common.constants import MEMORY_MAX_TOKENS_NUM
+from chatgpt_tool_hub.apps import App
+from chatgpt_tool_hub.apps import AppFactory
+from chatgpt_tool_hub.bots import initialize_bot
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.database import ConversationTokenBufferMemory
+from chatgpt_tool_hub.models import MEMORY_MAX_TOKENS_NUM
 from chatgpt_tool_hub.models.model_factory import ModelFactory
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.load_tools import load_tools
 
 
 class Victorinox(App):
     def __init__(self, **app_kwargs):
         super().__init__()
         if not self.init_flag:
@@ -22,26 +23,26 @@
         if tools_list is None:
             tools_list = []
         if not self._check_mandatory_tools(tools_list):
             raise ValueError("check mandatory tools failed")
         if self.tools or self.tools_kwargs:
             LOG.warning("refresh the config of tools")
 
-        map(self.tools.add, tools_list)
+        for tool in tools_list:
+            self.tools.add(tool)
         self.tools_kwargs = tools_kwargs
 
         try:
-            tools = load_tools(tools_list, **tools_kwargs)
+            tools = load_tools(list(self.tools), main_tool_register, **tools_kwargs)
         except ValueError as e:
             LOG.error(str(e))
             raise RuntimeError("tool初始化失败")
 
         # loading tools from config.
-        LOG.info(f"Initializing {self.get_class_name()} success, "
-                 f"use_tools={tools_list}, params: {str(tools_kwargs)}")
+        LOG.info(f"use_tools={list(self.tools)}, params: {str(tools_kwargs)}")
 
         # create bots
         self.bot = initialize_bot(tools, self.llm, bot="chat-bot", verbose=True,
                                   memory=self.memory, max_iterations=3, early_stopping_method="generate")
 
     def add_tool(self, tools_list: list, **tools_kwargs):
         """todo: I think there have better way to implement"""
@@ -50,15 +51,15 @@
             return
 
         map(self.tools.add, tools_list)
         for tool_key in tools_kwargs:
             self.tools_kwargs[tool_key] = tools_kwargs[tool_key]
 
         try:
-            new_tools_list = load_tools(list(self.tools), **self.tools_kwargs)
+            new_tools_list = load_tools(list(self.tools), main_tool_register, **tools_kwargs)
         except ValueError as e:
             LOG.error(str(e))
             raise RuntimeError("tool初始化失败")
 
         # loading tools from config.
         LOG.info(f"add_tool {self.get_class_name()} success, "
                  f"use_tools={new_tools_list}, params: {str(self.tools_kwargs)}")
@@ -77,14 +78,15 @@
             raise ValueError("请求为空")
 
         # 更新session
         if chat_history is not None:
             self._refresh_memory(chat_history)
 
         try:
+            LOG.info(f"提问: {query}")
             return self.bot.run(query)
         except Exception as e:
             LOG.error(f"[APP] catch a Exception: {str(e)}")
             if retry_num < 1:
                 return self.ask(query, chat_history, retry_num + 1)
             else:
                 LOG.error("exceed retry_num")
@@ -106,10 +108,10 @@
                 outputs["output"] = item.get('content')
                 self.memory.save_context(inputs, outputs)
 
         LOG.debug("Now memory: {}".format(self.memory.chat_memory.messages))
 
 
 if __name__ == "__main__":
-    bot = load_app(tools_list=["wikipedia"])
+    bot = AppFactory().create_app(tools_list=["wikipedia"])
     content = bot.ask("")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Chain that takes in an input and produces an action and action input."""
 from __future__ import annotations
 
 import json
+import os
+import tempfile
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import yaml
 from pydantic import BaseModel, root_validator
 
 from chatgpt_tool_hub.chains import LLMChain
-from chatgpt_tool_hub.common.calculate_token import num_tokens_from_messages
+from chatgpt_tool_hub.common.calculate_token import count_string_tokens
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
-from chatgpt_tool_hub.common.constants import ALL_MAX_TOKENS_NUM, BOT_SCRATCHPAD_MAX_TOKENS_NUM
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.schema import BotAction, BotFinish, BaseMessage
+from chatgpt_tool_hub.models import ALL_MAX_TOKENS_NUM, BOT_SCRATCHPAD_MAX_TOKENS_NUM
 from chatgpt_tool_hub.models.base import BaseLLM
 from chatgpt_tool_hub.prompts import BasePromptTemplate
 from chatgpt_tool_hub.prompts import PromptTemplate
+from chatgpt_tool_hub.tools import SummaryTool
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 
 class Bot(BaseModel):
     """Class responsible for calling the language model and deciding the action.
 
     This is driven by an LLMChain. The prompt in the LLMChain MUST include
@@ -63,43 +66,43 @@
 
     def _crop_full_input(self, inputs: str) -> str:
         """ crop too long text """
         if not inputs:
             return inputs
         _input = inputs
 
-        while num_tokens_from_messages([{"user": "assistant", "content": _input}]) >= BOT_SCRATCHPAD_MAX_TOKENS_NUM:
-            _input_list = _input.split("\n")
+        while count_string_tokens(_input) >= BOT_SCRATCHPAD_MAX_TOKENS_NUM:
+
+            # compress text size
+            temp_file = tempfile.mkstemp()
+            file_path = temp_file[1]
+
+            with open(file_path, "w") as f:
+                f.write(_input + "\n")
+            _input = SummaryTool(max_segment_length=2000).run(str(file_path) + ", 0")
+            os.remove(file_path)
 
-            # 单个长文本处理
-            if len(_input_list) <= 2 and _input_list[0].startswith(self.observation_prefix):
-                return _input_list[0][:BOT_SCRATCHPAD_MAX_TOKENS_NUM]
-
-            _input = "\n".join(_input_list[1:])
-        # else:
-        #     LOG.debug("\nafter crop: " + str(_input))
         return _input
 
     def _get_next_action(self, full_inputs: Dict[str, str]) -> BotAction:
         full_output = self.llm_chain.predict(**full_inputs)
         parsed_output = self._extract_tool_and_input(full_output)
 
         action_input = "None" if parsed_output is None else parsed_output[1]
-        LOG.info(f"行动输入: {action_input}")
+        LOG.info(f"输入: {action_input}")
         retry_num = 0
         while parsed_output is None:
             retry_num += 1
             if retry_num > self.max_parse_retry_num:
                 raise ValueError(f"Could not parse LLM output: `{parsed_output}`")
 
             full_output = self._fix_text(full_output)
             full_inputs["bot_scratchpad"] += full_output
             output = self.llm_chain.predict(**full_inputs)
-            LOG.debug("(fix_text): retry response: " + str(output))
-            # full_output += output
+            # LOG.debug("(fix_text): retry response: " + str(output))
             parsed_output = self._extract_tool_and_input(output)
         return BotAction(
             tool=parsed_output[0], tool_input=parsed_output[1], log=full_output
         )
 
     def plan(
         self, intermediate_steps: List[Tuple[BotAction, str]], **kwargs: Any
@@ -201,14 +204,15 @@
         tool_names = [tool.name for tool in tools]
         return cls(llm_chain=llm_chain, allowed_tools=tool_names, **kwargs)
 
     def return_stopped_response(
         self,
         early_stopping_method: str,
         intermediate_steps: List[Tuple[BotAction, str]],
+        max_iterations: int,
         **kwargs: Any,
     ) -> BotFinish:
         """Return response when bot has been stopped due to max iterations."""
         if early_stopping_method == "force":
             # `force` just returns a constant string
             return BotFinish({"output": "Bot stopped due to max iterations."}, "")
         elif early_stopping_method == "generate":
@@ -217,16 +221,17 @@
             for action, observation in intermediate_steps:
                 thoughts += action.log
                 thoughts += (
                     f"\n{self.observation_prefix}{observation}\n{self.llm_prefix}"
                 )
             # Adding to the previous steps, we now tell the LLM to make a final pred
             thoughts += (
-                "\n\nI have exceeded the limit of tool usage and "
-                "now need to summarize all the information collected so far to generate a final answer:"
+                f"你超过了tool使用次数限制: 最多{max_iterations}次。"
+                "你现在需要总结当前你了解到的所有信息，来反馈给人类。"
+                "你需要生成一个final answer:"
             )
             new_inputs = {"bot_scratchpad": thoughts, "stop": self._stop}
             full_inputs = {**kwargs, **new_inputs}
             full_output = self.llm_chain.predict(**full_inputs)
             # We try to extract a final answer
             parsed_output = self._extract_tool_and_input(full_output)
             if parsed_output is None:
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot_executor.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/engine/tool_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from pydantic import BaseModel, root_validator
-from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.bots.bot import Bot
+
 from chatgpt_tool_hub.chains.base import Chain
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
 from chatgpt_tool_hub.common.input import get_color_mapping
+from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.schema import BotAction, BotFinish
+from chatgpt_tool_hub.engine import Bot
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.tool import InvalidTool
 
 
-class BotExecutor(Chain, BaseModel):
+class ToolEngine(Chain, BaseModel):
     """Consists of an bot using tools."""
 
     bot: Bot
     tools: Sequence[BaseTool]
     return_intermediate_steps: bool = False
     max_iterations: Optional[int] = 10
     early_stopping_method: str = "force"
@@ -130,15 +131,16 @@
             observation = InvalidTool().run(
                 output.tool,
                 verbose=self.verbose,
                 color=None,
                 llm_prefix="",
                 observation_prefix=self.bot.observation_prefix,
             )
-        LOG.debug("llm received: `" + str(observation.strip()) + f"` from [{output.tool}]")
+            # todo news tool catch `<property object at 0x7fcea0d914f0>`
+        LOG.debug("llm received: `" + repr(observation.strip()) + f"` from [{output.tool}]")
         return output, observation
 
     def _call(self, inputs: Dict[str, str]) -> Dict[str, Any]:
         """Run text through and get bot response."""
         # Do any preparation necessary when receiving a new input.
         self.bot.prepare_for_new_call()
         # Construct a mapping of tool name to tool for easy lookup
@@ -148,31 +150,38 @@
             [tool.name for tool in self.tools], excluded_colors=["green"]
         )
         intermediate_steps: List[Tuple[BotAction, str]] = []
         # Let's start tracking the iterations the bot has gone through
         iterations = 0
         # We now enter the bot loop (until it returns something).
         while self._should_continue(iterations):
-            LOG.debug("CoT 迭代次数: {}\n".format(str(iterations+1)))
+            # LOG.debug("CoT 迭代次数: {}\n".format(str(iterations+1)))
             next_step_output = self._take_next_step(
                 name_to_tool_map,
                 color_mapping,
                 inputs, intermediate_steps
             )
             if isinstance(next_step_output, BotFinish):
                 return self._return(next_step_output, intermediate_steps)
 
+            # todo test below
+            try:
+                action, observation = next_step_output
+                LOG.info(f"[{action.tool}]输出: {observation}")
+            except Exception as e:
+                LOG.debug(f"parsing next_step_output error: {repr(e)}")
+
             intermediate_steps.append(next_step_output)
             # See if tool should return directly
             tool_return = self._get_tool_return(next_step_output)
             if tool_return is not None:
                 return self._return(tool_return, intermediate_steps)
             iterations += 1
         output = self.bot.return_stopped_response(
-            self.early_stopping_method, intermediate_steps, **inputs
+            self.early_stopping_method, intermediate_steps, self.max_iterations, **inputs
         )
         return self._return(output, intermediate_steps)
 
     def _get_tool_return(
         self, next_step_output: Tuple[BotAction, str]
     ) -> Optional[BotFinish]:
         """Check if the tool is a returning tool."""
@@ -212,15 +221,15 @@
             # See if tool should return directly
             tool_return = self._get_tool_return(next_step_output)
             if tool_return is not None:
                 return await self._areturn(tool_return, intermediate_steps)
 
             iterations += 1
         output = self.bot.return_stopped_response(
-            self.early_stopping_method, intermediate_steps, **inputs
+            self.early_stopping_method, intermediate_steps, self.max_iterations, **inputs
         )
         return await self._areturn(output, intermediate_steps)
 
     async def _atake_next_step(
         self,
         name_to_tool_map: Dict[str, BaseTool],
         color_mapping: Dict[str, str],
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """An bot designed to hold a conversation in addition to using tools."""
 from __future__ import annotations
 
 import re
 from typing import Any, List, Optional, Sequence, Tuple
 
-from chatgpt_tool_hub.bots.bot import Bot
 from chatgpt_tool_hub.bots.chat_bot.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
 from chatgpt_tool_hub.chains import LLMChain
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
+from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.engine import Bot
 from chatgpt_tool_hub.models.base import BaseLLM
 from chatgpt_tool_hub.prompts import PromptTemplate
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.common.log import LOG
 
 
 class ChatBot(Bot):
     """An bot designed to hold a conversation in addition to using tools."""
 
     ai_prefix: str = "AI"
 
@@ -37,15 +37,14 @@
         instruction_text = FORMAT_INSTRUCTIONS.format(
             tool_names=tool_names, ai_prefix=self.ai_prefix
         )
         _text = ("\n\n"
                  f"You just told me: {text}, but it doesn't meet the format I mentioned to you. \n\n"
                  f"format: {instruction_text}. \n\n"
                  "You should understand why you did not input the correct format, correct it and try again. \n\n")
-        LOG.debug("(fix_text): fix_text: " + repr(_text))
         return _text
 
     @property
     def llm_prefix(self) -> str:
         """Prefix to append the llm call with."""
         return "Thought:"
 
@@ -83,24 +82,23 @@
             tool_names=tool_names, ai_prefix=ai_prefix
         )
         template = "\n\n".join([prefix, tool_strings, instruction_text, suffix])
         if input_variables is None:
             input_variables = ["input", "chat_history", "bot_scratchpad"]
         prompt = PromptTemplate(template=template, input_variables=input_variables)
 
-        LOG.debug("\nprompt: " + str(prompt) + "\n")
         return prompt
 
     @property
     def finish_tool_name(self) -> str:
         """Name of the tool to use to finish the chain."""
         return self.ai_prefix
 
     def _extract_tool_and_input(self, llm_output: str) -> Optional[Tuple[str, str]]:
-        # this is bad parsing rule
+        # todo this is bad parsing rule
         if f"{self.ai_prefix}:" in llm_output:
             return self.ai_prefix, llm_output.split(f"{self.ai_prefix}:")[-1].strip()
         regex = r"Action: (.*?)[\n]*Action Input: (.*)"
         match = re.search(regex, llm_output, re.DOTALL)
         if not match:
             return None
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/prompt.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/chat_bot/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 Assistant has access to the following tools:
 
 TOOLS:
 ------"""
 
 FORMAT_INSTRUCTIONS = """To use a tool, you MUST use the following format:
 ```
-Thought: Do I need to use a tool? Yes
+Thought: you should always think about what to do and which tool to choose
 Action: the action to take, should be one of [{tool_names}]
 Action Input: the input to the action
 Observation: the result of the action
 ```
 
 When you know the final answer or if you do not need to use a tool, you MUST use the format:
 ```
-Thought: Do I need to use a tool? No
+Thought: you can think about how you found the final answer
 {ai_prefix}: the final answer to the original input question. the final answer MUST be in chinese all the time!   
 ```
 """
 
 SUFFIX = """Begin!
 
 Previous conversation history:
 {chat_history}
 
 New input: {input}
 {bot_scratchpad}
 
 You should provide feedback on whether the task has been completed, 
 explain what you have done, what you have seen and what the outcome was to the Human. 
+Please note that the prefix "AI:" is very important for me to parse your response, so please be sure to add this prefix.
 Don't make up you response.
 """
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/initialize.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/initialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Load bot."""
 from typing import Any, Optional, Sequence
 
 from chatgpt_tool_hub.bots.all_bot_list import BOT_TO_CLASS
-from chatgpt_tool_hub.bots.bot_executor import BotExecutor
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
 from chatgpt_tool_hub.common.callbacks import get_callback_manager
+from chatgpt_tool_hub.engine import ToolEngine
 from chatgpt_tool_hub.models.base import BaseLanguageModel
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 
 def initialize_bot(
     tools: Sequence[BaseTool],
     llm: BaseLanguageModel,
     bot: Optional[str] = None,
     callback_manager: Optional[BaseCallbackManager] = get_callback_manager(),
     bot_kwargs: Optional[dict] = None,
     **kwargs: Any,
-) -> BotExecutor:
+) -> ToolEngine:
     """Load an bot executor given tools and LLM.
 
     Args:
         tools: List of tools this bot has access to.
         llm: Language model to use as the bot.
         bot: A string that specified the bot type to use. Valid options are:
             `qa-bot`
@@ -47,13 +47,13 @@
     bot_cls = BOT_TO_CLASS[bot]
 
     bot_kwargs = bot_kwargs or {}
     bot_obj = bot_cls.from_llm_and_tools(
         llm, tools, callback_manager=callback_manager, **bot_kwargs
     )
 
-    return BotExecutor.from_bot_and_tools(
+    return ToolEngine.from_bot_and_tools(
         bot=bot_obj,
         tools=tools,
         callback_manager=callback_manager,
         **kwargs,
     )
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import re
 from typing import Any, List, Optional, Sequence, Tuple
 
-from chatgpt_tool_hub.bots.bot import Bot
 from chatgpt_tool_hub.bots.qa_bot.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
-from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
 from chatgpt_tool_hub.chains import LLMChain
+from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
+from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.engine import Bot
 from chatgpt_tool_hub.models.base import BaseLLM
 from chatgpt_tool_hub.prompts import PromptTemplate
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 FINAL_ANSWER_ACTION = "Final Answer:"
 
 
@@ -28,14 +29,26 @@
         return "Observation: "
 
     @property
     def llm_prefix(self) -> str:
         """Prefix to append the llm call with."""
         return "Thought:"
 
+    def _fix_text(self, text: str) -> str:
+        if not self.allowed_tools:
+            tool_names = ""
+        else:
+            tool_names = ", ".join([tool for tool in self.allowed_tools])
+        instruction_text = FORMAT_INSTRUCTIONS.format(tool_names=tool_names)
+        _text = ("\n\n"
+                 f"You just told me: {text}, but it doesn't meet the format I mentioned to you. \n\n"
+                 f"format: {instruction_text}. \n\n"
+                 "You should understand why you did not input the correct format, correct it and try again. \n\n")
+        return _text
+
     @classmethod
     def create_prompt(
         cls,
         tools: Sequence[BaseTool],
         prefix: str = PREFIX,
         suffix: str = SUFFIX,
         format_instructions: str = FORMAT_INSTRUCTIONS,
@@ -108,12 +121,14 @@
         with "Action Input:" should be separated by a newline.
         """
         if FINAL_ANSWER_ACTION in text:
             return "Final Answer", text.split(FINAL_ANSWER_ACTION)[-1].strip()
         regex = r"Action: (.*?)[\n]*Action Input: (.*)"
         match = re.search(regex, text, re.DOTALL)
         if not match:
-            raise ValueError(f"Could not parse LLM output: `{text}`")
-            # todo 这里可以直接返回
+            return None
+
         action = match.group(1).strip()
         action_input = match.group(2)
+        LOG.info(f"执行Tool: {action}中...")
+
         return action, action_input.strip(" ").strip('"')
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/calculate_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 from chatgpt_tool_hub.common.log import LOG
 
 
 # refer to https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
-def num_tokens_from_messages(messages, model: str = "gpt-3.5-turbo"):
+def count_message_tokens(messages, model: str = "gpt-3.5-turbo"):
     """Returns the number of tokens used by a list of messages."""
     import tiktoken
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         LOG.debug("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
     if model == "gpt-3.5-turbo":
-        return num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301")
+        return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
     elif model == "gpt-4":
-        return num_tokens_from_messages(messages, model="gpt-4-0314")
+        return count_message_tokens(messages, model="gpt-4-0314")
     elif model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         tokens_per_name = -1  # if there's a name, the role is omitted
     elif model == "gpt-4-0314":
         tokens_per_message = 3
         tokens_per_name = 1
     else:
-        LOG.warn(f"num_tokens_from_messages() is not implemented for model {model}. "
+        LOG.warn(f"count_message_tokens() is not implemented for model {model}. "
                  f"Returning num tokens assuming gpt-3.5-turbo-0301.")
-        return num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301")
+        return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
     num_tokens = 0
     for message in messages:
         num_tokens += tokens_per_message
         for key, value in message.items():
             num_tokens += len(encoding.encode(value))
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
+
+
+def count_string_tokens(string: str, model_name: str = "gpt-3.5-turbo") -> int:
+    """
+    Returns the number of tokens in a text string.
+
+    Args:
+    string (str): The text string.
+    model_name (str): The name of the encoding to use. (e.g., "gpt-3.5-turbo")
+
+    Returns:
+    int: The number of tokens in the text string.
+    """
+    import tiktoken
+    encoding = tiktoken.encoding_for_model(model_name)
+    return len(encoding.encode(string))
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/log.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/log.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.models.chatgpt.base import BaseChatModel
 
 
 def _create_retry_decorator(llm: ChatOpenAI) -> Callable[[Any], Any]:
     import openai
 
-    min_seconds = 4
-    max_seconds = 10
+    min_seconds = 15
+    max_seconds = 30
     # Wait 2^x * 1 second between each retry starting with
     # 4 seconds, then up to 10 seconds, then 10 seconds afterwards
     return retry(
         reraise=True,
         stop=stop_after_attempt(llm.max_retries),
         wait=wait_exponential(multiplier=1, min=min_seconds, max=max_seconds),
         retry=(
@@ -201,16 +201,16 @@
             "n": self.n,
             **self.model_kwargs,
         }
 
     def _create_retry_decorator(self) -> Callable[[Any], Any]:
         import openai
 
-        min_seconds = 4
-        max_seconds = 10
+        min_seconds = 15
+        max_seconds = 30
         # Wait 2^x * 1 second between each retry starting with
         # 4 seconds, then up to 10 seconds, then 10 seconds afterwards
         return retry(
             reraise=True,
             stop=stop_after_attempt(self.max_retries),
             wait=wait_exponential(multiplier=1, min=min_seconds, max=max_seconds),
             retry=(
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/model_factory.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/openai.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/models/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,16 @@
         ]
     }
 
 
 def _create_retry_decorator(llm: Union[BaseOpenAI, OpenAIChat]) -> Callable[[Any], Any]:
     import openai
 
-    min_seconds = 4
-    max_seconds = 10
+    min_seconds = 15
+    max_seconds = 30
     # Wait 2^x * 1 second between each retry starting with
     # 4 seconds, then up to 10 seconds, then 10 seconds afterwards
     return retry(
         reraise=True,
         stop=stop_after_attempt(llm.max_retries),
         wait=wait_exponential(multiplier=1, min=min_seconds, max=max_seconds),
         retry=(
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/arxiv_search.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.arxiv_search.wrapper import ArxivAPIWrapper
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 
+default_tool_name = "arxiv"
+
+
 class ArxivTool(BaseTool):
-    """ a tool to call arxiv api: """
+    """ a tool to call arxiv api """
 
-    name = "arxiv"
+    name = default_tool_name
     description = (
         "Useful for when you need to answer questions about scientific research or search for papers "
         "Like: which papers has a certain author published? what are some papers in a specific field? "
         "Input should be a search_query in english. There is not any quotation marks in any search_query"
         
         "In the tool, each paper is divided up into a number of fields that can individually be searched. "
         "A field consists of field prefix, a colon, and search term. Fields can be combined by a boolean operator. "
@@ -28,11 +32,14 @@
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the Arxiv tool asynchronously."""
         raise NotImplementedError("ArxivTool does not support async")
 
 
+main_tool_register.register_tool(default_tool_name, lambda kwargs: ArxivTool(**kwargs), [])
+
+
 if __name__ == "__main__":
     tool = ArxivTool(api_wrapper=ArxivAPIWrapper())
     content = tool.run("au:Adam Coates")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/arxiv_search/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
     arxiv_client: Any
     top_k_results: int = 3
 
     class Config:
         """Configuration for this pydantic object."""
 
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
         try:
             import arxiv
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/base_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Base implementation for tools."""
-
 from abc import abstractmethod
 from typing import Any, Optional
 
 from pydantic import BaseModel, Extra, Field, validator
 
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
 from chatgpt_tool_hub.common.callbacks import get_callback_manager
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/bing_search.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tool for the Bing search API."""
 
-from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.bing_search.wrapper import BingSearchAPIWrapper
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 
+from chatgpt_tool_hub.tools.base_tool import BaseTool
+from chatgpt_tool_hub.tools.bing_search import BingSearchAPIWrapper
 
 default_tool_name = "bing-search"
 
 
 class BingSearch(BaseTool):
     """Tool that adds the capability to query the Bing search API.
 
@@ -28,9 +28,10 @@
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("BingSearch does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: BingSearch(api_wrapper=BingSearchAPIWrapper(**kwargs)),
-              tool_input_keys=["bing_subscription_key"])
+main_tool_register.register_tool(default_tool_name,
+                                 lambda kwargs: BingSearch(api_wrapper=BingSearchAPIWrapper(**kwargs)),
+                                 tool_input_keys=["bing_subscription_key"])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Util that calls Bing Search."""
 import json
 from typing import Dict, List
 
-from pydantic import BaseModel, Extra, root_validator
+from pydantic import BaseModel, Extra, validator, root_validator
 
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.tools.web_requests import filter_text
 from chatgpt_tool_hub.tools.web_requests.wrapper import RequestsWrapper
 
 
@@ -16,25 +16,25 @@
     bing_subscription_key: str
     bing_search_url: str
     top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
 
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     def _bing_search_results(self, search_term: str, count: int) -> List[dict]:
         headers = {"Ocp-Apim-Subscription-Key": self.bing_subscription_key}
         params = {
             "q": search_term,
             "count": count,
             "textDecorations": True,
             "textFormat": "HTML",
         }
-        response = RequestsWrapper(headers=headers).get(self.bing_search_url, params, raise_for_status=True)
+        response = RequestsWrapper(headers=headers).get(self.bing_search_url, params=params, raise_for_status=True)
 
         search_results = json.loads(response)
         try:
             result = search_results["webPages"]["value"]
             LOG.debug("[bing_search] output: " + str(result))
         except Exception as e:
             result = []
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/debug.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/debug/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 
 from pydantic import Field
 
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 default_tool_name = "debug"
 
 
 def _print_func(text: str) -> None:
     print("\n")
@@ -31,8 +31,8 @@
         return self.input_func()
 
     async def _arun(self, query: str) -> str:
         """Use the DebugTool asynchronously."""
         raise NotImplementedError("DebugTool does not support async")
 
 
-register_tool(default_tool_name, lambda _: DebugTool(), [])
+main_tool_register.register_tool(default_tool_name, lambda _: DebugTool(), [])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/google_search.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tool for the Google search API."""
 
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.google_search.wrapper import GoogleSearchAPIWrapper
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
-
 
 default_tool_name = "google-search"
 
+
 class GoogleSearch(BaseTool):
     """Tool that adds the capability to query the Google search API."""
 
     name = default_tool_name
     description = (
         "A wrapper around Google Search. "
         "Useful for when you need to answer questions about current events. "
@@ -43,9 +43,9 @@
         return str(self.api_wrapper.results(query))
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("GoogleSearchRun does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: GoogleSearchJson(api_wrapper=GoogleSearchAPIWrapper(**kwargs)),
+main_tool_register.register_tool(default_tool_name, lambda kwargs: GoogleSearchJson(api_wrapper=GoogleSearchAPIWrapper(**kwargs)),
               tool_input_keys=["google_api_key", "google_cse_id"])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Util that calls Google Search."""
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Extra, root_validator
 
-from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.tools.web_requests import filter_text
 
+
 class GoogleSearchAPIWrapper(BaseModel):
     """Wrapper for Google Search API."""
 
     search_engine: Any
     google_api_key: Optional[str] = None
     google_cse_id: Optional[str] = None
     top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
 
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     def _google_search_results(self, search_term: str, **kwargs: Any) -> List[dict]:
         res = (
             self.search_engine.cse()
             .list(q=search_term, cx=self.google_cse_id, **kwargs)
             .execute()
         )
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/load_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 """Load tools."""
 from typing import Any, List
 from typing import Optional
 
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
 from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.tools.all_tool_list import get_all_tool_dict
 from chatgpt_tool_hub.tools.base_tool import BaseTool
+from chatgpt_tool_hub.tools.tool_register import ToolRegister
 
 
 def load_tools(
     tool_names: List[str],
+    tool_register: ToolRegister,
     callback_manager: Optional[BaseCallbackManager] = None,
     **kwargs: Any,
 ) -> List[BaseTool]:
     """Load tools based on their name.
 
     Args:
         tool_names: name of tools to load.
+        tool_register: the registered object of tools
         callback_manager: Optional callback manager. If not provided, default global callback manager will be used.
     Returns:
         List of tools.
     """
     tools = []
-    all_tool_dict = get_all_tool_dict()
+    all_tool_dict = tool_register.get_registered_tool()
     for name in tool_names:
         if name in all_tool_dict:
             _get_tool_func, extra_keys = all_tool_dict[name]
 
             # consistency validation between input and required params
-            missing_keys = set(extra_keys).difference(kwargs)
-            if missing_keys:
-                raise ValueError(
-                    f"Tool {name} requires some parameters that were not "
-                    f"provided: {missing_keys}"
-                )
-
-            sub_kwargs = {k: kwargs[k] for k in extra_keys if k in kwargs}
-            tool = _get_tool_func(sub_kwargs)
+            try:
+                missing_keys = set(extra_keys).difference(kwargs)
+                if missing_keys:
+                    raise ValueError(
+                        f"Tool {name} requires some parameters that were not "
+                        f"provided: {missing_keys}"
+                    )
+            except Exception as e:
+                LOG.info(f"[{name}] init failed, error_info: {repr(e)}")
+                tool_register.unregister_tool(name)
+                continue
+
+            # todo double check here
+            #
+            try:
+                # sub_kwargs = {k: kwargs[k] for k in extra_keys if k in kwargs}
+                tool = _get_tool_func(kwargs)
+            except Exception as e:
+                LOG.info(f"[{name}] init failed, error_info: {repr(e)}")
+                tool_register.unregister_tool(name)
+                continue
 
             if callback_manager is not None:
                 tool.callback_manager = callback_manager
 
             tools.append(tool)
         else:
-            LOG.error("All the tools currently supported are："+str(list(all_tool_dict)))
+            LOG.error("Now registered tools are："+str(list(all_tool_dict)))
             raise ValueError(f"Got unknown tool: {name}")
     filter_tools = crop_tools(tools)
     return filter_tools
 
 
 def crop_tools(tools: List[BaseTool]) -> List[BaseTool]:
-    if len(tools) > 8:
-        LOG.warning(f"get too many tools, tools after {tools[8].name} will be ignored...")
-        return tools[:8]
+    if len(tools) > 10:
+        LOG.warning(f"loading too many tools, some tools after {tools[10].name} will be ignored...")
+        return tools[:10]
     # todo: 检查description是否超出限制
-    for tool in tools:
-        pass
     return tools
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/docs_prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,13 +50,19 @@
 WMO Weather interpretation codes (WW)
 Code	Description
 0	Clear sky
 1, 2, 3	Mainly clear, partly cloudy, and overcast
 45, 48	Fog and depositing rime fog
 51, 53, 55	Drizzle: Light, moderate, and dense intensity
 56, 57	Freezing Drizzle: Light and dense intensity
+61, 63, 65	Rain: Slight, moderate and heavy intensity
+66, 67	Freezing Rain: Light and heavy intensity
+71, 73, 75	Snow fall: Slight, moderate, and heavy intensity
+77	Snow grains
+80, 81, 82	Rain showers: Slight, moderate, and violent
+85, 86	Snow showers slight and heavy
 
 If daily weather variables are specified, parameter timezone is required.
 Parameter past_days is mutually exclusive with start_date and end_date.
 
 Your output can only be a URL, no need for explanation.
 """
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/meteo_weather.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/meteo/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime
 
 from chatgpt_tool_hub.chains.api import APIChain
 from chatgpt_tool_hub.models import build_model_params
 from chatgpt_tool_hub.models.model_factory import ModelFactory
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
+
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.meteo.api_docs_prompts import OPEN_METEO_DOCS
+from chatgpt_tool_hub.tools.meteo.docs_prompt import OPEN_METEO_DOCS
 
 default_tool_name = "meteo-weather"
 
 
 class MeteoWeatherTool(BaseTool):
     name: str = default_tool_name
     description: str = (
@@ -36,8 +37,8 @@
         return self.api_chain.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("MeteoWeatherTool does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: MeteoWeatherTool(**kwargs), [])
+main_tool_register.register_tool(default_tool_name, lambda kwargs: MeteoWeatherTool(**kwargs), [])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/morning_news.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from typing import Any
 
 from chatgpt_tool_hub.chains import LLMChain
+from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.models import build_model_params
 from chatgpt_tool_hub.models.model_factory import ModelFactory
 from chatgpt_tool_hub.prompts import PromptTemplate
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.morning_news.summary_prompt import SUMMARY_DOCS
+from chatgpt_tool_hub.tools.news import news_tool_register
+from chatgpt_tool_hub.tools.news.morning_news.prompt import SUMMARY_DOCS
 from chatgpt_tool_hub.tools.web_requests.get import RequestsWrapper
-from chatgpt_tool_hub.common.log import LOG
 
 default_tool_name = "morning-news"
 
 
 class MorningNewsTool(BaseTool):
     name: str = default_tool_name
     description: str = (
         "Use this tool when you want to get information about Daily 60 seconds morning news today. "
-        "The input should be a question in natural language that this API can answer."
+        "input is None."
     )
     bot: Any = None
     zaobao_api_key: str = ""
 
     def __init__(self, **tool_kwargs: Any):
         # 这个工具直接返回内容
         super().__init__(return_direct=True)
+
+        self.zaobao_api_key = get_from_dict_or_env(tool_kwargs, "zaobao_api_key", "ZAOBAO_API_KEY")
+
         llm = ModelFactory().create_llm_model(**build_model_params(tool_kwargs))
         prompt = PromptTemplate(
             input_variables=["morning_news"],
             template=SUMMARY_DOCS,
         )
         self.bot = LLMChain(llm=llm, prompt=prompt)
 
-        self.zaobao_api_key = get_from_dict_or_env(tool_kwargs, "zaobao_api_key", "ZAOBAO_API_KEY")
-
     def _run(self, query: str) -> str:
         """Use the tool."""
         if not query:
             return "the input of tool is empty"
 
         morning_news_url = "https://v2.alapi.cn/api/zaobao?token={}&format={}".format(self.zaobao_api_key, "json")
         _response = RequestsWrapper().get(morning_news_url)
@@ -47,15 +48,15 @@
         return _return
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("NewsTool does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: MorningNewsTool(**kwargs), ["zaobao_api_key"])
+news_tool_register.register_tool(default_tool_name, lambda kwargs: MorningNewsTool(**kwargs), ["zaobao_api_key"])
 
 
 if __name__ == "__main__":
     tool = MorningNewsTool(zaobao_api_key="xx")
     content = tool.run("给我发一下早报？")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/summary_prompt.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/morning_news/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/api_docs_prompts.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/docs_prompts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-NEWS_DOCS = """API documentation:
+NEWS_DOCS = """
+API documentation:
 Endpoint: https://newsapi.org
 Top headlines /v2/top-headlines
 
 This endpoint provides live top and breaking headlines for a country, specific category in a country, single source, or multiple sources. You can also search with keywords. Articles are sorted by the earliest date published first.
 
 This endpoint is great for retrieving headlines for use with news tickers or similar.
 Request parameters
@@ -24,8 +25,10 @@
     description | string | A description or snippet from the article.
     url | string | The direct URL to the article.
     urlToImage | string | The URL to a relevant image for the article.
     publishedAt | string | The date and time that the article was published, in UTC (+000)
     content | string | The unformatted content of the article, where available. This is truncated to 200 chars.
 
 Use page size: 2
+The endpoint and prefix of the document are absolutely correct, and that other URL prefixes should not be fabricated.
+the url must not contain apiKey param
 """
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/news.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/news/news_api/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Any
 
 from chatgpt_tool_hub.chains.api import APIChain
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.models import build_model_params
 from chatgpt_tool_hub.models.model_factory import ModelFactory
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.news.api_docs_prompts import NEWS_DOCS
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.news import news_tool_register
+from chatgpt_tool_hub.tools.news.news_api.docs_prompts import NEWS_DOCS
 
+default_tool_name = "news-api"
 
-default_tool_name = "news"
 
-
-class NewsTool(BaseTool):
+class NewsApiTool(BaseTool):
     name: str = default_tool_name
     description: str = (
         "Use this when you want to get information about the top headlines of current news stories. "
         "The input should be a question in natural language that this API can answer."
     )
     api_chain: APIChain = None
 
@@ -41,8 +40,8 @@
         return self.api_chain.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("NewsTool does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: NewsTool(**kwargs), ["news_api_key"])
+news_tool_register.register_tool(default_tool_name, lambda kwargs: NewsApiTool(**kwargs), ["news_api_key"])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/python_repl.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/python/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import sys
 from io import StringIO
 from typing import Dict, Optional
 
 from pydantic import Field, BaseModel
 
 from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
-from chatgpt_tool_hub.tools.base_tool import BaseTool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 
+from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 default_tool_name = "python"
 
 
 class PythonREPL(BaseModel):
     """Simulates a standalone Python REPL."""
 
@@ -60,8 +60,8 @@
         return self.python_repl.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("PythonReplTool does not support async")
 
 
-register_tool(default_tool_name, lambda _: PythonREPLTool(), [])
+main_tool_register.register_tool(default_tool_name, lambda _: PythonREPLTool(), [])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/searxng.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tool for the SearxNG search API."""
 from pydantic import Extra
 
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
+
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.searxng_search.wrapper import SearxSearchWrapper
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
-
 
-default_tool_name =  "searxng-search"
+default_tool_name = "searxng-search"
 
 class SearxSearchTool(BaseTool):
     """Tool that adds the capability to query a Searx instance."""
 
     name = default_tool_name
     description = (
         "A meta search engine."
@@ -39,20 +39,20 @@
     )
     api_wrapper: SearxSearchWrapper
     num_results: int = 4
 
     class Config:
         """Pydantic config."""
 
-        extra = Extra.allow
+        extra = Extra.ignore
 
     def _run(self, query: str) -> str:
         """Use the tool."""
         return str(self.api_wrapper.results(query, self.num_results))
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         return (await self.api_wrapper.aresults(query, self.num_results)).__str__()
 
 
-register_tool(default_tool_name, lambda kwargs: SearxSearchTool(api_wrapper=SearxSearchWrapper(**kwargs)),
+main_tool_register.register_tool(default_tool_name, lambda kwargs: SearxSearchTool(api_wrapper=SearxSearchWrapper(**kwargs)),
               tool_input_keys=["searx_host"])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/searxng_search/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         )
 
         return values
 
     class Config:
         """Configuration for this pydantic object."""
 
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     def _searx_api_query(self, params: dict) -> SearxResults:
         """Actual request to searx API."""
         requests_wrapper = RequestsWrapper(headers=self.headers)
         raw_result = requests_wrapper.get(self.searx_host, params=params,
                                           raise_for_status=True, verify=not self.unsecure)
         # test if http result is ok
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import sys
 import string
 import subprocess
+import sys
 from typing import List, Union
 
 from pydantic import Field
 
-from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 
+from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 default_tool_name = "terminal"
 
 
 class BashProcess:
     """Executes bash commands and returns the output."""
 
@@ -90,15 +90,15 @@
         return output
 
 
 def _get_default_bash_process() -> BashProcess:
     return BashProcess()
 
 
-class Terminal(BaseTool):
+class TerminalTool(BaseTool):
     name = default_tool_name
     description = (
         f"Executes commands in a terminal. Input should be valid commands in {sys.platform} platform, "
         "and the output will be any output from running that command."
         "Don't input any backquote to this tool."
     )
 
@@ -109,14 +109,14 @@
         return self.bash_process.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("[Terminal] does not support async")
 
 
-register_tool(default_tool_name, lambda _: Terminal(), [])
+main_tool_register.register_tool(default_tool_name, lambda _: TerminalTool(), [])
 
 
 if __name__ == "__main__":
     bash = BashProcess()
     content = bash.run("`poweroff; sudo ls -l; pwd`")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/text2image.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/visual_dl/text2image.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import torch
 from PIL import Image
 from transformers import BlipProcessor, BlipForConditionalGeneration
 
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
+
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 default_tool_name = "image2text"
 
 
 class ImageCaptionTool(BaseTool):
     """Tool for get image captioning from image_path or url"""
@@ -42,14 +43,14 @@
         return captions
 
     def _arun(self, query: str) -> str:
         """Use the ImageCaptioningTool asynchronously."""
         raise NotImplementedError("ImageCaptioningTool does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: ImageCaptionTool(**kwargs), [])
+main_tool_register.register_tool(default_tool_name, lambda kwargs: ImageCaptionTool(**kwargs), [])
 
 
 if __name__ == "__main__":
     tool = ImageCaptionTool()
     content = tool.run("/Users/goldfish/PycharmProjects/chatgpt-tool-hub/chatgpt_tool_hub/demo2.jpg")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Tools for making requests to an API endpoint."""
 import json
+import os
+import tempfile
 from typing import Any, Dict
 
 from bs4 import BeautifulSoup
 from pydantic import BaseModel
 
+from chatgpt_tool_hub.tools import SummaryTool
+
 
 def filter_text(html: str) -> str:
     soup = BeautifulSoup(html, "lxml")
     # kill all script and style elements
     for script in soup(["script", "style"]):
         script.extract()
 
@@ -17,28 +21,35 @@
 
     # break into lines and remove leading and trailing space on each
     lines = (line.strip() for line in text.splitlines())
     # break multi-headlines into a line each
     chunks = (phrase.strip() for line in lines for phrase in line.split("  "))
     # drop blank lines
     text = '\n'.join(chunk for chunk in chunks if chunk)
+
     # compress text size
-    # todo gpt-index
-    text = text[:500]
+    temp_file = tempfile.mkstemp()
+    file_path = temp_file[1]
 
-    return text.encode('utf-8').decode()
+    with open(file_path, "w") as f:
+        f.write(text + "\n")
+    _summary = SummaryTool().run(str(file_path) + ", 0")
+    os.remove(file_path)
+
+    return _summary.encode('utf-8').decode()
 
 
 def _parse_input(text: str) -> Dict[str, Any]:
     """Parse the json string into a dict."""
     return json.loads(text)
 
 
 DEFAULT_HEADER = {
-    'User-Agent': "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.100 Safari/537.36",
+    'User-Agent': "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) "
+                  "Chrome/54.0.2840.100 Safari/537.36",
     "Accept-Encoding": "*"
 }
 
 from chatgpt_tool_hub.tools.web_requests.wrapper import RequestsWrapper
 
 
 class BaseRequestsTool(BaseModel):
@@ -50,15 +61,17 @@
 from chatgpt_tool_hub.tools.web_requests.browser import BrowserTool
 from chatgpt_tool_hub.tools.web_requests.delete import RequestsDeleteTool
 from chatgpt_tool_hub.tools.web_requests.get import RequestsGetTool
 from chatgpt_tool_hub.tools.web_requests.patch import RequestsPatchTool
 from chatgpt_tool_hub.tools.web_requests.post import RequestsPostTool
 from chatgpt_tool_hub.tools.web_requests.put import RequestsPutTool
 
+
 __all__ = (
+    "BrowserTool",
     "BaseRequestsTool",
     "RequestsWrapper",
     "RequestsDeleteTool",
     "RequestsGetTool",
     "RequestsPatchTool",
     "RequestsPostTool",
     "RequestsPutTool"
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-import logging
-
-from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool, filter_text, RequestsWrapper
+from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool, _parse_input
 
 
-class BrowserTool(BaseRequestsTool, BaseTool):
-    """Tool for making a GET request to an API endpoint."""
+class RequestsPatchTool(BaseRequestsTool, BaseTool):
+    """Tool for making a PATCH request to an API endpoint."""
 
-    name = "Web browser"
-    # todo: browser prompt should update later
-    description = "A portal to the internet. Use this when you need to get specific content from a website. Input " \
-                  "should be a  url (i.e. https://www.google.com). The output will be the text response of the GET " \
-                  "request."
+    name = "requests_patch"
+    description = """Use this when you want to PATCH to a website.
+    Input should be a json string with two keys: "url" and "data".
+    The value of "url" should be a string, and the value of "data" should be a dictionary of 
+    key-value pairs you want to PATCH to the url.
+    Be careful to always use double quotes for strings in the json string
+    The output will be the text response of the PATCH request.
+    """
 
-    def _run(self, url: str) -> str:
+    def _run(self, text: str) -> str:
         """Run the tool."""
         try:
-            html = self.requests_wrapper.get(url)
-            _content = filter_text(html)
-            LOG.debug("[browser] output: " + str(_content))
+            data = _parse_input(text)
+            return self.requests_wrapper.patch(data["url"], data["data"])
         except Exception as e:
-            LOG.error("[browser] " + str(e))
-            _content = repr(e)
-        return _content
+            return repr(e)
 
-    async def _arun(self, url: str) -> str:
+    async def _arun(self, text: str) -> str:
         """Run the tool asynchronously."""
-        raise NotImplementedError("not support run this tool in async")
-
-
-if __name__ == "__main__":
-    LOG.setLevel(logging.DEBUG)
-    requests_wrapper = RequestsWrapper()
-    tool = BrowserTool(requests_wrapper=requests_wrapper)
+        try:
+            data = _parse_input(text)
+            return await self.requests_wrapper.apatch(data["url"], data["data"])
+        except Exception as e:
+            return repr(e)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool
 
 
 class RequestsDeleteTool(BaseRequestsTool, BaseTool):
     """Tool for making a DELETE request to an API endpoint."""
 
     name = "requests_delete"
-    description = "A portal to the internet. Use this when you need to make a DELETE request to a URL. Input should " \
-                  "be a specific url, and the output will be the text response of the DELETE request."
+    description = (
+        "A portal to the internet. Use this when you need to make a DELETE request to a URL. Input should "
+        "be a specific url, and the output will be the text response of the DELETE request."
+    )
 
     def _run(self, url: str) -> str:
         """Run the tool."""
         return self.requests_wrapper.delete(url)
 
     async def _arun(self, url: str) -> str:
         """Run the tool asynchronously."""
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/get.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 
 from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool, filter_text, RequestsWrapper
 
-
 default_tool_name = "url-get"
 
 
 class RequestsGetTool(BaseRequestsTool, BaseTool):
     """Tool for making a GET request to an API endpoint."""
 
     name = default_tool_name
-    description = "A portal to the internet. Use this when you need to get specific content from a website. Input " \
-                  "should be a  url (i.e. https://www.google.com). The output will be the text response of the GET " \
-                  "request."
+    description = (
+        "A portal to the internet. Use this when you need to get specific content from a website. "
+        "Input should be a url (i.e. https://www.google.com). "
+        "The output will be the text response of the GET request."
+    )
 
     def _run(self, url: str) -> str:
         """Run the tool."""
         try:
             html = self.requests_wrapper.get(url)
             _content = filter_text(html)
             LOG.debug("[url-get] output: " + str(_content))
@@ -36,15 +37,15 @@
             LOG.debug("[url-get] output: " + str(_content))
         except Exception as e:
             LOG.error("[url-get] " + str(e))
             _content = repr(e)
         return _content
 
 
-register_tool(default_tool_name, lambda _: RequestsGetTool(requests_wrapper=RequestsWrapper()), [])
+main_tool_register.register_tool(default_tool_name, lambda _: RequestsGetTool(requests_wrapper=RequestsWrapper()), [])
 
 
 if __name__ == "__main__":
     LOG.setLevel(logging.DEBUG)
     requests_wrapper = RequestsWrapper()
     tool = RequestsGetTool(requests_wrapper=requests_wrapper)
     content = tool.run("https://github.com/goldfishh/chatgpt-tool-hub")
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,56 @@
+import json
+import logging
+
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool, _parse_input
+from chatgpt_tool_hub.tools.web_requests import BaseRequestsTool, _parse_input, RequestsWrapper
+from chatgpt_tool_hub.common.log import LOG
 
 
-class RequestsPatchTool(BaseRequestsTool, BaseTool):
-    """Tool for making a PATCH request to an API endpoint."""
+class RequestsPostTool(BaseRequestsTool, BaseTool):
+    """Tool for making a POST request to an API endpoint."""
 
-    name = "requests_patch"
-    description = """Use this when you want to PATCH to a website.
+    name = "requests_post"
+    description = """Use this when you want to POST to a website.
     Input should be a json string with two keys: "url" and "data".
     The value of "url" should be a string, and the value of "data" should be a dictionary of 
-    key-value pairs you want to PATCH to the url.
+    key-value pairs you want to POST to the url.
     Be careful to always use double quotes for strings in the json string
-    The output will be the text response of the PATCH request.
+    The output will be the text response of the POST request.
     """
 
     def _run(self, text: str) -> str:
         """Run the tool."""
         try:
-            data = _parse_input(text)
-            return self.requests_wrapper.patch(data["url"], data["data"])
+            _data = _parse_input(text)
+            _content = self.requests_wrapper.post(_data["url"], _data["data"])
+            LOG.debug(("[requests_post] output: " + str(_content)))
+            return _content
         except Exception as e:
+            LOG.error("[requests_post] " + str(e))
             return repr(e)
 
     async def _arun(self, text: str) -> str:
         """Run the tool asynchronously."""
         try:
-            data = _parse_input(text)
-            return await self.requests_wrapper.apatch(data["url"], data["data"])
+            _data = _parse_input(text)
+            _content = await self.requests_wrapper.apost(_data["url"], _data["data"])
+            LOG.debug(("[requests_post] output: " + str(_content)))
+            return _content
         except Exception as e:
+            LOG.error("[requests_post] " + str(e))
             return repr(e)
+
+
+if __name__ == "__main__":
+    LOG.setLevel(logging.DEBUG)
+    requests_wrapper = RequestsWrapper()
+    url = "https://api.live.bilibili.com/xlive/web-room/v1/dM/gethistory"
+    data = {
+        "roomid": 10661147,
+        "csrf_token": "",
+        "csrf": "",
+        "visit_id": "",
+    }
+    tool = RequestsPostTool(requests_wrapper=requests_wrapper)
+    content = tool.run(json.dumps({"url": url, "data": data}))
+    print(content)
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tool for the Wikipedia API."""
 
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.wikipedia.wrapper import WikipediaAPIWrapper
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
-
 
 default_tool_name = "wikipedia"
 
+
 class WikipediaTool(BaseTool):
     """Tool that adds the capability to search using the Wikipedia API."""
 
     name = default_tool_name
     description = (
         "Useful for when you need to answer general questions about "
         "people, places, companies, historical events, or other subjects. "
@@ -23,8 +23,8 @@
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the Wikipedia tool asynchronously."""
         raise NotImplementedError("WikipediaQueryRun does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: WikipediaTool(api_wrapper=WikipediaAPIWrapper(**kwargs)), [])
+main_tool_register.register_tool(default_tool_name, lambda kwargs: WikipediaTool(api_wrapper=WikipediaAPIWrapper(**kwargs)), [])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
 
     wiki_client: Any  #: :meta private:
     top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
         try:
             import wikipedia
             # 本土化
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tool for the Wolfram Alpha API."""
 
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.wolfram_alpha.wrapper import WolframAlphaAPIWrapper
-from chatgpt_tool_hub.tools.all_tool_list import register_tool
+from chatgpt_tool_hub.tools.all_tool_list import main_tool_register
+
 
 
 default_tool_name = "wolfram-alpha"
 
 class WolframAlphaTool(BaseTool):
     """Tool that adds the capability to query using the Wolfram Alpha SDK."""
 
@@ -24,9 +25,9 @@
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the WolframAlpha tool asynchronously."""
         raise NotImplementedError("WolframAlphaTool does not support async")
 
 
-register_tool(default_tool_name, lambda kwargs: WolframAlphaTool(api_wrapper=WolframAlphaAPIWrapper(**kwargs)),
+main_tool_register.register_tool(default_tool_name, lambda kwargs: WolframAlphaTool(api_wrapper=WolframAlphaAPIWrapper(**kwargs)),
               tool_input_keys=["wolfram_alpha_appid"])
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     wolfram_client: Any  #: :meta private:
     wolfram_alpha_appid: Optional[str] = None
 
     class Config:
         """Configuration for this pydantic object."""
 
-        extra = Extra.forbid
+        extra = Extra.ignore
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         wolfram_alpha_appid = get_from_dict_or_env(
             values, "wolfram_alpha_appid", "WOLFRAM_ALPHA_APPID"
         )
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.3.9
+Version: 0.4.1
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -95,15 +95,15 @@
       "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
       "no_default": false,  // 控制是否加载默认工具
       "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
   }
 }
 ```
 
-#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+#### (4). `python3 test.py 你的问题1 [你的问题2 ......]`
 
 > chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
 
 #### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
 
 --- 
 
@@ -119,19 +119,19 @@
 
 `pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
 
 #### (2). 示例代码：
 
 ```python
 import os
-from chatgpt_tool_hub.apps import load_app
-os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
-os.environ["PROXY"] = "http://192.168.7.1:7890"
-app = load_app()
-reply = app.ask(YOUR_QUESTION_TO_HERE)
+from chatgpt_tool_hub.apps import AppFactory
+os.environ["OPENAI_API_KEY"] = "YOUR_OPENAI_API_KEY"
+os.environ["PROXY"] = "YOUR_PROXY_ADDRESS"
+app = AppFactory().create_app()
+reply = app.ask("YOUR_QUESTION_TO_HERE")
 print(reply)
 ```
   
 > 如果有需求，我会更新接入的文档，欢迎提issue
 
 ---
```

### Comparing `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.4.1/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 chatgpt_tool_hub/version.py
 chatgpt_tool_hub.egg-info/PKG-INFO
 chatgpt_tool_hub.egg-info/SOURCES.txt
 chatgpt_tool_hub.egg-info/dependency_links.txt
 chatgpt_tool_hub.egg-info/requires.txt
 chatgpt_tool_hub.egg-info/top_level.txt
 chatgpt_tool_hub/apps/__init__.py
-chatgpt_tool_hub/apps/all_app_list.py
 chatgpt_tool_hub/apps/app.py
 chatgpt_tool_hub/apps/app_factory.py
+chatgpt_tool_hub/apps/auto_app.py
 chatgpt_tool_hub/apps/lite_app.py
-chatgpt_tool_hub/apps/load_app.py
 chatgpt_tool_hub/apps/victorinox.py
 chatgpt_tool_hub/bots/__init__.py
 chatgpt_tool_hub/bots/all_bot_list.py
-chatgpt_tool_hub/bots/bot.py
-chatgpt_tool_hub/bots/bot_executor.py
 chatgpt_tool_hub/bots/initialize.py
 chatgpt_tool_hub/bots/chat_bot/__init__.py
 chatgpt_tool_hub/bots/chat_bot/base.py
 chatgpt_tool_hub/bots/chat_bot/prompt.py
 chatgpt_tool_hub/bots/qa_bot/__init__.py
 chatgpt_tool_hub/bots/qa_bot/base.py
 chatgpt_tool_hub/bots/qa_bot/prompt.py
@@ -32,27 +29,31 @@
 chatgpt_tool_hub/chains/api/__init__.py
 chatgpt_tool_hub/chains/api/base.py
 chatgpt_tool_hub/chains/api/prompt.py
 chatgpt_tool_hub/common/__init__.py
 chatgpt_tool_hub/common/cache.py
 chatgpt_tool_hub/common/calculate_token.py
 chatgpt_tool_hub/common/callbacks.py
+chatgpt_tool_hub/common/config.py
 chatgpt_tool_hub/common/constants.py
 chatgpt_tool_hub/common/document.py
 chatgpt_tool_hub/common/formatting.py
 chatgpt_tool_hub/common/input.py
 chatgpt_tool_hub/common/log.py
 chatgpt_tool_hub/common/schema.py
 chatgpt_tool_hub/common/singleton.py
 chatgpt_tool_hub/common/text_splitter.py
 chatgpt_tool_hub/common/utils.py
 chatgpt_tool_hub/database/__init__.py
 chatgpt_tool_hub/database/chat_memory.py
 chatgpt_tool_hub/database/token_buffer.py
 chatgpt_tool_hub/database/utils.py
+chatgpt_tool_hub/engine/__init__.py
+chatgpt_tool_hub/engine/bot.py
+chatgpt_tool_hub/engine/tool_engine.py
 chatgpt_tool_hub/models/__init__.py
 chatgpt_tool_hub/models/base.py
 chatgpt_tool_hub/models/model_factory.py
 chatgpt_tool_hub/models/openai.py
 chatgpt_tool_hub/models/chatgpt/__init__.py
 chatgpt_tool_hub/models/chatgpt/base.py
 chatgpt_tool_hub/models/chatgpt/chatgpt.py
@@ -61,39 +62,48 @@
 chatgpt_tool_hub/prompts/chat.py
 chatgpt_tool_hub/prompts/prompt.py
 chatgpt_tool_hub/tools/__init__.py
 chatgpt_tool_hub/tools/all_tool_list.py
 chatgpt_tool_hub/tools/base_tool.py
 chatgpt_tool_hub/tools/load_tools.py
 chatgpt_tool_hub/tools/tool.py
+chatgpt_tool_hub/tools/tool_register.py
 chatgpt_tool_hub/tools/arxiv_search/__init__.py
-chatgpt_tool_hub/tools/arxiv_search/arxiv_search.py
+chatgpt_tool_hub/tools/arxiv_search/tool.py
 chatgpt_tool_hub/tools/arxiv_search/wrapper.py
 chatgpt_tool_hub/tools/bing_search/__init__.py
-chatgpt_tool_hub/tools/bing_search/bing_search.py
+chatgpt_tool_hub/tools/bing_search/tool.py
 chatgpt_tool_hub/tools/bing_search/wrapper.py
 chatgpt_tool_hub/tools/debug/__init__.py
-chatgpt_tool_hub/tools/debug/debug.py
+chatgpt_tool_hub/tools/debug/tool.py
 chatgpt_tool_hub/tools/google_search/__init__.py
-chatgpt_tool_hub/tools/google_search/google_search.py
+chatgpt_tool_hub/tools/google_search/tool.py
 chatgpt_tool_hub/tools/google_search/wrapper.py
 chatgpt_tool_hub/tools/meteo/__init__.py
-chatgpt_tool_hub/tools/meteo/api_docs_prompts.py
-chatgpt_tool_hub/tools/meteo/meteo_weather.py
-chatgpt_tool_hub/tools/morning_news/__init__.py
-chatgpt_tool_hub/tools/morning_news/morning_news.py
-chatgpt_tool_hub/tools/morning_news/summary_prompt.py
+chatgpt_tool_hub/tools/meteo/docs_prompt.py
+chatgpt_tool_hub/tools/meteo/tool.py
 chatgpt_tool_hub/tools/news/__init__.py
-chatgpt_tool_hub/tools/news/api_docs_prompts.py
-chatgpt_tool_hub/tools/news/news.py
+chatgpt_tool_hub/tools/news/tool.py
+chatgpt_tool_hub/tools/news/finance_news/__init__.py
+chatgpt_tool_hub/tools/news/finance_news/tool.py
+chatgpt_tool_hub/tools/news/morning_news/__init__.py
+chatgpt_tool_hub/tools/news/morning_news/prompt.py
+chatgpt_tool_hub/tools/news/morning_news/tool.py
+chatgpt_tool_hub/tools/news/news_api/__init__.py
+chatgpt_tool_hub/tools/news/news_api/docs_prompts.py
+chatgpt_tool_hub/tools/news/news_api/tool.py
 chatgpt_tool_hub/tools/python/__init__.py
-chatgpt_tool_hub/tools/python/python_repl.py
+chatgpt_tool_hub/tools/python/tool.py
 chatgpt_tool_hub/tools/searxng_search/__init__.py
-chatgpt_tool_hub/tools/searxng_search/searxng.py
+chatgpt_tool_hub/tools/searxng_search/tool.py
 chatgpt_tool_hub/tools/searxng_search/wrapper.py
+chatgpt_tool_hub/tools/summary/__init__.py
+chatgpt_tool_hub/tools/summary/map_prompt.py
+chatgpt_tool_hub/tools/summary/reduce_prompt.py
+chatgpt_tool_hub/tools/summary/tool.py
 chatgpt_tool_hub/tools/terminal/__init__.py
 chatgpt_tool_hub/tools/terminal/base.py
 chatgpt_tool_hub/tools/visual_dl/__init__.py
 chatgpt_tool_hub/tools/visual_dl/text2image.py
 chatgpt_tool_hub/tools/web_requests/__init__.py
 chatgpt_tool_hub/tools/web_requests/browser.py
 chatgpt_tool_hub/tools/web_requests/delete.py
```

### Comparing `chatgpt-tool-hub-0.3.9/setup.py` & `chatgpt-tool-hub-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         "arxiv",
         "wikipedia",
         "wolframalpha",
         'aiohttp~=3.8.4',
         'requests~=2.28.2',
         "google-api-python-client",
         "SQLAlchemy~=2.0.7",
+        "selenium",
+        "webdriver_manager",
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

