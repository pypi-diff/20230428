# Comparing `tmp/markdownparser-0.3.8.tar.gz` & `tmp/markdownparser-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.3.8.tar", max compression
+gzip compressed data, was "markdownparser-0.3.9.tar", max compression
```

## Comparing `markdownparser-0.3.8.tar` & `markdownparser-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.3.8/LICENSE
--rw-r--r--   0        0        0       64 2023-01-30 08:56:40.322545 markdownparser-0.3.8/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5582 2023-02-24 16:35:08.540552 markdownparser-0.3.8/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    22372 2023-03-10 15:22:35.273053 markdownparser-0.3.8/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     1229 2023-03-10 15:23:11.063781 markdownparser-0.3.8/MarkdownParser/core.py
--rw-r--r--   0        0        0     3424 2023-02-24 17:09:55.604004 markdownparser-0.3.8/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    20712 2023-03-05 06:26:13.122009 markdownparser-0.3.8/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-03-10 15:24:47.439245 markdownparser-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4131 2023-03-05 08:18:30.678129 markdownparser-0.3.8/README.md
--rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 markdownparser-0.3.8/setup.py
--rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 markdownparser-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.3.9/LICENSE
+-rw-r--r--   0        0        0       64 2023-01-30 08:56:40.322545 markdownparser-0.3.9/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5599 2023-04-27 07:15:55.104457 markdownparser-0.3.9/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    22430 2023-04-27 07:27:40.965222 markdownparser-0.3.9/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     1229 2023-04-27 10:25:53.137955 markdownparser-0.3.9/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3329 2023-04-27 07:28:20.519261 markdownparser-0.3.9/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    20772 2023-04-27 10:27:47.162481 markdownparser-0.3.9/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-04-27 11:08:32.799699 markdownparser-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4331 2023-04-27 10:51:20.047839 markdownparser-0.3.9/README.md
+-rw-r--r--   0        0        0     5064 1970-01-01 00:00:00.000000 markdownparser-0.3.9/setup.py
+-rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 markdownparser-0.3.9/PKG-INFO
```

### Comparing `markdownparser-0.3.8/LICENSE` & `markdownparser-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.3.8/MarkdownParser/base_class.py` & `markdownparser-0.3.9/MarkdownParser/base_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             # block类名-唯一标识符 : block类对象
             #
         }
 
         self._counter = 0
         self.__str__ = self.__repr__
 
-    def __repr__(self) -> str:
+    def __repr__(self) -> str: # pragma: no cover
 
         split_line = '-' * 50 + '\n'
         info = f'Total number: {self._counter}\n\n'
 
         for k, v in self._container.items():
             info += f'[{k}]'.ljust(30)
             if v.input.get('word') is not None:
@@ -46,24 +46,19 @@
         self.is_sorted = False
 
     def _sort(self):
 
         # 按照优先级从高到低排序,使得解析时依次调用方法
         self._handlers.sort(key=lambda item: item['priority'], reverse=True)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs): # pragma: no cover
 
         raise NotImplementedError
 
-    def __getitem__(self, key):
-        for method in self._handlers:
-            if method['name'] == key:
-                return method['object']
-
-    def info(self):
+    def info(self): # pragma: no cover
         # 查看所有已注册的方法
         if not self.is_sorted:
             self._sort()
         for method in self._handlers:
             name = method['name']
             class_name = method['object'].__class__.__name__
             priority = method['priority']
@@ -115,42 +110,42 @@
                 self.addBlock(class_object)
             count += 1
 
     def addBlock(self, block):
 
         self.sub_blocks.append(block)
 
-    def __str__(self):
+    def __str__(self): # pragma: no cover
 
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
 
-    def info(self, deep: int = 0):
+    def info(self, deep: int = 0): # pragma: no cover
         # root.info()
         # 递归输出信息
 
         if self.sub_blocks == []:
             return
         else:
             for block in self.sub_blocks:
                 print(' '*4*deep, end='')
                 print(f'[{block.__class__.__name__}] {str(block)}')
                 block.info(deep+1)
 
-    def printInfo(self, deep: int = 0) -> str:
+    def printInfo(self, deep: int = 0) -> str: # pragma: no cover
         # print(root.printInfo())
         # 递归输出信息
         output_str = ''
         if self.sub_blocks == []:
             return output_str
         else:
             for block in self.sub_blocks:
