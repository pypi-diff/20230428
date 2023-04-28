# Comparing `tmp/ChatLLM-2023.4.28.14.25.57.tar.gz` & `tmp/ChatLLM-2023.4.28.14.33.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.28.14.25.57.tar", last modified: Fri Apr 28 06:25:58 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.28.14.33.15.tar", last modified: Fri Apr 28 06:33:16 2023, max compression
```

## Comparing `ChatLLM-2023.4.28.14.25.57.tar` & `ChatLLM-2023.4.28.14.33.15.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.186381 ChatLLM-2023.4.28.14.25.57/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.14.25.57/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.146347 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5627 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 06:25:58.000000 ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5627 2023-04-28 06:25:58.186228 ChatLLM-2023.4.28.14.25.57/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.14.25.57/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.14.25.57/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.146968 ChatLLM-2023.4.28.14.25.57/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.148357 ChatLLM-2023.4.28.14.25.57/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.14.25.57/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.14.25.57/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.14.25.57/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.14.25.57/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.148842 ChatLLM-2023.4.28.14.25.57/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.14.25.57/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.14.25.57/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.152181 ChatLLM-2023.4.28.14.25.57/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3864 2023-04-28 06:25:56.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.14.25.57/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.14.25.57/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.152816 ChatLLM-2023.4.28.14.25.57/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.14.25.57/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.14.25.57/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.153325 ChatLLM-2023.4.28.14.25.57/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.14.25.57/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.14.25.57/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.154518 ChatLLM-2023.4.28.14.25.57/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.14.25.57/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.14.25.57/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2033 2023-04-28 04:49:58.000000 ChatLLM-2023.4.28.14.25.57/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.14.25.57/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.156234 ChatLLM-2023.4.28.14.25.57/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.14.25.57/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.160240 ChatLLM-2023.4.28.14.25.57/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.167543 ChatLLM-2023.4.28.14.25.57/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.14.25.57/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.14.25.57/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.14.25.57/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.14.25.57/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.14.25.57/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.171279 ChatLLM-2023.4.28.14.25.57/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.14.25.57/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.14.25.57/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.25.57/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.25.57/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.25.57/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.14.25.57/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.25.57/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.185068 ChatLLM-2023.4.28.14.25.57/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.14.25.57/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.14.25.57/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.14.25.57/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.14.25.57/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.14.25.57/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 06:25:58.186433 ChatLLM-2023.4.28.14.25.57/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.14.25.57/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:25:58.185513 ChatLLM-2023.4.28.14.25.57/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.14.25.57/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.25.57/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.072651 ChatLLM-2023.4.28.14.33.15/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.14.33.15/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.035728 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5627 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 06:33:15.000000 ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5627 2023-04-28 06:33:16.072486 ChatLLM-2023.4.28.14.33.15/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.14.33.15/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.14.33.15/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.036207 ChatLLM-2023.4.28.14.33.15/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.037164 ChatLLM-2023.4.28.14.33.15/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.14.33.15/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.14.33.15/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.14.33.15/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.14.33.15/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.037573 ChatLLM-2023.4.28.14.33.15/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.14.33.15/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.14.33.15/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.040036 ChatLLM-2023.4.28.14.33.15/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3864 2023-04-28 06:33:14.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.14.33.15/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.14.33.15/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.040568 ChatLLM-2023.4.28.14.33.15/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1672 2023-04-28 06:33:14.000000 ChatLLM-2023.4.28.14.33.15/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.14.33.15/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.040915 ChatLLM-2023.4.28.14.33.15/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.14.33.15/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.14.33.15/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.041590 ChatLLM-2023.4.28.14.33.15/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.14.33.15/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.14.33.15/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2033 2023-04-28 04:49:58.000000 ChatLLM-2023.4.28.14.33.15/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.14.33.15/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.043019 ChatLLM-2023.4.28.14.33.15/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.14.33.15/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.046764 ChatLLM-2023.4.28.14.33.15/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.053696 ChatLLM-2023.4.28.14.33.15/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.14.33.15/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.14.33.15/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.14.33.15/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.14.33.15/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.14.33.15/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.057279 ChatLLM-2023.4.28.14.33.15/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.14.33.15/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.14.33.15/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.33.15/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.33.15/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.33.15/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.14.33.15/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.14.33.15/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.071315 ChatLLM-2023.4.28.14.33.15/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.14.33.15/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.14.33.15/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.14.33.15/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.14.33.15/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.14.33.15/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 06:33:16.072712 ChatLLM-2023.4.28.14.33.15/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.14.33.15/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 06:33:16.071826 ChatLLM-2023.4.28.14.33.15/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.14.33.15/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.14.33.15/tox.ini
```

### Comparing `ChatLLM-2023.4.28.14.25.57/.gitignore` & `ChatLLM-2023.4.28.14.33.15/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/.travis.yml` & `ChatLLM-2023.4.28.14.33.15/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/CONTRIBUTING.rst` & `ChatLLM-2023.4.28.14.33.15/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.14.25.57
+Version: 2023.4.28.14.33.15
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.14.25.57/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.28.14.33.15/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/LICENSE` & `ChatLLM-2023.4.28.14.33.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/Makefile` & `ChatLLM-2023.4.28.14.33.15/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/PKG-INFO` & `ChatLLM-2023.4.28.14.33.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.14.25.57
+Version: 2023.4.28.14.33.15
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.14.25.57/README.md` & `ChatLLM-2023.4.28.14.33.15/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/_his/_qa.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/api/stream_api.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatann.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/chatyuan.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/embedding.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/utils/common.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.28.14.33.15/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.28.14.33.15/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/imgs/LLM.png` & `ChatLLM-2023.4.28.14.33.15/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.28.14.33.15/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.28.14.33.15/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/imgs/role.png` & `ChatLLM-2023.4.28.14.33.15/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.28.14.33.15/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/医/古今医统大全.txt` & `ChatLLM-2023.4.28.14.33.15/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/姚明.txt` & `ChatLLM-2023.4.28.14.33.15/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/王治郅.txt` & `ChatLLM-2023.4.28.14.33.15/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/科比.txt` & `ChatLLM-2023.4.28.14.33.15/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/data/财报.pdf` & `ChatLLM-2023.4.28.14.33.15/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/docs/INSTALL.md` & `ChatLLM-2023.4.28.14.33.15/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/docs/Makefile` & `ChatLLM-2023.4.28.14.33.15/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/docs/README.md` & `ChatLLM-2023.4.28.14.33.15/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/docs/conf.py` & `ChatLLM-2023.4.28.14.33.15/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/docs/make.bat` & `ChatLLM-2023.4.28.14.33.15/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/setup.py` & `ChatLLM-2023.4.28.14.33.15/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/tests/test_llm4gpt.py` & `ChatLLM-2023.4.28.14.33.15/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.14.25.57/tests/内存型.ipynb` & `ChatLLM-2023.4.28.14.33.15/tests/内存型.ipynb`

 * *Files identical despite different names*

