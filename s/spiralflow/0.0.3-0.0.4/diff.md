# Comparing `tmp/spiralflow-0.0.3.tar.gz` & `tmp/spiralflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralflow-0.0.3.tar", last modified: Wed Apr 26 01:42:57 2023, max compression
+gzip compressed data, was "spiralflow-0.0.4.tar", last modified: Fri Apr 28 17:13:56 2023, max compression
```

## Comparing `spiralflow-0.0.3.tar` & `spiralflow-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.185700 spiralflow-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12978 2023-04-26 01:42:57.181188 spiralflow-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12452 2023-04-24 19:26:36.000000 spiralflow-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 01:42:57.185700 spiralflow-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-04-26 01:42:31.000000 spiralflow-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.165616 spiralflow-0.0.3/spiralflow/
--rw-rw-rw-   0        0        0       23 2023-04-26 01:42:42.000000 spiralflow-0.0.3/spiralflow/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/chat_llm.py
--rw-rw-rw-   0        0        0    53659 2023-04-26 01:41:18.000000 spiralflow-0.0.3/spiralflow/flow.py
--rw-rw-rw-   0        0        0     6835 2023-04-26 01:38:32.000000 spiralflow-0.0.3/spiralflow/memory.py
--rw-rw-rw-   0        0        0    16849 2023-04-24 19:26:36.000000 spiralflow-0.0.3/spiralflow/message.py
--rw-rw-rw-   0        0        0     7464 2023-04-26 01:41:35.000000 spiralflow-0.0.3/spiralflow/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-26 01:42:57.179188 spiralflow-0.0.3/spiralflow.egg-info/
--rw-rw-rw-   0        0        0    12978 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-26 01:42:57.000000 spiralflow-0.0.3/spiralflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 01:42:56.000000 spiralflow-0.0.3/spiralflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.851030 spiralflow-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    13703 2023-04-28 17:13:56.846029 spiralflow-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13177 2023-04-28 16:52:05.000000 spiralflow-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:13:56.851030 spiralflow-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-04-28 16:34:47.000000 spiralflow-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.831405 spiralflow-0.0.4/spiralflow/
+-rw-rw-rw-   0        0        0       23 2023-04-28 15:44:36.000000 spiralflow-0.0.4/spiralflow/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/chat_llm.py
+-rw-rw-rw-   0        0        0     4257 2023-04-28 17:13:32.000000 spiralflow-0.0.4/spiralflow/chunking.py
+-rw-rw-rw-   0        0        0    53659 2023-04-26 01:41:18.000000 spiralflow-0.0.4/spiralflow/flow.py
+-rw-rw-rw-   0        0        0     6128 2023-04-28 17:00:18.000000 spiralflow-0.0.4/spiralflow/loading.py
+-rw-rw-rw-   0        0        0     6810 2023-04-26 01:46:56.000000 spiralflow-0.0.4/spiralflow/memory.py
+-rw-rw-rw-   0        0        0    16849 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/message.py
+-rw-rw-rw-   0        0        0     7464 2023-04-26 01:41:35.000000 spiralflow-0.0.4/spiralflow/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.844029 spiralflow-0.0.4/spiralflow.egg-info/
+-rw-rw-rw-   0        0        0    13703 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/top_level.txt
```

### Comparing `spiralflow-0.0.3/LICENSE` & `spiralflow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/PKG-INFO` & `spiralflow-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# spiralflow (Work-In-Progress)
+# spiralflow
 A framework for creating guided spirals for Large Language Models
 
-This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
+This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
 *   `InputJSONMessage`: A class to create input messages with pre-defined content formats that are able to access Dict variables.
 *   `OutputJSONMessage`: A class to create output messages and extract JSON formated dict variables from them.
 *   `ChatLLM`: A class to interface with OpenAI's chat models.
