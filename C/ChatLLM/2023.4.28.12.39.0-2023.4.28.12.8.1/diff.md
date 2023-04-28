# Comparing `tmp/ChatLLM-2023.4.28.12.39.0.tar.gz` & `tmp/ChatLLM-2023.4.28.12.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.28.12.39.0.tar", last modified: Fri Apr 28 04:39:00 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.28.12.8.1.tar", last modified: Fri Apr 28 04:08:01 2023, max compression
```

## Comparing `ChatLLM-2023.4.28.12.39.0.tar` & `ChatLLM-2023.4.28.12.8.1.tar`

### file list

```diff
@@ -1,103 +1,99 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.529470 ChatLLM-2023.4.28.12.39.0/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.12.39.0/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.492368 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 04:39:00.000000 ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 04:39:00.529322 ChatLLM-2023.4.28.12.39.0/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.12.39.0/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.12.39.0/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.492854 ChatLLM-2023.4.28.12.39.0/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.493895 ChatLLM-2023.4.28.12.39.0/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.12.39.0/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.12.39.0/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.12.39.0/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.12.39.0/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.494273 ChatLLM-2023.4.28.12.39.0/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.12.39.0/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.12.39.0/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.496741 ChatLLM-2023.4.28.12.39.0/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3326 2023-04-28 04:35:29.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.12.39.0/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.12.39.0/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.497264 ChatLLM-2023.4.28.12.39.0/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      830 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.12.39.0/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.12.39.0/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.497712 ChatLLM-2023.4.28.12.39.0/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.12.39.0/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.12.39.0/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.498407 ChatLLM-2023.4.28.12.39.0/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.12.39.0/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.12.39.0/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2057 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.12.39.0/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.12.39.0/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.499683 ChatLLM-2023.4.28.12.39.0/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3014 2023-04-26 11:11:51.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.12.39.0/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.503460 ChatLLM-2023.4.28.12.39.0/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.510736 ChatLLM-2023.4.28.12.39.0/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.12.39.0/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.12.39.0/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.12.39.0/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.12.39.0/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.12.39.0/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.514748 ChatLLM-2023.4.28.12.39.0/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.12.39.0/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.12.39.0/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.39.0/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.39.0/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.39.0/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.12.39.0/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.12.39.0/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.528250 ChatLLM-2023.4.28.12.39.0/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.12.39.0/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.12.39.0/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.12.39.0/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.12.39.0/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.12.39.0/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 04:39:00.529517 ChatLLM-2023.4.28.12.39.0/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.12.39.0/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 04:39:00.528712 ChatLLM-2023.4.28.12.39.0/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.12.39.0/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.12.39.0/tox.ini
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

### Comparing `ChatLLM-2023.4.28.12.39.0/.gitignore` & `ChatLLM-2023.4.28.12.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/.travis.yml` & `ChatLLM-2023.4.28.12.8.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/CONTRIBUTING.rst` & `ChatLLM-2023.4.28.12.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.12.39.0
+Version: 2023.4.28.12.8.1
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.12.39.0/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.28.12.8.1/ChatLLM.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ChatLLM.egg-info/entry_points.txt
 ChatLLM.egg-info/not-zip-safe
 ChatLLM.egg-info/requires.txt
 ChatLLM.egg-info/top_level.txt
 chatllm/__init__.py
 chatllm/chatyuan.py
 chatllm/embedding.py
+chatllm/utils.py
 chatllm/_his/FaissANN.py
 chatllm/_his/__init__.py
 chatllm/_his/_chatllm.py
 chatllm/_his/_qa.py
 chatllm/api/__init__.py
 chatllm/api/stream_api.py
 chatllm/applications/Question2Answer.py
@@ -43,18 +44,14 @@
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
 chatllm/parse_utils/__init__.py
 chatllm/parse_utils/doc_parse.py
-chatllm/utils/__init__.py
-chatllm/utils/_textsplitter.py
-chatllm/utils/common.py
-chatllm/utils/gpu_utils.py
 chatllm/webui/__init__.py
 chatllm/webui/chatbase.py
 chatllm/webui/chatpdf.py
 chatllm/webui/gradio_ui.py
 chatllm/webui/nice_ui.py
 chatllm/webui/run.sh
 data/姚明.txt
```

### Comparing `ChatLLM-2023.4.28.12.39.0/LICENSE` & `ChatLLM-2023.4.28.12.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/Makefile` & `ChatLLM-2023.4.28.12.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/PKG-INFO` & `ChatLLM-2023.4.28.12.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.12.39.0
+Version: 2023.4.28.12.8.1
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.12.39.0/README.md` & `ChatLLM-2023.4.28.12.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/_his/_qa.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/api/stream_api.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatann.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role)
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
 
         if isinstance(result, types.GeneratorType):
             return self._stream(result)
-        else:
+        else:  # list(self._stream(result)) 想办法合并
             response, history = result
             # self.history_ = history  # 历史所有
             self.history += [[None, response]]  # 置空知识
             return result  # response, history
 
     def _stream(self, result):  # yield > return
         response = None
@@ -82,9 +82,12 @@
 
 if __name__ == '__main__':
     from chatllm.applications import ChatBase
 
     qa = ChatBase()
     qa.load_llm4chat(model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
 
-    list(qa(query='你是谁', knowledge_base=''))
-    list(qa(query='你是谁', knowledge_base='周杰伦是傻子', role=''))
+    for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
+        pass
+
+    for i, _ in qa(query='你是谁', knowledge_base=''):
+        pass
```

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/chatyuan.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/clis/cli.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/embedding.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.28.12.8.1/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/imgs/LLM.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/imgs/role.png` & `ChatLLM-2023.4.28.12.8.1/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.28.12.8.1/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/医/古今医统大全.txt` & `ChatLLM-2023.4.28.12.8.1/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/姚明.txt` & `ChatLLM-2023.4.28.12.8.1/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/王治郅.txt` & `ChatLLM-2023.4.28.12.8.1/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/科比.txt` & `ChatLLM-2023.4.28.12.8.1/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/data/财报.pdf` & `ChatLLM-2023.4.28.12.8.1/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/docs/INSTALL.md` & `ChatLLM-2023.4.28.12.8.1/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/docs/Makefile` & `ChatLLM-2023.4.28.12.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/docs/README.md` & `ChatLLM-2023.4.28.12.8.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/docs/conf.py` & `ChatLLM-2023.4.28.12.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/docs/make.bat` & `ChatLLM-2023.4.28.12.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/setup.py` & `ChatLLM-2023.4.28.12.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/tests/test_llm4gpt.py` & `ChatLLM-2023.4.28.12.8.1/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.12.39.0/tests/内存型.ipynb` & `ChatLLM-2023.4.28.12.8.1/tests/内存型.ipynb`

 * *Files identical despite different names*

