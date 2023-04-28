# Comparing `tmp/catprompt-0.0.4.tar.gz` & `tmp/catprompt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.0.4.tar", last modified: Fri Apr 21 11:04:04 2023, max compression
+gzip compressed data, was "catprompt-0.1.0.tar", last modified: Fri Apr 28 11:19:20 2023, max compression
```

## Comparing `catprompt-0.0.4.tar` & `catprompt-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857942 catprompt-0.0.4/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.0.4/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     6136 2023-04-21 11:04:04.857839 catprompt-0.0.4/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     4509 2023-04-21 10:59:07.000000 catprompt-0.0.4/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.856885 catprompt-0.0.4/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.0.4/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     2601 2023-04-21 11:00:22.000000 catprompt-0.0.4/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857579 catprompt-0.0.4/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     6136 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-21 11:02:41.000000 catprompt-0.0.4/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-21 11:04:04.857978 catprompt-0.0.4/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.0.4/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857698 catprompt-0.0.4/test/
--rw-r--r--   0 juanre     (501) staff       (20)     2230 2023-04-21 10:50:54.000000 catprompt-0.0.4/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.303316 catprompt-0.1.0/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.1.0/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     6900 2023-04-28 11:19:20.303215 catprompt-0.1.0/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     5273 2023-04-28 11:18:41.000000 catprompt-0.1.0/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.302213 catprompt-0.1.0/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.1.0/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     4055 2023-04-28 11:16:44.000000 catprompt-0.1.0/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.302839 catprompt-0.1.0/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     6900 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      328 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-28 11:18:09.000000 catprompt-0.1.0/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-28 11:19:20.303346 catprompt-0.1.0/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.1.0/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.303064 catprompt-0.1.0/test/
+-rw-r--r--   0 juanre     (501) staff       (20)      796 2023-04-28 10:52:58.000000 catprompt-0.1.0/test/test_example.py
+-rw-r--r--   0 juanre     (501) staff       (20)     3546 2023-04-24 11:39:03.000000 catprompt-0.1.0/test/test_prompter.py
```

### Comparing `catprompt-0.0.4/LICENSE` & `catprompt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.4/PKG-INFO` & `catprompt-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.4
+Version: 0.1.0
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -47,17 +47,17 @@
 
 5. **Documentation:** The prompt files can serve as a foundation for your project's documentation, making it easier to keep the documentation up-to-date and in sync with the code.
 
 ## Usage
 
 1. Install catprompt
 2. Create your prompt files
-3. Run catprompt with the main prompt file as a command-line argument:
+3. Run catprompt with the main prompt file[s] as a command-line argument:
 
-`catprompt path/to/prompt.txt`
+`catprompt path/to/prompt.txt [path/to/other-prompts.txt]`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
 `pip install catprompt`
 
@@ -72,58 +72,90 @@
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
 - Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
+- Segments of a file can be tagged by adding a line that contains :prompt:tag at the beginning, and :/prompt:tag at the end. Include them by adding [tag] after the file name.
 
 ### Example
 
 Let's consider the following example with three files:
 
-**main_prompt.txt**
+**main-prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
-+= sub_prompt_1.txt
-+- code_snippet.py The snippet of code
++= sub-prompt-1.txt
++- code-snippet.py The snippet of code
++- code-snippet.py [tag-1] The snippet of code limited to tag-1
 
 This is the end of the main prompt.
 ```
 
-**sub_prompt_1.txt**
+**sub-prompt-1.txt**
 
 ```
 This is the sub-prompt 1.
 +# Ignore the rest of this file
 This line will be ignored.
 
 This is useful to record the prompt that you used with this file,  which
 you probably don't want when the file is included by another file
 ```
 
-**code_snippet.py**
+**code-snippet.py**
 
 ```python
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+
+def example_function_3():
+    return "F3"
+
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
 ```
 
-When running `catprompt main_prompt.txt`, the processed content will be:
+When running `catprompt main-prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
 The snippet of code follows delimited by +-----
 +-----
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+def example_function_3():
+    return "F3"
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
++-----
+The snippet of code limited to tag-1 follows delimited by +-----
++-----
+def example_function_2():
+    return "F2"
+def example_function_4():
+    return "F4"
 +-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
