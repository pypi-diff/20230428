# Comparing `tmp/llm_bot-0.0.2a1.tar.gz` & `tmp/llm_bot-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.2a1.tar", max compression
+gzip compressed data, was "llm_bot-0.0.2a2.tar", max compression
```

## Comparing `llm_bot-0.0.2a1.tar` & `llm_bot-0.0.2a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.2a1/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.2a1/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.2a1/llm_bot/__init__.py
--rw-r--r--   0        0        0    13194 2023-04-28 12:48:41.107773 llm_bot-0.0.2a1/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-04-28 12:49:21.583518 llm_bot-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/llm_bot/__init__.py
+-rw-r--r--   0        0        0    13612 2023-04-28 17:32:02.416488 llm_bot-0.0.2a2/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-04-28 17:32:24.904104 llm_bot-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.2a2/PKG-INFO
```

### Comparing `llm_bot-0.0.2a1/LICENSE` & `llm_bot-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.2a1/llm_bot/core.py` & `llm_bot-0.0.2a2/llm_bot/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,28 @@
 
     @abstractmethod
     def add_to_index(self, *args, **kwargs) -> None:
         """
         Adds the given data to the index and the vector store.
         """
 
+    def fetch_from_index(self, query: str, n_results: int) -> List[Document]:
+        """
+        Fetches the most relevant documents from the index.
+
+        Args:
+            query (str): The query to search for.
+            n_results (int): The number of results to return.
+
+        Returns:
+            List[Document]: The most relevant documents.
+        """
+        docs: List[Document] = self._store.similarity_search(query, k=n_results)
+        return docs
+
     def save(self, path: Union[str, Path]) -> None:
         """
         Saves the index and the vector store to the given path.
 
         Args:
             path (Union[str, Path]): The path to save the index and vector store to.
         """
@@ -174,17 +188,15 @@
         # Start list of messages with the personality prompt
         messages: List[BaseMessage] = [SystemMessage(content=personality_prompt)]
 
         # If we are using context, search for context documents and add them to the prompt
         sources: List[str] = []
         if use_context:
             messages.append(SystemMessage(content=context_prompt))
-            docs: List[Document] = self._store.similarity_search(
-                user_message, k=number_of_context_docs
-            )
+            docs = self.fetch_from_index(query=user_message, k=number_of_context_docs)
             sources = list(set([doc.metadata["source"] for doc in docs]))
             for doc in docs:
                 messages.append(SystemMessage(content=f"- {doc.page_content}"))
 
         # If chat history is provided, add messages for it
         if chat_history:
             messages.append(SystemMessage(content=chat_history_prompt))
```

### Comparing `llm_bot-0.0.2a1/pyproject.toml` & `llm_bot-0.0.2a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.2a1"
+version = "0.0.2a2"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.2a1/PKG-INFO` & `llm_bot-0.0.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

