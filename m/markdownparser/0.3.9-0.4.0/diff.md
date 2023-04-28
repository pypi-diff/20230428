# Comparing `tmp/markdownparser-0.3.9.tar.gz` & `tmp/markdownparser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.3.9.tar", max compression
+gzip compressed data, was "markdownparser-0.4.0.tar", max compression
```

## Comparing `markdownparser-0.3.9.tar` & `markdownparser-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.3.9/LICENSE
--rw-r--r--   0        0        0       64 2023-01-30 08:56:40.322545 markdownparser-0.3.9/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5599 2023-04-27 07:15:55.104457 markdownparser-0.3.9/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    22430 2023-04-27 07:27:40.965222 markdownparser-0.3.9/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     1229 2023-04-27 10:25:53.137955 markdownparser-0.3.9/MarkdownParser/core.py
--rw-r--r--   0        0        0     3329 2023-04-27 07:28:20.519261 markdownparser-0.3.9/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    20772 2023-04-27 10:27:47.162481 markdownparser-0.3.9/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-04-27 11:08:32.799699 markdownparser-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     4331 2023-04-27 10:51:20.047839 markdownparser-0.3.9/README.md
--rw-r--r--   0        0        0     5064 1970-01-01 00:00:00.000000 markdownparser-0.3.9/setup.py
--rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 markdownparser-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.4.0/LICENSE
+-rw-r--r--   0        0        0       98 2023-04-28 15:33:12.004410 markdownparser-0.4.0/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.4.0/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    23439 2023-04-28 16:47:50.909285 markdownparser-0.4.0/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     6590 2023-04-28 17:29:34.098824 markdownparser-0.4.0/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.4.0/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    20799 2023-04-28 12:36:46.656399 markdownparser-0.4.0/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-04-28 17:30:29.693658 markdownparser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4747 2023-04-28 17:29:33.196411 markdownparser-0.4.0/README.md
+-rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 markdownparser-0.4.0/setup.py
+-rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 markdownparser-0.4.0/PKG-INFO
```

### Comparing `markdownparser-0.3.9/LICENSE` & `markdownparser-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.3.9/MarkdownParser/base_class.py` & `markdownparser-0.4.0/MarkdownParser/base_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             # block类名-唯一标识符 : block类对象
             #
         }
 
         self._counter = 0
         self.__str__ = self.__repr__
 
-    def __repr__(self) -> str: # pragma: no cover
+    def __repr__(self) -> str:  # pragma: no cover
 
         split_line = '-' * 50 + '\n'
         info = f'Total number: {self._counter}\n\n'
 
         for k, v in self._container.items():
             info += f'[{k}]'.ljust(30)
             if v.input.get('word') is not None:
@@ -46,19 +46,19 @@
         self.is_sorted = False
 
     def _sort(self):
 
         # 按照优先级从高到低排序,使得解析时依次调用方法
         self._handlers.sort(key=lambda item: item['priority'], reverse=True)
 
-    def __call__(self, *args, **kwargs): # pragma: no cover
+    def __call__(self, *args, **kwargs):  # pragma: no cover
 
         raise NotImplementedError
 
-    def info(self): # pragma: no cover
+    def info(self):  # pragma: no cover
         # 查看所有已注册的方法
         if not self.is_sorted:
             self._sort()
         for method in self._handlers:
             name = method['name']
             class_name = method['object'].__class__.__name__
             priority = method['priority']
@@ -74,17 +74,17 @@
         self._handlers.append(new_method)
 
 
 class Block:
 
     def __init__(self, **kwargs) -> None:
         self.input = kwargs
-        # input['text']: 输入的纯文本,用于恢复原始信息
-        # input['word']: 解析提取后的核心文本信息
-        self.sub_blocks = []
+        self.input['text']: str  # 输入的纯文本,用于恢复原始信息
+        self.input['word']: str  # 解析提取后的核心文本信息
+        self.sub_blocks = []   # 子模块
         self.block_name = self.__class__.__name__
 
     def register(self, class_object):
 
         global CONTAINER
         return CONTAINER.register(class_object)
 
@@ -110,85 +110,88 @@
                 self.addBlock(class_object)
             count += 1
 
     def addBlock(self, block):
 
         self.sub_blocks.append(block)
 
-    def __str__(self): # pragma: no cover
+    def __str__(self):  # pragma: no cover
 
         if not self.input:
             return ''
         output = '< '
         for k, v in self.input.items():
             if k == 'text':
                 continue
             output += f'{k} = \"{v}\" | '
         if output == '< ':
             output = ''
         else:
             output = output[:-3] + ' >'
         return output
 
-    def info(self, deep: int = 0): # pragma: no cover
+    def info(self, deep: int = 0):  # pragma: no cover
         # root.info()
         # 递归输出信息
 
         if self.sub_blocks == []:
             return
         else:
             for block in self.sub_blocks:
                 print(' '*4*deep, end='')
                 print(f'[{block.__class__.__name__}] {str(block)}')
                 block.info(deep+1)
 
-    def printInfo(self, deep: int = 0) -> str: # pragma: no cover
+    def printInfo(self, deep: int = 0) -> str:  # pragma: no cover
         # print(root.printInfo())
         # 递归输出信息
         output_str = ''
         if self.sub_blocks == []:
             return output_str
         else:
             for block in self.sub_blocks:
                 output_str += ' '*4*deep
                 output_str += f'[{block.__class__.__name__}] {str(block)}\n'
                 output_str += block.printInfo(deep+1)
             return output_str
 
-    def toHTML(self):
+    def toHTML(self, header_navigater=None):
         # 转换成HTML格式
         content = ''
         for block in self.sub_blocks:
             content += block.toHTML()
-        return f"<div class='markdown-body'>{content}</div>"
+        if header_navigater:
+            return f"{header_navigater}<div class='markdown-body'>{content}</div>"
+        else:
+            return f"<div class='markdown-body'>{content}</div>"
 
 
 class Handler:
 
     def __init__(self, parser=None) -> None:
 
         self.RE = None
         self.parser: Parser = parser
 
-    def match(self, text: str, *args): # pragma: no cover
+    def match(self, text: str, *args):  # pragma: no cover
 
         if self.RE is None:
             raise NotImplementedError
 
         return bool(self.RE.search(text))
 
-    def __call__(self, root: Block, text: str): # pragma: no cover
+    def __call__(self, root: Block, text: str):  # pragma: no cover
 
         raise NotImplementedError
 
 
 class Optimizer:
 
     def __init__(self) -> None:
 
         # 优化器针对的Block
         self.target_block_names = []
         self.is_match = False
 
-    def __call__(self, root: Block): # pragma: no cover
+    def __call__(self, root: Block):  # pragma: no cover
 
         raise NotImplementedError
```

### Comparing `markdownparser-0.3.9/MarkdownParser/block_parser.py` & `markdownparser-0.4.0/MarkdownParser/block_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,44 +30,44 @@
                 return
 
 
 class ComplexBlock(Block):
     # 用于处理复杂嵌套
 
     def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs) # pragma: no cover
+        super().__init__(**kwargs)  # pragma: no cover
 
     def toHTML(self):
 
         content = ''
         for block in self.sub_blocks:
             content += block.toHTML()
 
         return content
 
 
 class HTMLBlock(Block):
     # 处理HTML标签
     def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs) # pragma: no cover
+        super().__init__(**kwargs)  # pragma: no cover
 
     def __str__(self):
-        return '<html>' # pragma: no cover
+        return '<html>'  # pragma: no cover
 
     def toHTML(self):
         return self.input['text']
 
 
 class AnnotateBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def __str__(self):
-        return '<!-->' # pragma: no cover
+        return '<!-->'  # pragma: no cover
 
     def toHTML(self):
         return ''
 
 
 class EmptyBlockHandler(Handler):
     # 处理空行
@@ -127,15 +127,15 @@
 
     def toHTML(self):
         return self.input['word']
 
 # 已废弃
 
 
-class ExtensionBlockHandler(Handler): # pragma: no cover
+class ExtensionBlockHandler(Handler):  # pragma: no cover
     # 自定义扩展
     # {% note %}
     # asdklja
     # {%end%}
 
     def __init__(self, parser=None) -> None:
         super().__init__(parser)
@@ -161,15 +161,15 @@
                 tag = v
                 break
 
         self.block = ExtensionBlock(text=text, tag=tag)
         root.addBlock(self.block)
 
 
-class ExtensionBlock(Block): # pragma: no cover
+class ExtensionBlock(Block):  # pragma: no cover
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
 
         tag = self.input['tag']
@@ -190,15 +190,15 @@
 
 
 class SplitBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
-    def __str__(self): # pragma: no cover
+    def __str__(self):  # pragma: no cover
         return '---<hr>---'
 
     def toHTML(self):
         return '<hr>'
 
 
 class HierarchyIndentHandler(Handler):
@@ -213,17 +213,21 @@
 
     def __call__(self, root: Block, text: str):
 
         match_group = re.match(self.RE, text)
         space_number = len(match_group.group(1))
         word = match_group.group(2)
 
-        block = HierarchyBlock(space_number=space_number, text=text)
-        self.parser.match(block, word)
-        root.addBlock(block)
+        self.block = HierarchyBlock(space_number=space_number, text=text)
+        self.parser.match(self.block, word)
+        # 因为多重 Complex 传递的问题导致的 escape 字符的bug(test8.md)
+        # 暂时没有更好的修改方法...
+        if len(self.block.sub_blocks) == 1:
+            self.block.input['text'] = ' ' * space_number + self.block.sub_blocks[0].input['text']
+        root.addBlock(self.block)
 
 
 class HierarchyBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
@@ -290,37 +294,58 @@
         root.addBlock(block)
 
 
 class HashHeaderBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
+        self.child_blocks = []
+        self.parent_block = None
+        self.UID = None
 
     def toHTML(self):
-
-        tag = 'h' + str(self.input['level'])
-        return f'<{tag}>{self.sub_blocks[0].toHTML()}</{tag}>'
-
+        
+        head_level = str(self.input['level'])
+        tag = f'h{head_level}'
+        if self.UID is not None:
+            tag_id = f'id=\"{tag}-{str(self.UID)}\"'
+        else:
+            tag_id = ''
+        return f'<{tag} {tag_id}>{self.sub_blocks[0].toHTML()}</{tag}>'
+    
+    def to_href(self):
+        '''
+        纯文字形式
+        '''
+        word = ''
+        if self.sub_blocks[0].block_name == "ComplexBlock":
+            block = self.sub_blocks[0]
+            for sblock in block.sub_blocks:
+                word += sblock.input['word']
+        else:
+            word = self.sub_blocks[0].input['word']
+        return word
 
 class TaskListHandler(Handler):
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
         self.RE = re.compile(r'(?<=^[-+\*] )\[([ x])\] (.*)')
 
     def subFunc(self, match: re.Match):
         is_complete = match.group(1)
         word = match.group(2)
 
-        task_block = TaskListBlock(complete=is_complete, word=word, text=match.group())
+        task_block = TaskListBlock(
+            complete=is_complete, word=word, text=match.group())
         replace_name = self.block.register(task_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-        
+
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
@@ -678,36 +703,37 @@
     def __call__(self, root: Block, text: str):
 
         global CONTAINER
         RE = re.compile(r'({-%.*?%-})')
         split_strings = RE.split(text.strip())
 
         count = 0
-
         temp_block = ComplexBlock(text=text)
 
         for string in split_strings:
             # 正常文本字符
             if count % 2 == 0:
                 if string:
                     temp_block.addBlock(TextBlock(word=string, text=string))
             else:
                 id = string[3:-3]
                 class_object: Block = CONTAINER[id]
+                replace_str = class_object.input['text']
                 if class_object is not None:
                     class_object.restore(TextBlock)
                     temp_block.input['text'] = temp_block.input['text'].replace(
-                        string, class_object.input['text'])
+                        string, replace_str)
                     root.input['text'] = root.input['text'].replace(
-                        string, class_object.input['text'])
+                        string, replace_str)
                     temp_block.addBlock(class_object)
                 else:
                     # 由于在解析过程中中间变量使用了{-%.*?%-}的格式进行代替
                     # 所以如果原本的Markdown输入中就包含类似的 {-%asdjkl%-}文字则会出现无法找到的情况