```

### Comparing `catprompt-0.0.4/README.md` & `catprompt-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 5. **Documentation:** The prompt files can serve as a foundation for your project's documentation, making it easier to keep the documentation up-to-date and in sync with the code.
 
 ## Usage
 
 1. Install catprompt
 2. Create your prompt files
-3. Run catprompt with the main prompt file as a command-line argument:
+3. Run catprompt with the main prompt file[s] as a command-line argument:
 
-`catprompt path/to/prompt.txt`
+`catprompt path/to/prompt.txt [path/to/other-prompts.txt]`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
 `pip install catprompt`
 
@@ -39,58 +39,90 @@
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
 - Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
+- Segments of a file can be tagged by adding a line that contains :prompt:tag at the beginning, and :/prompt:tag at the end. Include them by adding [tag] after the file name.
 
 ### Example
 
 Let's consider the following example with three files:
 
-**main_prompt.txt**
+**main-prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
-+= sub_prompt_1.txt
-+- code_snippet.py The snippet of code
++= sub-prompt-1.txt
++- code-snippet.py The snippet of code
++- code-snippet.py [tag-1] The snippet of code limited to tag-1
 
 This is the end of the main prompt.
 ```
 
-**sub_prompt_1.txt**
+**sub-prompt-1.txt**
 
 ```
 This is the sub-prompt 1.
 +# Ignore the rest of this file
 This line will be ignored.
 
 This is useful to record the prompt that you used with this file,  which
 you probably don't want when the file is included by another file
 ```
 
-**code_snippet.py**
+**code-snippet.py**
 
 ```python
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+
+def example_function_3():
+    return "F3"
+
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
 ```
 
-When running `catprompt main_prompt.txt`, the processed content will be:
+When running `catprompt main-prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
 The snippet of code follows delimited by +-----
 +-----
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+def example_function_3():
+    return "F3"
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
++-----
+The snippet of code limited to tag-1 follows delimited by +-----
++-----
+def example_function_2():
+    return "F2"
+def example_function_4():
+    return "F4"
 +-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
```

### Comparing `catprompt-0.0.4/catprompt/prompter.py` & `catprompt-0.1.0/catprompt/prompter.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,46 +6,81 @@
 import tiktoken
 
 
 # pylint: disable=inconsistent-return-statements
 def process_line(line, base_dir, processed_lines):
     if line.startswith('++'):
         return
-    if line.startswith('+='):
-        file_to_include = line[2:].strip()
+    if line.startswith('+=') or line.startswith('+-'):
+        file_to_include, tag, description = parse_file_and_tag(line)
         file_path = base_dir / file_to_include
         if not file_path.is_file():
             file_path = Path(file_to_include)
         if file_path.is_file():
-            print(f'Including {str(file_path)}')
-            process_file(file_path, processed_lines)
-        else:
-            raise RuntimeError(f'Cannot find {file_to_include}')
-    elif line.startswith('+-'):
-        file_to_include, description = line[2:].strip().split(maxsplit=1)
-        file_path = base_dir / file_to_include
-        if not file_path.is_file():
-            file_path = Path(file_to_include)
-        if file_path.is_file():
-            with file_path.open(encoding='utf-8') as f:
-                content = f.read().strip()
-            processed_lines.extend([
-                f"{description} follows delimited by +-----",
-                "+-----",
-                content,
-                "+-----"
-            ])
+            print(f'Inserting {str(file_path)}')
+            process_included_file(file_path, tag, processed_lines,
+                                  with_delimiter=line.startswith('+-'),
+                                  description=description)
         else:
             raise RuntimeError(f'Cannot find {file_to_include}')
     elif line.startswith('+#'):
         return False
     else:
         processed_lines.append(line)
 
 