@@ -170,30 +165,30 @@
 class Handler:
 
     def __init__(self, parser=None) -> None:
 
         self.RE = None
         self.parser: Parser = parser
 
-    def match(self, text: str, *args):
+    def match(self, text: str, *args): # pragma: no cover
 
         if self.RE is None:
             raise NotImplementedError
 
         return bool(self.RE.search(text))
 
-    def __call__(self, root: Block, text: str):
+    def __call__(self, root: Block, text: str): # pragma: no cover
 
         raise NotImplementedError
 
 
 class Optimizer:
 
     def __init__(self) -> None:
 
         # 优化器针对的Block
         self.target_block_names = []
         self.is_match = False
 
-    def __call__(self, root: Block):
+    def __call__(self, root: Block): # pragma: no cover
 
         raise NotImplementedError
```

### Comparing `markdownparser-0.3.8/MarkdownParser/block_parser.py` & `markdownparser-0.3.9/MarkdownParser/block_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,53 +24,50 @@
     def match(self, root: Block, text: str):
 
         for method in self._handlers:
             if method['object'].match(text):
                 # print(method['object'].__class__.__name__,'matched')
                 method['object'](root, text)
                 return
-            else:
-                # print(method['name'] + ' missed')
-                pass
 
 
 class ComplexBlock(Block):
     # 用于处理复杂嵌套
 
     def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
+        super().__init__(**kwargs) # pragma: no cover
 
     def toHTML(self):
 
         content = ''
         for block in self.sub_blocks:
             content += block.toHTML()
 
         return content
 
 
 class HTMLBlock(Block):
     # 处理HTML标签
     def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
+        super().__init__(**kwargs) # pragma: no cover
 
     def __str__(self):
-        return '<html>'
+        return '<html>' # pragma: no cover
 
     def toHTML(self):
         return self.input['text']
 
 
 class AnnotateBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def __str__(self):
-        return '<!-->'
+        return '<!-->' # pragma: no cover
 
     def toHTML(self):
         return ''
 
 
 class EmptyBlockHandler(Handler):
     # 处理空行
@@ -130,15 +127,15 @@
 
     def toHTML(self):
         return self.input['word']
 
 # 已废弃
 
 
-class ExtensionBlockHandler(Handler):
+class ExtensionBlockHandler(Handler): # pragma: no cover
     # 自定义扩展
     # {% note %}
     # asdklja
     # {%end%}
 
     def __init__(self, parser=None) -> None:
         super().__init__(parser)
@@ -164,15 +161,15 @@
                 tag = v
                 break
 
         self.block = ExtensionBlock(text=text, tag=tag)
         root.addBlock(self.block)
 
 
-class ExtensionBlock(Block):
+class ExtensionBlock(Block): # pragma: no cover
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
 
         tag = self.input['tag']
@@ -193,15 +190,15 @@
 
 
 class SplitBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
-    def __str__(self):
+    def __str__(self): # pragma: no cover
         return '---<hr>---'
 
     def toHTML(self):
         return '<hr>'
 
 
 class HierarchyIndentHandler(Handler):
@@ -702,15 +699,15 @@
                         string, class_object.input['text'])
                     root.input['text'] = root.input['text'].replace(
                         string, class_object.input['text'])
                     temp_block.addBlock(class_object)
                 else:
                     # 由于在解析过程中中间变量使用了{-%.*?%-}的格式进行代替
                     # 所以如果原本的Markdown输入中就包含类似的 {-%asdjkl%-}文字则会出现无法找到的情况
-                    temp_block.addBlock(TextBlock(word=string, text=string))
+                    temp_block.addBlock(TextBlock(word=string, text=string)) # pragma: no cover
             count += 1
 
         if len(temp_block.sub_blocks) <= 1:
             root.addBlock(temp_block.sub_blocks[0])
         else:
             root.addBlock(temp_block)
```

### Comparing `markdownparser-0.3.8/MarkdownParser/core.py` & `markdownparser-0.3.9/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.3.8/MarkdownParser/preprocess_parser.py` & `markdownparser-0.3.9/MarkdownParser/preprocess_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
         # 按优先级逐步执行相应处理方法
         for method in self._handlers:
             data = method['object'](data)
 
         lines = data.split('\n')
         return lines
 