-                    temp_block.addBlock(TextBlock(word=string, text=string)) # pragma: no cover
+                    temp_block.addBlock(
+                        TextBlock(word=string, text=string))  # pragma: no cover
             count += 1
 
         if len(temp_block.sub_blocks) <= 1:
             root.addBlock(temp_block.sub_blocks[0])
         else:
             root.addBlock(temp_block)
```

### Comparing `markdownparser-0.3.9/MarkdownParser/preprocess_parser.py` & `markdownparser-0.4.0/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.3.9/MarkdownParser/tree_parser.py` & `markdownparser-0.4.0/MarkdownParser/tree_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
             else:
                 first_number = None
                 new_sub_blocks.append(block)
 
 # abort
 
 
-class ExtensionOptimizer(Optimizer): # pragma: no cover
+class ExtensionOptimizer(Optimizer):  # pragma: no cover
 
     def __init__(self) -> None:
         super().__init__()
         self.target_block_names = ['ExtensionBlock']
         self.extension_tag = ['note', 'info', 'success']
 
     def __call__(self, root: Block):
@@ -427,15 +427,16 @@
                     else:
                         # 将TableBlock变为纯文本
                         new_sub_blocks.append(
                             TextBlock(text=block.input['text'], word=block.input['text']))
                         match_table = False
                 else:
                     # 第一步匹配失败则将 block 回退为 TextBlock
-                    block = TextBlock(text=block.input['text'], word=block.input['text'])
+                    block = TextBlock(
+                        text=block.input['text'], word=block.input['text'])
                     new_sub_blocks.append(block)
             else:
                 new_sub_blocks.append(block)
 
         if table_block is not None:
             new_sub_blocks.append(table_block)
         root.sub_blocks = new_sub_blocks
```

### Comparing `markdownparser-0.3.9/README.md` & `markdownparser-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 
 html = MarkdownParser.parse('# Hello World!')
 print(html)
 
 #<div class='markdown-body'><h1>Hello World!</h1></div>
 ```
 
-其他接口函数
+接口函数
 
-- `parseFile(file_name:str)->str`: 解析文件
-
-接口类
+```python
+# 解析markdown text
+def parse(text: str) -> str:
 
-- `Markdown`
+# 解析markdown 文件
+def parseFile(file_name: str) -> str:
 
-  使用类创建对象后可以利用 `self.preprocess_parser` `self.block_parser` `self.tree_parser` 控制解析过程
+# 见下方补充说明
+def parse_withtag(text: str) -> str:
 
-  其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构
+def parseFile_withtag(file_name: str) -> str:
+```
 
-  tree可以通过内部toHTML()方法得到HTML元素
+第二个参数为可选项, `has_tag` 表示是否将
 
 ## 测试
 
 ```bash
 python generate.py <FILE_NAME>
 
 # python generate.py ./testfiles/test1.md
@@ -47,14 +50,16 @@
 运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比
 
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)
 
 代码覆盖率
 
 ```bash
+pip install coverage
+
 coverage run -m unittest
 coverage html
 ```
 
 ## 实现思路
 
 [Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)
@@ -79,19 +84,14 @@
 
 ## 不支持
 
 - 四个空格变为代码段
 - [^1]的引用方式
 - Setext 形式的标题
 - 上标 / 下标 / 下划线
-- TOC与锚点
-
-  锚点的添加通常和目录的跳转有关,而目录树的生成可以考虑解析tree的根Block的所有子HashHeaderBlock来构建.
-  
-  因为跳转的功能是js实现,锚点id的加入也会影响html结构,所以暂不支持
 
 ## 补充说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
 - 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
@@ -103,14 +103,35 @@
 
   .markdown-body  ul>li:has(input)>ul {
     list-style-type: none;
     padding-left: 8px;
   }
   ```
 
+- 您可以使用 `parse_withtag` 将 HashHeadBlock 提取出来组成目录树, 得到一个 `<div class="header-navigator">...</div>` 并添加到返回的 HTML 元素中, 您可能还需要一些 js 相关的代码实现跳转, 具体可以参考 [template.html](./template.html)
+
+  ```js
+  let links = document.querySelectorAll('div a[href^="#"]');
+    links.forEach(link => {
+      link.addEventListener('click', function(event) {
+        event.preventDefault();
+        let target = document.querySelector(this.getAttribute('href'));
+        target.scrollIntoView({ behavior: 'smooth' });
+      });
+    });
+  ```
+
+  以及一些样式美化
+
+  ```css
+  .header-navigator {
+    position: fixed;
+  }
+  ```
+
 - 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`
 
   ```html
   <script type="module">
     const codeBlocks = document.querySelectorAll('.language-mermaid');
     codeBlocks.forEach(codeBlock => {
         codeBlock.classList.remove('language-mermaid');
@@ -134,14 +155,15 @@
       };
       </script>
   <script id="MathJax-script" async
   src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
   </script>
   ```
 