+def parse_file_and_tag(line):
+    file_and_tag = line[2:].strip().split(maxsplit=1)
+    file_to_include = file_and_tag[0].strip()
+    tag = None
+    description = None
+    if len(file_and_tag) > 1:
+        if '[' in file_and_tag[1]:
+            tag_start = file_and_tag[1].index('[')
+            tag_end = file_and_tag[1].index(']')
+            tag = file_and_tag[1][tag_start+1:tag_end].strip()
+            if line.startswith('+-'):
+                description = (file_and_tag[1][:tag_start].strip() +
+                               file_and_tag[1][tag_end+1:].strip())
+        else:
+            if line.startswith('+-'):
+                description = file_and_tag[1].strip()
+    return file_to_include, tag, description
+
+
+def process_included_file(file_path, tag, processed_lines, with_delimiter, description=None):
+    base_dir = file_path.parent
+    include = not tag
+    tag_start = f":prompt:{tag}"
+    tag_end = f":/prompt:{tag}"
+    if with_delimiter:
+        description = description if description else file_path.name
+        processed_lines.extend([
+            f"{description} follows delimited by +-----",
+            "+-----",
+        ])
+
+    with file_path.open() as f:
+        for line in f:
+            line = line.rstrip()
+            if tag and tag_start in line:
+                include = True
+                continue
+            if tag and tag_end in line:
+                include = False
+                continue
+            if include:
+                should_stop = process_line(line, base_dir, processed_lines)
+                if should_stop is False:
+                    break
+
+    if with_delimiter:
+        processed_lines.append("+-----")
+
+
 def process_file(file_path, processed_lines=None):
     if processed_lines is None:
         processed_lines = []
     base_dir = file_path.parent
     with file_path.open() as f:
         for line in f:
             line = line.rstrip()
@@ -59,26 +94,34 @@
     processed_lines = process_file(file_path)
     processed_content = "\n".join(filter(None, processed_lines))
     clipboard.copy(processed_content)
     return processed_content
 
 
 def main():
-    if len(sys.argv) != 2:
-        print("Usage: catprompt <input_file>")
+    if len(sys.argv) < 2:
+        print("Usage: catprompt <input_file> [<input_files>]")
         sys.exit(1)
 
-    input_file = sys.argv[1]
-    file_path = Path(input_file)
+    input_files = sys.argv[1:]
+    processed_lines = []
 
-    if not file_path.is_file():
-        print(f"Error: '{input_file}' not found.")
-        sys.exit(1)
+    for input_file in input_files:
+        file_path = Path(input_file)
+
+        if not file_path.is_file():
+            print(f"Error: '{input_file}' not found.")
+            sys.exit(1)
+
+        print(f'Reading {input_file}')
+        process_file(file_path, processed_lines)
+
+    processed_content = "\n".join(filter(None, processed_lines))
+    clipboard.copy(processed_content)
 
-    processed_content = process_and_copy_to_clipboard(file_path)
     encoding = 'cl100k_base'
     tokenizer = tiktoken.get_encoding(encoding)
     tokens = tokenizer.encode(processed_content)
     print(f"Processed content copied to clipboard, {len(tokens)} {encoding} tokens")
 
 
 if __name__ == "__main__":
```

### Comparing `catprompt-0.0.4/catprompt.egg-info/PKG-INFO` & `catprompt-0.1.0/catprompt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.4
+Version: 0.1.0
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -47,17 +47,17 @@
 
 5. **Documentation:** The prompt files can serve as a foundation for your project's documentation, making it easier to keep the documentation up-to-date and in sync with the code.
 
 ## Usage
 
 1. Install catprompt
 2. Create your prompt files
-3. Run catprompt with the main prompt file as a command-line argument:
+3. Run catprompt with the main prompt file[s] as a command-line argument:
 
