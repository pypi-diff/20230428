# Comparing `tmp/ChatLLM-2023.4.27.18.6.56.tar.gz` & `tmp/ChatLLM-2023.4.28.12.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.27.18.6.56.tar", last modified: Thu Apr 27 10:06:57 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.28.12.8.1.tar", last modified: Fri Apr 28 04:08:01 2023, max compression
```

## Comparing `ChatLLM-2023.4.27.18.6.56.tar` & `ChatLLM-2023.4.28.12.8.1.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.021376 ChatLLM-2023.4.27.18.6.56/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.27.18.6.56/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.984465 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     4120 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1768 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-27 10:06:56.000000 ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4120 2023-04-27 10:06:57.021227 ChatLLM-2023.4.27.18.6.56/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.6.56/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     3304 2023-04-27 06:03:48.000000 ChatLLM-2023.4.27.18.6.56/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.985271 ChatLLM-2023.4.27.18.6.56/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.985923 ChatLLM-2023.4.27.18.6.56/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.27.18.6.56/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.988523 ChatLLM-2023.4.27.18.6.56/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3400 2023-04-27 09:24:25.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.27.18.6.56/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.27.18.6.56/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.989082 ChatLLM-2023.4.27.18.6.56/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.6.56/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.27.18.6.56/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.989569 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.27.18.6.56/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3533 2023-04-27 04:23:17.000000 ChatLLM-2023.4.27.18.6.56/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.991027 ChatLLM-2023.4.27.18.6.56/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.27.18.6.56/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.994925 ChatLLM-2023.4.27.18.6.56/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:56.998749 ChatLLM-2023.4.27.18.6.56/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf_ann_df.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.005481 ChatLLM-2023.4.27.18.6.56/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.27.18.6.56/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.27.18.6.56/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.27.18.6.56/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.27.18.6.56/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.020622 ChatLLM-2023.4.27.18.6.56/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.27.18.6.56/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     3260 2023-04-26 08:57:26.000000 ChatLLM-2023.4.27.18.6.56/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.27.18.6.56/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.27.18.6.56/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.27.18.6.56/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.27.18.6.56/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-27 10:06:57.021421 ChatLLM-2023.4.27.18.6.56/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.27.18.6.56/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-27 10:06:57.020980 ChatLLM-2023.4.27.18.6.56/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.27.18.6.56/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.621317 ChatLLM-2023.4.28.12.8.1/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.12.8.1/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.584139 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5625 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1824 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 04:08:01.000000 ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5625 2023-04-28 04:08:01.621167 ChatLLM-2023.4.28.12.8.1/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.12.8.1/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.12.8.1/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.585042 ChatLLM-2023.4.28.12.8.1/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.585564 ChatLLM-2023.4.28.12.8.1/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.12.8.1/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.12.8.1/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.12.8.1/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.12.8.1/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.586080 ChatLLM-2023.4.28.12.8.1/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.12.8.1/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.12.8.1/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.587926 ChatLLM-2023.4.28.12.8.1/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3410 2023-04-27 10:30:13.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.12.8.1/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.12.8.1/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.588583 ChatLLM-2023.4.28.12.8.1/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.12.8.1/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.12.8.1/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.588955 ChatLLM-2023.4.28.12.8.1/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.12.8.1/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.12.8.1/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3725 2023-04-28 04:07:23.000000 ChatLLM-2023.4.28.12.8.1/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.590059 ChatLLM-2023.4.28.12.8.1/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.12.8.1/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.594124 ChatLLM-2023.4.28.12.8.1/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.600504 ChatLLM-2023.4.28.12.8.1/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.12.8.1/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.606042 ChatLLM-2023.4.28.12.8.1/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.12.8.1/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.12.8.1/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.8.1/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.8.1/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.8.1/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.12.8.1/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.8.1/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.620494 ChatLLM-2023.4.28.12.8.1/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.12.8.1/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.12.8.1/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.12.8.1/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.12.8.1/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.12.8.1/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 04:08:01.621368 ChatLLM-2023.4.28.12.8.1/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.12.8.1/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:08:01.620907 ChatLLM-2023.4.28.12.8.1/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.12.8.1/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.8.1/tox.ini
```

### Comparing `ChatLLM-2023.4.27.18.6.56/.gitignore` & `ChatLLM-2023.4.28.12.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/.travis.yml` & `ChatLLM-2023.4.28.12.8.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/CONTRIBUTING.rst` & `ChatLLM-2023.4.28.12.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 chatllm/chatyuan.py
 chatllm/embedding.py
 chatllm/utils.py
 chatllm/_his/FaissANN.py
 chatllm/_his/__init__.py
 chatllm/_his/_chatllm.py
 chatllm/_his/_qa.py
