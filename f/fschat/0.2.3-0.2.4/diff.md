# Comparing `tmp/fschat-0.2.3.tar.gz` & `tmp/fschat-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.3.tar", last modified: Fri Apr 21 09:16:52 2023, max compression
+gzip compressed data, was "fschat-0.2.4.tar", last modified: Fri Apr 28 16:37:51 2023, max compression
```

## Comparing `fschat-0.2.3.tar` & `fschat-0.2.4.tar`

### file list

```diff
@@ -1,68 +1,205 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.877371 fschat-0.2.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13822 2023-04-21 09:16:52.877371 fschat-0.2.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13328 2023-04-20 20:43:00.000000 fschat-0.2.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-21 08:18:30.000000 fschat-0.2.3/fastchat/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-18 08:21:09.000000 fschat-0.2.3/fastchat/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/client/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/client/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8880 2023-04-21 07:20:06.000000 fschat-0.2.3/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5826 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5979 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      616 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3200 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3166 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5998 2023-04-21 08:31:12.000000 fschat-0.2.3/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1688 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-18 08:21:09.000000 fschat-0.2.3/fastchat/protocol/chat_completion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5295 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11251 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5773 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3908 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7364 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17731 2023-04-21 08:09:53.000000 fschat-0.2.3/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15008 2023-04-21 08:09:56.000000 fschat-0.2.3/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10824 2023-04-21 07:20:06.000000 fschat-0.2.3/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7636 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2480 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8126 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5051 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.877371 fschat-0.2.3/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13822 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1657 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2023-04-21 08:17:20.000000 fschat-0.2.3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-21 09:16:52.877371 fschat-0.2.3/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14167 2023-04-28 16:37:51.441497 fschat-0.2.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13673 2023-04-28 16:37:35.000000 fschat-0.2.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/fastchat/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/client/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10534 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3166 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5998 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1688 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.417497 fschat-0.2.4/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/protocol/chat_completion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6637 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11251 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6177 2023-04-27 21:49:08.000000 fschat-0.2.4/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6921 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13979 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13609 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5205 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11425 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8045 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.4/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2480 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8627 2023-04-27 23:41:46.000000 fschat-0.2.4/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14871 2023-04-28 16:37:35.000000 fschat-0.2.4/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-27 21:14:01.000000 fschat-0.2.4/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5407 2023-04-28 16:34:37.000000 fschat-0.2.4/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14167 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-04-28 16:37:51.000000 fschat-0.2.4/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-28 16:37:35.000000 fschat-0.2.4/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-28 16:37:51.441497 fschat-0.2.4/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/latest-run/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.421497 fschat-0.2.4/wandb/latest-run/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.4/wandb/latest-run/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.401497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8305 2023-04-23 12:16:11.000000 fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8235 2023-04-23 12:33:09.000000 fschat-0.2.4/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8252 2023-04-23 12:33:55.000000 fschat-0.2.4/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8026 2023-04-23 12:44:12.000000 fschat-0.2.4/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.425497 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8027 2023-04-23 12:45:40.000000 fschat-0.2.4/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8050 2023-04-23 12:47:12.000000 fschat-0.2.4/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-04-23 12:48:16.000000 fschat-0.2.4/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2023-04-23 12:49:50.000000 fschat-0.2.4/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.429497 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8172 2023-04-23 12:50:49.000000 fschat-0.2.4/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8177 2023-04-23 12:51:43.000000 fschat-0.2.4/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.405497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8217 2023-04-23 12:53:11.000000 fschat-0.2.4/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:15:57.000000 fschat-0.2.4/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:17:37.000000 fschat-0.2.4/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:22:26.000000 fschat-0.2.4/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.433497 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:28:07.000000 fschat-0.2.4/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:28:26.000000 fschat-0.2.4/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:29:26.000000 fschat-0.2.4/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8722 2023-04-25 09:30:15.000000 fschat-0.2.4/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.437497 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:31:04.000000 fschat-0.2.4/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.409497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:32:09.000000 fschat-0.2.4/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.413497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 16:37:51.441497 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.4/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
```

### Comparing `fschat-0.2.3/LICENSE` & `fschat-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/PKG-INFO` & `fschat-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: fschat
-Version: 0.2.3
-Summary: An open platform for training, serving, and evaluating large language model based chatbots.
-Project-URL: Homepage, https://github.com/lm-sys/fastchat
-Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # FastChat
+| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
-
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
 
+- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
+
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
-Join our [Discord](https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://twitter.com/lmsysorg) to get the latest updates.
-
 ## Contents
 - [Install](#install)
 - [Vicuna Weights](#vicuna-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
@@ -74,27 +62,33 @@
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v1.1
+    --base-model-path /path/to/llama-7b \
+    --target-model-path /output/path/to/vicuna-7b \
+    --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v1.1
+    --base-model-path /path/to/llama-13b \
+    --target-model-path /output/path/to/vicuna-13b \
+    --delta-path lmsys/vicuna-13b-delta-v1.1
+```
+
+### Fastchat-T5
+This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
 
 ### Low CPU Memory Conversion
```

#### html2text {}

```diff
@@ -1,87 +1,86 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.3 Summary: An open platform for
-training, serving, and evaluating large language model based chatbots. Project-
-URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
-https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat An open platform for training, serving,
-and evaluating large language model based chatbots. ## Release
+# FastChat | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://
+twitter.com/lmsysorg) | An open platform for training, serving, and evaluating
+large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
-- ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
-ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
-[demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
-(https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
-twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
-(#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
-Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
-(#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
-fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
-the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
-FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
-``fschat >= 0.2.0``. Please update your local packages accordingly. If you
-follow the above commands to do a fresh install, then you should get all the
-correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
-CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
-enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
-llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
-See the "Low CPU Memory Conversion" section below if you do not have enough
-memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
-13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
-``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ### Low CPU Memory Conversion
-You can try these methods to reduce the CPU RAM requirement of weight
-conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
-large weight files into smaller ones and use the disk as temporary storage.
-This can keep the peak memory at less than 16GB. 2. Create a large swap file
-and rely on the operating system to automatically utilize the disk as virtual
-memory. ## Inference with Command Line Interface (Experimental Feature: You can
-specify `--style rich` to enable rich text output and better text streaming
-quality for some non-ASCII content. This may not work properly on certain
-terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
-requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
-Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
-memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
-``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
-from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
-the CPU only and does not require GPU. It requires around 60GB of CPU memory
-for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
-Other Platforms If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
---model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
-exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. Here
-are the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
+[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
+Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
+vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
+## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+[Inference with Command Line Interface](#inference-with-command-line-interface)
+- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
+(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
+```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
+repository and navigate to the FastChat folder ```bash git clone https://
+github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
+```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
+release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
+with the LLaMA model license. You can add our delta to the original LLaMA
+weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
+weights in the huggingface format by following the instructions [here](https://
+huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
+scripts to get Vicuna weights by applying our delta. They will automatically
+download delta weights from our Hugging Face [account](https://huggingface.co/
+lmsys). **NOTE**: Weights v1.1 are only compatible with
+```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
+packages accordingly. If you follow the above commands to do a fresh install,
+then you should get all the correct versions. ### Vicuna-7B This conversion
+command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
+section below if you do not have enough memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
+model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
+``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+the "Low CPU Memory Conversion" section below if you do not have enough memory.
+```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
+llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
+lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
+Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
+run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
+model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
+weights_version.md](docs/weights_version.md) for all versions of weights and
+their differences. ### Low CPU Memory Conversion You can try these methods to
+reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
+to the commands above, which will split large weight files into smaller ones
+and use the disk as temporary storage. This can keep the peak memory at less
+than 16GB. 2. Create a large swap file and rely on the operating system to
+automatically utilize the disk as virtual memory. ## Inference with Command
+Line Interface (Experimental Feature: You can specify `--style rich` to enable
+rich text output and better text streaming quality for some non-ASCII content.
+This may not work properly on certain terminals.) [assets/screenshot_cli.png]
+#### Single GPU The command below requires around 28GB of GPU memory for
+Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
+section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
+GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
+on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
+does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
+around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
+Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
+acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
+turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
+M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
+If you do not have enough memory, you can enable 8-bit compression by adding `-
+-load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
+to make the model easier to run on more platforms. Contributions and pull
+requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
+serve using the web UI, you need three main components: web servers that
+interface with users, model workers that host one or more models, and a
+controller to coordinate the webserver and model workers. Here are the commands
+to follow in your terminal: #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.3/README.md` & `fschat-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,36 @@
+Metadata-Version: 2.1
+Name: fschat
+Version: 0.2.4
+Summary: An open platform for training, serving, and evaluating large language model based chatbots.
+Project-URL: Homepage, https://github.com/lm-sys/fastchat
+Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # FastChat
+| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
-
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
 
+- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
+
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
-Join our [Discord](https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://twitter.com/lmsysorg) to get the latest updates.
-
 ## Contents
 - [Install](#install)
 - [Vicuna Weights](#vicuna-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
@@ -61,27 +75,33 @@
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v1.1
+    --base-model-path /path/to/llama-7b \
+    --target-model-path /output/path/to/vicuna-7b \
+    --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v1.1
+    --base-model-path /path/to/llama-13b \
+    --target-model-path /output/path/to/vicuna-13b \
+    --delta-path lmsys/vicuna-13b-delta-v1.1
+```
+
+### Fastchat-T5
+This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
 
 ### Low CPU Memory Conversion
```

#### html2text {}

```diff
@@ -1,81 +1,92 @@
-# FastChat An open platform for training, serving, and evaluating large
-language model based chatbots. ## Release
+Metadata-Version: 2.1 Name: fschat Version: 0.2.4 Summary: An open platform for
+training, serving, and evaluating large language model based chatbots. Project-
+URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
+https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # FastChat | [Discord](https://discord.gg/h6kCZb72G7)
+| [Twitter](https://twitter.com/lmsysorg) | An open platform for training,
+serving, and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
-- ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
-ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
-[demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
-(https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
-twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
-(#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
-Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
-(#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
-fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
-the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
-FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
-``fschat >= 0.2.0``. Please update your local packages accordingly. If you
-follow the above commands to do a fresh install, then you should get all the
-correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
-CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
-enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
-llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
-See the "Low CPU Memory Conversion" section below if you do not have enough
-memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
-13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
-``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ### Low CPU Memory Conversion
-You can try these methods to reduce the CPU RAM requirement of weight
-conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
-large weight files into smaller ones and use the disk as temporary storage.
-This can keep the peak memory at less than 16GB. 2. Create a large swap file
-and rely on the operating system to automatically utilize the disk as virtual
-memory. ## Inference with Command Line Interface (Experimental Feature: You can
-specify `--style rich` to enable rich text output and better text streaming
-quality for some non-ASCII content. This may not work properly on certain
-terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
-requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
-Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
-memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
-``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
-from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
-the CPU only and does not require GPU. It requires around 60GB of CPU memory
-for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
-Other Platforms If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
---model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
-exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. Here
-are the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
+[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
+Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
+vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
+## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+[Inference with Command Line Interface](#inference-with-command-line-interface)
+- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
+(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
+```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
+repository and navigate to the FastChat folder ```bash git clone https://
+github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
+```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
+release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
+with the LLaMA model license. You can add our delta to the original LLaMA
+weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
+weights in the huggingface format by following the instructions [here](https://
+huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
+scripts to get Vicuna weights by applying our delta. They will automatically
+download delta weights from our Hugging Face [account](https://huggingface.co/
+lmsys). **NOTE**: Weights v1.1 are only compatible with
+```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
+packages accordingly. If you follow the above commands to do a fresh install,
+then you should get all the correct versions. ### Vicuna-7B This conversion
+command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
+section below if you do not have enough memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
+model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
+``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+the "Low CPU Memory Conversion" section below if you do not have enough memory.
+```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
+llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
+lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
+Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
+run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
+model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
+weights_version.md](docs/weights_version.md) for all versions of weights and
+their differences. ### Low CPU Memory Conversion You can try these methods to
+reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
+to the commands above, which will split large weight files into smaller ones
+and use the disk as temporary storage. This can keep the peak memory at less
+than 16GB. 2. Create a large swap file and rely on the operating system to
+automatically utilize the disk as virtual memory. ## Inference with Command
+Line Interface (Experimental Feature: You can specify `--style rich` to enable
+rich text output and better text streaming quality for some non-ASCII content.
+This may not work properly on certain terminals.) [assets/screenshot_cli.png]
+#### Single GPU The command below requires around 28GB of GPU memory for
+Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
+section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
+GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
+on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
+does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
+around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
+Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
+acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
+turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
+M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
+If you do not have enough memory, you can enable 8-bit compression by adding `-
+-load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
+to make the model easier to run on more platforms. Contributions and pull
+requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
+serve using the web UI, you need three main components: web servers that
+interface with users, model workers that host one or more models, and a
+controller to coordinate the webserver and model workers. Here are the commands
+to follow in your terminal: #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.3/fastchat/client/api.py` & `fschat-0.2.4/fastchat/client/api.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/client/test_client.py` & `fschat-0.2.4/fastchat/client/test_client.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/conversation.py` & `fschat-0.2.4/fastchat/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Now we support
 - Vicuna
 - Koala
 - OpenAssistant/oasst-sft-1-pythia-12b
 - StabilityAI/stablelm-tuned-alpha-7b
 - databricks/dolly-v2-12b
 - THUDM/chatglm-6b
+- project-baize/baize-lora-7B
 - Alpaca/LLaMa
 """
 
 import dataclasses
 from enum import auto, Enum
 from typing import List, Tuple, Any
 
@@ -19,31 +20,34 @@
 class SeparatorStyle(Enum):
     """Different separator style."""
 
     SINGLE = auto()
     TWO = auto()
     DOLLY = auto()
     OASST_PYTHIA = auto()
+    BAIZE = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
 
     system: str
     roles: List[str]
     messages: List[List[str]]
     offset: int
     sep_style: SeparatorStyle = SeparatorStyle.SINGLE
     sep: str = "###"
     sep2: str = None
 
-    # Used for gradio server
-    skip_next: bool = False
+    # Used for the state in the gradio servers.
+    # TODO(lmzheng): refactor this
     conv_id: Any = None
+    skip_next: bool = False
+    model_name: str = None
 
     def get_prompt(self):
         if self.sep_style == SeparatorStyle.SINGLE:
             ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += self.sep + " " + role + ": " + message
@@ -74,14 +78,22 @@
             ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + message + self.sep
                 else:
                     ret += role
             return ret
+        elif self.sep_style == SeparatorStyle.BAIZE:
+            ret = self.system
+            for role, message in self.messages:
+                if message:
+                    ret += "\n" + role + message
+                else:
+                    ret += "\n" + role
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role, message):
         self.messages.append([role, message])
 
     def to_gradio_chatbot(self):
@@ -99,25 +111,27 @@
             roles=self.roles,
             messages=[[x, y] for x, y in self.messages],
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
             conv_id=self.conv_id,
+            model_name=self.model_name,
         )
 
     def dict(self):
         return {
             "system": self.system,
             "roles": self.roles,
             "messages": self.messages,
             "offset": self.offset,
             "sep": self.sep,
             "sep2": self.sep2,
             "conv_id": self.conv_id,
+            "model_name": self.model_name,
         }
 
 
 conv_one_shot = Conversation(
     system="A chat between a curious human and an artificial intelligence assistant. "
     "The assistant gives helpful, detailed, and polite answers to the human's questions.",
     roles=("Human", "Assistant"),
@@ -205,57 +219,78 @@
     roles=("<|USER|>", "<|ASSISTANT|>"),
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.OASST_PYTHIA,
     sep="",
 )
 
+conv_baize = Conversation(
+    system="The following is a conversation between a human and an AI assistant named Baize (named after a mythical creature in Chinese folklore). Baize is an open-source AI assistant developed by UCSD and Sun Yat-Sen University. The human and the AI assistant take turns chatting. Human statements start with [|Human|] and AI assistant statements start with [|AI|]. The AI assistant always provides responses in as much detail as possible, and in Markdown format. The AI assistant always declines to engage with topics, questions and instructions related to unethical, controversial, or sensitive issues. Complete the transcript in exactly that format.",
+    roles=("[|Human|]", "[|AI|]"),
+    messages=(
+        ("[|Human|]", "Hello!"),
+        ("[|AI|]", "Hi!"),
+    ),
+    offset=2,
+    sep_style=SeparatorStyle.BAIZE,
+    sep="[|Human|]",
+)
+
+
 conv_templates = {
     "conv_one_shot": conv_one_shot,
     "vicuna_v1.1": conv_vicuna_v1_1,
     "koala_v1": conv_koala_v1,
     "dolly": conv_dolly,
     "oasst": conv_oasst,
+    "baize": conv_baize,
 }
 
 
 def get_default_conv_template(model_name):
     model_name = model_name.lower()
     if "vicuna" in model_name or "output" in model_name:
         return conv_vicuna_v1_1
     elif "koala" in model_name:
         return conv_koala_v1
     elif "dolly-v2" in model_name:
         return conv_dolly
     elif "oasst" in model_name and "pythia" in model_name:
         return conv_oasst
+    elif "baize" in model_name:
+        return conv_baize
     elif "stablelm" in model_name:
         return conv_stablelm
     return conv_one_shot
 
 
 def compute_skip_echo_len(model_name, conv, prompt):
     model_name = model_name.lower()
     if "chatglm" in model_name:
         skip_echo_len = len(conv.messages[-2][1]) + 1
     elif "dolly-v2" in model_name:
         special_toks = ["### Instruction:", "### Response:", "### End"]
         skip_echo_len = len(prompt)
         for tok in special_toks:
             skip_echo_len -= prompt.count(tok) * len(tok)
+    elif "t5" in model_name:
+         skip_echo_len = len(prompt)
     elif "oasst" in model_name and "pythia" in model_name:
         special_toks = ["<|prompter|>", "<|assistant|>", "<|endoftext|>"]
         skip_echo_len = len(prompt)
         for tok in special_toks:
             skip_echo_len -= prompt.count(tok) * len(tok)
     elif "stablelm" in model_name:
         special_toks = ["<|SYSTEM|>", "<|USER|>", "<|ASSISTANT|>"]
         skip_echo_len = len(prompt)
         for tok in special_toks:
             skip_echo_len -= prompt.count(tok) * len(tok)
+    elif "baize" in model_name:
+        skip_echo_len = len(prompt)
     else:
         skip_echo_len = len(prompt) + 1 - prompt.count("</s>") * 3
     return skip_echo_len
 
 
 if __name__ == "__main__":
+    default_conversation = conv_templates["vicuna_v1.1"]
     print(default_conversation.get_prompt())
```

### Comparing `fschat-0.2.3/fastchat/data/alpaca-converter.py` & `fschat-0.2.4/fastchat/data/alpaca-converter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/data/clean_sharegpt.py` & `fschat-0.2.4/fastchat/data/clean_sharegpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 - Convert html to markdown with basic data cleaning.
 - Deduplication.
 
 Usage:
 python3 -m fastchat.data.clean_sharegpt --in sharegpt_html.json --out sharegpt_clean.json
 """
 import argparse
+from concurrent.futures import ProcessPoolExecutor
 import json
 import logging
 import re
 from typing import Dict, Union
 
 import bs4
 import markdownify  # == 0.11.6
-import tqdm
+from tqdm import tqdm
 
 
 div_pattern = re.compile("<div.*?>")
 span_pattern = re.compile("<span.*?>")
 code_lang_pattern = re.compile(
     "```\s*" + "(.*?)" + "(?:Copy code)+" + "(.+?)" + "\s*?```", re.DOTALL
 )
@@ -55,136 +56,140 @@
     val = re.sub(copy_chars_pattern, "", val)
     # Remove empty code block ```\nCopy code\n```
     val = re.sub(copy_code_pattern, "", val)
 
     # Strip
     val = val.replace("\n\n\n", "\n").strip()
 
-    if args.debug:
-        print(val)
-        exit()
-
     return val
 
 
-def should_filter(val: str) -> bool:
-    black_list = ["openai", "chatgpt"]
-    for w in black_list:
+def contain_blocked_words(val: str) -> bool:
+    blocked_words = ["openai", "chatgpt"]
+    for w in blocked_words:
         if w in val.lower():
             return True
     return False
 
 
-def clean_html_source(content, begin, end, check_tag, check_num):
-    """
-    Clean the input json content.
+def clean_html_one_sample(sample):
+    roles = ["human", "gpt"]
+
+    if len(sample["conversations"]) <= 1:
+        return (sample, 1)
+
+    # Adjust the offset for cases like https://sharegpt.com/c/VyaZlh4
+    if sample["conversations"][0]["from"] != "human":
+        sample["conversations"] = sample["conversations"][1:]
+    if len(sample["conversations"]) <= 1:
+        return (sample, 1)
+
+    if sample["conversations"][-1]["from"] == "human":
+        sample["conversations"] = sample["conversations"][:-1]
+    if len(sample["conversations"]) <= 1:
+        return (sample, 1)
+
+    for i, c in enumerate(sample["conversations"]):
+        if c["from"] != roles[i % 2]:
+            return (sample, 2)
+
+        if contain_blocked_words(c["value"]):
+            return (sample, 3)
+
+        try:
+            new_val = html_to_markdown(c["value"])
+        except (bs4.builder.ParserRejectedMarkup, AssertionError):
+            return (sample, 4)
+
+        c["value"] = new_val
 
-    Args:
-        content: json file loaded in memory.
-        check_tag: a debug purpose arg. If a conversation contains the tag, log
-          it before and after cleaning.
-        check_num: number of matched conversations logged.
+    return (sample, 0)
+
+
+def clean_html_all(content, begin, end):
+    """
+    Clean the source html files.
     """
-    BARRIER = "\n" + "=" * 20 + "\n"
     cnt_skip = 0
+    cnt_blocked_words = 0
+    cnt_wrong_format = 0
+    cnt_parser_error = 0
     cnt_too_short = 0
     cnt_id_duplication = 0
     cnt_value_duplication = 0
-    cnt_filter = 0
     cnt_tag = 0
-    visited = {}
 
     content = content[begin:end]
-    new_content = []
+    processed = []
+    with ProcessPoolExecutor() as executor:
+        for result in tqdm(
+            executor.map(clean_html_one_sample, content), total=len(content)
+        ):
+            processed.append(result)
 
-    for sample in tqdm.tqdm(content):
-        skipped = False
+    visited = {}
+    new_content = []
+    for sample, error_code in tqdm(processed):
         cid = sample["id"]
+        skipped = True
 
-        if len(sample["conversations"]) <= 1:
-            print(f"id {cid} is too short")
-            cnt_too_short += 1
-            skipped = True
+        if error_code != 0:
+            if error_code == 1:
+                print(f"id {cid} is too short")
+                cnt_too_short += 1
+            elif error_code == 2:
+                print(f"id {cid} has a wrong format")
+                cnt_wrong_format += 1
+            elif error_code == 3:
+                print(f"id {cid} contains blocked words")
+                cnt_blocked_words += 1
+            elif error_code == 4:
+                print(f"id {cid} contains parser errors")
+                cnt_parser_error += 1
+            else:
+                raise ValueError(f"Invalid error_code: {error_code}")
         elif cid in visited:
             print(f"id {cid} is an id duplication of {visited[cid]}")
             cnt_id_duplication += 1
-            skipped = True
         elif (
             sample["conversations"][1]["value"],
             len(sample["conversations"]),
         ) in visited:
             key = (sample["conversations"][1]["value"], len(sample["conversations"]))
             print(f"id {cid} is a value duplication of {visited[key]}")
             cnt_value_duplication += 1
-            skipped = True
         else:
             key = (sample["conversations"][1]["value"], len(sample["conversations"]))
             visited[cid] = visited[key] = cid
-
-            for c in sample["conversations"]:
-                if should_filter(c["value"]):
-                    print(f"id {cid} is filtered out")
-                    cnt_filter += 1
-                    skipped = True
-                    break
-
-                try:
-                    new_val = html_to_markdown(c["value"])
-                except (bs4.builder.ParserRejectedMarkup, AssertionError):
-                    skipped = True
-                    break
-
-                c["value"] = new_val
-
-                # Debug
-                if (
-                    check_tag is not None
-                    and check_tag in c["value"]
-                    and cnt_tag < check_num
-                ):
-                    logging.debug(
-                        BARRIER
-                        + c["value"]
-                        + "\n"
-                        + BARRIER
-                        + new_val
-                        + "\n"
-                        + BARRIER
-                        + "\n"
-                    )
-                    cnt_tag += 1
-                    if cnt_tag == check_num:
-                        break
+            skipped = False
 
         if not skipped:
             new_content.append(sample)
         else:
             cnt_skip += 1
 
     print(
         f"total: {len(content)}, skip: {cnt_skip}, new: {len(new_content)}, "
+        f"cnt_blocked_words: {cnt_blocked_words}, cnt_parser_error: {cnt_parser_error}, "
+        f"cnt_wrong_format: {cnt_wrong_format}, "
         f"cnt_too_short: {cnt_too_short}, cnt_id_duplication: {cnt_id_duplication}, "
-        f"cnt_value_duplication: {cnt_value_duplication}, cnt_filter: {cnt_filter}"
+        f"cnt_value_duplication: {cnt_value_duplication}, "
     )
 
     return new_content
 
 
 def main(args):
     content = json.load(open(args["in_file"], "r"))
-    content = clean_html_source(
-        content, args["begin"], args["end"], args["check_tag"], args["check_num"]
-    )
+    content = clean_html_all(content, args["begin"], args["end"])
     json.dump(content, open(args["out_file"], "w"), indent=2)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--in-file", type=str, required=True)
     parser.add_argument("--out-file", type=str, default="sharegpt_clean.json")
     parser.add_argument("--begin", type=int)
     parser.add_argument("--end", type=int)
     parser.add_argument("--debug", action="store_true")
-    parser.add_argument("--check-tag", type=str)
-    parser.add_argument("--check-num", type=int, default=1)
     args = parser.parse_args()
     main(vars(args))
```

### Comparing `fschat-0.2.3/fastchat/data/hardcoded_questions.py` & `fschat-0.2.4/fastchat/data/hardcoded_questions.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                         ],
                     }
                 )
 
     questions = [
         "Who are you?",
         "What is your name?",
+        "Can you introduce yourself?",
         "What's your name?",
         "What are you called?",
         "What are you?",
         "Tell me your name.",
         "Tell me about yourself.",
         "Tell me about you.",
         "Tell me who you are.",
```

### Comparing `fschat-0.2.3/fastchat/data/inspect.py` & `fschat-0.2.4/fastchat/data/sample.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """
-Usage:
-python3 -m fastchat.data.inspect --in sharegpt_20230322_clean_lang_split.json
+Sample some conversations from a file.
+
+Usage: python3 -m fastchat.data.sample --in sharegpt.json --out sampled.json
 """
 import argparse
 import json
-
-import tqdm
+from typing import Dict, Sequence, Optional
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--in-file", type=str, required=True)
-    parser.add_argument("--begin", type=int)
+    parser.add_argument("--out-file", type=str, default="sampled.json")
+    parser.add_argument("--begin", type=int, default=0)
+    parser.add_argument("--end", type=int, default=100)
+    parser.add_argument("--max-length", type=int, default=128)
     args = parser.parse_args()
 
     content = json.load(open(args.in_file, "r"))
-    for sample in tqdm.tqdm(content[args.begin :]):
-        print(f"id: {sample['id']}")
-        for conv in sample["conversations"]:
-            print(conv["from"] + ": ")
-            print(conv["value"])
-            input()
+    new_content = []
+    for i in range(args.begin, args.end):
+        sample = content[i]
+        concat = ""
+        for s in sample["conversations"]:
+            concat += s["value"]
+
+        if len(concat) > args.max_length:
+            continue
+
+        new_content.append(sample)
+
+    json.dump(new_content, open(args.out_file, "w"), indent=2)
```

### Comparing `fschat-0.2.3/fastchat/data/merge.py` & `fschat-0.2.4/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/data/optional_clean.py` & `fschat-0.2.4/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/data/split_long_conversation.py` & `fschat-0.2.4/fastchat/data/split_long_conversation.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,60 +3,78 @@
 
 Usage: python3 -m fastchat.data.split_long_conversation \
     --in sharegpt_clean.json \
     --out sharegpt_split.json \
     --model-name-or-path $<model-name>
 """
 import argparse
+from concurrent.futures import ProcessPoolExecutor
 import json
 from typing import Dict, Sequence, Optional
 
 import transformers
-import tqdm
+from tqdm import tqdm
 
 from fastchat import conversation as conversation_lib
 
 
-def split_sample(sample, start_idx, end_idx):
+def make_sample(sample, start_idx, end_idx):
     assert (end_idx - start_idx) % 2 == 0
     return {
         "id": sample["id"] + "_" + str(start_idx),
         "conversations": sample["conversations"][start_idx:end_idx],
     }
 
 
-def split_contents(content, begin, end, tokenizer, max_length):
+tokenizer = max_length = None
+
+
+def split_one_sample(sample):
+    tokenized_lens = []
+    conversations = sample["conversations"]
+    conversations = conversations[: len(conversations) // 2 * 2]
+    for c in conversations:
+        length = len(tokenizer(c["value"]).input_ids) + 6
+        tokenized_lens.append(length)
+
+    start_idx = 0
+    cur_len = 0
+
+    if len(conversations) % 2 != 0 or len(conversations) < 2:
+        return []
+
+    new_samples = []
+    for i in range(0, len(conversations), 2):
+        tmp_len = tokenized_lens[i] + tokenized_lens[i + 1]
+        if cur_len + tmp_len > max_length:
+            new_samples.append(make_sample(sample, start_idx, i))
+            start_idx = i
+            cur_len = 0
+        elif i == len(conversations) - 2:
+            new_samples.append(make_sample(sample, start_idx, i + 2))
+
+        cur_len += tmp_len
+
+    return new_samples
+
+
+def split_all(content, begin, end, tokenizer_, max_length_):
     """
     Keep the maximum round of conversations within the max token length constraint
     """
+    global tokenizer, max_length
+    tokenizer = tokenizer_
+    max_length = max_length_
+
     content = content[begin:end]
     new_content = []
 
-    for sample in tqdm.tqdm(content):
-        tokenized_lens = []
-        conversations = sample["conversations"]
-        conversations = conversations[: len(conversations) // 2 * 2]
-        for c in conversations:
-            length = len(tokenizer(c["value"]).input_ids) + 5
-            tokenized_lens.append(length)
-
-        start_idx = 0
-        cur_len = 0
-        sample
-        assert len(conversations) % 2 == 0, f"id: {sample['id']}"
-        for i in range(0, len(conversations), 2):
-            tmp_len = tokenized_lens[i] + tokenized_lens[i + 1]
-            if cur_len + tmp_len > max_length:
-                new_content.append(split_sample(sample, start_idx, i))
-                start_idx = i
-                cur_len = 0
-            elif i == len(conversations) - 2:
-                new_content.append(split_sample(sample, start_idx, i + 2))
-
-            cur_len += tmp_len
+    with ProcessPoolExecutor() as executor:
+        for result in tqdm(executor.map(split_one_sample, content), total=len(content)):
+            new_content.extend(result)
 
     return new_content
 
 
 def filter_invalid_roles(content):
     new_content = []
     for i, c in enumerate(content):
@@ -80,17 +98,15 @@
     content = json.load(open(args.in_file, "r"))
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         args.model_name_or_path,
         model_max_length=args.max_length,
         padding_side="right",
         use_fast=False,
     )
-    new_content = split_contents(
-        content, args.begin, args.end, tokenizer, args.max_length
-    )
+    new_content = split_all(content, args.begin, args.end, tokenizer, args.max_length)
     new_content = filter_invalid_roles(new_content)
 
     print(f"total: {len(content)}, new: {len(new_content)}")
     json.dump(new_content, open(args.out_file, "w"), indent=2)
 
 
 if __name__ == "__main__":
```

### Comparing `fschat-0.2.3/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.4/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.4/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/eval/get_model_answer.py` & `fschat-0.2.4/fastchat/eval/get_model_answer.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.4/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/model/apply_delta.py` & `fschat-0.2.4/fastchat/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/model/convert_fp16.py` & `fschat-0.2.4/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/model/make_delta.py` & `fschat-0.2.4/fastchat/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/protocol/chat_completion.py` & `fschat-0.2.4/fastchat/protocol/chat_completion.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/api.py` & `fschat-0.2.4/fastchat/serve/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 Usage:
 
 python3 -m fastchat.serve.api
 
 Reference: https://platform.openai.com/docs/api-reference/chat/create
 """
-
+import asyncio
 from typing import Union, Dict, List, Any
 
 import argparse
 import json
 import logging
 
 import fastapi
+from fastapi.middleware.cors import CORSMiddleware
 import httpx
 import uvicorn
 from pydantic import BaseSettings
 
 from fastchat.protocol.chat_completion import (
     ChatCompletionRequest,
     ChatCompletionResponse,
@@ -36,29 +37,45 @@
 
 
 app_settings = AppSettings()
 app = fastapi.FastAPI()
 headers = {"User-Agent": "FastChat API Server"}
 
 
+@app.get("/v1/models")
+async def show_available_models():
+    controller_url = app_settings.FASTCHAT_CONTROLLER_URL
+    async with httpx.AsyncClient() as client:
+        ret = await client.post(controller_url + "/refresh_all_workers")
+        ret = await client.post(controller_url + "/list_models")
+    models = ret.json()["models"]
+    models.sort()
+    return {"data": [{"id": m} for m in models], "object": "list"}
+
+
 @app.post("/v1/chat/completions")
 async def create_chat_completion(request: ChatCompletionRequest):
     """Creates a completion for the chat message"""
     payload, skip_echo_len = generate_payload(
         request.model,
         request.messages,
         temperature=request.temperature,
         max_tokens=request.max_tokens,
         stop=request.stop,
     )
 
     choices = []
     # TODO: batch the requests. maybe not necessary if using CacheFlow worker
+    chat_completions = []
     for i in range(request.n):
-        content = await chat_completion(request.model, payload, skip_echo_len)
+        content = asyncio.create_task(chat_completion(request.model, payload, skip_echo_len))
+        chat_completions.append(content)
+
+    for i, content_task in enumerate(chat_completions):
+        content = await content_task
         choices.append(
             ChatCompletionResponseChoice(
                 index=i,
                 message=ChatMessage(role="assistant", content=content),
                 # TODO: support other finish_reason
                 finish_reason="stop",
             )
@@ -165,10 +182,25 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="FastChat ChatGPT-compatible Restful API server."
     )
     parser.add_argument("--host", type=str, default="localhost", help="host name")
     parser.add_argument("--port", type=int, default=8000, help="port number")
+    parser.add_argument("--allow-credentials", action="store_true", help="allow credentials")
+    parser.add_argument("--allowed-origins", type=json.loads, default=["*"], help="allowed origins")
+    parser.add_argument("--allowed-methods", type=json.loads, default=["*"], help="allowed methods")
+    parser.add_argument("--allowed-headers", type=json.loads, default=["*"], help="allowed headers")
 
     args = parser.parse_args()
+
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=args.allowed_origins,
+        allow_credentials=args.allow_credentials,
+        allow_methods=args.allowed_methods,
+        allow_headers=args.allowed_headers,
+    )
+
+    logger.debug(f"==== args ====\n{args}")
+
     uvicorn.run("fastchat.serve.api:app", host=args.host, port=args.port, reload=True)
```

### Comparing `fschat-0.2.3/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.4/fastchat/serve/cacheflow_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/cli.py` & `fschat-0.2.4/fastchat/serve/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Chat with a model with command line interface.
 
 Usage:
 python3 -m fastchat.serve.cli --model ~/model_weights/llama-7b
 """
 import argparse
+import os
 import re
 
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from rich.console import Console
@@ -97,14 +98,18 @@
                 # Update the Live console output
                 live.update(markdown)
         self._console.print()
         return outputs[skip_echo_len:]
 
 
 def main(args):
+    if args.gpus:
+        if args.num_gpus and len(args.gpus.split(",")) < int(args.num_gpus):
+            raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
+        os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
     if args.style == "simple":
         chatio = SimpleChatIO()
     elif args.style == "rich":
         chatio = RichChatIO()
     else:
         raise ValueError(f"Invalid style for console: {args.style}")
     try:
@@ -131,14 +136,20 @@
         type=str,
         default="facebook/opt-350m",
         help="The path to the weights",
     )
     parser.add_argument(
         "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
     )
+    parser.add_argument(
+        "--gpus",
+        type=str,
+        default=None,
+        help="A single GPU like 1 or multiple GPUs like 0,2"
+    )
     parser.add_argument("--num-gpus", type=str, default="1")
     parser.add_argument(
         "--max-gpu-memory",
         type=str,
         help="The maximum memory per gpu. Use a string like '13Gib'",
     )
     parser.add_argument(
```

### Comparing `fschat-0.2.3/fastchat/serve/controller.py` & `fschat-0.2.4/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/gradio_css.py` & `fschat-0.2.4/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/gradio_patch.py` & `fschat-0.2.4/fastchat/serve/gradio_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Adopted from https://github.com/gradio-app/gradio/blob/main/gradio/components.py
 Fix a markdown render problem.
 """
 from __future__ import annotations
 
 from gradio.components import *
 from markdown2 import Markdown
+import nh3
 
 
 class _Keywords(Enum):
     NO_VALUE = "NO_VALUE"  # Used as a sentinel to determine if nothing is provided as a argument for `value` in `Component.update()`
     FINISHED_ITERATING = "FINISHED_ITERATING"  # Used to skip processing of a component's value (needed for generators + state)
 
 
@@ -140,15 +141,15 @@
             assert (
                 len(message_pair) == 2
             ), f"Expected a list of lists of length 2 or list of tuples of length 2. Received: {message_pair}"
             processed_messages.append(
                 (
                     # self._process_chat_messages(message_pair[0]),
                     '<pre style="font-family: var(--font)">'
-                    + message_pair[0]
+                    + nh3.clean(message_pair[0])
                     + "</pre>",
                     self._process_chat_messages(message_pair[1]),
                 )
             )
         return processed_messages
 
     def style(self, height: int | None = None, **kwargs):
```

### Comparing `fschat-0.2.3/fastchat/serve/gradio_web_server.py` & `fschat-0.2.4/fastchat/serve/gradio_web_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,31 +31,30 @@
 
 no_change_btn = gr.Button.update()
 enable_btn = gr.Button.update(interactive=True)
 disable_btn = gr.Button.update(interactive=False)
 
 controller_url = None
 enable_moderation = False
-models = []
+
 
 priority = {
     "vicuna-13b": "aaa",
     "koala-13b": "aab",
-    "oasst-sft-1-pythia-12b": "aac",
+    "oasst-pythia-12b": "aac",
     "dolly-v2-12b": "aad",
     "chatglm-6b": "aae",
     "stablelm-tuned-alpha-7b": "aaf",
 }
 
 
-def set_global_vars(controller_url_, enable_moderation_, models_):
-    global controller_url, enable_moderation, models
+def set_global_vars(controller_url_, enable_moderation_):
+    global controller_url, enable_moderation
     controller_url = controller_url_
     enable_moderation = enable_moderation_
-    models = models_
 
 
 def get_conv_log_filename():
     t = datetime.datetime.now()
     name = os.path.join(LOGDIR, f"{t.year}-{t.month:02d}-{t.day:02d}-conv.json")
     return name
 
@@ -70,21 +69,21 @@
     return models
 
 
 get_window_url_params = """
 function() {
     const params = new URLSearchParams(window.location.search);
     url_params = Object.fromEntries(params);
-    console.log(url_params);
+    console.log("url_params", url_params);
     return url_params;
     }
 """
 
 
-def load_demo_single(url_params):
+def load_demo_single(models, url_params):
     dropdown_update = gr.Dropdown.update(visible=True)
     if "model" in url_params:
         model = url_params["model"]
         if model in models:
             dropdown_update = gr.Dropdown.update(value=model, visible=True)
 
     state = None
@@ -97,15 +96,15 @@
         gr.Row.update(visible=True),
         gr.Accordion.update(visible=True),
     )
 
 
 def load_demo(url_params, request: gr.Request):
     logger.info(f"load_demo. ip: {request.client.host}. params: {url_params}")
-    return load_demo_single(url_params)
+    return load_demo_single(models, url_params)
 
 
 def vote_last_response(state, vote_type, model_selector, request: gr.Request):
     with open(get_conv_log_filename(), "a") as fout:
         data = {
             "tstamp": round(time.time(), 4),
             "type": vote_type,
@@ -195,14 +194,15 @@
         yield (state, state.to_gradio_chatbot()) + (no_change_btn,) * 5
         return
 
     if len(state.messages) == state.offset + 2:
         # First round of conversation
         new_state = get_default_conv_template(model_name).copy()
         new_state.conv_id = uuid.uuid4().hex
+        new_state.model_name = state.model_name or model_selector
         new_state.append_message(new_state.roles[0], state.messages[-2][1])
         new_state.append_message(new_state.roles[1], None)
         state = new_state
 
     # Query worker address
     ret = requests.post(
         controller_url + "/get_worker_address", json={"model": model_name}
@@ -320,31 +320,31 @@
 #notice_markdown th {
     display: none;
 }
 """
 )
 
 
-def build_single_model_ui():
+def build_single_model_ui(models):
     notice_markdown = """
 # 🏔️ Chat with Open Large Language Models
-- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[GitHub]](https://github.com/lm-sys/FastChat) [[Evaluation]](https://vicuna.lmsys.org/eval/)
-- Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/) [[GitHub]](https://github.com/young-geng/EasyLM)
-- This demo server. [[GitHub]](https://github.com/lm-sys/FastChat)
+- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[Evaluation]](https://vicuna.lmsys.org/eval/)
+- Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/)
+- [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
-By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
+By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
 
 ### Choose a model to chat with
 | | |
-| --- | --- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. |
-| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open LLM by Databricks. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model 开源双语对话语言模型 | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models. |
+| ---- | ---- |
+| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
+| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. |
+| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
+| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
 """
 
     learn_more_markdown = """
 ### License
 The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
 """
 
@@ -438,15 +438,15 @@
         [state, model_selector, temperature, max_output_tokens],
         [state, chatbot] + btn_list,
     )
 
     return state, model_selector, chatbot, textbox, send_btn, button_row, parameter_row
 
 
-def build_demo():
+def build_demo(models):
     with gr.Blocks(
         title="Chat with Open Large Language Models",
         theme=gr.themes.Base(),
         css=block_css,
     ) as demo:
         url_params = gr.JSON(visible=False)
 
@@ -454,15 +454,15 @@
             state,
             model_selector,
             chatbot,
             textbox,
             send_btn,
             button_row,
             parameter_row,
-        ) = build_single_model_ui()
+        ) = build_single_model_ui(models)
 
         if args.model_list_mode == "once":
             demo.load(
                 load_demo,
                 [url_params],
                 [
                     state,
@@ -493,17 +493,17 @@
     parser.add_argument("--share", action="store_true")
     parser.add_argument(
         "--moderate", action="store_true", help="Enable content moderation"
     )
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
+    set_global_vars(args.controller_url, args.moderate)
     models = get_model_list(args.controller_url)
-    set_global_vars(args.controller_url, args.moderate, models)
 
     logger.info(args)
-    demo = build_demo()
+    demo = build_demo(models)
     demo.queue(
         concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
     ).launch(
         server_name=args.host, server_port=args.port, share=args.share, max_threads=200
     )
```

### Comparing `fschat-0.2.3/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.4/fastchat/serve/gradio_block_arena_named.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,70 @@
-import argparse
-from collections import defaultdict
-import datetime
 import json
-import os
 import time
-import uuid
 
 import gradio as gr
-import requests
+import numpy as np
 
-from fastchat.conversation import get_default_conv_template, SeparatorStyle
-from fastchat.constants import LOGDIR
+from fastchat.conversation import get_default_conv_template
 from fastchat.utils import (
     build_logger,
-    server_error_msg,
     violates_moderation,
     moderation_msg,
 )
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     http_bot,
-    set_global_vars,
-    get_window_url_params,
     get_conv_log_filename,
-    block_css,
-    build_single_model_ui,
     no_change_btn,
     enable_btn,
     disable_btn,
-    get_model_list,
-    load_demo_single,
 )
-from fastchat.serve.inference import compute_skip_echo_len
 
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 num_models = 2
+enable_moderation = False
 
 
-def load_demo_side_by_side(url_params):
+def set_global_vars_named(enable_moderation_):
+    global enable_moderation
+    enable_moderation = enable_moderation_
+
+
+def load_demo_side_by_side_named(models, url_params):
     states = (None,) * num_models
-    dropdown_updates = (gr.Dropdown.update(visible=True),) * num_models
+
+    model_left = models[0]
+    if len(models) > 1:
+        weights = ([8, 4, 2, 1] + [1] * 32)[:len(models) - 1]
+        weights = weights / np.sum(weights)
+        model_right = np.random.choice(models[1:], p=weights)
+    else:
+        model_right = model_left
+
+    selector_updates = (
+        gr.Dropdown.update(model_left, visible=True),
+        gr.Dropdown.update(model_right, visible=True),
+    )
 
     return (
         states
-        + dropdown_updates
+        + selector_updates
         + (gr.Chatbot.update(visible=True),) * num_models
         + (
             gr.Textbox.update(visible=True),
-            gr.Button.update(visible=True),
+            gr.Box.update(visible=True),
             gr.Row.update(visible=True),
             gr.Row.update(visible=True),
             gr.Accordion.update(visible=True),
         )
     )
 
 
-def load_demo(url_params, request: gr.Request):
-    logger.info(f"load_demo. ip: {request.client.host}. params: {url_params}")
-    selected = 0
-    if "compare" in url_params:
-        selected = 1
-    single_updates = load_demo_single(url_params)
-    side_by_side_updates = load_demo_side_by_side(url_params)
-    return (gr.Tabs.update(selected=selected),) + single_updates + side_by_side_updates
-
-
 def vote_last_response(states, vote_type, model_selectors, request: gr.Request):
     with open(get_conv_log_filename(), "a") as fout:
         data = {
             "tstamp": round(time.time(), 4),
             "type": vote_type,
             "models": [x for x in model_selectors],
             "states": [x.dict() for x in states],
@@ -78,57 +72,66 @@
         }
         fout.write(json.dumps(data) + "\n")
 
 
 def leftvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"leftvote. ip: {request.client.host}")
+    logger.info(f"leftvote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "leftvote", [model_selector0, model_selector1], request
     )
     return ("",) + (disable_btn,) * 3
 
 
 def rightvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"rightvote. ip: {request.client.host}")
+    logger.info(f"rightvote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "rightvote", [model_selector0, model_selector1], request
     )
     return ("",) + (disable_btn,) * 3
 
 
 def tievote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"tievote. ip: {request.client.host}")
+    logger.info(f"tievote (named). ip: {request.client.host}")
     vote_last_response(
         [state0, state1], "tievote", [model_selector0, model_selector1], request
     )
     return ("",) + (disable_btn,) * 3
 
 
 def regenerate(state0, state1, request: gr.Request):
-    logger.info(f"regenerate. ip: {request.client.host}")
+    logger.info(f"regenerate (named). ip: {request.client.host}")
     states = [state0, state1]
     for i in range(num_models):
         states[i].messages[-1][-1] = None
         states[i].skip_next = False
     return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 5
 
 
 def clear_history(request: gr.Request):
-    logger.info(f"clear_history. ip: {request.client.host}")
+    logger.info(f"clear_history (named). ip: {request.client.host}")
     return [None] * num_models + [None] * num_models + [""] + [disable_btn] * 5
 
 
+def share_click(state0, state1, model_selector0, model_selector1,
+                request: gr.Request):
+    logger.info(f"share (named). ip: {request.client.host}")
+    if state0 is not None and state1 is not None:
+        vote_last_response(
+            [state0, state1], "share", [model_selector0, model_selector1], request
+        )
+
+
 def add_text(state0, state1, text, request: gr.Request):
-    logger.info(f"add_text. ip: {request.client.host}. len: {len(text)}")
+    logger.info(f"add_text (named). ip: {request.client.host}. len: {len(text)}")
     states = [state0, state1]
 
     for i in range(num_models):
         if states[i] is None:
             states[i] = get_default_conv_template("vicuna").copy()
 
     if len(text) <= 0:
@@ -140,18 +143,18 @@
             + [""]
             + [
                 no_change_btn,
             ]
             * 5
         )
 
-    if args.moderate:
+    if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
-            logger.info(f"violate moderation. ip: {request.client.host}. text: {text}")
+            logger.info(f"violate moderation (named). ip: {request.client.host}. text: {text}")
             for i in range(num_models):
                 states[i].skip_next = True
             return (
                 states
                 + [x.to_gradio_chatbot() for x in states]
                 + [moderation_msg]
                 + [
@@ -182,15 +185,15 @@
     state1,
     model_selector0,
     model_selector1,
     temperature,
     max_new_tokens,
     request: gr.Request,
 ):
-    logger.info(f"http_bot_all. ip: {request.client.host}")
+    logger.info(f"http_bot_all (named). ip: {request.client.host}")
     states = [state0, state1]
     model_selector = [model_selector0, model_selector1]
     gen = []
     for i in range(num_models):
         gen.append(
             http_bot(states[i], model_selector[i], temperature, max_new_tokens, request)
         )
@@ -206,79 +209,94 @@
                 stop = False
             except StopIteration:
                 pass
         yield states + chatbots + list(buttons)
         if stop:
             break
 
+    for i in range(10):
+        if i % 2 == 0:
+            yield states + chatbots + [disable_btn] * 3 + list(buttons)[3:]
+        else:
+            yield states + chatbots + list(buttons)
+        time.sleep(0.2)
+
 
-def build_side_by_side_ui():
+def build_side_by_side_ui_named(models):
     notice_markdown = """
-# ⚔️  Compare Open Large Language Models Side-by-Side
-Chat with two models side-by-side and vote for which one is better!
+# ⚔️  Chatbot Arena ⚔️ 
+Rules:
+- Chat with two models side-by-side and vote for which one is better!
+- You pick the models you want to chat with.
+- You can continue chating and voting or click "Clear history" to start a new round.
+- A leaderboard will be available soon.
+- [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
-By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
+By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
 The demo works better on desktop devices with a wide screen.
 
 ### Choose two models to chat with
 | | |
 | ---- | ---- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. |
-| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open LLM by Databricks. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model 开源双语对话语言模型 | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models. |
+| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
+| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. |
+| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
+| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
 """
 
     learn_more_markdown = """
 ### License
 The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
 """
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
     notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
-    with gr.Row():
-        for i in range(num_models):
-            with gr.Column():
-                model_selectors[i] = gr.Dropdown(
-                    choices=models,
-                    value=models[i] if len(models) > i else "",
-                    interactive=True,
-                    show_label=False,
-                ).style(container=False)
+    with gr.Box(elem_id="share-region"):
+        with gr.Row():
+            for i in range(num_models):
+                with gr.Column():
+                    model_selectors[i] = gr.Dropdown(
+                        choices=models,
+                        value=models[i] if len(models) > i else "",
+                        interactive=True,
+                        show_label=False,
+                    ).style(container=False)
 
-    with gr.Row():
-        for i in range(num_models):
-            with gr.Column():
-                chatbots[i] = grChatbot(elem_id="chatbot", visible=False).style(
-                    height=550
-                )
-
-    with gr.Row(visible=False) as button_row:
-        leftvote_btn = gr.Button(value="👈 Left is better", interactive=False)
-        tie_btn = gr.Button(value="🤝 Tie", interactive=False)
-        rightvote_btn = gr.Button(value="👉 Right is better", interactive=False)
+        with gr.Row():
+            for i in range(num_models):
+                label = "Model A" if i == 0 else "Model B"
+                with gr.Column():
+                    chatbots[i] = grChatbot(label=label, elem_id=f"chatbot{i}",
+                        visible=False).style(height=550)
+
+        with gr.Box() as button_row:
+            with gr.Row():
+                leftvote_btn = gr.Button(value="👈  A is better", interactive=False)
+                tie_btn = gr.Button(value="🤝  Tie", interactive=False)
+                rightvote_btn = gr.Button(value="👉  B is better", interactive=False)
 
     with gr.Row():
         with gr.Column(scale=20):
             textbox = gr.Textbox(
                 show_label=False,
                 placeholder="Enter text and press ENTER",
                 visible=False,
             ).style(container=False)
         with gr.Column(scale=1, min_width=50):
             send_btn = gr.Button(value="Send", visible=False)
 
     with gr.Row() as button_row2:
         regenerate_btn = gr.Button(value="🔄  Regenerate", interactive=False)
         clear_btn = gr.Button(value="🗑️  Clear history", interactive=False)
+        share_btn = gr.Button(value="📷  Share")
 
     with gr.Accordion("Parameters", open=False, visible=True) as parameter_row:
         temperature = gr.Slider(
             minimum=0.0,
             maximum=1.0,
             value=0.7,
             step=0.1,
@@ -318,14 +336,36 @@
     ).then(
         http_bot_all,
         states + model_selectors + [temperature, max_output_tokens],
         states + chatbots + btn_list,
     )
     clear_btn.click(clear_history, None, states + chatbots + [textbox] + btn_list)
 
+    share_js="""
+function (a, b, c, d) {
+    const captureElement = document.querySelector('#share-region');
+    html2canvas(captureElement)
+        .then(canvas => {
+            canvas.style.display = 'none'
+            document.body.appendChild(canvas)
+            return canvas
+        })
+        .then(canvas => {
+            const image = canvas.toDataURL('image/png')
+            const a = document.createElement('a')
+            a.setAttribute('download', 'chatbot-arena.png')
+            a.setAttribute('href', image)
+            a.click()
+            canvas.remove()
+        });
+    return [a, b, c, d];
+}
+"""
+    share_btn.click(share_click, states + model_selectors, [], _js=share_js)
+
     for i in range(num_models):
         model_selectors[i].change(
             clear_history, None, states + chatbots + [textbox] + btn_list
         )
 
     textbox.submit(
         add_text, states + [textbox], states + chatbots + [textbox] + btn_list
@@ -349,100 +389,7 @@
         textbox,
         send_btn,
         button_row,
         button_row2,
         parameter_row,
     )
 
-
-def build_demo():
-    with gr.Blocks(
-        title="Chat with Open Large Language Models",
-        theme=gr.themes.Base(),
-        css=block_css,
-    ) as demo:
-        with gr.Tabs() as tabs:
-            with gr.Tab("Single Model", id=0):
-                (
-                    a_state,
-                    a_model_selector,
-                    a_chatbot,
-                    a_textbox,
-                    a_send_btn,
-                    a_button_row,
-                    a_parameter_row,
-                ) = build_single_model_ui()
-                a_list = [
-                    a_state,
-                    a_model_selector,
-                    a_chatbot,
-                    a_textbox,
-                    a_send_btn,
-                    a_button_row,
-                    a_parameter_row,
-                ]
-
-            with gr.Tab("Side-by-Side", id=1):
-                (
-                    b_states,
-                    b_model_selectors,
-                    b_chatbots,
-                    b_textbox,
-                    b_send_btn,
-                    b_button_row,
-                    b_button_row2,
-                    b_parameter_row,
-                ) = build_side_by_side_ui()
-                b_list = (
-                    b_states
-                    + b_model_selectors
-                    + b_chatbots
-                    + [
-                        b_textbox,
-                        b_send_btn,
-                        b_button_row,
-                        b_button_row2,
-                        b_parameter_row,
-                    ]
-                )
-
-        url_params = gr.JSON(visible=False)
-
-        if args.model_list_mode == "once":
-            demo.load(
-                load_demo,
-                [url_params],
-                [tabs] + a_list + b_list,
-                _js=get_window_url_params,
-            )
-        else:
-            raise ValueError(f"Unknown model list mode: {args.model_list_mode}")
-
-    return demo
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--host", type=str, default="0.0.0.0")
-    parser.add_argument("--port", type=int)
-    parser.add_argument("--controller-url", type=str, default="http://localhost:21001")
-    parser.add_argument("--concurrency-count", type=int, default=10)
-    parser.add_argument(
-        "--model-list-mode", type=str, default="once", choices=["once", "reload"]
-    )
-    parser.add_argument("--share", action="store_true")
-    parser.add_argument(
-        "--moderate", action="store_true", help="Enable content moderation"
-    )
-    args = parser.parse_args()
-    logger.info(f"args: {args}")
-
-    models = get_model_list(args.controller_url)
-    set_global_vars(args.controller_url, args.moderate, models)
-
-    logger.info(args)
-    demo = build_demo()
-    demo.queue(
-        concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
-    ).launch(
-        server_name=args.host, server_port=args.port, share=args.share, max_threads=200
-    )
```

### Comparing `fschat-0.2.3/fastchat/serve/huggingface_api.py` & `fschat-0.2.4/fastchat/serve/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/inference.py` & `fschat-0.2.4/fastchat/serve/inference.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,36 @@
     from transformers import (
         AutoTokenizer,
         AutoModelForCausalLM,
         LlamaTokenizer,
         LlamaForCausalLM,
         AutoModel,
         AutoModelForSeq2SeqLM,
+        T5Tokenizer,
+        AutoConfig,
     )
 except ImportError:
     from transformers import (
         AutoTokenizer,
         AutoModelForCausalLM,
         LLaMATokenizer,
         LLamaForCausalLM,
         AutoModel,
         AutoModelForSeq2SeqLM,
+        T5Tokenizer,
+        AutoConfig,
     )
 
 from fastchat.conversation import (
     conv_templates,
     get_default_conv_template,
     compute_skip_echo_len,
     SeparatorStyle,
 )
-from fastchat.serve.compression import compress_module
+from fastchat.serve.compression import load_compress_model
 from fastchat.serve.monkey_patch_non_inplace import (
     replace_llama_attn_with_non_inplace_operations,
 )
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 
 
 def raise_warning_for_old_weights(model_path, model):
@@ -73,15 +77,15 @@
     return gpu_memory
 
 
 def load_model(
     model_path, device, num_gpus, max_gpu_memory=None, load_8bit=False, debug=False
 ):
     if device == "cpu":
-        kwargs = {}
+        kwargs = {"torch_dtype": torch.float32}
     elif device == "cuda":
         kwargs = {"torch_dtype": torch.float16}
         if num_gpus == "auto":
             kwargs["device_map"] = "auto"
         else:
             num_gpus = int(num_gpus)
             if num_gpus != 1:
@@ -100,25 +104,30 @@
         print("init_kwargs", kwargs)
     elif device == "mps":
         kwargs = {"torch_dtype": torch.float16}
         # Avoid bugs in mps backend by not using in-place operations.
         replace_llama_attn_with_non_inplace_operations()
     else:
         raise ValueError(f"Invalid device: {device}")
+    
+    if load_8bit:
+        if num_gpus != 1 and num_gpus != "1":
+            warnings.warn("8-bit quantization is not supported for multi-gpu inference.")
+        else:
+            return load_compress_model(model_path=model_path, device=device, torch_dtype=kwargs["torch_dtype"])
 
     if "chatglm" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, trust_remote_code=True)
         model = AutoModel.from_pretrained(
             model_path, trust_remote_code=True, **kwargs
         ).cuda()
-    elif "google/flan-t5" in model_path:
-        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
-        model = AutoModelForSeq2SeqLM.from_pretrained(
-            model_path, low_cpu_mem_usage=True, **kwargs
-        )
+    elif "t5" in model_path:
+         model = AutoModelForSeq2SeqLM.from_pretrained(model_path,
+                                                       low_cpu_mem_usage=True, **kwargs)
+         tokenizer = T5Tokenizer.from_pretrained(model_path, use_fast=False)
     elif "dolly" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
         model = AutoModelForCausalLM.from_pretrained(
             model_path, low_cpu_mem_usage=True, **kwargs
         )
         # 50277 means "### End"
         tokenizer.eos_token_id = 50277
@@ -130,16 +139,14 @@
     else:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
         model = AutoModelForCausalLM.from_pretrained(
             model_path, low_cpu_mem_usage=True, **kwargs
         )
         raise_warning_for_old_weights(model_path, model)
 
-    if load_8bit:
-        compress_module(model, device)
 
     if (device == "cuda" and num_gpus == 1) or device == "mps":
         model.to(device)
 
     if debug:
         print(model)
 
@@ -156,57 +163,54 @@
     max_new_tokens = int(params.get("max_new_tokens", 256))
     stop_str = params.get("stop", None)
     stop_token_ids = params.get("stop_ids", [tokenizer.eos_token_id])
 
     input_ids = tokenizer(prompt).input_ids
     output_ids = list(input_ids)
 
-    max_src_len = context_len - max_new_tokens - 8
+    if model.config.is_encoder_decoder:
+         max_src_len = context_len
+    else:
+         max_src_len = context_len - max_new_tokens - 8
+
     input_ids = input_ids[-max_src_len:]
 
+    if model.config.is_encoder_decoder:
+         encoder_output = model.encoder(input_ids=torch.as_tensor([input_ids],
+                                                      device=device))[0]
+         start_ids = torch.as_tensor([[model.generation_config.decoder_start_token_id]],
+                     dtype=torch.int64, device=device)
+
     for i in range(max_new_tokens):
         if i == 0:
             if model.config.is_encoder_decoder:
-                encoder_outputs = model.encoder(
-                    input_ids=torch.as_tensor([input_ids], device=device)
-                )
-                out = model(
-                    torch.as_tensor([input_ids], device=device),
-                    decoder_input_ids=torch.as_tensor(
-                        [[model.generation_config.decoder_start_token_id]],
-                        device=device,
-                    ),
-                    encoder_outputs=encoder_outputs,
-                    use_cache=True,
-                )
-                logits = out.logits
-                past_key_values = out.past_key_values
+                 out = model.decoder(input_ids=start_ids,
+                                     encoder_hidden_states=encoder_output,
+                                     use_cache=True)
+                 logits = model.lm_head(out[0])
             else:
                 out = model(torch.as_tensor([input_ids], device=device), use_cache=True)
                 logits = out.logits
-                past_key_values = out.past_key_values
+            past_key_values = out.past_key_values
         else:
             if model.config.is_encoder_decoder:
-                out = model(
-                    input_ids=torch.as_tensor([input_ids], device=device),
-                    use_cache=True,
-                    encoder_outputs=encoder_outputs,
-                    decoder_input_ids=torch.as_tensor([[token]], device=device),
-                    past_key_values=past_key_values,
-                )
-                logits = out.logits
-                past_key_values = out.past_key_values
+                out = model.decoder(input_ids=torch.as_tensor([[token]], device=device),
+                             encoder_hidden_states=encoder_output,
+                             use_cache=True,
+                             past_key_values=past_key_values)
+
+                logits = model.lm_head(out[0])
             else:
                 out = model(
                     input_ids=torch.as_tensor([[token]], device=device),
                     use_cache=True,
                     past_key_values=past_key_values,
                 )
                 logits = out.logits
-                past_key_values = out.past_key_values
+            past_key_values = out.past_key_values
 
         last_token_logits = logits[0][-1]
 
         if device == "mps":
             # Switch to CPU by avoiding some bugs in mps backend.
             last_token_logits = last_token_logits.float().to("cpu")
 
@@ -220,15 +224,19 @@
 
         if token in stop_token_ids:
             stopped = True
         else:
             stopped = False
 
         if i % stream_interval == 0 or i == max_new_tokens - 1 or stopped:
-            output = tokenizer.decode(output_ids, skip_special_tokens=True)
+            if "t5" in model.config._name_or_path:
+                output = tokenizer.decode(output_ids, skip_special_tokens=True, 
+                                          spaces_between_special_tokens=False)
+            else:
+                output = tokenizer.decode(output_ids, skip_special_tokens=True)
             if stop_str:
                 pos = output.rfind(stop_str, l_prompt)
                 if pos != -1:
                     output = output[:pos]
                     stopped = True
             yield output
 
@@ -292,21 +300,26 @@
             prompt = conv.messages[conv.offset :]
             generate_stream_func = chatglm_generate_stream
         else:
             generate_stream_func = generate_stream
             prompt = conv.get_prompt()
 
         skip_echo_len = compute_skip_echo_len(model_path, conv, prompt)
+        stop_str = (
+            conv.sep
+            if conv.sep_style in [SeparatorStyle.SINGLE, SeparatorStyle.BAIZE]
+            else None
+        )
 
         params = {
             "model": model_path,
             "prompt": prompt,
             "temperature": temperature,
             "max_new_tokens": max_new_tokens,
-            "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else None,
+            "stop": stop_str,
         }
 
         chatio.prompt_for_output(conv.roles[1])
         output_stream = generate_stream_func(model, tokenizer, params, device)
         outputs = chatio.stream_output(output_stream, skip_echo_len)
         # NOTE: strip is important to align with the training data.
         conv.messages[-1][-1] = outputs.strip()
```

### Comparing `fschat-0.2.3/fastchat/serve/model_worker.py` & `fschat-0.2.4/fastchat/serve/model_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 A model worker executes the model.
 """
 import argparse
 import asyncio
 import dataclasses
 import logging
 import json
+import os
 import time
 from typing import List, Union
 import threading
 import uuid
 
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.responses import StreamingResponse
@@ -226,25 +227,36 @@
     )
     parser.add_argument("--model-name", type=str, help="Optional name")
     parser.add_argument(
         "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
     )
     parser.add_argument("--num-gpus", type=int, default=1)
     parser.add_argument(
+        "--gpus",
+        type=str,
+        default=None,
+        help="A single GPU like 1 or multiple GPUs like 0,2"
+    )
+    parser.add_argument(
         "--max-gpu-memory",
         type=str,
         help="The maximum memory per gpu. Use a string like '13Gib'",
     )
     parser.add_argument("--load-8bit", action="store_true")
     parser.add_argument("--limit-model-concurrency", type=int, default=5)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
+    if args.gpus:
+        if args.num_gpus and len(args.gpus.split(",")) < int(args.num_gpus):
+            raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
+        os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
+    
     worker = ModelWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
         args.no_register,
         args.model_path,
         args.model_name,
```

### Comparing `fschat-0.2.3/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.4/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/register_worker.py` & `fschat-0.2.4/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/serve_chatglm.py` & `fschat-0.2.4/fastchat/serve/serve_chatglm.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/test_message.py` & `fschat-0.2.4/fastchat/serve/test_message.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/serve/test_throughput.py` & `fschat-0.2.4/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.4/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/train/train.py` & `fschat-0.2.4/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
         super(SupervisedDataset, self).__init__()
         rank0_print("Loading data...")
         list_data_dict = json.load(open(data_path, "r"))
 
         rank0_print("Formatting inputs...")
         sources = [example["conversations"] for example in list_data_dict]
         data_dict = preprocess(sources, tokenizer)
+        print("!")
+        exit()
 
         self.input_ids = data_dict["input_ids"]
         self.labels = data_dict["labels"]
         self.attention_mask = data_dict["attention_mask"]
 
     def __len__(self):
         return len(self.input_ids)
@@ -216,16 +218,20 @@
     global local_rank
 
     parser = transformers.HfArgumentParser(
         (ModelArguments, DataArguments, TrainingArguments)
     )
     model_args, data_args, training_args = parser.parse_args_into_dataclasses()
     local_rank = training_args.local_rank
+    #model = transformers.AutoModelForCausalLM.from_pretrained(
+    #    model_args.model_name_or_path,
+    #    cache_dir=training_args.cache_dir,
+    #)
     model = transformers.AutoModelForCausalLM.from_pretrained(
-        model_args.model_name_or_path,
+        "facebook/opt-350m",
         cache_dir=training_args.cache_dir,
     )
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
         model_max_length=training_args.model_max_length,
         padding_side="right",
```

### Comparing `fschat-0.2.3/fastchat/train/train_lora.py` & `fschat-0.2.4/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.3/fastchat/utils.py` & `fschat-0.2.4/fastchat/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import datetime
 import logging
 import logging.handlers
 import os
 import sys
 import json
+import warnings
+import platform
 
 import requests
 import torch
 
 from fastchat.constants import LOGDIR
 
 server_error_msg = (
@@ -26,15 +27,22 @@
     formatter = logging.Formatter(
         fmt="%(asctime)s | %(levelname)s | %(name)s | %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     # Set the format of root handlers
     if not logging.getLogger().handlers:
-        logging.basicConfig(level=logging.INFO, encoding="utf-8")
+        if sys.version_info[1] >= 9:
+            # This is for windows
+            logging.basicConfig(level=logging.INFO, encoding="utf-8")
+        else:
+            if platform.system() == "Windows":
+                warnings.warn("If you are running on Windows, "
+                              "we recommend you use Python >= 3.9 for UTF-8 encoding.")
+            logging.basicConfig(level=logging.INFO)
     logging.getLogger().handlers[0].setFormatter(formatter)
 
     # Redirect stdout and stderr to loggers
     stdout_logger = logging.getLogger("stdout")
     stdout_logger.setLevel(logging.INFO)
     sl = StreamToLogger(stdout_logger, logging.INFO)
     sys.stdout = sl
```

### Comparing `fschat-0.2.3/fschat.egg-info/PKG-INFO` & `fschat-0.2.4/fschat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.3
+Version: 0.2.4
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastChat
+| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
-
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
 </p>
 
+- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
+
 - 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
-Join our [Discord](https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://twitter.com/lmsysorg) to get the latest updates.
-
 ## Contents
 - [Install](#install)
 - [Vicuna Weights](#vicuna-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
 - [Serving with Web GUI](#serving-with-web-gui)
 - [API](#api)
 - [Evaluation](#evaluation)
@@ -74,27 +75,33 @@
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v1.1
+    --base-model-path /path/to/llama-7b \
+    --target-model-path /output/path/to/vicuna-7b \
+    --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v1.1
+    --base-model-path /path/to/llama-13b \
+    --target-model-path /output/path/to/vicuna-13b \
+    --delta-path lmsys/vicuna-13b-delta-v1.1
+```
+
+### Fastchat-T5
+This model is stored in a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply run the line below to start chatting.
+```bash
+python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
 
 ### Low CPU Memory Conversion
```

#### html2text {}

```diff
@@ -1,87 +1,92 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.3 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.4 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat An open platform for training, serving,
-and evaluating large language model based chatbots. ## Release
+dev License-File: LICENSE # FastChat | [Discord](https://discord.gg/h6kCZb72G7)
+| [Twitter](https://twitter.com/lmsysorg) | An open platform for training,
+serving, and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
-- ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
-ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
-[demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
-(https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
-twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
-(#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
-Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
-(#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
-fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
-the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
-FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
-``fschat >= 0.2.0``. Please update your local packages accordingly. If you
-follow the above commands to do a fresh install, then you should get all the
-correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
-CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
-enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
-llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
-See the "Low CPU Memory Conversion" section below if you do not have enough
-memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
-13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
-``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ### Low CPU Memory Conversion
-You can try these methods to reduce the CPU RAM requirement of weight
-conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
-large weight files into smaller ones and use the disk as temporary storage.
-This can keep the peak memory at less than 16GB. 2. Create a large swap file
-and rely on the operating system to automatically utilize the disk as virtual
-memory. ## Inference with Command Line Interface (Experimental Feature: You can
-specify `--style rich` to enable rich text output and better text streaming
-quality for some non-ASCII content. This may not work properly on certain
-terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
-requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
-Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
-memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
-``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
-from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
-the CPU only and does not require GPU. It requires around 60GB of CPU memory
-for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
-Other Platforms If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
---model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
-exploring more methods to make the model easier to run on more platforms.
-Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. Here
-are the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
+[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
+Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
+vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
+## Contents - [Install](#install) - [Vicuna Weights](#vicuna-weights) -
+[Inference with Command Line Interface](#inference-with-command-line-interface)
+- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
+(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
+```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
+repository and navigate to the FastChat folder ```bash git clone https://
+github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
+```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
+upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Vicuna Weights We
+release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply
+with the LLaMA model license. You can add our delta to the original LLaMA
+weights to obtain the Vicuna weights. Instructions: 1. Get the original LLaMA
+weights in the huggingface format by following the instructions [here](https://
+huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
+scripts to get Vicuna weights by applying our delta. They will automatically
+download delta weights from our Hugging Face [account](https://huggingface.co/
+lmsys). **NOTE**: Weights v1.1 are only compatible with
+```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
+packages accordingly. If you follow the above commands to do a fresh install,
+then you should get all the correct versions. ### Vicuna-7B This conversion
+command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
+section below if you do not have enough memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
+model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
+``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
+the "Low CPU Memory Conversion" section below if you do not have enough memory.
+```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
+llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
+lmsys/vicuna-13b-delta-v1.1 ``` ### Fastchat-T5 This model is stored in a
+Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). Simply
+run the line below to start chatting. ```bash python3 -m fastchat.serve.cli --
+model-path lmsys/fastchat-t5-3b-v1.0 ``` ### Old weights See [docs/
+weights_version.md](docs/weights_version.md) for all versions of weights and
+their differences. ### Low CPU Memory Conversion You can try these methods to
+reduce the CPU RAM requirement of weight conversion. 1. Append `--low-cpu-mem`
+to the commands above, which will split large weight files into smaller ones
+and use the disk as temporary storage. This can keep the peak memory at less
+than 16GB. 2. Create a large swap file and rely on the operating system to
+automatically utilize the disk as virtual memory. ## Inference with Command
+Line Interface (Experimental Feature: You can specify `--style rich` to enable
+rich text output and better text streaming quality for some non-ASCII content.
+This may not work properly on certain terminals.) [assets/screenshot_cli.png]
+#### Single GPU The command below requires around 28GB of GPU memory for
+Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory"
+section below if you do not have enough memory. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights ``` #### Multiple
+GPUs You can use model parallelism to aggregate GPU memory from multiple GPUs
+on the same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and
+does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and
+around 30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device cpu ``` #### Metal Backend (Mac
+Computers with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU
+acceleration on Mac computers (requires torch >= 2.0). Use `--load-8bit` to
+turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB
+M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other Platforms
+If you do not have enough memory, you can enable 8-bit compression by adding `-
+-load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+vicuna/weights --load-8bit ``` Besides, we are actively exploring more methods
+to make the model easier to run on more platforms. Contributions and pull
+requests are welcome. ## Serving with Web GUI [assets/screenshot_gui.png] To
+serve using the web UI, you need three main components: web servers that
+interface with users, model workers that host one or more models, and a
+controller to coordinate the webserver and model workers. Here are the commands
+to follow in your terminal: #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.3/pyproject.toml` & `fschat-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.3"
+version = "0.2.4"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "accelerate", "fastapi", "gradio==3.23", "markdown2[all]", "numpy",
     "prompt_toolkit>=3.0.0", "requests", "rich>=10.0.0", "sentencepiece",
-    "shortuuid", "transformers>=4.28.0", "tokenizers>=0.12.1", "torch",
-    "uvicorn", "wandb", "httpx", "shortuuid", "pydantic",
+    "shortuuid", "transformers>=4.28.0,<4.29.0", "tokenizers>=0.12.1", "torch",
+    "uvicorn", "wandb", "httpx", "shortuuid", "pydantic", "nh3",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
```

