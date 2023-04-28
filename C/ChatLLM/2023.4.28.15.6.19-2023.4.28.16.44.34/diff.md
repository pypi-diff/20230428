# Comparing `tmp/ChatLLM-2023.4.28.15.6.19.tar.gz` & `tmp/ChatLLM-2023.4.28.16.44.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.28.15.6.19.tar", last modified: Fri Apr 28 07:06:19 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.28.16.44.34.tar", last modified: Fri Apr 28 08:44:34 2023, max compression
```

## Comparing `ChatLLM-2023.4.28.15.6.19.tar` & `ChatLLM-2023.4.28.16.44.34.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.791951 ChatLLM-2023.4.28.15.6.19/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.15.6.19/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.752747 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1915 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 07:06:19.000000 ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5626 2023-04-28 07:06:19.791788 ChatLLM-2023.4.28.15.6.19/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.6.19/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4810 2023-04-28 00:52:16.000000 ChatLLM-2023.4.28.15.6.19/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.753382 ChatLLM-2023.4.28.15.6.19/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.754430 ChatLLM-2023.4.28.15.6.19/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.15.6.19/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.754902 ChatLLM-2023.4.28.15.6.19/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.15.6.19/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.15.6.19/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.757663 ChatLLM-2023.4.28.15.6.19/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-28 07:06:18.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1377 2023-04-27 05:00:51.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.15.6.19/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.15.6.19/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.758290 ChatLLM-2023.4.28.15.6.19/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.4.28.15.6.19/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.15.6.19/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.758776 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.15.6.19/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.759731 ChatLLM-2023.4.28.15.6.19/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2142 2023-04-28 07:05:00.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.15.6.19/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.761335 ChatLLM-2023.4.28.15.6.19/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.15.6.19/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.765662 ChatLLM-2023.4.28.15.6.19/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.772001 ChatLLM-2023.4.28.15.6.19/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.15.6.19/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.777544 ChatLLM-2023.4.28.15.6.19/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.15.6.19/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.15.6.19/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.15.6.19/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.15.6.19/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.790426 ChatLLM-2023.4.28.15.6.19/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.15.6.19/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.15.6.19/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      278 2023-04-27 03:14:44.000000 ChatLLM-2023.4.28.15.6.19/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       98 2023-04-27 02:55:48.000000 ChatLLM-2023.4.28.15.6.19/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.28.15.6.19/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 07:06:19.792001 ChatLLM-2023.4.28.15.6.19/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1527 2023-04-26 08:21:45.000000 ChatLLM-2023.4.28.15.6.19/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 07:06:19.791016 ChatLLM-2023.4.28.15.6.19/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.15.6.19/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.15.6.19/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.303230 ChatLLM-2023.4.28.16.44.34/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.16.44.34/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.283469 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5810 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1963 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      172 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5810 2023-04-28 08:44:34.303057 ChatLLM-2023.4.28.16.44.34/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.16.44.34/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.4.28.16.44.34/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.283831 ChatLLM-2023.4.28.16.44.34/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.284342 ChatLLM-2023.4.28.16.44.34/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.284608 ChatLLM-2023.4.28.16.44.34/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.16.44.34/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.16.44.34/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286242 ChatLLM-2023.4.28.16.44.34/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-28 07:06:18.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.16.44.34/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286621 ChatLLM-2023.4.28.16.44.34/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.16.44.34/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286892 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.287397 ChatLLM-2023.4.28.16.44.34/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2142 2023-04-28 07:05:00.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.288167 ChatLLM-2023.4.28.16.44.34/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.291668 ChatLLM-2023.4.28.16.44.34/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.293144 ChatLLM-2023.4.28.16.44.34/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.295270 ChatLLM-2023.4.28.16.44.34/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.16.44.34/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.16.44.34/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.16.44.34/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.302345 ChatLLM-2023.4.28.16.44.34/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.16.44.34/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.16.44.34/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.4.28.16.44.34/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.4.28.16.44.34/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.4.28.16.44.34/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-28 08:44:32.000000 ChatLLM-2023.4.28.16.44.34/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.4.28.16.44.34/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 08:44:34.303293 ChatLLM-2023.4.28.16.44.34/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.4.28.16.44.34/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.302761 ChatLLM-2023.4.28.16.44.34/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.16.44.34/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tox.ini
```

### Comparing `ChatLLM-2023.4.28.15.6.19/.gitignore` & `ChatLLM-2023.4.28.16.44.34/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/.travis.yml` & `ChatLLM-2023.4.28.16.44.34/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/CONTRIBUTING.rst` & `ChatLLM-2023.4.28.16.44.34/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.15.6.19
+Version: 2023.4.28.16.44.34
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,18 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: api
+Provides-Extra: pdf
+Provides-Extra: streamlit
+Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
@@ -40,15 +44,15 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 - 支持角色扮演
 ![img.png](data/imgs/role.png)
 
 ## ChatPDF
@@ -138,15 +142,15 @@
   - [ ] 添加输出内容及错误提示
   - [ ] 引用标注
   - [ ] 增加知识库管理
     - [ ] 选择知识库开始问答
     - [ ] 上传文件/文件夹至知识库
     - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [ ] 利用 Fastapi/Flask/Grpc 实现流式接口
+  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
   - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 ## 交流群
 ![二维码]()
 
 </details>
```

### Comparing `ChatLLM-2023.4.28.15.6.19/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 MANIFEST.in
 Makefile
 README.bak.md
 README.md
 git_init.sh
 pypi.sh
 requirements.txt
+requirements_api.txt
 requirements_pdf.txt
