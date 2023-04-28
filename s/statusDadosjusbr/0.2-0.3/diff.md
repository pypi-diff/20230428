# Comparing `tmp/statusDadosjusbr-0.2.tar.gz` & `tmp/statusDadosjusbr-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statusDadosjusbr-0.2.tar", last modified: Thu Mar  2 18:44:10 2023, max compression
+gzip compressed data, was "statusDadosjusbr-0.3.tar", last modified: Fri Apr 28 15:18:26 2023, max compression
```

## Comparing `statusDadosjusbr-0.2.tar` & `statusDadosjusbr-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-03-02 18:44:10.391664 statusDadosjusbr-0.2/
--rw-rw-r--   0 joellen   (1000) joellen   (1000)     2828 2023-03-02 18:44:10.391664 statusDadosjusbr-0.2/PKG-INFO
--rw-rw-r--   0 joellen   (1000) joellen   (1000)     1883 2023-02-08 19:55:18.000000 statusDadosjusbr-0.2/README.md
--rw-rw-r--   0 joellen   (1000) joellen   (1000)       38 2023-03-02 18:44:10.391664 statusDadosjusbr-0.2/setup.cfg
--rw-rw-r--   0 joellen   (1000) joellen   (1000)      636 2023-03-02 18:43:46.000000 statusDadosjusbr-0.2/setup.py
-drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-03-02 18:44:10.391664 statusDadosjusbr-0.2/status/
--rw-rw-r--   0 joellen   (1000) joellen   (1000)       20 2023-03-02 18:32:44.000000 statusDadosjusbr-0.2/status/__init__.py
--rw-rw-r--   0 joellen   (1000) joellen   (1000)     1273 2023-02-08 20:36:32.000000 statusDadosjusbr-0.2/status/status.py
-drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-03-02 18:44:10.391664 statusDadosjusbr-0.2/statusDadosjusbr.egg-info/
--rw-rw-r--   0 joellen   (1000) joellen   (1000)     2828 2023-03-02 18:44:10.000000 statusDadosjusbr-0.2/statusDadosjusbr.egg-info/PKG-INFO
--rw-rw-r--   0 joellen   (1000) joellen   (1000)      214 2023-03-02 18:44:10.000000 statusDadosjusbr-0.2/statusDadosjusbr.egg-info/SOURCES.txt
--rw-rw-r--   0 joellen   (1000) joellen   (1000)        1 2023-03-02 18:44:10.000000 statusDadosjusbr-0.2/statusDadosjusbr.egg-info/dependency_links.txt
--rw-rw-r--   0 joellen   (1000) joellen   (1000)        7 2023-03-02 18:44:10.000000 statusDadosjusbr-0.2/statusDadosjusbr.egg-info/top_level.txt
+drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-04-28 15:18:26.473175 statusDadosjusbr-0.3/
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)     2933 2023-04-28 15:18:26.473175 statusDadosjusbr-0.3/PKG-INFO
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)     1980 2023-04-28 15:18:12.000000 statusDadosjusbr-0.3/README.md
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)       38 2023-04-28 15:18:26.473175 statusDadosjusbr-0.3/setup.cfg
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)      636 2023-04-28 15:17:34.000000 statusDadosjusbr-0.3/setup.py
+drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-04-28 15:18:26.473175 statusDadosjusbr-0.3/status/
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)       20 2023-03-02 18:32:44.000000 statusDadosjusbr-0.3/status/__init__.py
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)     1345 2023-04-28 15:13:37.000000 statusDadosjusbr-0.3/status/status.py
+drwxrwxr-x   0 joellen   (1000) joellen   (1000)        0 2023-04-28 15:18:26.473175 statusDadosjusbr-0.3/statusDadosjusbr.egg-info/
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)     2933 2023-04-28 15:18:26.000000 statusDadosjusbr-0.3/statusDadosjusbr.egg-info/PKG-INFO
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)      214 2023-04-28 15:18:26.000000 statusDadosjusbr-0.3/statusDadosjusbr.egg-info/SOURCES.txt
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)        1 2023-04-28 15:18:26.000000 statusDadosjusbr-0.3/statusDadosjusbr.egg-info/dependency_links.txt
+-rw-rw-r--   0 joellen   (1000) joellen   (1000)        7 2023-04-28 15:18:26.000000 statusDadosjusbr-0.3/statusDadosjusbr.egg-info/top_level.txt
```

### Comparing `statusDadosjusbr-0.2/PKG-INFO` & `statusDadosjusbr-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statusDadosjusbr
-Version: 0.2
+Version: 0.3
 Summary: Contém os status de execução dos coletores do DadosjusBr
 Home-page: https://github.com/dadosjusbr/status/
 Author: Dadosjusbr
 Author-email: dadosjusbr@gmail.com
 License: UNKNOWN
 Description: # Status Package
         