+chatllm/api/__init__.py
+chatllm/api/stream_api.py
 chatllm/applications/Question2Answer.py
 chatllm/applications/__init__.py
 chatllm/applications/chatann.py
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatpdf.py
@@ -57,25 +59,25 @@
 data/科比.txt
 data/财报.pdf
 data/马保国.txt
 data/imgs/LLM.drawio.png
 data/imgs/LLM.png
 data/imgs/chatpdf.gif
 data/imgs/chatpdf_ann_df.png
+data/imgs/role.png
 data/医/500种中药现代研究.txt
 data/医/古今医统大全.txt
 docs/INSTALL.md
 docs/Makefile
 docs/README.md
 docs/_config.yml
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
-docs/img.png
 docs/index.rst
-docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
-tests/test_llm4gpt.py
+tests/test_llm4gpt.py
+tests/内存型.ipynb
```

### Comparing `ChatLLM-2023.4.27.18.6.56/LICENSE` & `ChatLLM-2023.4.28.12.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/Makefile` & `ChatLLM-2023.4.28.12.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/_his/_qa.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatann.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,34 @@
 from chatllm.utils import DEVICE, load_llm4chat
 
 
 class ChatBase(object):
 
     def __init__(self, chat_func=None, prompt_template=None, role=''):
         self.chat_func = chat_func
-        self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
-        self.role = role or os.environ.get('LLM_ROLE', '')
+        self.prompt_template = prompt_template or self.default_document_prompt
 
         #
         self.history = []
         self.knowledge_base = None
+        self.role = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
     def qa(self, query, knowledge_base='', **kwargs):
-        """可重写"""
+        """重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
-    def _qa(self, query, knowledge_base='', max_turns=1):
+    def _qa(self, query, knowledge_base='', role='', max_turns=1):
+        self.role = role or os.environ.get('LLM_ROLE', '')
         self.knowledge_base = knowledge_base if knowledge_base.strip() else '请自由回答'
 
         query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role)
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
```

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/chatyuan.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/clis/cli.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/embedding.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/utils.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # @Software     : PyCharm
 # @Description  :
 import torch
 from transformers import AutoTokenizer, AutoModel
 
 from meutils.pipe import *
 
+# os.environ["CUDA_VISIBLE_DEVICES"] = "0,1,2"
+
 DEVICE = (
     os.environ['DEVICE']
     if 'DEVICE' in os.environ else "cuda"
     if torch.cuda.is_available() else "mps"
     if torch.backends.mps.is_available() else "cpu"
 )
 
@@ -30,64 +32,69 @@
     model, tokenizer = load_llm(model_name_or_path, device, **kwargs)
     if stream and hasattr(model, 'stream_chat'):
         return partial(model.stream_chat, tokenizer=tokenizer)
     else:
         return partial(model.chat, tokenizer=tokenizer)
 
 
-def load_llm(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, device_map: Optional[Dict[str, int]] = None,
+def load_llm(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, num_gpus=1, checkpoint="chatglm_checkpoint",
              **kwargs):
     tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
-    model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True, **kwargs)
+    model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True)
 
     if torch.cuda.is_available() and device.lower().startswith("cuda"):
-        # 根据当前设备GPU数量决定是否进行多卡部署
-        num_gpus = torch.cuda.device_count()
-        if num_gpus < 2 and device_map is None:
+        if num_gpus == 1:  # 单卡
             model = model.half().cuda()
             # model.transformer.prefix_encoder.float()
-
-        else:
-            from accelerate import dispatch_model
-            # 可传入device_map自定义每张卡的部署情况
-            if device_map is None:
-                device_map = auto_configure_device_map(num_gpus)
-
-            model = dispatch_model(model, device_map=device_map).half().cuda()
+        elif 'chatglm' in model_name_or_path:  # 多卡
+            num_gpus = min(num_gpus, torch.cuda.device_count())
+            model = load_chatglm_on_gpus(model, model_name_or_path, num_gpus, checkpoint=checkpoint)
 
     else:
         model = model.float().to(device)
 
     return model.eval(), tokenizer
 
 
-def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
-    # transformer.word_embeddings 占用1层
-    # transformer.final_layernorm 和 lm_head 占用1层
-    # transformer.layers 占用 28 层
-    # 总共30层分配到num_gpus张卡上
-    num_trans_layers = 28
-    per_gpu_layers = 30 / num_gpus
+def load_chatglm_on_gpus(model, model_name_or_path, num_gpus=2, checkpoint="chatglm_checkpoint"):
+    """https://github.com/THUDM/ChatGLM-6B/issues/200"""
+    from accelerate import load_checkpoint_and_dispatch
+
+    device_map = auto_configure_device_map(num_gpus)
+    try:
+        model = load_checkpoint_and_dispatch(model, model_name_or_path, device_map=device_map, offload_folder="offload",
+                                             offload_state_dict=True).half()
+    except ValueError:
+        logger.info('多卡加载，第一次需要缓存模型')
+        model.save_pretrained(checkpoint, max_shard_size='2GB')
+        model = load_checkpoint_and_dispatch(model, checkpoint, device_map=device_map,
+                                             offload_folder="offload", offload_state_dict=True).half()
+    return model
 
