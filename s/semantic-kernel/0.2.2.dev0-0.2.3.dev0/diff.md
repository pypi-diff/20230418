# Comparing `tmp/semantic_kernel-0.2.2.dev0.tar.gz` & `tmp/semantic_kernel-0.2.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.2.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.3.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.2.dev0.tar` & `semantic_kernel-0.2.3.dev0.tar`

### file list

```diff
@@ -1,87 +1,86 @@
--rw-r--r--   0        0        0     3551 2023-04-12 23:56:31.410821 semantic_kernel-0.2.2.dev0/README.md
--rw-r--r--   0        0        0      632 2023-04-13 16:54:30.911515 semantic_kernel-0.2.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     1571 2023-04-12 22:05:31.580912 semantic_kernel-0.2.2.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-12 22:05:31.581386 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/ai_exception.py
--rw-r--r--   0        0        0      495 2023-04-12 22:05:31.582034 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-12 22:05:31.582752 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-12 22:05:31.583090 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-12 22:05:31.583566 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      479 2023-04-12 22:05:31.584661 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
--rw-r--r--   0        0        0      817 2023-04-12 22:05:31.585246 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-12 22:05:31.585643 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2763 2023-04-12 22:05:31.586104 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2758 2023-04-12 22:05:31.586442 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4007 2023-04-12 22:05:31.586811 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4441 2023-04-12 22:05:31.587200 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2427 2023-04-12 22:05:31.587604 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      476 2023-04-12 22:05:31.588583 semantic_kernel-0.2.2.dev0/semantic_kernel/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      383 2023-04-12 22:05:31.589728 semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-12 22:05:31.590356 semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     4641 2023-04-12 22:05:31.590848 semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-12 22:05:31.591221 semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5613 2023-04-12 22:05:31.591873 semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    10609 2023-04-12 22:05:31.592352 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2342 2023-04-12 22:05:31.593121 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     3097 2023-04-12 22:05:31.593480 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_builder.py
--rw-r--r--   0        0        0     9134 2023-04-12 22:05:31.593857 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-12 22:05:31.594188 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-12 22:05:31.594647 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-12 22:05:31.595234 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     2374 2023-04-12 22:05:31.595685 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-12 22:05:31.596036 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1531 2023-04-12 22:05:31.596386 semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-12 22:05:31.596719 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-12 22:05:31.597744 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     1598 2023-04-12 22:05:31.598322 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0      299 2023-04-12 22:05:31.598702 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-12 22:05:31.599652 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     2499 2023-04-12 22:05:31.600010 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1237 2023-04-12 22:05:31.600857 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0      836 2023-04-12 22:05:31.601236 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/data_entry.py
--rw-r--r--   0        0        0      953 2023-04-12 22:05:31.601585 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/data_store_base.py
--rw-r--r--   0        0        0     1989 2023-04-12 22:05:31.601968 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/volatile_data_store.py
--rw-r--r--   0        0        0     4050 2023-04-12 22:05:31.602694 semantic_kernel-0.2.2.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2328 2023-04-12 22:05:31.603066 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-12 22:05:31.603429 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-12 22:05:31.603972 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-12 22:05:31.604867 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7322 2023-04-12 22:05:31.605267 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16307 2023-04-12 22:51:26.861573 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6960 2023-04-12 22:05:31.605974 semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-12 22:05:31.606846 semantic_kernel-0.2.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-12 22:05:31.607654 semantic_kernel-0.2.2.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-12 22:05:31.608084 semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-12 22:05:31.608393 semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-12 22:05:31.609233 semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4125 2023-04-13 16:37:57.288016 semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-12 22:05:31.609791 semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-12 22:05:31.610905 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-12 22:05:31.611255 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-12 22:05:31.612110 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-12 22:05:31.612544 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-12 22:05:31.612960 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-12 22:05:31.613397 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-12 22:05:31.613912 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-12 22:05:31.615521 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-12 22:05:31.615999 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-12 22:05:31.616402 semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-12 22:05:31.616773 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-12 22:05:31.617051 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-12 22:05:31.617307 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4566 2023-04-12 22:05:31.617596 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-12 22:05:31.617846 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-12 22:05:31.618137 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-12 22:05:31.618371 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-12 22:05:31.618768 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-12 22:05:31.619109 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-12 22:05:31.619489 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-12 22:05:31.619840 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-12 22:05:31.620223 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-12 22:05:31.620505 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-12 22:05:31.620825 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-12 22:05:31.621394 semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      403 2023-04-12 22:05:31.622359 semantic_kernel-0.2.2.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-12 22:05:31.622736 semantic_kernel-0.2.2.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-12 22:05:31.623641 semantic_kernel-0.2.2.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-12 22:05:31.623896 semantic_kernel-0.2.2.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 semantic_kernel-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0      663 2023-04-17 21:24:30.416680 semantic_kernel-0.2.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     4569 2023-04-17 21:24:30.414681 semantic_kernel-0.2.3.dev0/README.md
+-rw-r--r--   0        0        0     1302 2023-04-17 21:24:30.417680 semantic_kernel-0.2.3.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/ai_exception.py
+-rw-r--r--   0        0        0      495 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-17 21:24:30.418680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-17 21:24:30.419680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-17 21:24:30.419680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      479 2023-04-17 21:24:30.420680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
+-rw-r--r--   0        0        0      817 2023-04-17 21:24:30.420680 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2771 2023-04-17 21:24:30.421681 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2763 2023-04-17 21:24:30.422187 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2758 2023-04-17 21:24:30.422187 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4007 2023-04-17 21:24:30.423196 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4441 2023-04-17 21:24:30.424202 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2427 2023-04-17 21:24:30.424202 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      476 2023-04-17 21:24:30.425203 semantic_kernel-0.2.3.dev0/semantic_kernel/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      383 2023-04-17 21:24:30.425203 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-17 21:24:30.426203 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-17 21:24:30.427205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-17 21:24:30.428205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5613 2023-04-17 21:24:30.428205 semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    11351 2023-04-17 21:24:30.429204 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2342 2023-04-17 21:24:30.429204 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     9134 2023-04-17 21:24:30.430322 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-17 21:24:30.430322 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-17 21:24:30.431831 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-17 21:24:30.432872 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     2374 2023-04-17 21:24:30.432872 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-17 21:24:30.433873 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1531 2023-04-17 21:24:30.433873 semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-17 21:24:30.434874 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-17 21:24:30.435885 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     1598 2023-04-17 21:24:30.435885 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0      299 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     2499 2023-04-17 21:24:30.437008 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1237 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0      836 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_entry.py
+-rw-r--r--   0        0        0      953 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_store_base.py
+-rw-r--r--   0        0        0     1989 2023-04-17 21:24:30.438370 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/volatile_data_store.py
+-rw-r--r--   0        0        0     4050 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2328 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-17 21:24:30.439653 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-17 21:24:30.440988 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16307 2023-04-17 21:24:30.441995 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6960 2023-04-17 21:24:30.441995 semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-17 21:24:30.443431 semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-17 21:24:30.443431 semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-17 21:24:30.444515 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-17 21:24:30.445527 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-17 21:24:30.445527 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-17 21:24:30.446537 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-17 21:24:30.446537 semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-17 21:24:30.447927 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-17 21:24:30.447927 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-17 21:24:30.448939 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-17 21:24:30.448939 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-17 21:24:30.449936 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-17 21:24:30.449936 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-17 21:24:30.451019 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-17 21:24:30.451526 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-17 21:24:30.451526 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-17 21:24:30.452719 semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0      830 2023-04-17 21:24:30.453727 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-17 21:24:30.453727 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4566 2023-04-17 21:24:30.454753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-17 21:24:30.455752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-17 21:24:30.455752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-17 21:24:30.456753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-17 21:24:30.456753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-17 21:24:30.457753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-17 21:24:30.457753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-17 21:24:30.458753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-17 21:24:30.458753 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-17 21:24:30.459752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-17 21:24:30.459752 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     1115 2023-04-17 21:24:30.452719 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0     7637 2023-04-17 21:24:30.460755 semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      403 2023-04-17 21:24:30.460755 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-17 21:24:30.461753 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-17 21:24:30.461753 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-17 21:24:30.462995 semantic_kernel-0.2.3.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 semantic_kernel-0.2.3.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.2.dev0/pyproject.toml` & `semantic_kernel-0.2.3.dev0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.2.dev"
+version = "0.2.3.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -20,10 +20,13 @@
 pytest = "7.2.0"
 ruff = "^0.0.257"
 pytest-asyncio = "^0.21.0"
 
 [tool.isort]
 profile = "black"
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel import core_skills, memory
 from semantic_kernel.kernel import Kernel
-from semantic_kernel.kernel_builder import KernelBuilder
 from semantic_kernel.kernel_config import KernelConfig
-from semantic_kernel.memory.null_memory import NullMemory
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.semantic_functions.chat_prompt_template import ChatPromptTemplate
 from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
 from semantic_kernel.semantic_functions.prompt_template_config import (
     PromptTemplateConfig,
@@ -18,25 +16,18 @@
 )
 from semantic_kernel.utils.null_logger import NullLogger
 from semantic_kernel.utils.settings import (
     azure_openai_settings_from_dot_env,
     openai_settings_from_dot_env,
 )
 
-
-def create_kernel() -> Kernel:
-    return KernelBuilder.create_kernel()
-
-
-def kernel_builder() -> KernelBuilder:
-    return KernelBuilder(KernelConfig(), NullMemory(), NullLogger())
-
-
 __all__ = [
-    "create_kernel",
+    "Kernel",
+    "KernelConfig",
+    "NullLogger",
     "openai_settings_from_dot_env",
     "azure_openai_settings_from_dot_env",
     "PromptTemplateConfig",
     "PromptTemplate",
     "ChatPromptTemplate",
     "SemanticFunctionConfig",
     "ContextVariables",
```

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/ai_exception.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/chat_request_settings.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/complete_request_settings.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/__init__.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,53 +9,63 @@
 from semantic_kernel.ai.chat_request_settings import ChatRequestSettings
 from semantic_kernel.ai.complete_request_settings import CompleteRequestSettings
 from semantic_kernel.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.kernel_base import KernelBase
 from semantic_kernel.kernel_config import KernelConfig
 from semantic_kernel.kernel_exception import KernelException
 from semantic_kernel.kernel_extensions import KernelExtensions