@@ -31,28 +31,35 @@
 *   `NoHistory`: A class to block the flow of specific histories whether in or out of the flow.
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
+*   `TextLoader`: A class to load text files, optionally splitting them into chunks using a specified chunker.
+*   `PDFLoader`: A class to load PDF files, utilizing the fitz (PyMuPDF) library to extract text content.
+*   `HTMLLoader`: A class to load HTML files, extracting text content using the BeautifulSoup library.
+*   `DirectoryLoader`: A class to load files from a directory, using a specified loader instance for each file, with options for recursion and filtering by file names.
+*   `DirectoryMultiLoader`: A class to load files from a directory, using different loader instances based on file names, with options for recursion.
+*   `Chunker`: A class to split text into chunks of a specified size with overlap.
+*   `SmartChunker`: A class that splits text into chunks while respecting delimiters, tolerances, and overlap.
+
 
 Example Projects
 ------------
 [Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
-2.  Install the `openai`, `tiktoken`, `pandas`, packages: `pip install openai tiktoken pandas`.
-3.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
-3.  Install the this package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
+2.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
+3.  Install the this package: `git clone https://github.com/Tiger767/Spiralflow.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
```

### Comparing `spiralflow-0.0.3/README.md` & `spiralflow-0.0.4/spiralflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,25 @@
-# spiralflow (Work-In-Progress)
+Metadata-Version: 2.1
+Name: spiralflow
+Version: 0.0.4
+Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
+Home-page: https://github.com/Tiger767/Spiralflow
+Author: Travis Hammond
+License: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# spiralflow
 A framework for creating guided spirals for Large Language Models
 
-This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
+This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
 *   `InputJSONMessage`: A class to create input messages with pre-defined content formats that are able to access Dict variables.
 *   `OutputJSONMessage`: A class to create output messages and extract JSON formated dict variables from them.
 *   `ChatLLM`: A class to interface with OpenAI's chat models.
@@ -17,28 +31,35 @@
 *   `NoHistory`: A class to block the flow of specific histories whether in or out of the flow.
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
+*   `TextLoader`: A class to load text files, optionally splitting them into chunks using a specified chunker.
+*   `PDFLoader`: A class to load PDF files, utilizing the fitz (PyMuPDF) library to extract text content.
+*   `HTMLLoader`: A class to load HTML files, extracting text content using the BeautifulSoup library.
+*   `DirectoryLoader`: A class to load files from a directory, using a specified loader instance for each file, with options for recursion and filtering by file names.
+*   `DirectoryMultiLoader`: A class to load files from a directory, using different loader instances based on file names, with options for recursion.
+*   `Chunker`: A class to split text into chunks of a specified size with overlap.
+*   `SmartChunker`: A class that splits text into chunks while respecting delimiters, tolerances, and overlap.
+
 
 Example Projects
 ------------
 [Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
-2.  Install the `openai`, `tiktoken`, `pandas`, packages: `pip install openai tiktoken pandas`.
-3.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
-3.  Install the this package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
+2.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
+3.  Install the this package: `git clone https://github.com/Tiger767/Spiralflow.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
```

### Comparing `spiralflow-0.0.3/setup.py` & `spiralflow-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiralflow",
-    version="0.0.3",
+    version="0.0.4",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/Spiralflow",
     packages=setuptools.find_packages(),
-    install_requires=[
-        "regex",
-        "openai",
-        "pandas",
-        "tiktoken",
-    ],
+    install_requires=["regex", "openai", "pandas", "tiktoken", "pymupdf", "bs4"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     license="MIT License",
```

### Comparing `spiralflow-0.0.3/spiralflow/chat_history.py` & `spiralflow-0.0.4/spiralflow/chat_history.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/spiralflow/chat_llm.py` & `spiralflow-0.0.4/spiralflow/chat_llm.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/spiralflow/flow.py` & `spiralflow-0.0.4/spiralflow/flow.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/spiralflow/memory.py` & `spiralflow-0.0.4/spiralflow/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,16 +143,14 @@
 
         # get embedding of query
         embeded_query = np.array([get_embedding(query, engine=self.embedding_model)])
 
         # search for the indexes with similar embeddings
         scores, similar_indexes = self.index.search(embeded_query, k=k)
 
-        print(scores)
-
         # get the memory values at the found indexes
         memories = []
 
         for score, i in zip(scores[0], similar_indexes[0]):
             memory = {
                 "text": self.data.iloc[i, 0],
                 "metadata": self.data.iloc[i, 1],
```

### Comparing `spiralflow-0.0.3/spiralflow/message.py` & `spiralflow-0.0.4/spiralflow/message.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/spiralflow/tools.py` & `spiralflow-0.0.4/spiralflow/tools.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.3/spiralflow.egg-info/PKG-INFO` & `spiralflow-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: spiralflow
-Version: 0.0.3
-Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
-Home-page: https://github.com/Tiger767/Spiralflow
-Author: Travis Hammond
-License: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# spiralflow (Work-In-Progress)
+# spiralflow
 A framework for creating guided spirals for Large Language Models
 
-This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following key components:
+This project is designed to help with creating, formatting, and extracting data from text-based conversations with OpenAI language models to allow for more complicated ideas such as Flows and Spirals. It includes the following components:
 
 *   `Message`: A base class representing a message with content, role, and variables.
 *   `InputMessage`: A class to create input messages with pre-defined content formats.
 *   `OutputMessage`: A class to create output messages and extract variables from them.
 *   `InputJSONMessage`: A class to create input messages with pre-defined content formats that are able to access Dict variables.
 *   `OutputJSONMessage`: A class to create output messages and extract JSON formated dict variables from them.
 *   `ChatLLM`: A class to interface with OpenAI's chat models.
@@ -31,28 +17,35 @@
 *   `NoHistory`: A class to block the flow of specific histories whether in or out of the flow.
 *   `History`: A class that allows for more complicated flows of histories, utilizing the ChatHistoryManager.
 *   `MemoryChatFlow`: A class that allows a chat flow to query external memory.
 *   `ConditonalChatFlow`: A class to represent a conversation flow with multiple branches that depend on an output of a flow.
 *   `SequentialChatFlows`: A class to represent multiple conversation flows, flowing sequentially.
 *   `ConcurrentChatFlows`: A class to represent multiple conversation flows, flowing separately and concurrently.
 *   `ChatSpiral`: A class to represent a spiral of conversation flows.
+*   `TextLoader`: A class to load text files, optionally splitting them into chunks using a specified chunker.
+*   `PDFLoader`: A class to load PDF files, utilizing the fitz (PyMuPDF) library to extract text content.
+*   `HTMLLoader`: A class to load HTML files, extracting text content using the BeautifulSoup library.
+*   `DirectoryLoader`: A class to load files from a directory, using a specified loader instance for each file, with options for recursion and filtering by file names.
+*   `DirectoryMultiLoader`: A class to load files from a directory, using different loader instances based on file names, with options for recursion.
+*   `Chunker`: A class to split text into chunks of a specified size with overlap.
+*   `SmartChunker`: A class that splits text into chunks while respecting delimiters, tolerances, and overlap.
+
 
 Example Projects
 ------------
 [Data Chat](https://github.com/Tiger767/spiralflow-data-chat) - A constructued ChatFlow for responding to prompts using your data, google search results, and general LLM knowledge.
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
 1.  Install Python 3.9 or higher.
-2.  Install the `openai`, `tiktoken`, `pandas`, packages: `pip install openai tiktoken pandas`.
-3.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
-3.  Install the this package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
+2.  Install faiss package: `conda install -c conda-forge pytorch faiss-cpu`
+3.  Install the this package: `git clone https://github.com/Tiger767/Spiralflow.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
```