-  注意,这里仅支持
+  注意,这里仅支持很少一部分数学公式
+
 
 ## 相关参考
 
 - [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)
 - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)
 - [MathJax](https://docs.mathjax.org/en/latest/web/start.html)
```

#### html2text {}

```diff
@@ -1,51 +1,58 @@
 # MarkdownParser [![codecov](https://codecov.io/gh/luzhixing12345/
 MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/
 luzhixing12345/MarkdownParser) MarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢ ## å®è£ ```bash pip
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
-``` å¶ä»æ¥å£å½æ° - `parseFile(file_name:str)->str`: è§£ææä»¶
-æ¥å£ç±» - `Markdown` ä½¿ç¨ç±»åå»ºå¯¹è±¡åå¯ä»¥å©ç¨
-`self.preprocess_parser` `self.block_parser` `self.tree_parser`
-æ§å¶è§£æè¿ç¨ å¶ä¸­Blockç±»å±æ§è§[base_class.py](MarkdownParser/
-base_class.py),å¯ä»¥éè¿è°ç¨block.info()å½æ°æ¥çæ çç»æ
-treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´  ## æµè¯ ```bash python
-generate.py  # python generate.py ./testfiles/test1.md # python generate.py
-README.md ``` è¿è¡ä¼çæindex.html,
+``` æ¥å£å½æ° ```python # è§£æmarkdown text def parse(text: str) -> str: #
+è§£æmarkdown æä»¶ def parseFile(file_name: str) -> str: #
+è§ä¸æ¹è¡¥åè¯´æ def parse_withtag(text: str) -> str: def
+parseFile_withtag(file_name: str) -> str: ``` ç¬¬äºä¸ªåæ°ä¸ºå¯éé¡¹,
+`has_tag` è¡¨ç¤ºæ¯å¦å° ## æµè¯ ```bash python generate.py  # python
+generate.py ./testfiles/test1.md # python generate.py README.md ```
+è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png) ä»£ç è¦çç ```bash coverage run -m unittest coverage
-html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://
-www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
+20230218202400.png) ä»£ç è¦çç ```bash pip install coverage coverage run -
+m unittest coverage html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°]
+(https://www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
 MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
 text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
 self.preprocess_parser(text) # print(lines) #
 éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser(lines) #
 root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree = self.tree_parser
 (root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶ return tree.toHTML()
 ``` ## ä¸æ¯æ - åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ - [^1]çå¼ç¨æ¹å¼ - Setext
-å½¢å¼çæ é¢ - ä¸æ  / ä¸æ  / ä¸åçº¿ - TOCä¸éç¹
-éç¹çæ·»å éå¸¸åç®å½çè·³è½¬æå³,èç®å½æ ççæå¯ä»¥èèè§£ætreeçæ ¹Blockçææå­HashHeaderBlockæ¥æå»º.
-å ä¸ºè·³è½¬çåè½æ¯jså®ç°,éç¹idçå å¥ä¹ä¼å½±åhtmlç»æ,æä»¥æä¸æ¯æ
-## è¡¥åè¯´æ - çæçç»æå¦ä¸ `
+å½¢å¼çæ é¢ - ä¸æ  / ä¸æ  / ä¸åçº¿ ## è¡¥åè¯´æ -
+çæçç»æå¦ä¸ `
 markdownåå®¹
 ` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
 ```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
 .markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
-} ``` - å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ,
-æ¨å¯åè[mermaid plugin](https://mermaid.js.org/intro/n00b-
-gettingStarted.html#_2-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
+} ``` - æ¨å¯ä»¥ä½¿ç¨ `parse_withtag` å° HashHeadBlock
+æååºæ¥ç»æç®å½æ , å¾å°ä¸ä¸ª `
+...
+` å¹¶æ·»å å°è¿åç HTML åç´ ä¸­, æ¨å¯è½è¿éè¦ä¸äº js
+ç¸å³çä»£ç å®ç°è·³è½¬, å·ä½å¯ä»¥åè [template.html](./
+template.html) ```js let links = document.querySelectorAll('div a[href^="#"]');
+links.forEach(link => { link.addEventListener('click', function(event)
+{ event.preventDefault(); let target = document.querySelector(this.getAttribute
+('href')); target.scrollIntoView({ behavior: 'smooth' }); }); }); ```
+ä»¥åä¸äºæ ·å¼ç¾å ```css .header-navigator { position: fixed; } ``` -
+å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ, æ¨å¯åè
+[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-
+using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
  ``` > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å -
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
- ``` æ³¨æ,è¿éä»æ¯æ ## ç¸å³åè - [Github Markdown CSS](https://
-cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css) - [Mermaid
-API](https://mermaid.js.org/intro/#mermaid-api) - [MathJax](https://
-docs.mathjax.org/en/latest/web/start.html)
+ ``` æ³¨æ,è¿éä»æ¯æå¾å°ä¸é¨åæ°å­¦å¬å¼ ## ç¸å³åè -
+[Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/
+github-markdown.css) - [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)
+- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)
```

### Comparing `markdownparser-0.3.9/setup.py` & `markdownparser-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['markdownparser']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'markdownparser',
-    'version': '0.3.9',
+    'version': '0.4.0',
     'description': '',
-    'long_description': '# MarkdownParser\n\n[![codecov](https://codecov.io/gh/luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/MarkdownParser)\n\nMarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换\n\n## 安装\n\n```bash\npip install markdownparser\n```\n\n## 快速使用\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse(\'# Hello World!\')\nprint(html)\n\n#<div class=\'markdown-body\'><h1>Hello World!</h1></div>\n```\n\n其他接口函数\n\n- `parseFile(file_name:str)->str`: 解析文件\n\n接口类\n\n- `Markdown`\n\n  使用类创建对象后可以利用 `self.preprocess_parser` `self.block_parser` `self.tree_parser` 控制解析过程\n\n  其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构\n\n  tree可以通过内部toHTML()方法得到HTML元素\n\n## 测试\n\n```bash\npython generate.py <FILE_NAME>\n\n# python generate.py ./testfiles/test1.md\n# python generate.py README.md\n```\n\n运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比\n\n![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)\n\n代码覆盖率\n\n```bash\ncoverage run -m unittest\ncoverage html\n```\n\n## 实现思路\n\n[Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)\n\n您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构\n\n```python\ndef parse(self, text: str) -> str:\n\n    # 去除空行/注释/html标签\n    lines = self.preprocess_parser(text)\n    # print(lines)\n    # 逐行解析,得到一颗未优化的树\n    root = self.block_parser(lines)\n    # root.info()\n    # 优化,得到正确的markdown解析树\n    tree = self.tree_parser(root)\n    # tree.info()\n    # 输出到屏幕 / 导出html文件\n    return tree.toHTML()\n```\n\n## 不支持\n\n- 四个空格变为代码段\n- [^1]的引用方式\n- Setext 形式的标题\n- 上标 / 下标 / 下划线\n- TOC与锚点\n\n  锚点的添加通常和目录的跳转有关,而目录树的生成可以考虑解析tree的根Block的所有子HashHeaderBlock来构建.\n  \n  因为跳转的功能是js实现,锚点id的加入也会影响html结构,所以暂不支持\n\n## 补充说明\n\n- 生成的结果如下 `<div class=\'markdown-body\'>markdown内容</div>`\n- 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`\n- 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正\n\n  ```css\n  .markdown-body > ul>li:has(input) {\n    padding-left: 0;\n    margin-bottom: 0;\n  }\n\n  .markdown-body  ul>li:has(input)>ul {\n    list-style-type: none;\n    padding-left: 8px;\n  }\n  ```\n\n- 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script type="module">\n    const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\n    codeBlocks.forEach(codeBlock => {\n        codeBlock.classList.remove(\'language-mermaid\');\n        codeBlock.classList.add(\'mermaid\');\n    });\n    import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\n    mermaid.initialize({ startOnLoad: true });\n  </script>\n  ```\n\n  > **请注意**, 由于本Markdown解析器的CodeBlock解析得到的类名为 `language-mermaid`, 而mermaid插件支持的类名格式为`mermaid`, 所以代码中手动修改了 `language-mermaid` 的类名\n\n- 如果您想添加对Latex数学公式的支持, 可以在html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script>\n      MathJax = {\n        tex: {\n          inlineMath: [[\'$\', \'$\'], [\'\\\\(\', \'\\\\)\']]\n        }\n      };\n      </script>\n  <script id="MathJax-script" async\n  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">\n  </script>\n  ```\n\n  注意,这里仅支持\n\n## 相关参考\n\n- [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)\n- [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)',
+    'long_description': '# MarkdownParser\n\n[![codecov](https://codecov.io/gh/luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/MarkdownParser)\n\nMarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换\n\n## 安装\n\n```bash\npip install markdownparser\n```\n\n## 快速使用\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse(\'# Hello World!\')\nprint(html)\n\n#<div class=\'markdown-body\'><h1>Hello World!</h1></div>\n```\n\n接口函数\n\n```python\n# 解析markdown text\ndef parse(text: str) -> str:\n\n# 解析markdown 文件\ndef parseFile(file_name: str) -> str:\n\n# 见下方补充说明\ndef parse_withtag(text: str) -> str:\n\ndef parseFile_withtag(file_name: str) -> str:\n```\n\n第二个参数为可选项, `has_tag` 表示是否将\n\n## 测试\n\n```bash\npython generate.py <FILE_NAME>\n\n# python generate.py ./testfiles/test1.md\n# python generate.py README.md\n```\n\n运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比\n\n![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)\n\n代码覆盖率\n\n```bash\npip install coverage\n\ncoverage run -m unittest\ncoverage html\n```\n\n## 实现思路\n\n[Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)\n\n您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构\n\n```python\ndef parse(self, text: str) -> str:\n\n    # 去除空行/注释/html标签\n    lines = self.preprocess_parser(text)\n    # print(lines)\n    # 逐行解析,得到一颗未优化的树\n    root = self.block_parser(lines)\n    # root.info()\n    # 优化,得到正确的markdown解析树\n    tree = self.tree_parser(root)\n    # tree.info()\n    # 输出到屏幕 / 导出html文件\n    return tree.toHTML()\n```\n\n## 不支持\n\n- 四个空格变为代码段\n- [^1]的引用方式\n- Setext 形式的标题\n- 上标 / 下标 / 下划线\n\n## 补充说明\n\n- 生成的结果如下 `<div class=\'markdown-body\'>markdown内容</div>`\n- 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`\n- 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正\n\n  ```css\n  .markdown-body > ul>li:has(input) {\n    padding-left: 0;\n    margin-bottom: 0;\n  }\n\n  .markdown-body  ul>li:has(input)>ul {\n    list-style-type: none;\n    padding-left: 8px;\n  }\n  ```\n\n- 您可以使用 `parse_withtag` 将 HashHeadBlock 提取出来组成目录树, 得到一个 `<div class="header-navigator">...</div>` 并添加到返回的 HTML 元素中, 您可能还需要一些 js 相关的代码实现跳转, 具体可以参考 [template.html](./template.html)\n\n  ```js\n  let links = document.querySelectorAll(\'div a[href^="#"]\');\n    links.forEach(link => {\n      link.addEventListener(\'click\', function(event) {\n        event.preventDefault();\n        let target = document.querySelector(this.getAttribute(\'href\'));\n        target.scrollIntoView({ behavior: \'smooth\' });\n      });\n    });\n  ```\n\n  以及一些样式美化\n\n  ```css\n  .header-navigator {\n    position: fixed;\n  }\n  ```\n\n- 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script type="module">\n    const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\n    codeBlocks.forEach(codeBlock => {\n        codeBlock.classList.remove(\'language-mermaid\');\n        codeBlock.classList.add(\'mermaid\');\n    });\n    import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\n    mermaid.initialize({ startOnLoad: true });\n  </script>\n  ```\n\n  > **请注意**, 由于本Markdown解析器的CodeBlock解析得到的类名为 `language-mermaid`, 而mermaid插件支持的类名格式为`mermaid`, 所以代码中手动修改了 `language-mermaid` 的类名\n\n- 如果您想添加对Latex数学公式的支持, 可以在html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script>\n      MathJax = {\n        tex: {\n          inlineMath: [[\'$\', \'$\'], [\'\\\\(\', \'\\\\)\']]\n        }\n      };\n      </script>\n  <script id="MathJax-script" async\n  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">\n  </script>\n  ```\n\n  注意,这里仅支持很少一部分数学公式\n\n\n## 相关参考\n\n- [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)\n- [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)',
     'author': 'luzhixing12345',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/MarkdownParser',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,66 +1,71 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['markdownparser'] package_data = \ {'': ['*']} setup_kwargs = { 'name':
-'markdownparser', 'version': '0.3.9', 'description': '', 'long_description': '#
+'markdownparser', 'version': '0.4.0', 'description': '', 'long_description': '#
 MarkdownParser\n\n[![codecov](https://codecov.io/gh/luzhixing12345/
 MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/
 luzhixing12345/MarkdownParser)\n\nMarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢\n\n##
 å®è£\n\n```bash\npip install markdownparser\n```\n\n##
 å¿«éä½¿ç¨\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse
 (\'# Hello World!\')\nprint(html)\n\n#
 ****** Hello World! ******
-\n```\n\nå¶ä»æ¥å£å½æ°\n\n- `parseFile(file_name:str)->str`:
-è§£ææä»¶\n\næ¥å£ç±»\n\n- `Markdown`\n\n
-ä½¿ç¨ç±»åå»ºå¯¹è±¡åå¯ä»¥å©ç¨ `self.preprocess_parser`
-`self.block_parser` `self.tree_parser` æ§å¶è§£æè¿ç¨\n\n
-å¶ä¸­Blockç±»å±æ§è§[base_class.py](MarkdownParser/
-base_class.py),å¯ä»¥éè¿è°ç¨block.info()å½æ°æ¥çæ çç»æ\n\n
-treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´ \n\n##
-æµè¯\n\n```bash\npython generate.py \n\n# python generate.py ./testfiles/
-test1.md\n# python generate.py README.md\n```\n\nè¿è¡ä¼çæindex.html,
+\n```\n\næ¥å£å½æ°\n\n```python\n# è§£æmarkdown text\ndef parse(text: str)
+-> str:\n\n# è§£æmarkdown æä»¶\ndef parseFile(file_name: str) -> str:\n\n#
+è§ä¸æ¹è¡¥åè¯´æ\ndef parse_withtag(text: str) -> str:\n\ndef
+parseFile_withtag(file_name: str) -> str:\n```\n\nç¬¬äºä¸ªåæ°ä¸ºå¯éé¡¹,
+`has_tag` è¡¨ç¤ºæ¯å¦å°\n\n## æµè¯\n\n```bash\npython generate.py \n\n#
+python generate.py ./testfiles/test1.md\n# python generate.py
+README.md\n```\n\nè¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯\n\n!
 [20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png)\n\nä»£ç è¦çç\n\n```bash\ncoverage run -
-m unittest\ncoverage html\n```\n\n## å®ç°æè·¯\n\n
+20230218202400.png)\n\nä»£ç è¦çç\n\n```bash\npip install
+coverage\n\ncoverage run -m unittest\ncoverage html\n```\n\n## å®ç°æè·¯\n\n
 [Markdownè§£æå¨çä»£ç å®ç°](https://www.bilibili.com/video/
 BV1LA411X7X3)\n\næ¨å¯éè¿åæ¶ [core.py](./MarkdownParser/core.py)
 æ³¨éæ¥è·åæ çç»æ\n\n```python\ndef parse(self, text: str) -> str:
 \n\n # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾\n lines = self.preprocess_parser(text)\n
 # print(lines)\n # éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ \n root =
 self.block_parser(lines)\n # root.info()\n #
 ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ \n tree = self.tree_parser(root)\n #
 tree.info()\n # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶\n return tree.toHTML
 ()\n```\n\n## ä¸æ¯æ\n\n- åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ\n-
-[^1]çå¼ç¨æ¹å¼\n- Setext å½¢å¼çæ é¢\n- ä¸æ  / ä¸æ  / ä¸åçº¿\n-
-TOCä¸éç¹\n\n
-éç¹çæ·»å éå¸¸åç®å½çè·³è½¬æå³,èç®å½æ ççæå¯ä»¥èèè§£ætreeçæ ¹Blockçææå­HashHeaderBlockæ¥æå»º.\n
-\n
-å ä¸ºè·³è½¬çåè½æ¯jså®ç°,éç¹idçå å¥ä¹ä¼å½±åhtmlç»æ,æä»¥æä¸æ¯æ\n\n##
-è¡¥åè¯´æ\n\n- çæçç»æå¦ä¸ `
+[^1]çå¼ç¨æ¹å¼\n- Setext å½¢å¼çæ é¢\n- ä¸æ  / ä¸æ  /
+ä¸åçº¿\n\n## è¡¥åè¯´æ\n\n- çæçç»æå¦ä¸ `
 markdownåå®¹
 `\n- ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN`\n-
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£\n\n
 ```css\n .markdown-body > ul>li:has(input) {\n padding-left: 0;\n margin-
 bottom: 0;\n }\n\n .markdown-body ul>li:has(input)>ul {\n list-style-type:
-none;\n padding-left: 8px;\n }\n ```\n\n- å¦ææ¨æ³æ·»å å¯¹[Mermaid](https:
-//mermaid.js.org/)çæ¯æ, æ¨å¯åè[mermaid plugin](https://
-mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-
-plugins)å¨æ¨çhtmlé¡µé¢ `
+none;\n padding-left: 8px;\n }\n ```\n\n- æ¨å¯ä»¥ä½¿ç¨ `parse_withtag` å°
+HashHeadBlock æååºæ¥ç»æç®å½æ , å¾å°ä¸ä¸ª `
+...
+` å¹¶æ·»å å°è¿åç HTML åç´ ä¸­, æ¨å¯è½è¿éè¦ä¸äº js
+ç¸å³çä»£ç å®ç°è·³è½¬, å·ä½å¯ä»¥åè [template.html](./
+template.html)\n\n ```js\n let links = document.querySelectorAll(\'div a
+[href^="#"]\');\n links.forEach(link => {\n link.addEventListener(\'click\',
+function(event) {\n event.preventDefault();\n let target =
+document.querySelector(this.getAttribute(\'href\'));\n target.scrollIntoView(
+{ behavior: \'smooth\' });\n });\n });\n ```\n\n ä»¥åä¸äºæ ·å¼ç¾å\n\n
+```css\n .header-navigator {\n position: fixed;\n }\n ```\n\n-
+å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ, æ¨å¯åè
+[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-
+using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
 \n ```\n\n > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å\n\n-
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
 \n
 n src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">\n
-\n ```\n\n æ³¨æ,è¿éä»æ¯æ\n\n## ç¸å³åè\n\n- [Github Markdown CSS]
-(https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)\n-
-[Mermaid API](https://mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://
-docs.mathjax.org/en/latest/web/start.html)', 'author': 'luzhixing12345',
-'author_email': 'luzhixing12345@163.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/luzhixing12345/
-MarkdownParser', 'packages': packages, 'package_data': package_data,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+\n ```\n\n æ³¨æ,è¿éä»æ¯æå¾å°ä¸é¨åæ°å­¦å¬å¼\n\n\n##
+ç¸å³åè\n\n- [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-
+markdown-css@4.0.0/github-markdown.css)\n- [Mermaid API](https://
+mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://docs.mathjax.org/en/
+latest/web/start.html)', 'author': 'luzhixing12345', 'author_email':
+'luzhixing12345@163.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'https://github.com/luzhixing12345/MarkdownParser', 'packages':
+packages, 'package_data': package_data, 'python_requires': '>=3.7,<4.0', }
+setup(**setup_kwargs)
```

### Comparing `markdownparser-0.3.9/PKG-INFO` & `markdownparser-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 726b  : 2.1.Name: mark
 00000020: 646f 776e 7061 7273 6572 0a56 6572 7369  downparser.Versi
-00000030: 6f6e 3a20 302e 332e 390a 5375 6d6d 6172  on: 0.3.9.Summar
+00000030: 6f6e 3a20 302e 342e 300a 5375 6d6d 6172  on: 0.4.0.Summar
 00000040: 793a 200a 486f 6d65 2d70 6167 653a 2068  y: .Home-page: h
 00000050: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000060: 6d2f 6c75 7a68 6978 696e 6731 3233 3435  m/luzhixing12345
 00000070: 2f4d 6172 6b64 6f77 6e50 6172 7365 720a  /MarkdownParser.
 00000080: 4c69 6365 6e73 653a 204d 4954 0a41 7574  License: MIT.Aut
 00000090: 686f 723a 206c 757a 6869 7869 6e67 3132  hor: luzhixing12
 000000a0: 3334 350a 4175 7468 6f72 2d65 6d61 696c  345.Author-email
@@ -72,248 +72,274 @@
 00000470: 6172 6b64 6f77 6e50 6172 7365 722e 7061  arkdownParser.pa
 00000480: 7273 6528 2723 2048 656c 6c6f 2057 6f72  rse('# Hello Wor
 00000490: 6c64 2127 290a 7072 696e 7428 6874 6d6c  ld!').print(html
 000004a0: 290a 0a23 3c64 6976 2063 6c61 7373 3d27  )..#<div class='
 000004b0: 6d61 726b 646f 776e 2d62 6f64 7927 3e3c  markdown-body'><
 000004c0: 6831 3e48 656c 6c6f 2057 6f72 6c64 213c  h1>Hello World!<
 000004d0: 2f68 313e 3c2f 6469 763e 0a60 6060 0a0a  /h1></div>.```..
-000004e0: e585 b6e4 bb96 e68e a5e5 8fa3 e587 bde6  ................
-000004f0: 95b0 0a0a 2d20 6070 6172 7365 4669 6c65  ....- `parseFile
-00000500: 2866 696c 655f 6e61 6d65 3a73 7472 292d  (file_name:str)-
-00000510: 3e73 7472 603a 20e8 a7a3 e69e 90e6 9687  >str`: .........
-00000520: e4bb b60a 0ae6 8ea5 e58f a3e7 b1bb 0a0a  ................
-00000530: 2d20 604d 6172 6b64 6f77 6e60 0a0a 2020  - `Markdown`..  
-00000540: e4bd bfe7 94a8 e7b1 bbe5 889b e5bb bae5  ................
-00000550: afb9 e8b1 a1e5 908e e58f afe4 bba5 e588  ................
-00000560: a9e7 94a8 2060 7365 6c66 2e70 7265 7072  .... `self.prepr
-00000570: 6f63 6573 735f 7061 7273 6572 6020 6073  ocess_parser` `s
-00000580: 656c 662e 626c 6f63 6b5f 7061 7273 6572  elf.block_parser
-00000590: 6020 6073 656c 662e 7472 6565 5f70 6172  ` `self.tree_par
-000005a0: 7365 7260 20e6 8ea7 e588 b6e8 a7a3 e69e  ser` ...........
-000005b0: 90e8 bf87 e7a8 8b0a 0a20 20e5 85b6 e4b8  .........  .....
-000005c0: ad42 6c6f 636b e7b1 bbe5 b19e e680 a7e8  .Block..........
-000005d0: a781 5b62 6173 655f 636c 6173 732e 7079  ..[base_class.py
-000005e0: 5d28 4d61 726b 646f 776e 5061 7273 6572  ](MarkdownParser
-000005f0: 2f62 6173 655f 636c 6173 732e 7079 292c  /base_class.py),
-00000600: e58f afe4 bba5 e980 9ae8 bf87 e8b0 83e7  ................
-00000610: 94a8 626c 6f63 6b2e 696e 666f 2829 e587  ..block.info()..
-00000620: bde6 95b0 e69f a5e7 9c8b e6a0 91e7 9a84  ................
-00000630: e7bb 93e6 9e84 0a0a 2020 7472 6565 e58f  ........  tree..
-00000640: afe4 bba5 e980 9ae8 bf87 e586 85e9 83a8  ................
-00000650: 746f 4854 4d4c 2829 e696 b9e6 b395 e5be  toHTML()........
-00000660: 97e5 88b0 4854 4d4c e585 83e7 b4a0 0a0a  ....HTML........
-00000670: 2323 20e6 b58b e8af 950a 0a60 6060 6261  ## ........```ba
-00000680: 7368 0a70 7974 686f 6e20 6765 6e65 7261  sh.python genera
-00000690: 7465 2e70 7920 3c46 494c 455f 4e41 4d45  te.py <FILE_NAME
-000006a0: 3e0a 0a23 2070 7974 686f 6e20 6765 6e65  >..# python gene
-000006b0: 7261 7465 2e70 7920 2e2f 7465 7374 6669  rate.py ./testfi
-000006c0: 6c65 732f 7465 7374 312e 6d64 0a23 2070  les/test1.md.# p
-000006d0: 7974 686f 6e20 6765 6e65 7261 7465 2e70  ython generate.p
-000006e0: 7920 5245 4144 4d45 2e6d 640a 6060 600a  y README.md.```.
-000006f0: 0ae8 bf90 e8a1 8ce4 bc9a e794 9fe6 8890  ................
-00000700: 696e 6465 782e 6874 6d6c 2c20 e4bd bfe7  index.html, ....
-00000710: 94a8 e6b5 8fe8 a788 e599 a8e6 8993 e5bc  ................
-00000720: 80e7 949f e688 90e7 9a84 696e 6465 782e  ..........index.
-00000730: 6874 6d6c e58d b3e5 8faf e4b8 8ee6 82a8  html............
-00000740: e79a 844d 6172 6b64 6f77 6ee7 bc96 e8be  ...Markdown.....
-00000750: 91e5 99a8 e79a 84e9 a284 e69c 9fe6 b8b2  ................
-00000760: e69f 93e7 bb93 e69e 9ce5 afb9 e6af 940a  ................
-00000770: 0a21 5b32 3032 3330 3231 3832 3032 3430  .![2023021820240
-00000780: 305d 2868 7474 7073 3a2f 2f72 6177 2e67  0](https://raw.g
-00000790: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000007a0: 2e63 6f6d 2f6c 6561 726e 6572 2d6c 752f  .com/learner-lu/
-000007b0: 7069 6362 6564 2f6d 6173 7465 722f 3230  picbed/master/20
-000007c0: 3233 3032 3138 3230 3234 3030 2e70 6e67  230218202400.png
-000007d0: 290a 0ae4 bba3 e7a0 81e8 a686 e79b 96e7  )...............
-000007e0: 8e87 0a0a 6060 6062 6173 680a 636f 7665  ....```bash.cove
-000007f0: 7261 6765 2072 756e 202d 6d20 756e 6974  rage run -m unit
-00000800: 7465 7374 0a63 6f76 6572 6167 6520 6874  test.coverage ht
-00000810: 6d6c 0a60 6060 0a0a 2323 20e5 ae9e e78e  ml.```..## .....
-00000820: b0e6 809d e8b7 af0a 0a5b 4d61 726b 646f  .........[Markdo
-00000830: 776e e8a7 a3e6 9e90 e599 a8e7 9a84 e4bb  wn..............
-00000840: a3e7 a081 e5ae 9ee7 8eb0 5d28 6874 7470  ..........](http
-00000850: 733a 2f2f 7777 772e 6269 6c69 6269 6c69  s://www.bilibili
-00000860: 2e63 6f6d 2f76 6964 656f 2f42 5631 4c41  .com/video/BV1LA
-00000870: 3431 3158 3758 3329 0a0a e682 a8e5 8faf  411X7X3)........
-00000880: e980 9ae8 bf87 e58f 96e6 b688 205b 636f  ............ [co
-00000890: 7265 2e70 795d 282e 2f4d 6172 6b64 6f77  re.py](./Markdow
-000008a0: 6e50 6172 7365 722f 636f 7265 2e70 7929  nParser/core.py)
-000008b0: 20e6 b3a8 e987 8ae6 9da5 e88e b7e5 8f96   ...............
-000008c0: e6a0 91e7 9a84 e7bb 93e6 9e84 0a0a 6060  ..............``
-000008d0: 6070 7974 686f 6e0a 6465 6620 7061 7273  `python.def pars
-000008e0: 6528 7365 6c66 2c20 7465 7874 3a20 7374  e(self, text: st
-000008f0: 7229 202d 3e20 7374 723a 0a0a 2020 2020  r) -> str:..    
-00000900: 2320 e58e bbe9 99a4 e7a9 bae8 a18c 2fe6  # ............/.
-00000910: b3a8 e987 8a2f 6874 6d6c e6a0 87e7 adbe  ...../html......
-00000920: 0a20 2020 206c 696e 6573 203d 2073 656c  .    lines = sel
-00000930: 662e 7072 6570 726f 6365 7373 5f70 6172  f.preprocess_par
-00000940: 7365 7228 7465 7874 290a 2020 2020 2320  ser(text).    # 
-00000950: 7072 696e 7428 6c69 6e65 7329 0a20 2020  print(lines).   
-00000960: 2023 20e9 8090 e8a1 8ce8 a7a3 e69e 902c   # ............,
-00000970: e5be 97e5 88b0 e4b8 80e9 a297 e69c aae4  ................
-00000980: bc98 e58c 96e7 9a84 e6a0 910a 2020 2020  ............    
-00000990: 726f 6f74 203d 2073 656c 662e 626c 6f63  root = self.bloc
-000009a0: 6b5f 7061 7273 6572 286c 696e 6573 290a  k_parser(lines).
-000009b0: 2020 2020 2320 726f 6f74 2e69 6e66 6f28      # root.info(
-000009c0: 290a 2020 2020 2320 e4bc 98e5 8c96 2ce5  ).    # ......,.
-000009d0: be97 e588 b0e6 ada3 e7a1 aee7 9a84 6d61  ..............ma
-000009e0: 726b 646f 776e e8a7 a3e6 9e90 e6a0 910a  rkdown..........
-000009f0: 2020 2020 7472 6565 203d 2073 656c 662e      tree = self.
-00000a00: 7472 6565 5f70 6172 7365 7228 726f 6f74  tree_parser(root
-00000a10: 290a 2020 2020 2320 7472 6565 2e69 6e66  ).    # tree.inf
-00000a20: 6f28 290a 2020 2020 2320 e8be 93e5 87ba  o().    # ......
-00000a30: e588 b0e5 b18f e5b9 9520 2f20 e5af bce5  ......... / ....
-00000a40: 87ba 6874 6d6c e696 87e4 bbb6 0a20 2020  ..html.......   
-00000a50: 2072 6574 7572 6e20 7472 6565 2e74 6f48   return tree.toH
-00000a60: 544d 4c28 290a 6060 600a 0a23 2320 e4b8  TML().```..## ..
-00000a70: 8de6 94af e68c 810a 0a2d 20e5 9b9b e4b8  .........- .....
-00000a80: aae7 a9ba e6a0 bce5 8f98 e4b8 bae4 bba3  ................
-00000a90: e7a0 81e6 aeb5 0a2d 205b 5e31 5de7 9a84  .......- [^1]...
-00000aa0: e5bc 95e7 94a8 e696 b9e5 bc8f 0a2d 2053  .............- S
-00000ab0: 6574 6578 7420 e5bd a2e5 bc8f e79a 84e6  etext ..........
-00000ac0: a087 e9a2 980a 2d20 e4b8 8ae6 a087 202f  ......- ...... /
-00000ad0: 20e4 b88b e6a0 8720 2f20 e4b8 8be5 8892   ...... / ......
-00000ae0: e7ba bf0a 2d20 544f 43e4 b88e e994 9ae7  ....- TOC.......
-00000af0: 82b9 0a0a 2020 e994 9ae7 82b9 e79a 84e6  ....  ..........
-00000b00: b7bb e58a a0e9 809a e5b8 b8e5 928c e79b  ................
-00000b10: aee5 bd95 e79a 84e8 b7b3 e8bd ace6 9c89  ................
-00000b20: e585 b32c e880 8ce7 9bae e5bd 95e6 a091  ...,............
-00000b30: e79a 84e7 949f e688 90e5 8faf e4bb a5e8  ................
-00000b40: 8083 e899 91e8 a7a3 e69e 9074 7265 65e7  ...........tree.
-00000b50: 9a84 e6a0 b942 6c6f 636b e79a 84e6 8980  .....Block......
-00000b60: e69c 89e5 ad90 4861 7368 4865 6164 6572  ......HashHeader
-00000b70: 426c 6f63 6be6 9da5 e69e 84e5 bbba 2e0a  Block...........
-00000b80: 2020 0a20 20e5 9ba0 e4b8 bae8 b7b3 e8bd    .  ...........
-00000b90: ace7 9a84 e58a 9fe8 83bd e698 af6a 73e5  .............js.
-00000ba0: ae9e e78e b02c e994 9ae7 82b9 6964 e79a  .....,......id..
-00000bb0: 84e5 8aa0 e585 a5e4 b99f e4bc 9ae5 bdb1  ................
-00000bc0: e593 8d68 746d 6ce7 bb93 e69e 842c e689  ...html......,..
-00000bd0: 80e4 bba5 e69a 82e4 b88d e694 afe6 8c81  ................
-00000be0: 0a0a 2323 20e8 a1a5 e585 85e8 afb4 e698  ..## ...........
-00000bf0: 8e0a 0a2d 20e7 949f e688 90e7 9a84 e7bb  ...- ...........
-00000c00: 93e6 9e9c e5a6 82e4 b88b 2060 3c64 6976  .......... `<div
-00000c10: 2063 6c61 7373 3d27 6d61 726b 646f 776e   class='markdown
-00000c20: 2d62 6f64 7927 3e6d 6172 6b64 6f77 6ee5  -body'>markdown.
-00000c30: 8685 e5ae b93c 2f64 6976 3e60 0a2d 20e4  .....</div>`.- .
-00000c40: bba3 e7a0 81e6 aeb5 e4bc 9ae6 a0b9 e68d  ................
-00000c50: aee8 afad e8a8 80e5 8aa0 e585 a5e4 b880  ................
-00000c60: e4b8 aae7 b1bb e590 8de4 bebf e4ba 8ee5  ................
-00000c70: 908e e69c 9fe9 ab98 e4ba ae2c e4be 8be5  ...........,....
-00000c80: a682 2060 636c 6173 733d 226c 616e 6775  .. `class="langu
-00000c90: 6167 652d 6370 7022 602c 20e6 9caa e5ae  age-cpp"`, .....
-00000ca0: 9ae4 b989 e8af ade8 a880 e588 99e4 b8ba  ................
-00000cb0: 2060 6c61 6e67 7561 6765 2d55 4e4b 4e4f   `language-UNKNO
-00000cc0: 574e 600a 2d20 e9bb 98e8 aea4 e5af bce5  WN`.- ..........
-00000cd0: 87ba e79a 8448 544d 4ce4 b8ad e5b1 82e7  .....HTML.......
-00000ce0: baa7 e4bb bbe5 8aa1 e588 97e8 a1a8 e4bc  ................
-00000cf0: 9ae6 9c89 e698 bee7 a4ba e997 aee9 a298  ................
-00000d00: 2ce8 bf99 e698 afe5 9ba0 e4b8 bae4 bdbf  ,...............
-00000d10: e794 a8e4 ba86 756c 2b6c 692b 6368 6563  ......ul+li+chec
-00000d20: 6b62 6f78 e79a 84e6 96b9 e5bc 8f2c e682  kbox.........,..
-00000d30: a8e9 9c80 e8a6 81e6 b7bb e58a a0e4 bba5  ................
-00000d40: e4b8 8b63 7373 e6a0 b7e5 bc8f e4bf aee6  ...css..........
-00000d50: ada3 0a0a 2020 6060 6063 7373 0a20 202e  ....  ```css.  .
-00000d60: 6d61 726b 646f 776e 2d62 6f64 7920 3e20  markdown-body > 
-00000d70: 756c 3e6c 693a 6861 7328 696e 7075 7429  ul>li:has(input)
-00000d80: 207b 0a20 2020 2070 6164 6469 6e67 2d6c   {.    padding-l
-00000d90: 6566 743a 2030 3b0a 2020 2020 6d61 7267  eft: 0;.    marg
-00000da0: 696e 2d62 6f74 746f 6d3a 2030 3b0a 2020  in-bottom: 0;.  
-00000db0: 7d0a 0a20 202e 6d61 726b 646f 776e 2d62  }..  .markdown-b
-00000dc0: 6f64 7920 2075 6c3e 6c69 3a68 6173 2869  ody  ul>li:has(i
-00000dd0: 6e70 7574 293e 756c 207b 0a20 2020 206c  nput)>ul {.    l
-00000de0: 6973 742d 7374 796c 652d 7479 7065 3a20  ist-style-type: 
-00000df0: 6e6f 6e65 3b0a 2020 2020 7061 6464 696e  none;.    paddin
-00000e00: 672d 6c65 6674 3a20 3870 783b 0a20 207d  g-left: 8px;.  }
-00000e10: 0a20 2060 6060 0a0a 2d20 e5a6 82e6 9e9c  .  ```..- ......
-00000e20: e682 a8e6 83b3 e6b7 bbe5 8aa0 e5af b95b  ...............[
-00000e30: 4d65 726d 6169 645d 2868 7474 7073 3a2f  Mermaid](https:/
-00000e40: 2f6d 6572 6d61 6964 2e6a 732e 6f72 672f  /mermaid.js.org/
-00000e50: 29e7 9a84 e694 afe6 8c81 2c20 e682 a8e5  )........., ....
-00000e60: 8faf e58f 82e8 8083 5b6d 6572 6d61 6964  ........[mermaid
-00000e70: 2070 6c75 6769 6e5d 2868 7474 7073 3a2f   plugin](https:/
-00000e80: 2f6d 6572 6d61 6964 2e6a 732e 6f72 672f  /mermaid.js.org/
-00000e90: 696e 7472 6f2f 6e30 3062 2d67 6574 7469  intro/n00b-getti
-00000ea0: 6e67 5374 6172 7465 642e 6874 6d6c 235f  ngStarted.html#_
-00000eb0: 322d 7573 696e 672d 6d65 726d 6169 642d  2-using-mermaid-
-00000ec0: 706c 7567 696e 7329 e59c a8e6 82a8 e79a  plugins)........
-00000ed0: 8468 746d 6ce9 a1b5 e99d a220 603c 626f  .html...... `<bo
-00000ee0: 6479 3e60 20e6 9cab e5b0 bee6 b7bb e58a  dy>` ...........
-00000ef0: a0e5 a682 e4b8 8b20 603c 7363 7269 7074  ....... `<script
-00000f00: 3e60 0a0a 2020 6060 6068 746d 6c0a 2020  >`..  ```html.  
-00000f10: 3c73 6372 6970 7420 7479 7065 3d22 6d6f  <script type="mo
-00000f20: 6475 6c65 223e 0a20 2020 2063 6f6e 7374  dule">.    const
-00000f30: 2063 6f64 6542 6c6f 636b 7320 3d20 646f   codeBlocks = do
-00000f40: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
-00000f50: 6374 6f72 416c 6c28 272e 6c61 6e67 7561  ctorAll('.langua
-00000f60: 6765 2d6d 6572 6d61 6964 2729 3b0a 2020  ge-mermaid');.  
-00000f70: 2020 636f 6465 426c 6f63 6b73 2e66 6f72    codeBlocks.for
-00000f80: 4561 6368 2863 6f64 6542 6c6f 636b 203d  Each(codeBlock =
-00000f90: 3e20 7b0a 2020 2020 2020 2020 636f 6465  > {.        code
-00000fa0: 426c 6f63 6b2e 636c 6173 734c 6973 742e  Block.classList.
-00000fb0: 7265 6d6f 7665 2827 6c61 6e67 7561 6765  remove('language
-00000fc0: 2d6d 6572 6d61 6964 2729 3b0a 2020 2020  -mermaid');.    
-00000fd0: 2020 2020 636f 6465 426c 6f63 6b2e 636c      codeBlock.cl
-00000fe0: 6173 734c 6973 742e 6164 6428 276d 6572  assList.add('mer
-00000ff0: 6d61 6964 2729 3b0a 2020 2020 7d29 3b0a  maid');.    });.
-00001000: 2020 2020 696d 706f 7274 206d 6572 6d61      import merma
-00001010: 6964 2066 726f 6d20 2768 7474 7073 3a2f  id from 'https:/
-00001020: 2f63 646e 2e6a 7364 656c 6976 722e 6e65  /cdn.jsdelivr.ne
-00001030: 742f 6e70 6d2f 6d65 726d 6169 6440 3130  t/npm/mermaid@10
-00001040: 2f64 6973 742f 6d65 726d 6169 642e 6573  /dist/mermaid.es
-00001050: 6d2e 6d69 6e2e 6d6a 7327 3b0a 2020 2020  m.min.mjs';.    
-00001060: 6d65 726d 6169 642e 696e 6974 6961 6c69  mermaid.initiali
-00001070: 7a65 287b 2073 7461 7274 4f6e 4c6f 6164  ze({ startOnLoad
-00001080: 3a20 7472 7565 207d 293b 0a20 203c 2f73  : true });.  </s
-00001090: 6372 6970 743e 0a20 2060 6060 0a0a 2020  cript>.  ```..  
-000010a0: 3e20 2a2a e8af b7e6 b3a8 e684 8f2a 2a2c  > **.........**,
-000010b0: 20e7 94b1 e4ba 8ee6 9cac 4d61 726b 646f   .........Markdo
-000010c0: 776e e8a7 a3e6 9e90 e599 a8e7 9a84 436f  wn............Co
-000010d0: 6465 426c 6f63 6be8 a7a3 e69e 90e5 be97  deBlock.........
-000010e0: e588 b0e7 9a84 e7b1 bbe5 908d e4b8 ba20  ............... 
-000010f0: 606c 616e 6775 6167 652d 6d65 726d 6169  `language-mermai
-00001100: 6460 2c20 e880 8c6d 6572 6d61 6964 e68f  d`, ...mermaid..
-00001110: 92e4 bbb6 e694 afe6 8c81 e79a 84e7 b1bb  ................
-00001120: e590 8de6 a0bc e5bc 8fe4 b8ba 606d 6572  ............`mer
-00001130: 6d61 6964 602c 20e6 8980 e4bb a5e4 bba3  maid`, .........
-00001140: e7a0 81e4 b8ad e689 8be5 8aa8 e4bf aee6  ................
-00001150: 94b9 e4ba 8620 606c 616e 6775 6167 652d  ..... `language-
-00001160: 6d65 726d 6169 6460 20e7 9a84 e7b1 bbe5  mermaid` .......
-00001170: 908d 0a0a 2d20 e5a6 82e6 9e9c e682 a8e6  ....- ..........
-00001180: 83b3 e6b7 bbe5 8aa0 e5af b94c 6174 6578  ...........Latex
-00001190: e695 b0e5 ada6 e585 ace5 bc8f e79a 84e6  ................
-000011a0: 94af e68c 812c 20e5 8faf e4bb a5e5 9ca8  ....., .........
-000011b0: 6874 6d6c e9a1 b5e9 9da2 2060 3c62 6f64  html...... `<bod
-000011c0: 793e 6020 e69c abe5 b0be e6b7 bbe5 8aa0  y>` ............
-000011d0: e5a6 82e4 b88b 2060 3c73 6372 6970 743e  ...... `<script>
-000011e0: 600a 0a20 2060 6060 6874 6d6c 0a20 203c  `..  ```html.  <
-000011f0: 7363 7269 7074 3e0a 2020 2020 2020 4d61  script>.      Ma
-00001200: 7468 4a61 7820 3d20 7b0a 2020 2020 2020  thJax = {.      
-00001210: 2020 7465 783a 207b 0a20 2020 2020 2020    tex: {.       
-00001220: 2020 2069 6e6c 696e 654d 6174 683a 205b     inlineMath: [
-00001230: 5b27 2427 2c20 2724 275d 2c20 5b27 5c5c  ['$', '$'], ['\\
-00001240: 2827 2c20 275c 5c29 275d 5d0a 2020 2020  (', '\\)']].    
-00001250: 2020 2020 7d0a 2020 2020 2020 7d3b 0a20      }.      };. 
-00001260: 2020 2020 203c 2f73 6372 6970 743e 0a20       </script>. 
-00001270: 203c 7363 7269 7074 2069 643d 224d 6174   <script id="Mat
-00001280: 684a 6178 2d73 6372 6970 7422 2061 7379  hJax-script" asy
-00001290: 6e63 0a20 2073 7263 3d22 6874 7470 733a  nc.  src="https:
-000012a0: 2f2f 6364 6e2e 6a73 6465 6c69 7672 2e6e  //cdn.jsdelivr.n
-000012b0: 6574 2f6e 706d 2f6d 6174 686a 6178 4033  et/npm/mathjax@3
-000012c0: 2f65 7335 2f74 6578 2d63 6874 6d6c 2e6a  /es5/tex-chtml.j
-000012d0: 7322 3e0a 2020 3c2f 7363 7269 7074 3e0a  s">.  </script>.
-000012e0: 2020 6060 600a 0a20 20e6 b3a8 e684 8f2c    ```..  ......,
-000012f0: e8bf 99e9 878c e4bb 85e6 94af e68c 810a  ................
-00001300: 0a23 2320 e79b b8e5 85b3 e58f 82e8 8083  .## ............
-00001310: 0a0a 2d20 5b47 6974 6875 6220 4d61 726b  ..- [Github Mark
-00001320: 646f 776e 2043 5353 5d28 6874 7470 733a  down CSS](https:
-00001330: 2f2f 6364 6e2e 6a73 6465 6c69 7672 2e6e  //cdn.jsdelivr.n
-00001340: 6574 2f6e 706d 2f67 6974 6875 622d 6d61  et/npm/github-ma
-00001350: 726b 646f 776e 2d63 7373 4034 2e30 2e30  rkdown-css@4.0.0
-00001360: 2f67 6974 6875 622d 6d61 726b 646f 776e  /github-markdown
-00001370: 2e63 7373 290a 2d20 5b4d 6572 6d61 6964  .css).- [Mermaid
-00001380: 2041 5049 5d28 6874 7470 733a 2f2f 6d65   API](https://me
-00001390: 726d 6169 642e 6a73 2e6f 7267 2f69 6e74  rmaid.js.org/int
-000013a0: 726f 2f23 6d65 726d 6169 642d 6170 6929  ro/#mermaid-api)
-000013b0: 0a2d 205b 4d61 7468 4a61 785d 2868 7474  .- [MathJax](htt
-000013c0: 7073 3a2f 2f64 6f63 732e 6d61 7468 6a61  ps://docs.mathja
-000013d0: 782e 6f72 672f 656e 2f6c 6174 6573 742f  x.org/en/latest/
-000013e0: 7765 622f 7374 6172 742e 6874 6d6c 290a  web/start.html).
+000004e0: e68e a5e5 8fa3 e587 bde6 95b0 0a0a 6060  ..............``
+000004f0: 6070 7974 686f 6e0a 2320 e8a7 a3e6 9e90  `python.# ......
+00000500: 6d61 726b 646f 776e 2074 6578 740a 6465  markdown text.de
+00000510: 6620 7061 7273 6528 7465 7874 3a20 7374  f parse(text: st
+00000520: 7229 202d 3e20 7374 723a 0a0a 2320 e8a7  r) -> str:..# ..
+00000530: a3e6 9e90 6d61 726b 646f 776e 20e6 9687  ....markdown ...
+00000540: e4bb b60a 6465 6620 7061 7273 6546 696c  ....def parseFil
+00000550: 6528 6669 6c65 5f6e 616d 653a 2073 7472  e(file_name: str
+00000560: 2920 2d3e 2073 7472 3a0a 0a23 20e8 a781  ) -> str:..# ...
+00000570: e4b8 8be6 96b9 e8a1 a5e5 8585 e8af b4e6  ................
+00000580: 988e 0a64 6566 2070 6172 7365 5f77 6974  ...def parse_wit
+00000590: 6874 6167 2874 6578 743a 2073 7472 2920  htag(text: str) 
+000005a0: 2d3e 2073 7472 3a0a 0a64 6566 2070 6172  -> str:..def par
+000005b0: 7365 4669 6c65 5f77 6974 6874 6167 2866  seFile_withtag(f
+000005c0: 696c 655f 6e61 6d65 3a20 7374 7229 202d  ile_name: str) -
+000005d0: 3e20 7374 723a 0a60 6060 0a0a e7ac ace4  > str:.```......
+000005e0: ba8c e4b8 aae5 8f82 e695 b0e4 b8ba e58f  ................
+000005f0: afe9 8089 e9a1 b92c 2060 6861 735f 7461  ......., `has_ta
+00000600: 6760 20e8 a1a8 e7a4 bae6 98af e590 a6e5  g` .............
+00000610: b086 0a0a 2323 20e6 b58b e8af 950a 0a60  ....## ........`
+00000620: 6060 6261 7368 0a70 7974 686f 6e20 6765  ``bash.python ge
+00000630: 6e65 7261 7465 2e70 7920 3c46 494c 455f  nerate.py <FILE_
+00000640: 4e41 4d45 3e0a 0a23 2070 7974 686f 6e20  NAME>..# python 
+00000650: 6765 6e65 7261 7465 2e70 7920 2e2f 7465  generate.py ./te
+00000660: 7374 6669 6c65 732f 7465 7374 312e 6d64  stfiles/test1.md
+00000670: 0a23 2070 7974 686f 6e20 6765 6e65 7261  .# python genera
+00000680: 7465 2e70 7920 5245 4144 4d45 2e6d 640a  te.py README.md.
+00000690: 6060 600a 0ae8 bf90 e8a1 8ce4 bc9a e794  ```.............
+000006a0: 9fe6 8890 696e 6465 782e 6874 6d6c 2c20  ....index.html, 
+000006b0: e4bd bfe7 94a8 e6b5 8fe8 a788 e599 a8e6  ................
+000006c0: 8993 e5bc 80e7 949f e688 90e7 9a84 696e  ..............in
+000006d0: 6465 782e 6874 6d6c e58d b3e5 8faf e4b8  dex.html........
+000006e0: 8ee6 82a8 e79a 844d 6172 6b64 6f77 6ee7  .......Markdown.
+000006f0: bc96 e8be 91e5 99a8 e79a 84e9 a284 e69c  ................
+00000700: 9fe6 b8b2 e69f 93e7 bb93 e69e 9ce5 afb9  ................
+00000710: e6af 940a 0a21 5b32 3032 3330 3231 3832  .....![202302182
+00000720: 3032 3430 305d 2868 7474 7073 3a2f 2f72  02400](https://r
+00000730: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000740: 7465 6e74 2e63 6f6d 2f6c 6561 726e 6572  tent.com/learner
+00000750: 2d6c 752f 7069 6362 6564 2f6d 6173 7465  -lu/picbed/maste
+00000760: 722f 3230 3233 3032 3138 3230 3234 3030  r/20230218202400
+00000770: 2e70 6e67 290a 0ae4 bba3 e7a0 81e8 a686  .png)...........
+00000780: e79b 96e7 8e87 0a0a 6060 6062 6173 680a  ........```bash.
+00000790: 7069 7020 696e 7374 616c 6c20 636f 7665  pip install cove
+000007a0: 7261 6765 0a0a 636f 7665 7261 6765 2072  rage..coverage r
+000007b0: 756e 202d 6d20 756e 6974 7465 7374 0a63  un -m unittest.c
+000007c0: 6f76 6572 6167 6520 6874 6d6c 0a60 6060  overage html.```
+000007d0: 0a0a 2323 20e5 ae9e e78e b0e6 809d e8b7  ..## ...........
+000007e0: af0a 0a5b 4d61 726b 646f 776e e8a7 a3e6  ...[Markdown....
+000007f0: 9e90 e599 a8e7 9a84 e4bb a3e7 a081 e5ae  ................
+00000800: 9ee7 8eb0 5d28 6874 7470 733a 2f2f 7777  ....](https://ww
+00000810: 772e 6269 6c69 6269 6c69 2e63 6f6d 2f76  w.bilibili.com/v
+00000820: 6964 656f 2f42 5631 4c41 3431 3158 3758  ideo/BV1LA411X7X
+00000830: 3329 0a0a e682 a8e5 8faf e980 9ae8 bf87  3)..............
+00000840: e58f 96e6 b688 205b 636f 7265 2e70 795d  ...... [core.py]
+00000850: 282e 2f4d 6172 6b64 6f77 6e50 6172 7365  (./MarkdownParse
+00000860: 722f 636f 7265 2e70 7929 20e6 b3a8 e987  r/core.py) .....
+00000870: 8ae6 9da5 e88e b7e5 8f96 e6a0 91e7 9a84  ................
+00000880: e7bb 93e6 9e84 0a0a 6060 6070 7974 686f  ........```pytho
+00000890: 6e0a 6465 6620 7061 7273 6528 7365 6c66  n.def parse(self
+000008a0: 2c20 7465 7874 3a20 7374 7229 202d 3e20  , text: str) -> 
+000008b0: 7374 723a 0a0a 2020 2020 2320 e58e bbe9  str:..    # ....
+000008c0: 99a4 e7a9 bae8 a18c 2fe6 b3a8 e987 8a2f  ......../....../
+000008d0: 6874 6d6c e6a0 87e7 adbe 0a20 2020 206c  html.......    l
+000008e0: 696e 6573 203d 2073 656c 662e 7072 6570  ines = self.prep
+000008f0: 726f 6365 7373 5f70 6172 7365 7228 7465  rocess_parser(te
+00000900: 7874 290a 2020 2020 2320 7072 696e 7428  xt).    # print(
+00000910: 6c69 6e65 7329 0a20 2020 2023 20e9 8090  lines).    # ...
+00000920: e8a1 8ce8 a7a3 e69e 902c e5be 97e5 88b0  .........,......
+00000930: e4b8 80e9 a297 e69c aae4 bc98 e58c 96e7  ................
+00000940: 9a84 e6a0 910a 2020 2020 726f 6f74 203d  ......    root =
+00000950: 2073 656c 662e 626c 6f63 6b5f 7061 7273   self.block_pars
+00000960: 6572 286c 696e 6573 290a 2020 2020 2320  er(lines).    # 
+00000970: 726f 6f74 2e69 6e66 6f28 290a 2020 2020  root.info().    
+00000980: 2320 e4bc 98e5 8c96 2ce5 be97 e588 b0e6  # ......,.......
+00000990: ada3 e7a1 aee7 9a84 6d61 726b 646f 776e  ........markdown
+000009a0: e8a7 a3e6 9e90 e6a0 910a 2020 2020 7472  ..........    tr
+000009b0: 6565 203d 2073 656c 662e 7472 6565 5f70  ee = self.tree_p
+000009c0: 6172 7365 7228 726f 6f74 290a 2020 2020  arser(root).    
+000009d0: 2320 7472 6565 2e69 6e66 6f28 290a 2020  # tree.info().  
+000009e0: 2020 2320 e8be 93e5 87ba e588 b0e5 b18f    # ............
+000009f0: e5b9 9520 2f20 e5af bce5 87ba 6874 6d6c  ... / ......html
+00000a00: e696 87e4 bbb6 0a20 2020 2072 6574 7572  .......    retur
+00000a10: 6e20 7472 6565 2e74 6f48 544d 4c28 290a  n tree.toHTML().
+00000a20: 6060 600a 0a23 2320 e4b8 8de6 94af e68c  ```..## ........
+00000a30: 810a 0a2d 20e5 9b9b e4b8 aae7 a9ba e6a0  ...- ...........
+00000a40: bce5 8f98 e4b8 bae4 bba3 e7a0 81e6 aeb5  ................
+00000a50: 0a2d 205b 5e31 5de7 9a84 e5bc 95e7 94a8  .- [^1].........
+00000a60: e696 b9e5 bc8f 0a2d 2053 6574 6578 7420  .......- Setext 
+00000a70: e5bd a2e5 bc8f e79a 84e6 a087 e9a2 980a  ................
+00000a80: 2d20 e4b8 8ae6 a087 202f 20e4 b88b e6a0  - ...... / .....
+00000a90: 8720 2f20 e4b8 8be5 8892 e7ba bf0a 0a23  . / ...........#
+00000aa0: 2320 e8a1 a5e5 8585 e8af b4e6 988e 0a0a  # ..............
+00000ab0: 2d20 e794 9fe6 8890 e79a 84e7 bb93 e69e  - ..............
+00000ac0: 9ce5 a682 e4b8 8b20 603c 6469 7620 636c  ....... `<div cl
+00000ad0: 6173 733d 276d 6172 6b64 6f77 6e2d 626f  ass='markdown-bo
+00000ae0: 6479 273e 6d61 726b 646f 776e e586 85e5  dy'>markdown....
+00000af0: aeb9 3c2f 6469 763e 600a 2d20 e4bb a3e7  ..</div>`.- ....
+00000b00: a081 e6ae b5e4 bc9a e6a0 b9e6 8dae e8af  ................
+00000b10: ade8 a880 e58a a0e5 85a5 e4b8 80e4 b8aa  ................
+00000b20: e7b1 bbe5 908d e4be bfe4 ba8e e590 8ee6  ................
+00000b30: 9c9f e9ab 98e4 baae 2ce4 be8b e5a6 8220  ........,...... 
+00000b40: 6063 6c61 7373 3d22 6c61 6e67 7561 6765  `class="language
+00000b50: 2d63 7070 2260 2c20 e69c aae5 ae9a e4b9  -cpp"`, ........
+00000b60: 89e8 afad e8a8 80e5 8899 e4b8 ba20 606c  ............. `l
+00000b70: 616e 6775 6167 652d 554e 4b4e 4f57 4e60  anguage-UNKNOWN`
+00000b80: 0a2d 20e9 bb98 e8ae a4e5 afbc e587 bae7  .- .............
+00000b90: 9a84 4854 4d4c e4b8 ade5 b182 e7ba a7e4  ..HTML..........
+00000ba0: bbbb e58a a1e5 8897 e8a1 a8e4 bc9a e69c  ................
+00000bb0: 89e6 98be e7a4 bae9 97ae e9a2 982c e8bf  .............,..
+00000bc0: 99e6 98af e59b a0e4 b8ba e4bd bfe7 94a8  ................
+00000bd0: e4ba 8675 6c2b 6c69 2b63 6865 636b 626f  ...ul+li+checkbo
+00000be0: 78e7 9a84 e696 b9e5 bc8f 2ce6 82a8 e99c  x.........,.....
+00000bf0: 80e8 a681 e6b7 bbe5 8aa0 e4bb a5e4 b88b  ................
+00000c00: 6373 73e6 a0b7 e5bc 8fe4 bfae e6ad a30a  css.............
+00000c10: 0a20 2060 6060 6373 730a 2020 2e6d 6172  .  ```css.  .mar
+00000c20: 6b64 6f77 6e2d 626f 6479 203e 2075 6c3e  kdown-body > ul>
+00000c30: 6c69 3a68 6173 2869 6e70 7574 2920 7b0a  li:has(input) {.
+00000c40: 2020 2020 7061 6464 696e 672d 6c65 6674      padding-left
+00000c50: 3a20 303b 0a20 2020 206d 6172 6769 6e2d  : 0;.    margin-
+00000c60: 626f 7474 6f6d 3a20 303b 0a20 207d 0a0a  bottom: 0;.  }..
+00000c70: 2020 2e6d 6172 6b64 6f77 6e2d 626f 6479    .markdown-body
+00000c80: 2020 756c 3e6c 693a 6861 7328 696e 7075    ul>li:has(inpu
+00000c90: 7429 3e75 6c20 7b0a 2020 2020 6c69 7374  t)>ul {.    list
+00000ca0: 2d73 7479 6c65 2d74 7970 653a 206e 6f6e  -style-type: non
+00000cb0: 653b 0a20 2020 2070 6164 6469 6e67 2d6c  e;.    padding-l
+00000cc0: 6566 743a 2038 7078 3b0a 2020 7d0a 2020  eft: 8px;.  }.  
+00000cd0: 6060 600a 0a2d 20e6 82a8 e58f afe4 bba5  ```..- .........
+00000ce0: e4bd bfe7 94a8 2060 7061 7273 655f 7769  ...... `parse_wi
+00000cf0: 7468 7461 6760 20e5 b086 2048 6173 6848  thtag` ... HashH
+00000d00: 6561 6442 6c6f 636b 20e6 8f90 e58f 96e5  eadBlock .......
+00000d10: 87ba e69d a5e7 bb84 e688 90e7 9bae e5bd  ................
+00000d20: 95e6 a091 2c20 e5be 97e5 88b0 e4b8 80e4  ...., ..........
+00000d30: b8aa 2060 3c64 6976 2063 6c61 7373 3d22  .. `<div class="
+00000d40: 6865 6164 6572 2d6e 6176 6967 6174 6f72  header-navigator
+00000d50: 223e 2e2e 2e3c 2f64 6976 3e60 20e5 b9b6  ">...</div>` ...
+00000d60: e6b7 bbe5 8aa0 e588 b0e8 bf94 e59b 9ee7  ................
+00000d70: 9a84 2048 544d 4c20 e585 83e7 b4a0 e4b8  .. HTML ........
+00000d80: ad2c 20e6 82a8 e58f afe8 83bd e8bf 98e9  ., .............
+00000d90: 9c80 e8a6 81e4 b880 e4ba 9b20 6a73 20e7  ........... js .
+00000da0: 9bb8 e585 b3e7 9a84 e4bb a3e7 a081 e5ae  ................
+00000db0: 9ee7 8eb0 e8b7 b3e8 bdac 2c20 e585 b7e4  .........., ....
+00000dc0: bd93 e58f afe4 bba5 e58f 82e8 8083 205b  .............. [
+00000dd0: 7465 6d70 6c61 7465 2e68 746d 6c5d 282e  template.html](.
+00000de0: 2f74 656d 706c 6174 652e 6874 6d6c 290a  /template.html).
+00000df0: 0a20 2060 6060 6a73 0a20 206c 6574 206c  .  ```js.  let l
+00000e00: 696e 6b73 203d 2064 6f63 756d 656e 742e  inks = document.
+00000e10: 7175 6572 7953 656c 6563 746f 7241 6c6c  querySelectorAll
+00000e20: 2827 6469 7620 615b 6872 6566 5e3d 2223  ('div a[href^="#
+00000e30: 225d 2729 3b0a 2020 2020 6c69 6e6b 732e  "]');.    links.
+00000e40: 666f 7245 6163 6828 6c69 6e6b 203d 3e20  forEach(link => 
+00000e50: 7b0a 2020 2020 2020 6c69 6e6b 2e61 6464  {.      link.add
+00000e60: 4576 656e 744c 6973 7465 6e65 7228 2763  EventListener('c
+00000e70: 6c69 636b 272c 2066 756e 6374 696f 6e28  lick', function(
+00000e80: 6576 656e 7429 207b 0a20 2020 2020 2020  event) {.       
+00000e90: 2065 7665 6e74 2e70 7265 7665 6e74 4465   event.preventDe
+00000ea0: 6661 756c 7428 293b 0a20 2020 2020 2020  fault();.       
+00000eb0: 206c 6574 2074 6172 6765 7420 3d20 646f   let target = do
+00000ec0: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
+00000ed0: 6374 6f72 2874 6869 732e 6765 7441 7474  ctor(this.getAtt
+00000ee0: 7269 6275 7465 2827 6872 6566 2729 293b  ribute('href'));
+00000ef0: 0a20 2020 2020 2020 2074 6172 6765 742e  .        target.
+00000f00: 7363 726f 6c6c 496e 746f 5669 6577 287b  scrollIntoView({
+00000f10: 2062 6568 6176 696f 723a 2027 736d 6f6f   behavior: 'smoo
+00000f20: 7468 2720 7d29 3b0a 2020 2020 2020 7d29  th' });.      })
+00000f30: 3b0a 2020 2020 7d29 3b0a 2020 6060 600a  ;.    });.  ```.
+00000f40: 0a20 20e4 bba5 e58f 8ae4 b880 e4ba 9be6  .  .............
+00000f50: a0b7 e5bc 8fe7 be8e e58c 960a 0a20 2060  .............  `
+00000f60: 6060 6373 730a 2020 2e68 6561 6465 722d  ``css.  .header-
+00000f70: 6e61 7669 6761 746f 7220 7b0a 2020 2020  navigator {.    
+00000f80: 706f 7369 7469 6f6e 3a20 6669 7865 643b  position: fixed;
+00000f90: 0a20 207d 0a20 2060 6060 0a0a 2d20 e5a6  .  }.  ```..- ..
+00000fa0: 82e6 9e9c e682 a8e6 83b3 e6b7 bbe5 8aa0  ................
+00000fb0: e5af b95b 4d65 726d 6169 645d 2868 7474  ...[Mermaid](htt
+00000fc0: 7073 3a2f 2f6d 6572 6d61 6964 2e6a 732e  ps://mermaid.js.
+00000fd0: 6f72 672f 29e7 9a84 e694 afe6 8c81 2c20  org/)........., 
+00000fe0: e682 a8e5 8faf e58f 82e8 8083 5b6d 6572  ............[mer
+00000ff0: 6d61 6964 2070 6c75 6769 6e5d 2868 7474  maid plugin](htt
+00001000: 7073 3a2f 2f6d 6572 6d61 6964 2e6a 732e  ps://mermaid.js.
+00001010: 6f72 672f 696e 7472 6f2f 6e30 3062 2d67  org/intro/n00b-g
+00001020: 6574 7469 6e67 5374 6172 7465 642e 6874  ettingStarted.ht
+00001030: 6d6c 235f 322d 7573 696e 672d 6d65 726d  ml#_2-using-merm
+00001040: 6169 642d 706c 7567 696e 7329 e59c a8e6  aid-plugins)....
+00001050: 82a8 e79a 8468 746d 6ce9 a1b5 e99d a220  .....html...... 
+00001060: 603c 626f 6479 3e60 20e6 9cab e5b0 bee6  `<body>` .......
+00001070: b7bb e58a a0e5 a682 e4b8 8b20 603c 7363  ........... `<sc
+00001080: 7269 7074 3e60 0a0a 2020 6060 6068 746d  ript>`..  ```htm
+00001090: 6c0a 2020 3c73 6372 6970 7420 7479 7065  l.  <script type
+000010a0: 3d22 6d6f 6475 6c65 223e 0a20 2020 2063  ="module">.    c
+000010b0: 6f6e 7374 2063 6f64 6542 6c6f 636b 7320  onst codeBlocks 
+000010c0: 3d20 646f 6375 6d65 6e74 2e71 7565 7279  = document.query
+000010d0: 5365 6c65 6374 6f72 416c 6c28 272e 6c61  SelectorAll('.la
+000010e0: 6e67 7561 6765 2d6d 6572 6d61 6964 2729  nguage-mermaid')
+000010f0: 3b0a 2020 2020 636f 6465 426c 6f63 6b73  ;.    codeBlocks
+00001100: 2e66 6f72 4561 6368 2863 6f64 6542 6c6f  .forEach(codeBlo
+00001110: 636b 203d 3e20 7b0a 2020 2020 2020 2020  ck => {.        
+00001120: 636f 6465 426c 6f63 6b2e 636c 6173 734c  codeBlock.classL
+00001130: 6973 742e 7265 6d6f 7665 2827 6c61 6e67  ist.remove('lang
+00001140: 7561 6765 2d6d 6572 6d61 6964 2729 3b0a  uage-mermaid');.
+00001150: 2020 2020 2020 2020 636f 6465 426c 6f63          codeBloc
+00001160: 6b2e 636c 6173 734c 6973 742e 6164 6428  k.classList.add(
+00001170: 276d 6572 6d61 6964 2729 3b0a 2020 2020  'mermaid');.    
+00001180: 7d29 3b0a 2020 2020 696d 706f 7274 206d  });.    import m
+00001190: 6572 6d61 6964 2066 726f 6d20 2768 7474  ermaid from 'htt
+000011a0: 7073 3a2f 2f63 646e 2e6a 7364 656c 6976  ps://cdn.jsdeliv
+000011b0: 722e 6e65 742f 6e70 6d2f 6d65 726d 6169  r.net/npm/mermai
+000011c0: 6440 3130 2f64 6973 742f 6d65 726d 6169  d@10/dist/mermai
+000011d0: 642e 6573 6d2e 6d69 6e2e 6d6a 7327 3b0a  d.esm.min.mjs';.
+000011e0: 2020 2020 6d65 726d 6169 642e 696e 6974      mermaid.init
+000011f0: 6961 6c69 7a65 287b 2073 7461 7274 4f6e  ialize({ startOn
+00001200: 4c6f 6164 3a20 7472 7565 207d 293b 0a20  Load: true });. 
+00001210: 203c 2f73 6372 6970 743e 0a20 2060 6060   </script>.  ```
+00001220: 0a0a 2020 3e20 2a2a e8af b7e6 b3a8 e684  ..  > **........
+00001230: 8f2a 2a2c 20e7 94b1 e4ba 8ee6 9cac 4d61  .**, .........Ma
+00001240: 726b 646f 776e e8a7 a3e6 9e90 e599 a8e7  rkdown..........
+00001250: 9a84 436f 6465 426c 6f63 6be8 a7a3 e69e  ..CodeBlock.....
+00001260: 90e5 be97 e588 b0e7 9a84 e7b1 bbe5 908d  ................
+00001270: e4b8 ba20 606c 616e 6775 6167 652d 6d65  ... `language-me
+00001280: 726d 6169 6460 2c20 e880 8c6d 6572 6d61  rmaid`, ...merma
+00001290: 6964 e68f 92e4 bbb6 e694 afe6 8c81 e79a  id..............
+000012a0: 84e7 b1bb e590 8de6 a0bc e5bc 8fe4 b8ba  ................
+000012b0: 606d 6572 6d61 6964 602c 20e6 8980 e4bb  `mermaid`, .....
+000012c0: a5e4 bba3 e7a0 81e4 b8ad e689 8be5 8aa8  ................
+000012d0: e4bf aee6 94b9 e4ba 8620 606c 616e 6775  ......... `langu
+000012e0: 6167 652d 6d65 726d 6169 6460 20e7 9a84  age-mermaid` ...
+000012f0: e7b1 bbe5 908d 0a0a 2d20 e5a6 82e6 9e9c  ........- ......
+00001300: e682 a8e6 83b3 e6b7 bbe5 8aa0 e5af b94c  ...............L
+00001310: 6174 6578 e695 b0e5 ada6 e585 ace5 bc8f  atex............
+00001320: e79a 84e6 94af e68c 812c 20e5 8faf e4bb  ........., .....
+00001330: a5e5 9ca8 6874 6d6c e9a1 b5e9 9da2 2060  ....html...... `
+00001340: 3c62 6f64 793e 6020 e69c abe5 b0be e6b7  <body>` ........
+00001350: bbe5 8aa0 e5a6 82e4 b88b 2060 3c73 6372  .......... `<scr
+00001360: 6970 743e 600a 0a20 2060 6060 6874 6d6c  ipt>`..  ```html
+00001370: 0a20 203c 7363 7269 7074 3e0a 2020 2020  .  <script>.    
+00001380: 2020 4d61 7468 4a61 7820 3d20 7b0a 2020    MathJax = {.  
+00001390: 2020 2020 2020 7465 783a 207b 0a20 2020        tex: {.   
+000013a0: 2020 2020 2020 2069 6e6c 696e 654d 6174         inlineMat
+000013b0: 683a 205b 5b27 2427 2c20 2724 275d 2c20  h: [['$', '$'], 
+000013c0: 5b27 5c5c 2827 2c20 275c 5c29 275d 5d0a  ['\\(', '\\)']].
+000013d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000013e0: 7d3b 0a20 2020 2020 203c 2f73 6372 6970  };.      </scrip
+000013f0: 743e 0a20 203c 7363 7269 7074 2069 643d  t>.  <script id=
+00001400: 224d 6174 684a 6178 2d73 6372 6970 7422  "MathJax-script"
+00001410: 2061 7379 6e63 0a20 2073 7263 3d22 6874   async.  src="ht
+00001420: 7470 733a 2f2f 6364 6e2e 6a73 6465 6c69  tps://cdn.jsdeli
+00001430: 7672 2e6e 6574 2f6e 706d 2f6d 6174 686a  vr.net/npm/mathj
+00001440: 6178 4033 2f65 7335 2f74 6578 2d63 6874  ax@3/es5/tex-cht
+00001450: 6d6c 2e6a 7322 3e0a 2020 3c2f 7363 7269  ml.js">.  </scri
+00001460: 7074 3e0a 2020 6060 600a 0a20 20e6 b3a8  pt>.  ```..  ...
+00001470: e684 8f2c e8bf 99e9 878c e4bb 85e6 94af  ...,............
+00001480: e68c 81e5 be88 e5b0 91e4 b880 e983 a8e5  ................
+00001490: 8886 e695 b0e5 ada6 e585 ace5 bc8f 0a0a  ................
+000014a0: 0a23 2320 e79b b8e5 85b3 e58f 82e8 8083  .## ............
+000014b0: 0a0a 2d20 5b47 6974 6875 6220 4d61 726b  ..- [Github Mark
+000014c0: 646f 776e 2043 5353 5d28 6874 7470 733a  down CSS](https:
+000014d0: 2f2f 6364 6e2e 6a73 6465 6c69 7672 2e6e  //cdn.jsdelivr.n
+000014e0: 6574 2f6e 706d 2f67 6974 6875 622d 6d61  et/npm/github-ma
+000014f0: 726b 646f 776e 2d63 7373 4034 2e30 2e30  rkdown-css@4.0.0
+00001500: 2f67 6974 6875 622d 6d61 726b 646f 776e  /github-markdown
+00001510: 2e63 7373 290a 2d20 5b4d 6572 6d61 6964  .css).- [Mermaid
+00001520: 2041 5049 5d28 6874 7470 733a 2f2f 6d65   API](https://me
+00001530: 726d 6169 642e 6a73 2e6f 7267 2f69 6e74  rmaid.js.org/int
+00001540: 726f 2f23 6d65 726d 6169 642d 6170 6929  ro/#mermaid-api)
+00001550: 0a2d 205b 4d61 7468 4a61 785d 2868 7474  .- [MathJax](htt
+00001560: 7073 3a2f 2f64 6f63 732e 6d61 7468 6a61  ps://docs.mathja
+00001570: 782e 6f72 672f 656e 2f6c 6174 6573 742f  x.org/en/latest/
+00001580: 7765 622f 7374 6172 742e 6874 6d6c 290a  web/start.html).
```