-    def getHtmlPosition(self):
-        return self.preprocess_parser['html'].match_results
-
 
 class TabHandler(Handler):
 
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, text: str):
```

### Comparing `markdownparser-0.3.8/MarkdownParser/tree_parser.py` & `markdownparser-0.3.9/MarkdownParser/tree_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,18 +229,16 @@
                 # 递进级层次缩进被打断
                 else:
                     new_sub_blocks.extend(block.sub_blocks)
             else:
                 # EmptyBlock 先补齐在 UList OListBlock 下
                 if block.block_name == 'EmptyBlock':
                     if deeper_indent:
-                        if len(activite_block.sub_blocks) == 0:
-                            activite_block.addBlock(block)
                         # 忽略连续的EmptyBlock
-                        elif activite_block.sub_blocks[-1].block_name != 'EmptyBlock':
+                        if activite_block.sub_blocks[-1].block_name != 'EmptyBlock':
                             activite_block.addBlock(block)
                     else:
                         if len(new_sub_blocks) > 1 and new_sub_blocks[-1].block_name == 'EmptyBlock':
                             continue
                         else:
                             new_sub_blocks.append(block)
                 else:
@@ -281,15 +279,15 @@
             else:
                 first_number = None
                 new_sub_blocks.append(block)
 
 # abort
 
 
-class ExtensionOptimizer(Optimizer):
+class ExtensionOptimizer(Optimizer): # pragma: no cover
 
     def __init__(self) -> None:
         super().__init__()
         self.target_block_names = ['ExtensionBlock']
         self.extension_tag = ['note', 'info', 'success']
 
     def __call__(self, root: Block):
@@ -428,14 +426,16 @@
                         new_sub_blocks.pop()
                     else:
                         # 将TableBlock变为纯文本
                         new_sub_blocks.append(
                             TextBlock(text=block.input['text'], word=block.input['text']))
                         match_table = False
                 else:
+                    # 第一步匹配失败则将 block 回退为 TextBlock
+                    block = TextBlock(text=block.input['text'], word=block.input['text'])
                     new_sub_blocks.append(block)
             else:
                 new_sub_blocks.append(block)
 
         if table_block is not None:
             new_sub_blocks.append(table_block)
         root.sub_blocks = new_sub_blocks
```

### Comparing `markdownparser-0.3.8/README.md` & `markdownparser-0.3.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # MarkdownParser
 