@@ -21,14 +21,15 @@
         |2|SystemError|Deve ser usado em casos como falha ao criar o diretório dos arquivos ou na leitura de arquivos.|
         |3|ConnectionError|Deve ser usado em problemas de conexão, como timeout ou serviço fora do ar.|
         |4|DataUnavailable|A informação solicitada não foi encontrada, provavelmente o órgão não disponibilizou ainda.|
         |5|InvalidFile|Deve ser usado para cenários onde o arquivo não é o esperado ou em caso de falhas na extração de dados.|
         |6|Unknown|Deve ser usando quando um erro inesperado ocorrer.|
         |7|InvalidInput|A entrada do estágio é inválida.|
         |8|OutputError|Quando o estágio não for capaz de imprimir a saída correta.|
+        |9|DeadlineExceeded|Quando uma determinada ação não foi concluída dentro do prazo esperado.|
         ______________
         
         ## Exemplo de uso em Go
         ```
         package main
         
         import (
```

### Comparing `statusDadosjusbr-0.2/README.md` & `statusDadosjusbr-0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 |2|SystemError|Deve ser usado em casos como falha ao criar o diretório dos arquivos ou na leitura de arquivos.|
 |3|ConnectionError|Deve ser usado em problemas de conexão, como timeout ou serviço fora do ar.|
 |4|DataUnavailable|A informação solicitada não foi encontrada, provavelmente o órgão não disponibilizou ainda.|
 |5|InvalidFile|Deve ser usado para cenários onde o arquivo não é o esperado ou em caso de falhas na extração de dados.|
 |6|Unknown|Deve ser usando quando um erro inesperado ocorrer.|
 |7|InvalidInput|A entrada do estágio é inválida.|
 |8|OutputError|Quando o estágio não for capaz de imprimir a saída correta.|
+|9|DeadlineExceeded|Quando uma determinada ação não foi concluída dentro do prazo esperado.|
 ______________
 
 ## Exemplo de uso em Go
 ```
 package main
 
 import (
```

### Comparing `statusDadosjusbr-0.2/setup.py` & `statusDadosjusbr-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='statusDadosjusbr',
-    version='0.2',
+    version='0.3',
     author="Dadosjusbr",
     author_email="dadosjusbr@gmail.com",
     description="Contém os status de execução dos coletores do DadosjusBr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dadosjusbr/status/",
     packages=['status'],
```

### Comparing `statusDadosjusbr-0.2/status/status.py` & `statusDadosjusbr-0.3/status/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 SystemError = 2
 ConnectionError = 3
 DataUnavailable = 4
 InvalidFile = 5
 Unknown = 6
 InvalidInput = 7
 OutputError = 8
+DeadlineExceeded = 9
 
 statusText = {
     OK: "OK",
     InvalidParameters: "Invalid Parameters",
     SystemError: "System Error",
     ConnectionError: "Connection Error",
     DataUnavailable: "Data Unavailable",
     InvalidFile: "Invalid File",
     Unknown: "Unknown",
     InvalidInput: "Invalid Input",
     OutputError: "Output Error",
+    DeadlineExceeded: "Context Deadline Exceeded",
 }
 
 # Text returns a text for a status code. It returns the empty
 # string if the code is unknown.
 def text(code: Code) -> str:
     return statusText.get(code, '')
```

### Comparing `statusDadosjusbr-0.2/statusDadosjusbr.egg-info/PKG-INFO` & `statusDadosjusbr-0.3/statusDadosjusbr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statusDadosjusbr
-Version: 0.2
+Version: 0.3
 Summary: Contém os status de execução dos coletores do DadosjusBr
 Home-page: https://github.com/dadosjusbr/status/
 Author: Dadosjusbr
 Author-email: dadosjusbr@gmail.com
 License: UNKNOWN
 Description: # Status Package
         
@@ -21,14 +21,15 @@
         |2|SystemError|Deve ser usado em casos como falha ao criar o diretório dos arquivos ou na leitura de arquivos.|
         |3|ConnectionError|Deve ser usado em problemas de conexão, como timeout ou serviço fora do ar.|
         |4|DataUnavailable|A informação solicitada não foi encontrada, provavelmente o órgão não disponibilizou ainda.|
         |5|InvalidFile|Deve ser usado para cenários onde o arquivo não é o esperado ou em caso de falhas na extração de dados.|
         |6|Unknown|Deve ser usando quando um erro inesperado ocorrer.|
         |7|InvalidInput|A entrada do estágio é inválida.|
         |8|OutputError|Quando o estágio não for capaz de imprimir a saída correta.|
+        |9|DeadlineExceeded|Quando uma determinada ação não foi concluída dentro do prazo esperado.|
         ______________
         
         ## Exemplo de uso em Go
         ```
         package main
         
         import (
```