+requirements_streamlit.txt
 setup.py
 tox.ini
 ChatLLM.egg-info/PKG-INFO
 ChatLLM.egg-info/SOURCES.txt
 ChatLLM.egg-info/dependency_links.txt
 ChatLLM.egg-info/entry_points.txt
 ChatLLM.egg-info/not-zip-safe
```

### Comparing `ChatLLM-2023.4.28.15.6.19/LICENSE` & `ChatLLM-2023.4.28.16.44.34/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/Makefile` & `ChatLLM-2023.4.28.16.44.34/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/PKG-INFO` & `ChatLLM-2023.4.28.16.44.34/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.15.6.19
+Version: 2023.4.28.16.44.34
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,18 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: api
+Provides-Extra: pdf
+Provides-Extra: streamlit
+Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
@@ -40,15 +44,15 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 - 支持角色扮演
 ![img.png](data/imgs/role.png)
 
 ## ChatPDF
@@ -138,15 +142,15 @@
   - [ ] 添加输出内容及错误提示
   - [ ] 引用标注
   - [ ] 增加知识库管理
     - [ ] 选择知识库开始问答
     - [ ] 上传文件/文件夹至知识库
     - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [ ] 利用 Fastapi/Flask/Grpc 实现流式接口
+  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
   - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 ## 交流群
 ![二维码]()
 
 </details>
```

### Comparing `ChatLLM-2023.4.28.15.6.19/README.md` & `ChatLLM-2023.4.28.16.44.34/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
 
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'))
+_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 - 支持角色扮演
 ![img.png](data/imgs/role.png)
 
 ## ChatPDF
@@ -116,15 +116,15 @@
   - [ ] 添加输出内容及错误提示
   - [ ] 引用标注
   - [ ] 增加知识库管理
     - [ ] 选择知识库开始问答
     - [ ] 上传文件/文件夹至知识库
     - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [ ] 利用 Fastapi/Flask/Grpc 实现流式接口
+  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
   - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 ## 交流群
 ![二维码]()
 
 </details>
```

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/_his/FaissANN.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/_his/_chatllm.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/_his/_qa.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/api/stream_api.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatann.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatpdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     # bytes_array = Path(filename).read_bytes()
     # texts = extract_text(bytes_array)
     # texts = textsplitter(texts)
     # print(texts)
     from chatllm.applications.chatpdf import ChatPDF
 
     qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')  # 自动建索引
-    qa.load_llm4chat(model_name_or_path='/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm', device='cpu')
     qa.create_index('../../data/财报.pdf')
+    qa.load_llm4chat(model_name_or_path='/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm', device='cpu')
 
-    for i, _ in qa(query='东北证券主营业务', topk=1, threshold=0.8):
-        pass
+    list(qa(query='东北证券主营业务', topk=1, threshold=0.8))
 
     # 召回结果
     print(qa.recall)
```

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/chatyuan.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/clis/cli.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/embedding.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/utils/common.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.28.16.44.34/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.drawio.png` & `ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/imgs/LLM.png` & `ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf.gif` & `ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/imgs/role.png` & `ChatLLM-2023.4.28.16.44.34/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.28.16.44.34/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/医/古今医统大全.txt` & `ChatLLM-2023.4.28.16.44.34/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/姚明.txt` & `ChatLLM-2023.4.28.16.44.34/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/王治郅.txt` & `ChatLLM-2023.4.28.16.44.34/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/科比.txt` & `ChatLLM-2023.4.28.16.44.34/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/data/财报.pdf` & `ChatLLM-2023.4.28.16.44.34/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/docs/INSTALL.md` & `ChatLLM-2023.4.28.16.44.34/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/docs/Makefile` & `ChatLLM-2023.4.28.16.44.34/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/docs/README.md` & `ChatLLM-2023.4.28.16.44.34/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/docs/conf.py` & `ChatLLM-2023.4.28.16.44.34/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/docs/make.bat` & `ChatLLM-2023.4.28.16.44.34/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/setup.py` & `ChatLLM-2023.4.28.16.44.34/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python
 
 """The setup script."""
 import time
+import pandas as pd
+from pathlib import Path
 from setuptools import setup, find_packages
 
+DIR = Path(__file__).resolve().parent
 version = time.strftime("%Y.%m.%d.%H.%M.%S", time.localtime())
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-with open('requirements.txt', encoding='utf-8') as f:
-    requirements = f.read().split('\n')
+get_requirements = lambda p='requirements.txt': pd.read_csv(p, comment='#', names=['name']).name.tolist()
+extras_require = {v.name.split('_')[1][:-4]: get_requirements(v) for v in DIR.glob('requirements_*')}
+extras_require['all'] = list(set(sum(extras_require.values(), [])))
 
 setup(
     author="yuanjie",
     author_email='313303303@qq.com',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -31,24 +35,25 @@
     ],
     description="Create a Python package.",
     entry_points={
         'console_scripts': [
             'chatllm-run=chatllm.clis.cli:cli'
         ],
     },
-    install_requires=requirements,
+    setup_requires=["pandas"],
+    install_requires=get_requirements(),
+    extras_require=extras_require,  # pip install -U meutils\[all\]
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='chatllm',
     name='ChatLLM',
     # name='ChatSearch', # 抢占包
 
     packages=find_packages(include=['chatllm', 'chatllm.*']),
 
     test_suite='tests',
     url='https://github.com/yuanjie-ai/ChatLLM',
-    version=version, # '0.0.0',
+    version=version,  # '0.0.0',
     zip_safe=False,
 )
-
```

### Comparing `ChatLLM-2023.4.28.15.6.19/tests/test_llm4gpt.py` & `ChatLLM-2023.4.28.16.44.34/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.15.6.19/tests/内存型.ipynb` & `ChatLLM-2023.4.28.16.44.34/tests/内存型.ipynb`

 * *Files identical despite different names*