+[![codecov](https://codecov.io/gh/luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/MarkdownParser)
+
 MarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换
 
 ## 安装
 
 ```bash
 pip install markdownparser
 ```
@@ -31,27 +33,32 @@
 
   其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构
 
   tree可以通过内部toHTML()方法得到HTML元素
 
 ## 测试
 
-您可以使用 `test.py` 测试Markdown解析是否正确
-
 ```bash
-python test.py <FILE_NAME>
+python generate.py <FILE_NAME>
 
-# python test.py ./testfiles/test1.md
-# python test.py README.md
+# python generate.py ./testfiles/test1.md
+# python generate.py README.md
 ```
 
 运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比
 
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)
 
+代码覆盖率
+
+```bash
+coverage run -m unittest
+coverage html
+```
+
 ## 实现思路
 
 [Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)
 
 您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构
 
 ```python
@@ -85,21 +92,22 @@
 ## 补充说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
 - 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
-  .markdown-body > ul:has(input) {
+  .markdown-body > ul>li:has(input) {
     padding-left: 0;
     margin-bottom: 0;
   }
 
-  .markdown-body  ul:has(input) {
-      list-style-type: none;
+  .markdown-body  ul>li:has(input)>ul {
+    list-style-type: none;
+    padding-left: 8px;
   }
   ```
 
 - 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`
 
   ```html
   <script type="module">
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-# MarkdownParser MarkdownParser æ¯ä¸ä¸ª Markdown
+# MarkdownParser [![codecov](https://codecov.io/gh/luzhixing12345/
+MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/
+luzhixing12345/MarkdownParser) MarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢ ## å®è£ ```bash pip
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
 ``` å¶ä»æ¥å£å½æ° - `parseFile(file_name:str)->str`: è§£ææä»¶
 æ¥å£ç±» - `Markdown` ä½¿ç¨ç±»åå»ºå¯¹è±¡åå¯ä»¥å©ç¨
 `self.preprocess_parser` `self.block_parser` `self.tree_parser`
 æ§å¶è§£æè¿ç¨ å¶ä¸­Blockç±»å±æ§è§[base_class.py](MarkdownParser/
 base_class.py),å¯ä»¥éè¿è°ç¨block.info()å½æ°æ¥çæ çç»æ
-treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´  ## æµè¯ æ¨å¯ä»¥ä½¿ç¨
-`test.py` æµè¯Markdownè§£ææ¯å¦æ­£ç¡® ```bash python test.py  # python
-test.py ./testfiles/test1.md # python test.py README.md ```
-è¿è¡ä¼çæindex.html,
+treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´  ## æµè¯ ```bash python
+generate.py  # python generate.py ./testfiles/test1.md # python generate.py
+README.md ``` è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png) ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://
+20230218202400.png) ä»£ç è¦çç ```bash coverage run -m unittest coverage
+html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://
 www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
 MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
 text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
 self.preprocess_parser(text) # print(lines) #
 éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser(lines) #
 root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree = self.tree_parser
 (root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶ return tree.toHTML()
@@ -27,19 +29,19 @@
 éç¹çæ·»å éå¸¸åç®å½çè·³è½¬æå³,èç®å½æ ççæå¯ä»¥èèè§£ætreeçæ ¹Blockçææå­HashHeaderBlockæ¥æå»º.
 å ä¸ºè·³è½¬çåè½æ¯jså®ç°,éç¹idçå å¥ä¹ä¼å½±åhtmlç»æ,æä»¥æä¸æ¯æ
 ## è¡¥åè¯´æ - çæçç»æå¦ä¸ `
 markdownåå®¹
 ` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
-```css .markdown-body > ul:has(input) { padding-left: 0; margin-bottom: 0; }
-.markdown-body ul:has(input) { list-style-type: none; } ``` -
-å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ, æ¨å¯åè
-[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-
-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
+```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
+.markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
+} ``` - å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ,
+æ¨å¯åè[mermaid plugin](https://mermaid.js.org/intro/n00b-
+gettingStarted.html#_2-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
  ``` > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å -
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
```

### Comparing `markdownparser-0.3.8/setup.py` & `markdownparser-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['markdownparser']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'markdownparser',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '',
-    'long_description': '# MarkdownParser\n\nMarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换\n\n## 安装\n\n```bash\npip install markdownparser\n```\n\n## 快速使用\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse(\'# Hello World!\')\nprint(html)\n\n#<div class=\'markdown-body\'><h1>Hello World!</h1></div>\n```\n\n其他接口函数\n\n- `parseFile(file_name:str)->str`: 解析文件\n\n接口类\n\n- `Markdown`\n\n  使用类创建对象后可以利用 `self.preprocess_parser` `self.block_parser` `self.tree_parser` 控制解析过程\n\n  其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构\n\n  tree可以通过内部toHTML()方法得到HTML元素\n\n## 测试\n\n您可以使用 `test.py` 测试Markdown解析是否正确\n\n```bash\npython test.py <FILE_NAME>\n\n# python test.py ./testfiles/test1.md\n# python test.py README.md\n```\n\n运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比\n\n![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)\n\n## 实现思路\n\n[Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)\n\n您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构\n\n```python\ndef parse(self, text: str) -> str:\n\n    # 去除空行/注释/html标签\n    lines = self.preprocess_parser(text)\n    # print(lines)\n    # 逐行解析,得到一颗未优化的树\n    root = self.block_parser(lines)\n    # root.info()\n    # 优化,得到正确的markdown解析树\n    tree = self.tree_parser(root)\n    # tree.info()\n    # 输出到屏幕 / 导出html文件\n    return tree.toHTML()\n```\n\n## 不支持\n\n- 四个空格变为代码段\n- [^1]的引用方式\n- Setext 形式的标题\n- 上标 / 下标 / 下划线\n- TOC与锚点\n\n  锚点的添加通常和目录的跳转有关,而目录树的生成可以考虑解析tree的根Block的所有子HashHeaderBlock来构建.\n  \n  因为跳转的功能是js实现,锚点id的加入也会影响html结构,所以暂不支持\n\n## 补充说明\n\n- 生成的结果如下 `<div class=\'markdown-body\'>markdown内容</div>`\n- 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`\n- 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正\n\n  ```css\n  .markdown-body > ul:has(input) {\n    padding-left: 0;\n    margin-bottom: 0;\n  }\n\n  .markdown-body  ul:has(input) {\n      list-style-type: none;\n  }\n  ```\n\n- 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script type="module">\n    const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\n    codeBlocks.forEach(codeBlock => {\n        codeBlock.classList.remove(\'language-mermaid\');\n        codeBlock.classList.add(\'mermaid\');\n    });\n    import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\n    mermaid.initialize({ startOnLoad: true });\n  </script>\n  ```\n\n  > **请注意**, 由于本Markdown解析器的CodeBlock解析得到的类名为 `language-mermaid`, 而mermaid插件支持的类名格式为`mermaid`, 所以代码中手动修改了 `language-mermaid` 的类名\n\n- 如果您想添加对Latex数学公式的支持, 可以在html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script>\n      MathJax = {\n        tex: {\n          inlineMath: [[\'$\', \'$\'], [\'\\\\(\', \'\\\\)\']]\n        }\n      };\n      </script>\n  <script id="MathJax-script" async\n  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">\n  </script>\n  ```\n\n  注意,这里仅支持\n\n## 相关参考\n\n- [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)\n- [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)',
+    'long_description': '# MarkdownParser\n\n[![codecov](https://codecov.io/gh/luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/MarkdownParser)\n\nMarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换\n\n## 安装\n\n```bash\npip install markdownparser\n```\n\n## 快速使用\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse(\'# Hello World!\')\nprint(html)\n\n#<div class=\'markdown-body\'><h1>Hello World!</h1></div>\n```\n\n其他接口函数\n\n- `parseFile(file_name:str)->str`: 解析文件\n\n接口类\n\n- `Markdown`\n\n  使用类创建对象后可以利用 `self.preprocess_parser` `self.block_parser` `self.tree_parser` 控制解析过程\n\n  其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构\n\n  tree可以通过内部toHTML()方法得到HTML元素\n\n## 测试\n\n```bash\npython generate.py <FILE_NAME>\n\n# python generate.py ./testfiles/test1.md\n# python generate.py README.md\n```\n\n运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比\n\n![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)\n\n代码覆盖率\n\n```bash\ncoverage run -m unittest\ncoverage html\n```\n\n## 实现思路\n\n[Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)\n\n您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构\n\n```python\ndef parse(self, text: str) -> str:\n\n    # 去除空行/注释/html标签\n    lines = self.preprocess_parser(text)\n    # print(lines)\n    # 逐行解析,得到一颗未优化的树\n    root = self.block_parser(lines)\n    # root.info()\n    # 优化,得到正确的markdown解析树\n    tree = self.tree_parser(root)\n    # tree.info()\n    # 输出到屏幕 / 导出html文件\n    return tree.toHTML()\n```\n\n## 不支持\n\n- 四个空格变为代码段\n- [^1]的引用方式\n- Setext 形式的标题\n- 上标 / 下标 / 下划线\n- TOC与锚点\n\n  锚点的添加通常和目录的跳转有关,而目录树的生成可以考虑解析tree的根Block的所有子HashHeaderBlock来构建.\n  \n  因为跳转的功能是js实现,锚点id的加入也会影响html结构,所以暂不支持\n\n## 补充说明\n\n- 生成的结果如下 `<div class=\'markdown-body\'>markdown内容</div>`\n- 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`\n- 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正\n\n  ```css\n  .markdown-body > ul>li:has(input) {\n    padding-left: 0;\n    margin-bottom: 0;\n  }\n\n  .markdown-body  ul>li:has(input)>ul {\n    list-style-type: none;\n    padding-left: 8px;\n  }\n  ```\n\n- 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script type="module">\n    const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\n    codeBlocks.forEach(codeBlock => {\n        codeBlock.classList.remove(\'language-mermaid\');\n        codeBlock.classList.add(\'mermaid\');\n    });\n    import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\n    mermaid.initialize({ startOnLoad: true });\n  </script>\n  ```\n\n  > **请注意**, 由于本Markdown解析器的CodeBlock解析得到的类名为 `language-mermaid`, 而mermaid插件支持的类名格式为`mermaid`, 所以代码中手动修改了 `language-mermaid` 的类名\n\n- 如果您想添加对Latex数学公式的支持, 可以在html页面 `<body>` 末尾添加如下 `<script>`\n\n  ```html\n  <script>\n      MathJax = {\n        tex: {\n          inlineMath: [[\'$\', \'$\'], [\'\\\\(\', \'\\\\)\']]\n        }\n      };\n      </script>\n  <script id="MathJax-script" async\n  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">\n  </script>\n  ```\n\n  注意,这里仅支持\n\n## 相关参考\n\n- [Github Markdown CSS](https://cdn.jsdelivr.net/npm/github-markdown-css@4.0.0/github-markdown.css)\n- [Mermaid API](https://mermaid.js.org/intro/#mermaid-api)\n- [MathJax](https://docs.mathjax.org/en/latest/web/start.html)',
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
@@ -1,53 +1,56 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['markdownparser'] package_data = \ {'': ['*']} setup_kwargs = { 'name':
-'markdownparser', 'version': '0.3.8', 'description': '', 'long_description': '#
-MarkdownParser\n\nMarkdownParser æ¯ä¸ä¸ª Markdown
+'markdownparser', 'version': '0.3.9', 'description': '', 'long_description': '#
+MarkdownParser\n\n[![codecov](https://codecov.io/gh/luzhixing12345/
+MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/
+luzhixing12345/MarkdownParser)\n\nMarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢\n\n##
 å®è£\n\n```bash\npip install markdownparser\n```\n\n##
 å¿«éä½¿ç¨\n\n```python\nimport MarkdownParser\n\nhtml = MarkdownParser.parse
 (\'# Hello World!\')\nprint(html)\n\n#
 ****** Hello World! ******
 \n```\n\nå¶ä»æ¥å£å½æ°\n\n- `parseFile(file_name:str)->str`:
 è§£ææä»¶\n\næ¥å£ç±»\n\n- `Markdown`\n\n
 ä½¿ç¨ç±»åå»ºå¯¹è±¡åå¯ä»¥å©ç¨ `self.preprocess_parser`
 `self.block_parser` `self.tree_parser` æ§å¶è§£æè¿ç¨\n\n
 å¶ä¸­Blockç±»å±æ§è§[base_class.py](MarkdownParser/
 base_class.py),å¯ä»¥éè¿è°ç¨block.info()å½æ°æ¥çæ çç»æ\n\n
 treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´ \n\n##
-æµè¯\n\næ¨å¯ä»¥ä½¿ç¨ `test.py`
-æµè¯Markdownè§£ææ¯å¦æ­£ç¡®\n\n```bash\npython test.py \n\n# python
-test.py ./testfiles/test1.md\n# python test.py
-README.md\n```\n\nè¿è¡ä¼çæindex.html,
+æµè¯\n\n```bash\npython generate.py \n\n# python generate.py ./testfiles/
+test1.md\n# python generate.py README.md\n```\n\nè¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯\n\n!
 [20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png)\n\n## å®ç°æè·¯\n\n[Markdownè§£æå¨çä»£ç å®ç°]
-(https://www.bilibili.com/video/BV1LA411X7X3)\n\næ¨å¯éè¿åæ¶ [core.py]
-(./MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ\n\n```python\ndef parse
-(self, text: str) -> str:\n\n # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾\n lines =
-self.preprocess_parser(text)\n # print(lines)\n #
-éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ \n root = self.block_parser(lines)\n #
-root.info()\n # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ \n tree =
-self.tree_parser(root)\n # tree.info()\n # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶\n
-return tree.toHTML()\n```\n\n## ä¸æ¯æ\n\n- åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ\n-
+20230218202400.png)\n\nä»£ç è¦çç\n\n```bash\ncoverage run -
+m unittest\ncoverage html\n```\n\n## å®ç°æè·¯\n\n
+[Markdownè§£æå¨çä»£ç å®ç°](https://www.bilibili.com/video/
+BV1LA411X7X3)\n\næ¨å¯éè¿åæ¶ [core.py](./MarkdownParser/core.py)
+æ³¨éæ¥è·åæ çç»æ\n\n```python\ndef parse(self, text: str) -> str:
+\n\n # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾\n lines = self.preprocess_parser(text)\n
+# print(lines)\n # éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ \n root =
+self.block_parser(lines)\n # root.info()\n #
+ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ \n tree = self.tree_parser(root)\n #
+tree.info()\n # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶\n return tree.toHTML
+()\n```\n\n## ä¸æ¯æ\n\n- åä¸ªç©ºæ ¼åä¸ºä»£ç æ®µ\n-
 [^1]çå¼ç¨æ¹å¼\n- Setext å½¢å¼çæ é¢\n- ä¸æ  / ä¸æ  / ä¸åçº¿\n-
 TOCä¸éç¹\n\n
 éç¹çæ·»å éå¸¸åç®å½çè·³è½¬æå³,èç®å½æ ççæå¯ä»¥èèè§£ætreeçæ ¹Blockçææå­HashHeaderBlockæ¥æå»º.\n
 \n
 å ä¸ºè·³è½¬çåè½æ¯jså®ç°,éç¹idçå å¥ä¹ä¼å½±åhtmlç»æ,æä»¥æä¸æ¯æ\n\n##
 è¡¥åè¯´æ\n\n- çæçç»æå¦ä¸ `
 markdownåå®¹
 `\n- ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN`\n-
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£\n\n
-```css\n .markdown-body > ul:has(input) {\n padding-left: 0;\n margin-bottom:
-0;\n }\n\n .markdown-body ul:has(input) {\n list-style-type: none;\n }\n
-```\n\n- å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ,
-æ¨å¯åè[mermaid plugin](https://mermaid.js.org/intro/n00b-
-gettingStarted.html#_2-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
+```css\n .markdown-body > ul>li:has(input) {\n padding-left: 0;\n margin-
+bottom: 0;\n }\n\n .markdown-body ul>li:has(input)>ul {\n list-style-type:
+none;\n padding-left: 8px;\n }\n ```\n\n- å¦ææ¨æ³æ·»å å¯¹[Mermaid](https:
+//mermaid.js.org/)çæ¯æ, æ¨å¯åè[mermaid plugin](https://
+mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-
+plugins)å¨æ¨çhtmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
 \n ```\n\n > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å\n\n-
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
```

### Comparing `markdownparser-0.3.8/PKG-INFO` & `markdownparser-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://luzhixing12345.github.io/MarkdownParser/
 Project-URL: Repository, https://github.com/luzhixing12345/MarkdownParser
 Description-Content-Type: text/markdown
 
 # MarkdownParser
 
+[![codecov](https://codecov.io/gh/luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/luzhixing12345/MarkdownParser)
+
 MarkdownParser 是一个 Markdown 语法解析器,用于实现md到html标签的转换
 
 ## 安装
 
 ```bash
 pip install markdownparser
 ```
@@ -51,27 +53,32 @@
 
   其中Block类属性见[base_class.py](MarkdownParser/base_class.py),可以通过调用block.info()函数查看树的结构
 
   tree可以通过内部toHTML()方法得到HTML元素
 
 ## 测试
 
-您可以使用 `test.py` 测试Markdown解析是否正确
-
 ```bash
-python test.py <FILE_NAME>
+python generate.py <FILE_NAME>
 
-# python test.py ./testfiles/test1.md
-# python test.py README.md
+# python generate.py ./testfiles/test1.md
+# python generate.py README.md
 ```
 
 运行会生成index.html, 使用浏览器打开生成的index.html即可与您的Markdown编辑器的预期渲染结果对比
 
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/20230218202400.png)
 
+代码覆盖率
+
+```bash
+coverage run -m unittest
+coverage html
+```
+
 ## 实现思路
 
 [Markdown解析器的代码实现](https://www.bilibili.com/video/BV1LA411X7X3)
 
 您可通过取消 [core.py](./MarkdownParser/core.py) 注释来获取树的结构
 
 ```python
@@ -105,21 +112,22 @@
 ## 补充说明
 
 - 生成的结果如下 `<div class='markdown-body'>markdown内容</div>`
 - 代码段会根据语言加入一个类名便于后期高亮,例如 `class="language-cpp"`, 未定义语言则为 `language-UNKNOWN`
 - 默认导出的HTML中层级任务列表会有显示问题,这是因为使用了ul+li+checkbox的方式,您需要添加以下css样式修正
 
   ```css
-  .markdown-body > ul:has(input) {
+  .markdown-body > ul>li:has(input) {
     padding-left: 0;
     margin-bottom: 0;
   }
 
-  .markdown-body  ul:has(input) {
-      list-style-type: none;
+  .markdown-body  ul>li:has(input)>ul {
+    list-style-type: none;
+    padding-left: 8px;
   }
   ```
 
 - 如果您想添加对[Mermaid](https://mermaid.js.org/)的支持, 您可参考[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-using-mermaid-plugins)在您的html页面 `<body>` 末尾添加如下 `<script>`
 
   ```html
   <script type="module">
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: markdownparser Version: 0.3.8 Summary: Home-page:
+Metadata-Version: 2.1 Name: markdownparser Version: 0.3.9 Summary: Home-page:
 https://github.com/luzhixing12345/MarkdownParser License: MIT Author:
 luzhixing12345 Author-email: luzhixing12345@163.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Project-URL: Documentation,
 https://luzhixing12345.github.io/MarkdownParser/ Project-URL: Repository,
 https://github.com/luzhixing12345/MarkdownParser Description-Content-Type:
-text/markdown # MarkdownParser MarkdownParser æ¯ä¸ä¸ª Markdown
+text/markdown # MarkdownParser [![codecov](https://codecov.io/gh/
+luzhixing12345/MarkdownParser/branch/main/graph/badge.svg?)](https://
+codecov.io/gh/luzhixing12345/MarkdownParser) MarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢ ## å®è£ ```bash pip
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
 ``` å¶ä»æ¥å£å½æ° - `parseFile(file_name:str)->str`: è§£ææä»¶
 æ¥å£ç±» - `Markdown` ä½¿ç¨ç±»åå»ºå¯¹è±¡åå¯ä»¥å©ç¨
 `self.preprocess_parser` `self.block_parser` `self.tree_parser`
 æ§å¶è§£æè¿ç¨ å¶ä¸­Blockç±»å±æ§è§[base_class.py](MarkdownParser/
 base_class.py),å¯ä»¥éè¿è°ç¨block.info()å½æ°æ¥çæ çç»æ
-treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´  ## æµè¯ æ¨å¯ä»¥ä½¿ç¨
-`test.py` æµè¯Markdownè§£ææ¯å¦æ­£ç¡® ```bash python test.py  # python
-test.py ./testfiles/test1.md # python test.py README.md ```
-è¿è¡ä¼çæindex.html,
+treeå¯ä»¥éè¿åé¨toHTML()æ¹æ³å¾å°HTMLåç´  ## æµè¯ ```bash python
+generate.py  # python generate.py ./testfiles/test1.md # python generate.py
+README.md ``` è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
-20230218202400.png) ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://
+20230218202400.png) ä»£ç è¦çç ```bash coverage run -m unittest coverage
+html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°](https://
 www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
 MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
 text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
 self.preprocess_parser(text) # print(lines) #
 éè¡è§£æ,å¾å°ä¸é¢æªä¼åçæ  root = self.block_parser(lines) #
 root.info() # ä¼å,å¾å°æ­£ç¡®çmarkdownè§£ææ  tree = self.tree_parser
 (root) # tree.info() # è¾åºå°å±å¹ / å¯¼åºhtmlæä»¶ return tree.toHTML()
@@ -37,19 +39,19 @@
 éç¹çæ·»å éå¸¸åç®å½çè·³è½¬æå³,èç®å½æ ççæå¯ä»¥èèè§£ætreeçæ ¹Blockçææå­HashHeaderBlockæ¥æå»º.
 å ä¸ºè·³è½¬çåè½æ¯jså®ç°,éç¹idçå å¥ä¹ä¼å½±åhtmlç»æ,æä»¥æä¸æ¯æ
 ## è¡¥åè¯´æ - çæçç»æå¦ä¸ `
 markdownåå®¹
 ` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
-```css .markdown-body > ul:has(input) { padding-left: 0; margin-bottom: 0; }
-.markdown-body ul:has(input) { list-style-type: none; } ``` -
-å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ, æ¨å¯åè
-[mermaid plugin](https://mermaid.js.org/intro/n00b-gettingStarted.html#_2-
-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
+```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
+.markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
+} ``` - å¦ææ¨æ³æ·»å å¯¹[Mermaid](https://mermaid.js.org/)çæ¯æ,
+æ¨å¯åè[mermaid plugin](https://mermaid.js.org/intro/n00b-
+gettingStarted.html#_2-using-mermaid-plugins)å¨æ¨çhtmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
  ``` > **è¯·æ³¨æ**,
 ç±äºæ¬Markdownè§£æå¨çCodeBlockè§£æå¾å°çç±»åä¸º `language-
 mermaid`, èmermaidæä»¶æ¯æçç±»åæ ¼å¼ä¸º`mermaid`,
 æä»¥ä»£ç ä¸­æå¨ä¿®æ¹äº `language-mermaid` çç±»å -
 å¦ææ¨æ³æ·»å å¯¹Latexæ°å­¦å¬å¼çæ¯æ, å¯ä»¥å¨htmlé¡µé¢ `
 ` æ«å°¾æ·»å å¦ä¸ `
```