+from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.memory.null_memory import NullMemory
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function import SKFunction
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
 from semantic_kernel.skill_definition.skill_collection import SkillCollection
 from semantic_kernel.skill_definition.skill_collection_base import SkillCollectionBase
+from semantic_kernel.template_engine.prompt_template_engine import PromptTemplateEngine
 from semantic_kernel.template_engine.protocols.prompt_templating_engine import (
     PromptTemplatingEngine,
 )
+from semantic_kernel.utils.null_logger import NullLogger
 from semantic_kernel.utils.validation import validate_function_name, validate_skill_name
 
 
 class Kernel(KernelBase, KernelExtensions):
     _log: Logger
     _config: KernelConfig
     _skill_collection: SkillCollectionBase
     _prompt_template_engine: PromptTemplatingEngine
     _memory: SemanticTextMemoryBase
 
     def __init__(
         self,
-        skill_collection: SkillCollectionBase,
-        prompt_template_engine: PromptTemplatingEngine,
-        memory: SemanticTextMemoryBase,
-        config: KernelConfig,
-        log: Logger,
+        skill_collection: Optional[SkillCollectionBase] = None,
+        prompt_template_engine: Optional[PromptTemplatingEngine] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
+        config: Optional[KernelConfig] = None,
+        log: Optional[Logger] = None,
     ) -> None:
-        self._log = log
-        self._config = config
-        self._skill_collection = skill_collection
-        self._prompt_template_engine = prompt_template_engine
-        self._memory = memory
+        self._log = log if log else NullLogger()
+        self._config = config if config else KernelConfig()
+        self._skill_collection = (
+            skill_collection if skill_collection else SkillCollection(self._log)
+        )
+        self._prompt_template_engine = (
+            prompt_template_engine
+            if prompt_template_engine
+            else PromptTemplateEngine(self._log)
+        )
+        self._memory = memory if memory else NullMemory()
 
     def kernel(self) -> KernelBase:
         return self
 
     @property
     def config(self) -> KernelConfig:
         return self._config
@@ -154,14 +164,17 @@
             return self.skills.get_native_function(skill_name, function_name)
 
         return self.skills.get_semantic_function(skill_name, function_name)
 
     def register_memory(self, memory: SemanticTextMemoryBase) -> None:
         self._memory = memory
 
+    def register_memory_store(self, memory_store: MemoryStoreBase) -> None:
+        self.use_memory(memory_store)
+
     def create_new_context(self) -> SKContext:
         return SKContext(
             ContextVariables(),
             self._memory,
             self.skills,
             self._log,
         )
```

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/data_entry.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_entry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/data_store_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/data_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/storage/volatile_data_store.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/storage/volatile_data_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,21 @@
         Read only skills collection.
 
         Returns:
             ReadOnlySkillCollectionBase -- The skills collection.
         """
         return self._skill_collection
 
+    @skills.setter
+    def skills(self, value: ReadOnlySkillCollectionBase) -> None:
+        """
+        Set the value of skills collection
+        """
+        self._skill_collection = value
+
     @property
     def log(self) -> Logger:
         """
         The logger.
 
         Returns:
             Logger -- The logger.
```

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,27 +56,33 @@
 
         # Some skills may not have input parameters defined
         config.input = PromptTemplateConfig.InputConfig()
         config.input.parameters = []
         if data.get("input") is not None:
             for parameter in data["input"]["parameters"]:
                 if "name" in parameter:
