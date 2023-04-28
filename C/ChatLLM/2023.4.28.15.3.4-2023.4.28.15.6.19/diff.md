# Comparing `tmp/ChatLLM-2023.4.28.15.3.4.tar.gz` & `tmp/ChatLLM-2023.4.28.15.6.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.28.15.3.4.tar", last modified: Fri Apr 28 07:03:05 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.28.15.6.19.tar", last modified: Fri Apr 28 07:06:19 2023, max compression
```

## Comparing `ChatLLM-2023.4.28.15.3.4.tar` & `ChatLLM-2023.4.28.15.6.19.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.119487 ChatLLM-2023.4.28.15.3.4/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.15.3.4/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.078849 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5625 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 07:03:05.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 07:03:04.000000 ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5625 2023-04-28 07:03:05.119292 ChatLLM-2023.4.28.15.3.4/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.3.4/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.15.3.4/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.079503 ChatLLM-2023.4.28.15.3.4/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.080642 ChatLLM-2023.4.28.15.3.4/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.15.3.4/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.3.4/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.15.3.4/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.3.4/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.081130 ChatLLM-2023.4.28.15.3.4/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.15.3.4/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.15.3.4/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.084277 ChatLLM-2023.4.28.15.3.4/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3835 2023-04-28 06:51:54.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.15.3.4/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.15.3.4/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.085172 ChatLLM-2023.4.28.15.3.4/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1313 2023-04-28 07:01:03.000000 ChatLLM-2023.4.28.15.3.4/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.15.3.4/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.085626 ChatLLM-2023.4.28.15.3.4/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.15.3.4/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.15.3.4/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.086728 ChatLLM-2023.4.28.15.3.4/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.15.3.4/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.15.3.4/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2033 2023-04-28 04:49:58.000000 ChatLLM-2023.4.28.15.3.4/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.15.3.4/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.088596 ChatLLM-2023.4.28.15.3.4/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.15.3.4/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.092789 ChatLLM-2023.4.28.15.3.4/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.100371 ChatLLM-2023.4.28.15.3.4/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.15.3.4/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.15.3.4/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.15.3.4/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.15.3.4/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.15.3.4/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.105373 ChatLLM-2023.4.28.15.3.4/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.15.3.4/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.15.3.4/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.3.4/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.3.4/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.3.4/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.15.3.4/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.3.4/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.118048 ChatLLM-2023.4.28.15.3.4/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.3.4/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.15.3.4/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.15.3.4/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.15.3.4/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.15.3.4/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 07:03:05.119557 ChatLLM-2023.4.28.15.3.4/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.15.3.4/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:03:05.118552 ChatLLM-2023.4.28.15.3.4/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.15.3.4/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.3.4/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.791951 ChatLLM-2023.4.28.15.6.19/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.15.6.19/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.752747 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 07:06:19.791788 ChatLLM-2023.4.28.15.6.19/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.6.19/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.15.6.19/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.753382 ChatLLM-2023.4.28.15.6.19/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.754430 ChatLLM-2023.4.28.15.6.19/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.754902 ChatLLM-2023.4.28.15.6.19/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.15.6.19/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.15.6.19/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.757663 ChatLLM-2023.4.28.15.6.19/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-28 07:06:18.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.15.6.19/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.758290 ChatLLM-2023.4.28.15.6.19/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.15.6.19/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.758776 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.759731 ChatLLM-2023.4.28.15.6.19/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2142 2023-04-28 07:05:00.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.761335 ChatLLM-2023.4.28.15.6.19/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.765662 ChatLLM-2023.4.28.15.6.19/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.772001 ChatLLM-2023.4.28.15.6.19/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.777544 ChatLLM-2023.4.28.15.6.19/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.15.6.19/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.15.6.19/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.15.6.19/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.790426 ChatLLM-2023.4.28.15.6.19/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.6.19/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.15.6.19/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.15.6.19/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.15.6.19/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.15.6.19/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 07:06:19.792001 ChatLLM-2023.4.28.15.6.19/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.15.6.19/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.791016 ChatLLM-2023.4.28.15.6.19/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.15.6.19/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tox.ini
```

### Comparing `ChatLLM-2023.4.28.15.3.4/.gitignore` & `ChatLLM-2023.4.28.15.6.19/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/.travis.yml` & `ChatLLM-2023.4.28.15.6.19/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/CONTRIBUTING.rst` & `ChatLLM-2023.4.28.15.6.19/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.15.3.4
+Version: 2023.4.28.15.6.19
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.15.3.4/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/LICENSE` & `ChatLLM-2023.4.28.15.6.19/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/Makefile` & `ChatLLM-2023.4.28.15.6.19/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/PKG-INFO` & `ChatLLM-2023.4.28.15.6.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.15.3.4
+Version: 2023.4.28.15.6.19
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.15.3.4/README.md` & `ChatLLM-2023.4.28.15.6.19/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/_his/_qa.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/api/stream_api.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatann.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         def gen(**input):
             for response, _ in self.qa(**input):
                 yield f"{response}\n"
 
         @app.route(rule=path, methods=['GET', 'POST'])
         def stream():
-            input = {'query': '你是谁'}
+            input = {'query': '1+1等于几'}
             input.update(request.args.to_dict())
             if request.data.startswith(b'{'):
                 input.update(json.loads(request.data))
 
             return Response(gen(**input), mimetype='text/event-stream')
 
         app.run(host=host, port=port, debug=False)
```

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/chatyuan.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/clis/cli.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/clis/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def f(a=1, **kw):
     print(a)
     print(kw)
 
 
 @cli.command(help="help")  # help会覆盖docstring
-def clitest(**kwargs):
+def clitest(**kwargs): # 不支持 **kwargs
     f(**kwargs)
 
 
 @cli.command()  # help会覆盖docstring
 def webui(name: str = 'chatpdf', port=8501):
     """
         chatllm-run webui --name chatpdf --port 8501
```

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/embedding.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/utils/common.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 DEVICE = (
     os.environ['DEVICE']
     if 'DEVICE' in os.environ else "cuda"
     if torch.cuda.is_available() else "mps"
     if torch.backends.mps.is_available() else "cpu"
 )
+if LOCAL_HOST.startswith('10.219'):
+    MODEL_PATH = "/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
 
 
 # todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
```

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.28.15.6.19/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/imgs/LLM.png` & `ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/imgs/role.png` & `ChatLLM-2023.4.28.15.6.19/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.28.15.6.19/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/医/古今医统大全.txt` & `ChatLLM-2023.4.28.15.6.19/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/姚明.txt` & `ChatLLM-2023.4.28.15.6.19/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/王治郅.txt` & `ChatLLM-2023.4.28.15.6.19/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/科比.txt` & `ChatLLM-2023.4.28.15.6.19/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/data/财报.pdf` & `ChatLLM-2023.4.28.15.6.19/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/docs/INSTALL.md` & `ChatLLM-2023.4.28.15.6.19/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/docs/Makefile` & `ChatLLM-2023.4.28.15.6.19/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/docs/README.md` & `ChatLLM-2023.4.28.15.6.19/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/docs/conf.py` & `ChatLLM-2023.4.28.15.6.19/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/docs/make.bat` & `ChatLLM-2023.4.28.15.6.19/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/setup.py` & `ChatLLM-2023.4.28.15.6.19/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/tests/test_llm4gpt.py` & `ChatLLM-2023.4.28.15.6.19/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.3.4/tests/内存型.ipynb` & `ChatLLM-2023.4.28.15.6.19/tests/内存型.ipynb`

 * *Files identical despite different names*