-    # bugfix: 在linux中调用torch.embedding传入的weight,input不在同一device上,导致RuntimeError
-    # windows下 model.device 会被设置成 transformer.word_embeddings.device
-    # linux下 model.device 会被设置成 lm_head.device
-    # 在调用chat或者stream_chat时,input_ids会被放到model.device上
-    # 如果transformer.word_embeddings.device和model.device不同,则会导致RuntimeError
-    # 因此这里将transformer.word_embeddings,transformer.final_layernorm,lm_head都放到第一张卡上
-    device_map = {'transformer.word_embeddings': 0,
-                  'transformer.final_layernorm': 0, 'lm_head': 0}
 
-    used = 2
+def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
+    # 总共占用13GB显存,28层transformer每层0.39GB左右
+    # 第一层 word_embeddings和最后一层 lm_head 层各占用1.2GB左右
+    num_trans_layers = 28
+    vram_per_layer = 0.39
+    average = 13 / num_gpus
+    used = 1.2
+    device_map = {
+        'transformer.word_embeddings': 0,
+        'transformer.final_layernorm': num_gpus - 1,
+        'lm_head': num_gpus - 1
+    }
     gpu_target = 0
     for i in range(num_trans_layers):
-        if used >= per_gpu_layers:
+        if used > average - vram_per_layer / 2 and gpu_target < num_gpus:
             gpu_target += 1
             used = 0
-        assert gpu_target < num_gpus
+        else:
+            used += vram_per_layer
+
         device_map[f'transformer.layers.{i}'] = gpu_target
         used += 1
 
     return device_map
 
 
 if __name__ == '__main__':
```

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/imgs/LLM.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.28.12.8.1/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/医/古今医统大全.txt` & `ChatLLM-2023.4.28.12.8.1/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/姚明.txt` & `ChatLLM-2023.4.28.12.8.1/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/王治郅.txt` & `ChatLLM-2023.4.28.12.8.1/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/科比.txt` & `ChatLLM-2023.4.28.12.8.1/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/data/财报.pdf` & `ChatLLM-2023.4.28.12.8.1/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/docs/INSTALL.md` & `ChatLLM-2023.4.28.12.8.1/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/docs/Makefile` & `ChatLLM-2023.4.28.12.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/docs/conf.py` & `ChatLLM-2023.4.28.12.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/docs/make.bat` & `ChatLLM-2023.4.28.12.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/setup.py` & `ChatLLM-2023.4.28.12.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.27.18.6.56/tests/test_llm4gpt.py` & `ChatLLM-2023.4.28.12.8.1/tests/test_llm4gpt.py`

 * *Files identical despite different names*