-                    name=parameter["name"]
+                    name = parameter["name"]
                 else:
-                    raise Exception(f"The input parameter doesn't have a name (function: {config.description})")
+                    raise Exception(
+                        f"The input parameter doesn't have a name (function: {config.description})"
+                    )
 
                 if "description" in parameter:
-                    description=parameter["description"]
+                    description = parameter["description"]
                 else:
-                    raise Exception(f"Input parameter '{name}' doesn't have a description (function: {config.description})")
+                    raise Exception(
+                        f"Input parameter '{name}' doesn't have a description (function: {config.description})"
+                    )
 
                 if "defaultValue" in parameter:
-                    defaultValue=parameter["defaultValue"]
+                    defaultValue = parameter["defaultValue"]
                 else:
-                    raise Exception(f"Input parameter '{name}' doesn't have a default value (function: {config.description})")
+                    raise Exception(
+                        f"Input parameter '{name}' doesn't have a default value (function: {config.description})"
+                    )
 
                 config.input.parameters.append(
                     PromptTemplateConfig.InputParameter(
                         name,
                         description,
                         defaultValue,
                     )
```

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.3.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.2.dev0/PKG-INFO` & `semantic_kernel-0.2.3.dev0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,48 @@
-Metadata-Version: 2.1
-Name: semantic-kernel
-Version: 0.2.2.dev0
-Summary: 
-Author: Microsoft
-Author-email: SK-Support@microsoft.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: openai (>=0.27.0,<0.28.0)
-Description-Content-Type: text/markdown
+# Get Started with Semantic Kernel ⚡
+
+Install the latest package:
+
+    python -m pip install --upgrade semantic-kernel
 
-# Setup
+
+# AI backends
 
 ## OpenAI / Azure OpenAI API keys
 
 Make sure you have an
 [Open AI API Key](https://openai.com/api/) or
 [Azure Open AI service key](https://learn.microsoft.com/azure/cognitive-services/openai/quickstart?pivots=rest-api)
 
 Copy those keys into a `.env` file (see the `.env.example` file):
 
 ```
 OPENAI_API_KEY=""
 OPENAI_ORG_ID=""
-AZURE_OPENAI_API_KEY=""
-AZURE_OPENAI_ENDPOINT=""
 AZURE_OPENAI_DEPLOYMENT_NAME=""
+AZURE_OPENAI_ENDPOINT=""
+AZURE_OPENAI_API_KEY=""
 ```
 
-## Using Poetry
-
-First, navigate to the directory containing this README using your chosen shell.
-You will need to have Python 3.10 installed.
-
-Install the Poetry package manager and create a project virtual environment. (Note: we require at least Poetry 1.2.0 and Python 3.10.)
-
-```bash
-# Install poetry package
-pip3 install poetry
-# Use poetry to install project deps
-poetry install
-# Use poetry to activate project venv
-poetry shell
-```
-
-
-# Get Started with Semantic Kernel ⚡
-
-## Example: Running a simple prompt.
+# Running a prompt
 
 ```python
 import semantic_kernel as sk
-from semantic_kernel.ai.open_ai import OpenAITextCompletion
+from semantic_kernel.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
 
-kernel = sk.create_kernel()
+kernel = sk.Kernel()
 
 # Prepare OpenAI backend using credentials stored in the `.env` file
 api_key, org_id = sk.openai_settings_from_dot_env()
 kernel.config.add_text_backend("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
 
+# Alternative using Azure:
+# deployment, api_key, endpoint = sk.azure_openai_settings_from_dot_env()
+# kernel.config.add_text_backend("dv", AzureTextCompletion(deployment, endpoint, api_key))
+
 # Wrap your prompt in a function
 prompt = kernel.create_semantic_function("""
 1) A robot may not injure a human being or, through inaction,
 allow a human being to come to harm.
 
 2) A robot must obey orders given it by human beings except where
 such orders would conflict with the First Law.
@@ -78,15 +52,15 @@
 
 Give me the TLDR in exactly 5 words.""")
 
 # Run your prompt
 print(prompt()) # => Robots must not harm humans.
 ```
 
-## Example: Turn prompts into **reusable functions** with input parameters.
+# Prompts are **semantic functions** with input parameters
 
 ```python
 # Create a reusable function with one input parameter
 summarize = kernel.create_semantic_function("{{$input}}\n\nOne line TLDR with the fewest words.")
 
 # Summarize the laws of thermodynamics
 print(summarize("""
@@ -101,17 +75,38 @@
 3. Whenever one object exerts a force on another object, the second object exerts an equal and opposite on the first."""))
 
 # Summarize the law of universal gravitation
 print(summarize("""
 Every point mass attracts every single other point mass by a force acting along the line intersecting both points.
 The force is proportional to the product of the two masses and inversely proportional to the square of the distance between them."""))
 
-# Output: 
-# Energy conserved, entropy increases, zero entropy at 0K.
-# Objects move in response to forces.
-# Gravitational force between two point masses is inversely proportional to the square of the distance between them.
+# Output:
+# > Energy conserved, entropy increases, zero entropy at 0K.
+# > Objects move in response to forces.
+# > Gravitational force between two point masses is inversely proportional to the square of the distance between them.
 ```
 
-## How does this compare to the C# version of Semantic Kernel?
+# Semantic Kernel Notebooks
+
+The repository contains a few Python and C# notebooks that demonstrates how to
+get started with the Semantic Kernel.
+
+Python notebooks:
 
-Refer to the [FEATURE_PARITY.md](FEATURE_PARITY.md) doc to see where
-things stand in matching the features and functionality of the main SK branch.
+* [Getting started with Semantic Kernel](../samples/notebooks/python/00-getting-started.ipynb)
+* [Loading and configuring Semantic Kernel](../samples/notebooks/python/01-basic-loading-the-kernel.ipynb)
+* [Running AI prompts from file](../samples/notebooks/python/02-running-prompts-from-file.ipynb)
+* [Creating Semantic Functions at runtime (i.e. inline functions)](../samples/notebooks/python/03-semantic-function-inline.ipynb)
+* [Using Context Variables to Build a Chat Experience](../samples/notebooks/python/04-context-variables-chat.ipynb)
+* [Building Memory with Embeddings](../samples/notebooks/python/06-memory-and-embeddings.ipynb)
+
+# Frequently asked questions
+
+* How does Python SK compare to the C# version of Semantic Kernel?
+
+  The two SDKs are compatible and at the core they follow the same design principles.
+  Some features are still available only in the C# version, and being ported
+  Refer to the [FEATURE PARITY](FEATURE_PARITY.md) doc to see where
+  things stand in matching the features and functionality of the main SK branch.
+  Over time there will be some features available only in the Python version, and
+  others only in the C# version, for example adapters to external services,
+  scientific libraries, etc.
```