-`catprompt path/to/prompt.txt`
+`catprompt path/to/prompt.txt [path/to/other-prompts.txt]`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
 `pip install catprompt`
 
@@ -72,58 +72,90 @@
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
 - Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
+- Segments of a file can be tagged by adding a line that contains :prompt:tag at the beginning, and :/prompt:tag at the end. Include them by adding [tag] after the file name.
 
 ### Example
 
 Let's consider the following example with three files:
 
-**main_prompt.txt**
+**main-prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
-+= sub_prompt_1.txt
-+- code_snippet.py The snippet of code
++= sub-prompt-1.txt
++- code-snippet.py The snippet of code
++- code-snippet.py [tag-1] The snippet of code limited to tag-1
 
 This is the end of the main prompt.
 ```
 
-**sub_prompt_1.txt**
+**sub-prompt-1.txt**
 
 ```
 This is the sub-prompt 1.
 +# Ignore the rest of this file
 This line will be ignored.
 
 This is useful to record the prompt that you used with this file,  which
 you probably don't want when the file is included by another file
 ```
 
-**code_snippet.py**
+**code-snippet.py**
 
 ```python
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+
+def example_function_3():
+    return "F3"
+
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
 ```
 
-When running `catprompt main_prompt.txt`, the processed content will be:
+When running `catprompt main-prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
 The snippet of code follows delimited by +-----
 +-----
-def example_function():
-    return "This is an example code snippet."
+def example_function_1():
+    return "F1"
+# :prompt:tag-1
+def example_function_2():
+    return "F2"
+# :/prompt:tag-1
+def example_function_3():
+    return "F3"
+# :prompt:tag-1
+def example_function_4():
+    return "F4"
+# :/prompt:tag-1
++-----
+The snippet of code limited to tag-1 follows delimited by +-----
++-----
+def example_function_2():
+    return "F2"
+def example_function_4():
+    return "F4"
 +-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
```

### Comparing `catprompt-0.0.4/pyproject.toml` & `catprompt-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.0.4"
+version = "0.1.0"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
```

### Comparing `catprompt-0.0.4/test/test_prompter.py` & `catprompt-0.1.0/test/test_prompter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# -*- coding: utf-8 -*-
+
+import os
 from pathlib import Path
 from catprompt.prompter import process_and_copy_to_clipboard
 import clipboard
 
 
 def test_process_file():
     # Prepare test data
@@ -56,7 +59,40 @@
     print(processed_content)
     print(expected_output)
     assert processed_content == expected_output
 
     # Check if processed content was copied to clipboard
     clipboard_content = clipboard.paste()
     assert processed_content == clipboard_content
+
+
+def test_process_file_with_tags_and_equals():
+    # Prepare test data
+    test_data_dir = Path(os.path.dirname(os.path.abspath(__file__))) / "data"
+    input_file = test_data_dir / "input-with-tags-and-equals.txt"
+    expected_output_file = test_data_dir / "expected-output-with-tags-and-equals.txt"
+
+    # Run process_and_copy_to_clipboard
+    processed_content = process_and_copy_to_clipboard(input_file)
+    print(processed_content)
+    print()
+
+    # Compare the processed content with the expected output
+    with expected_output_file.open() as f:
+        expected_output = f.read().rstrip()
+        print(expected_output)
+    assert processed_content == expected_output
+
+
+def test_process_file_with_tags_and_minus():
+    # Prepare test data
+    test_data_dir = Path(os.path.dirname(os.path.abspath(__file__))) / "data"
+    input_file = test_data_dir / "input-with-tags-and-minus.txt"
+    expected_output_file = test_data_dir / "expected-output-with-tags-and-minus.txt"
+
+    # Run process_and_copy_to_clipboard
+    processed_content = process_and_copy_to_clipboard(input_file)
+
+    # Compare the processed content with the expected output
+    with expected_output_file.open() as f:
+        expected_output = f.read().rstrip()
+    assert processed_content == expected_output
```

