# Comparing `tmp/arclet-alconna-1.7.0rc3.tar.gz` & `tmp/arclet-alconna-1.7.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc3.tar", last modified: Thu Apr 20 13:16:09 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc4.tar", last modified: Fri Apr 28 08:00:54 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc3.tar` & `arclet-alconna-1.7.0rc4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc3/LICENSE
--rw-r--r--   0        0        0     2934 2023-04-17 06:25:04.271711 arclet-alconna-1.7.0rc3/pyproject.toml
--rw-r--r--   0        0        0     5108 2023-04-17 05:33:14.505606 arclet-alconna-1.7.0rc3/README-EN.md
--rw-r--r--   0        0        0      928 2023-04-20 13:14:50.371493 arclet-alconna-1.7.0rc3/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc3/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    13932 2023-04-20 13:00:01.793211 arclet-alconna-1.7.0rc3/src/arclet/alconna/analyser.py
--rw-r--r--   0        0        0    11060 2023-04-20 09:42:19.098735 arclet-alconna-1.7.0rc3/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     6768 2023-04-20 12:31:38.881196 arclet-alconna-1.7.0rc3/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    12639 2023-04-17 05:44:49.700466 arclet-alconna-1.7.0rc3/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0     6734 2023-04-17 05:44:49.658976 arclet-alconna-1.7.0rc3/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     4384 2023-04-17 05:41:18.628904 arclet-alconna-1.7.0rc3/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     3515 2023-04-20 12:31:38.882195 arclet-alconna-1.7.0rc3/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     3348 2023-04-20 13:07:02.615788 arclet-alconna-1.7.0rc3/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    13657 2023-04-20 12:48:50.977968 arclet-alconna-1.7.0rc3/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc3/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc3/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0      823 2023-04-08 10:00:51.776731 arclet-alconna-1.7.0rc3/src/arclet/alconna/executor.py
--rw-r--r--   0        0        0     9772 2023-04-20 12:48:50.996903 arclet-alconna-1.7.0rc3/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0    18374 2023-04-20 13:00:17.125966 arclet-alconna-1.7.0rc3/src/arclet/alconna/handlers.py
--rw-r--r--   0        0        0     6033 2023-04-20 12:53:16.998627 arclet-alconna-1.7.0rc3/src/arclet/alconna/header.py
--rw-r--r--   0        0        0       65 2023-04-17 05:01:09.559175 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3217 2023-04-17 05:01:09.583116 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3200 2023-04-17 05:01:09.575993 arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    14589 2023-04-20 12:31:38.884196 arclet-alconna-1.7.0rc3/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc3/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc3/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc3/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc3/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc3/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     2401 2023-04-20 12:43:09.501490 arclet-alconna-1.7.0rc3/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0      895 2023-04-11 10:30:01.832860 arclet-alconna-1.7.0rc3/src/arclet/alconna/util.py
--rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc4/LICENSE
+-rw-r--r--   0        0        0     2731 2023-04-28 07:58:40.959628 arclet-alconna-1.7.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     5861 2023-04-27 14:49:51.354435 arclet-alconna-1.7.0rc4/README-EN.md
+-rw-r--r--   0        0        0      926 2023-04-28 07:41:36.946430 arclet-alconna-1.7.0rc4/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc4/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    13765 2023-04-24 13:50:47.402011 arclet-alconna-1.7.0rc4/src/arclet/alconna/analyser.py
+-rw-r--r--   0        0        0    11183 2023-04-27 14:14:53.516769 arclet-alconna-1.7.0rc4/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     7169 2023-04-28 06:02:12.116241 arclet-alconna-1.7.0rc4/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    12616 2023-04-27 14:25:54.921925 arclet-alconna-1.7.0rc4/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0     6745 2023-04-24 14:02:23.257763 arclet-alconna-1.7.0rc4/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     4384 2023-04-17 05:41:18.628904 arclet-alconna-1.7.0rc4/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     3486 2023-04-27 14:49:51.385435 arclet-alconna-1.7.0rc4/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     3455 2023-04-26 09:58:35.085641 arclet-alconna-1.7.0rc4/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14486 2023-04-27 14:34:40.178996 arclet-alconna-1.7.0rc4/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc4/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc4/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    10341 2023-04-26 10:45:37.334634 arclet-alconna-1.7.0rc4/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0    19181 2023-04-28 07:33:07.099623 arclet-alconna-1.7.0rc4/src/arclet/alconna/handlers.py
+-rw-r--r--   0        0        0     6382 2023-04-28 07:17:08.737239 arclet-alconna-1.7.0rc4/src/arclet/alconna/header.py
+-rw-r--r--   0        0        0       99 2023-04-24 13:02:08.850723 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3273 2023-04-26 10:32:37.466006 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3300 2023-04-26 10:28:23.789467 arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    14530 2023-04-24 14:13:48.282478 arclet-alconna-1.7.0rc4/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc4/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc4/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc4/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc4/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc4/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     2385 2023-04-26 10:52:37.893474 arclet-alconna-1.7.0rc4/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0      915 2023-04-26 10:51:56.274030 arclet-alconna-1.7.0rc4/src/arclet/alconna/util.py
+-rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc4/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc3/LICENSE` & `arclet-alconna-1.7.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/pyproject.toml` & `arclet-alconna-1.7.0rc4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<0.6.0, >=0.5.3",
-    "tarina>=0.3.0",
+    "nepattern<0.6.0, >=0.5.5",
+    "tarina>=0.3.3",
 ]
 dynamic = []
 requires-python = ">=3.8"
 readme = "README-EN.md"
 keywords = [
     "command",
     "argparse",
@@ -34,38 +34,27 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc3"
+version = "1.7.0rc4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
 
 [project.optional-dependencies]
 full = [
     "arclet-alconna-tools>=0.2.0",
 ]
-cli = [
-    "arclet-alconna-cli>=0.3.0",
-]
-graia = [
-    "arclet-alconna-graia>=0.9.0",
-]
-all = [
-    "arclet-alconna-cli>=0.3.0",
-    "arclet-alconna-graia>=0.8.0",
-    "arclet-alconna-tools>=0.2.0",
-]
 
 [tool.pdm.build]
 includes = [
     "src/arclet",
 ]
 
 [tool.pdm.dev-dependencies]
```

### Comparing `arclet-alconna-1.7.0rc3/README-EN.md` & `arclet-alconna-1.7.0rc4/README-EN.md`

 * *Files 14% similar despite different names*

```diff
@@ -57,23 +57,49 @@
 
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
-* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py) 
-* Simple and Flexible Constructor 
+* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
 * Powerful Automatic Type Parse and Conversion
-* Support Synchronous and Asynchronous Actions
-* Customizable Help Text Formatter, Command Analyser, etc.
-* Customizable Language File, Support i18n
+* Customizable Help Text Formatter and Control of Command Analyser
+* i18n Support
 * Cache of input command for quick response of repeated command
 * Easy-to-use Construct and Usage of Command Shortcut
-* Various Features (FuzzyMatch, Command Completion, etc.)
+* Can bind callback function to execute after command parsing
+* Can create command completion session to implement multi-round continuous completion prompt
+* Various Features (FuzzyMatch, Output Capture, etc.)
+
+Example of Callback Executor:
+
+```python
+# callback.py
+from arclet.alconna import Alconna, Args
+
+alc = Alconna("test", Args["foo", int]["bar", str])
+
+@alc.bind()
+def callback(foo: int, bar: str):
+    print(f"foo: {foo}")
+    print(f"bar: {bar}")
+    print(bar * foo)
+    
+if __name__ == "__main__":
+    alc()
+```
+
+```shell
+$ python callback.py test 3 hello
+foo: 3
+bar: hello
+hellohellohello
+```
+
 
 Example of Type Conversion:
 
 ```python
 from arclet.alconna import Alconna, Args
 from pathlib import Path
 
@@ -89,38 +115,52 @@
 '''
 <class 'bytes'>
 <class 'bytes'>
 <class 'bytes'>
 '''
 ```
 
-Example of FuzzyMatch:
-
+Example of Command Shortcut:
 ```python
-from arclet.alconna import Alconna, CommandMeta, Arg
+# shortcut.py
+from arclet.alconna import Alconna, Args
 
-alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
-alc.parse("！test_fuzy foo bar")
+alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
+alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
 
-'''
-！test_fuzy not matched. Are you mean "!test_fuzzy"?
-'''
+if __name__ == "__main__":
+    alc()
 ```
 
-Example of Command Shortcut:
+```shell
+$ python shortcut.py eval print(\"hello world\")
+hello world
+$ python shortcut.py echo hello world!
+hello world!
+```
+
+Example of Command Completion:
 ```python
-from arclet.alconna import Alconna, Args
+# completion.py
+from arclet.alconna import Alconna, Args, Option
 
-alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
-alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
-alc.parse("echo Hello World!")
+alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
 
-'''
-Hello World!
-'''
+if __name__ == "__main__":
+    alc.completion()
+```
+
+```shell
+$ python completion.py test ?
+next input maybe:
+> foo
+> int
+> -h
+> --help
+> fool
 ```
 
 Example of `typing` Support:
 ```python
 from typing import Annotated  # or typing_extensions.Annotated
 from arclet.alconna import Alconna, Args
 
@@ -130,32 +170,37 @@
 
 '''
 'foo': 2
 ParamsUnmatched: param 3 is incorrect
 '''
 ```
 
+Example of FuzzyMatch:
 
-Example of Command Completion:
 ```python
-from arclet.alconna import Alconna, Args, Option
+# fuzzy.py
+from arclet.alconna import Alconna, CommandMeta, Arg
 
-alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
-alc.parse("test --comp")
+alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
+
+if __name__ == "__main__":
+    alc()
 
-'''
-next input maybe:
-> foo
-> int
-> -h
-> --help
-> fool
-'''
 ```
 
+```shell
+$ python fuzzy.py /test_fuzzy foo bar
+/test_fuzy not matched. Are you mean "!test_fuzzy"?
+```
+
+
+
+
+
+
 ## License
 
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from nepattern import AllParam as AllParam, AnyOne as AnyOne  # noqa
 from tarina import Empty as Empty # noqa
 from .config import config, namespace, Namespace
 from .typing import MultiVar, KeyWordVar, Kw, Nargs
 from .args import Args, Field, ArgFlag, Arg
 from .base import CommandNode, Option, Subcommand
-from .completion import CompInterface
+from .completion import CompSession
 from .exceptions import ParamsUnmatched, NullMessage, InvalidParam
 from .analyser import Analyser
 from .argv import Argv
 from .core import Alconna, CommandMeta
 from .arparma import Arparma, ArparmaBehavior
 from .manager import command_manager, ShortcutArgs
 
 from .builtin import store_value, set_default, store_true, store_false
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc3"
+__version__ = "1.7.0rc4"
 
 Arpamar = Arparma
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/action.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/analyser.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/analyser.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import traceback
 from re import Match
 from typing import TYPE_CHECKING, Any, Generic, Callable
 from dataclasses import dataclass, field
 from typing_extensions import Self, TypeAlias
-from tarina.lang import lang
+from tarina import lang
 
 from .manager import command_manager, ShortcutArgs
 from .exceptions import (
     ParamsUnmatched,
     ArgumentMissing,
     FuzzyMatchSuccess,
     PauseTriggered,
@@ -18,39 +18,45 @@
 )
 from .args import Args
 from .header import Header
 from .base import Option, Subcommand
 from .completion import comp_ctx
 from .model import Sentence, HeadResult, OptionResult, SubcommandResult
 from .arparma import Arparma
-from .typing import TDataCollection
+from .typing import TDC
 from .config import Namespace
 from .output import output_manager
 from .handlers import (
     analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion, prompt
 )
-from .argv import Argv
 
 if TYPE_CHECKING:
+    from .argv import Argv
     from .core import Alconna
 
 _SPECIAL = {
     "help": handle_help,
     "shortcut": handle_shortcut,
     "completion": handle_completion
 }
 
 
-def _compile_opts(option: Option, data: dict[str, Sentence | list[Option] | SubAnalyser]):
+def _compile_opts(option: Option, data: dict[str, Sentence | Option | list[Option] | SubAnalyser]):
     for alias in option.aliases:
-        if (li := data.get(alias)) and isinstance(li, list):
-            li.append(option)  # type: ignore
-            li.sort(key=lambda x: x.priority, reverse=True)
+        if li := data.get(alias):
+            if isinstance(li, list):
+                li.append(option)
+            elif isinstance(li, Sentence):
+                data[alias] = option
+                continue
+            else:
+                data[alias] = [li, option]
+            data[alias].sort(key=lambda x: x.priority, reverse=True)
         else:
-            data[alias] = [option]
+            data[alias] = option
 
 
 def default_compiler(analyser: SubAnalyser, _config: Namespace, pids: set[str]):
     require_len = 0
     for opts in analyser.command.options:
         if isinstance(opts, Option):
             _compile_opts(opts, analyser.compile_params)  # type: ignore
@@ -69,21 +75,21 @@
                 analyser.compile_params.setdefault(k, Sentence(name=k))
     analyser.part_len = range(
         len(analyser.command.options) + analyser.need_main_args + require_len
     )
 
 
 @dataclass
-class SubAnalyser(Generic[TDataCollection]):
+class SubAnalyser(Generic[TDC]):
     command: Subcommand
     default_main_only: bool = field(default=False)  # 默认只有主参数
     part_len: range = field(default=range(0))  # 分段长度
     need_main_args: bool = field(default=False)  # 是否需要主参数
     default_separate: bool = field(default=True)
-    compile_params: dict[str, Sentence | list[Option] | SubAnalyser[TDataCollection]] = field(default_factory=dict)
+    compile_params: dict[str, Sentence | Option | list[Option] | SubAnalyser[TDC]] = field(default_factory=dict)
 
     self_args: Args = field(init=False)  # 自身参数
     subcommands_result: dict[str, SubcommandResult] = field(init=False)
     options_result: dict[str, OptionResult] = field(init=False)  # 存放解析到的所有选项
     args_result: dict[str, Any] = field(init=False)  # 参数的解析结果
     header_result: HeadResult | None = field(init=False)
     value_result: Any = field(init=False)
@@ -116,58 +122,57 @@
         self.args_result = {}
         self.options_result = {}
         self.subcommands_result = {}
         self.sentences = []
         self.value_result = None
         self.header_result = None
 
-    def process(self, argv: Argv[TDataCollection]) -> Self:
-        param = argv.context = self.command
-        if param.requires and self.sentences != param.requires:
-            raise ParamsUnmatched(f"{param.name}'s required is not '{' '.join(self.sentences)}'")
+    def process(self, argv: Argv[TDC]) -> Self:
+        sub = argv.context = self.command
+        if sub.requires and self.sentences != sub.requires:
+            raise ParamsUnmatched(f"{sub.name}'s required is not '{' '.join(self.sentences)}'")
         self.sentences = []
-        if param.is_compact:
-            name, _ = argv.popitem()
-            if not name.startswith(param.name):
-                raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
-            argv.pushback(name.lstrip(param.name), replace=True)
+        if sub.is_compact:
+            name, _ = argv.next()
+            if not name.startswith(sub.name):
+                raise ParamsUnmatched(f"{name} dose not matched with {sub.name}")
+            argv.rollback(name.lstrip(sub.name), replace=True)
         else:
-            name, _ = argv.popitem(param.separators)
-            if name != param.name:  # 先匹配选项名称
-                raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
+            name, _ = argv.next(sub.separators)
+            if name != sub.name:  # 先匹配选项名称
+                raise ParamsUnmatched(f"{name} dose not matched with {sub.name}")
 
         if self.part_len.stop == 0:
             self.value_result = Ellipsis
             return self
         return self.analyse(argv)
 
-    def analyse(self, argv: Argv[TDataCollection]) -> Self:
+    def analyse(self, argv: Argv[TDC]) -> Self:
         for _ in self.part_len:
-            analyse_param(self, argv, *argv.popitem(self.command.separators, move=False))
+            analyse_param(self, argv, self.command.separators)
         if self.default_main_only and not self.args_result:
             self.args_result = analyse_args(argv, self.self_args)
         if not self.args_result and self.need_main_args:
-            raise ArgumentMissing(lang.subcommand.args_missing.format(name=self.command.dest))
+            raise ArgumentMissing(lang.require("subcommand", "args_missing").format(name=self.command.dest))
         return self
 
-    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDataCollection] | None:
+    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TDC] | None:
         if target == self.command:
             return self
         for param in self.compile_params.values():
             if isinstance(param, SubAnalyser):
                 return param.get_sub_analyser(target)
 
 
-class Analyser(SubAnalyser[TDataCollection], Generic[TDataCollection]):
+class Analyser(SubAnalyser[TDC], Generic[TDC]):
     command: Alconna  # Alconna实例
     used_tokens: set[int]  # 已使用的token
-    # 命令头部
-    command_header: Header
+    command_header: Header  # 命令头部
 
-    def __init__(self, alconna: Alconna[TDataCollection], compiler: TCompile | None = None):
+    def __init__(self, alconna: Alconna[TDC], compiler: TCompile | None = None):
         super().__init__(alconna)
         self.fuzzy_match = alconna.meta.fuzzy_match
         self.used_tokens = set()
         self.command_header = Header.generate(alconna.command, alconna.prefixes)
         compiler = compiler or default_compiler
         compiler(
             self,
@@ -175,32 +180,28 @@
             command_manager.resolve(self.command).param_ids
         )
 
     def _clr(self):
         self.used_tokens.clear()
         super()._clr()
 
-    @staticmethod
-    def converter(command: str) -> TDataCollection:
-        return command  # type: ignore
-
     def __repr__(self):
         return f"<{self.__class__.__name__} of {self.command.path}>"
 
     def shortcut(
         self,
-        argv: Argv[TDataCollection],
+        argv: Argv[TDC],
         data: list[Any], short: Arparma | ShortcutArgs,
         reg: Match | None
-    ) -> Arparma[TDataCollection]:
+    ) -> Arparma[TDC]:
         if isinstance(short, Arparma):
             return short
         argv.build(short.get('command', self.command.command or self.command.name))
         if not short.get('fuzzy') and data:
-            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=data[0]))
+            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=data[0]))
             if self.command.meta.raise_exception:
                 raise exc
             return self.export(argv, True, exc)
         data_index = 0
         for i, unit in enumerate(argv.raw_data):
             if not data:
                 break
@@ -214,15 +215,15 @@
                 data_index += 1
             elif mat := re.search(r"\{\*(.*)\}", unit, re.DOTALL):
                 sep = mat[1]
                 argv.raw_data[i] = unit.replace(f"{{*{sep}}}", (sep or ' ').join(map(str, data)))
                 data.clear()
 
         argv.bak_data = argv.raw_data.copy()
-        argv.rebuild(*data).rebuild(*short.get('args', []))
+        argv.addon(*data).addon(*short.get('args', []))
         if reg:
             groups: tuple[str, ...] = reg.groups()
             gdict: dict[str, str] = reg.groupdict()
             for j, unit in enumerate(argv.raw_data):
                 if not isinstance(unit, str):
                     continue
                 for i, c in enumerate(groups):
@@ -230,35 +231,35 @@
                 for k, v in gdict.items():
                     unit = unit.replace(f"{{{k}}}", v)
                 argv.raw_data[j] = unit
         if argv.message_cache:
             argv.token = argv.generate_token(argv.raw_data)
         return self.process(argv)
 
-    def process(self, argv: Argv[TDataCollection]) -> Arparma[TDataCollection]:
+    def process(self, argv: Argv[TDC]) -> Arparma[TDC]:
         """主体解析函数, 应针对各种情况进行解析"""
         if (
             argv.message_cache and
             argv.token in self.used_tokens and
             (res := command_manager.get_record(argv.token))
         ):
             return res
         try:
             self.header_result = analyse_header(self.command_header, argv)
         except ParamsUnmatched as e:
             argv.raw_data = argv.bak_data.copy()
             argv.current_index = 0
             try:
-                _res = command_manager.find_shortcut(self.command, argv.popitem(move=False)[0])
+                _res = command_manager.find_shortcut(self.command, argv.next(move=False)[0])
             except ValueError as exc:
                 if self.command.meta.raise_exception:
                     raise e from exc
                 return self.export(argv, True, e)
             else:
-                argv.popitem()
+                argv.next()
                 data = argv.release()
                 self.reset()
                 argv.reset()
                 return self.shortcut(argv, data, *_res)
 
         except FuzzyMatchSuccess as Fuzzy:
             output_manager.send(self.command.name, lambda: str(Fuzzy))
@@ -272,27 +273,27 @@
 
         rest = argv.release()
         if len(rest) > 0:
             if isinstance(rest[-1], str) and rest[-1] in argv.completion_names:
                 last = argv.bak_data[-1]
                 argv.bak_data[-1] = last[:last.rfind(rest[-1])]
                 return handle_completion(self, argv, rest[-2])
-            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=argv.popitem(move=False)[0]))
+            exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=argv.next(move=False)[0]))
         else:
-            exc = ArgumentMissing(lang.analyser.param_missing)
+            exc = ArgumentMissing(lang.require("analyser", "param_missing"))
         if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
             raise PauseTriggered(prompt(self, argv))
         if self.command.meta.raise_exception:
             raise exc
         return self.export(argv, True, exc)
 
-    def analyse(self, argv: Argv[TDataCollection]) -> Arparma[TDataCollection] | None:
+    def analyse(self, argv: Argv[TDC]) -> Arparma[TDC] | None:
         for _ in self.part_len:
             try:
-                analyse_param(self, argv, *argv.popitem(move=False))
+                analyse_param(self, argv)
             except FuzzyMatchSuccess as e:
                 output_manager.send(self.command.name, lambda: str(e))
                 return self.export(argv, True)
             except SpecialOptionTriggered as sot:
                 return _SPECIAL[sot.args[0]](self, argv)
             except (ParamsUnmatched, ArgumentMissing) as e1:
                 if (rest := argv.release()) and isinstance(rest[-1], str):
@@ -311,18 +312,18 @@
                 break
 
         if self.default_main_only and not self.args_result:
             self.args_result = analyse_args(argv, self.self_args)
 
     def export(
         self,
-        argv: Argv[TDataCollection],
+        argv: Argv[TDC],
         fail: bool = False,
         exception: BaseException | None = None,
-    ) -> Arparma[TDataCollection]:
+    ) -> Arparma[TDC]:
         """创建arpamar, 其一定是一次解析的最后部分"""
         result = Arparma(self.command.path, argv.origin, not fail, self.header_result)
         if fail:
             result.error_info = repr(exception or traceback.format_exc(limit=1))
             result.error_data = argv.release()
         else:
             result.main_args = self.args_result
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import inspect
 import re
 from copy import deepcopy
 from dataclasses import field as dc_field
 from enum import Enum
 from functools import partial
 from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union, TYPE_CHECKING
-from tarina import Empty, get_signature
-from tarina.lang import lang
+from tarina import Empty, get_signature, lang
 from nepattern import AllParam, AnyOne, BasePattern, UnionPattern, type_parser
 from typing_extensions import Self
 
 from .exceptions import InvalidParam
 from .typing import KeyWordVar, MultiVar
 
 if TYPE_CHECKING:
@@ -63,26 +62,26 @@
         value: TAValue | None = None,
         field: Field[_T] | _T | None = None,
         seps: str | Iterable[str] = " ",
         notice: str | None = None,
         flags: list[ArgFlag] | None = None,
     ):
         if not isinstance(name, str) or name.startswith('$'):
-            raise InvalidParam(lang.args.name_error)
+            raise InvalidParam(lang.require("args", "name_error"))
         if not name.strip():
-            raise InvalidParam(lang.args.name_empty)
+            raise InvalidParam(lang.require("args", "name_empty"))
         self.name = name
         _value = type_parser(value or name)
         default = field if isinstance(field, Field) else Field(field)
         if isinstance(_value, UnionPattern) and _value.optional:
             default.default = Empty if default.default is None else default.default
         if default.default == "...":
             default.default = Empty
         if _value is Empty:
-            raise InvalidParam(lang.args.value_error.format(target=name))
+            raise InvalidParam(lang.require("args", "value_error").format(target=name))
         self.value = _value
         self.field = default
         self.notice = notice
         self.separators = (seps,) if isinstance(seps, str) else tuple(seps)
         flags = flags or []
         if res := re.match(r"^.+?#(?P<notice>[^;?!/#]+)", name):
             self.notice = res["notice"]
@@ -212,31 +211,31 @@
             if arg.name in self._visit:
                 continue
             self._visit.add(arg.name)
             _limit = False
             if isinstance(arg.value, MultiVar) and not _limit:
                 if isinstance(arg.value.base, KeyWordVar):
                     if self.var_keyword:
-                        raise InvalidParam(lang.args.duplicate_kwargs)
+                        raise InvalidParam(lang.require("args", "duplicate_kwargs"))
                     self.var_keyword = arg.name
                 elif self.var_positional:
-                    raise InvalidParam(lang.args.duplicate_varargs)
+                    raise InvalidParam(lang.require("args", "duplicate_varargs"))
                 else:
                     self.var_positional = arg.name
                 _limit = True
             if isinstance(arg.value, KeyWordVar):
                 if self.var_keyword or self.var_positional:
-                    raise InvalidParam(lang.args.exclude_mutable_args)
+                    raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.keyword_only.append(arg.name)
                 if arg.value.sep in arg.separators:
                     _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
                     _tmp[-1].value = arg.value.base
             if ArgFlag.OPTIONAL in arg.flag:
                 if self.var_keyword or self.var_positional:
-                    raise InvalidParam(lang.args.exclude_mutable_args)
+                    raise InvalidParam(lang.require("args", "exclude_mutable_args"))
                 self.optional_count += 1
         self.argument.clear()
         self.argument.extend(_tmp)
         del _tmp
         del _visit
 
     def __len__(self):
@@ -265,14 +264,15 @@
         elif isinstance(other, Sequence):
             self.__getitem__(tuple(other))
         return self
 
     __add__ = __merge__
     __iadd__ = __merge__
     __lshift__ = __merge__
+    __iter__ = lambda self: iter(self.argument)
 
     def __truediv__(self, other) -> Self:
         self.separate(*other if isinstance(other, (list, tuple, set)) else other)
         return self
 
     def __eq__(self, other):
         return self.argument == other.argument
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/argv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field, InitVar
 from typing import Any, Callable, Generic
 from typing_extensions import Self
-from tarina import split, split_once
-from tarina.lang import lang
+from tarina import split, split_once, lang
 
 from .args import Arg
 from .config import Namespace, config
 from .base import Option, Subcommand
 from .exceptions import NullMessage
-from .typing import TDataCollection
+from .typing import TDC
 
 _cache: dict[type, dict[str, Any]] = {}
 
 
 @dataclass(repr=True)
-class Argv(Generic[TDataCollection]):
+class Argv(Generic[TDC]):
     namespace: InitVar[Namespace] = field(default=config.default_namespace)
     fuzzy_match: bool = field(default=False)
     preprocessors: dict[str, Callable[..., Any]] = field(default_factory=dict)
     to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
     separators: tuple[str, ...] = field(default=(' ',))  # 分隔符
     filter_out: list[str] = field(default_factory=list)  # 元素黑名单
+    checker: Callable[[Any], bool] | None = field(default=None)
+    converter: Callable[[str | list], TDC] | None = field(default=lambda x: x)
     filter_crlf: bool = field(default=True)
     message_cache: bool = field(default=True)
     param_ids: set[str] = field(default_factory=set)
 
     context: Arg | Subcommand | Option | None = field(init=False)
     current_index: int = field(init=False)  # 当前数据的index
     ndata: int = field(init=False)  # 原始数据的长度
     bak_data: list[str | Any] = field(init=False)
     raw_data: list[str | Any] = field(init=False)
     token: int = field(init=False)  # 临时token
-    origin: TDataCollection = field(init=False)
+    origin: TDC = field(init=False)
     _sep: tuple[str, ...] | None = field(init=False)
 
     @classmethod
     def config(
         cls,
         preprocessors: dict[str, Callable[..., Any]] | None = None,
         to_text: Callable[[Any], str | None] | None = None,
-        filter_out: list[str] | None = None
+        filter_out: list[str] | None = None,
+        checker: Callable[[Any], bool] | None = None,
+        converter: Callable[[str | list], TDC] | None = None
     ):
         _cache.setdefault(cls, {}).update(locals())
 
     def __post_init__(self, namespace: Namespace):
         self.reset()
         self.special: dict[str, str] = {}
         self.special.update(
@@ -54,38 +57,42 @@
             [(i, "shortcut") for i in namespace.builtin_option_name['shortcut']]
         )
         self.completion_names = namespace.builtin_option_name['completion']
         if __cache := _cache.get(self.__class__, {}):
             self.preprocessors.update(__cache["preprocessors"] or {})
             self.filter_out.extend(__cache["filter_out"] or [])
             self.to_text = __cache["to_text"] or self.to_text
+            self.checker = __cache["checker"] or self.checker
+            self.converter = __cache["converter"] or self.converter
 
     def reset(self):
         self.current_index = 0
         self.ndata = 0
         self.bak_data = []
         self.raw_data = []
         self.token = 0
         self.origin = "None"
         self._sep = None
         self.context = None
 
     @staticmethod
-    def generate_token(data: list[Any | list[str]]) -> int:
-        return hash(str(data))
+    def generate_token(data: list) -> int:
+        return hash(repr(data))
 
     @property
     def done(self) -> bool:
         return self.current_index == self.ndata
 
-    def build(self, data: TDataCollection) -> Self:
+    def build(self, data: TDC) -> Self:
         """命令分析功能, 传入字符串或消息链"""
         self.reset()
+        if self.checker and not self.checker(data):
+            raise TypeError(data)
         self.origin = data
-        if isinstance(data, str):
+        if data.__class__ is str:
             data = [data]
         i, raw_data = 0, self.raw_data
         for unit in data:
             if (uname := unit.__class__.__name__) in self.filter_out:
                 continue
             if (proc := self.preprocessors.get(uname)) and (res := proc(unit)):
                 unit = res
@@ -93,22 +100,22 @@
                 raw_data.append(unit)
             elif not (res := text.strip()):
                 continue
             else:
                 raw_data.append(res)
             i += 1
         if i < 1:
-            raise NullMessage(lang.analyser_handle_null_message.format(target=data))
+            raise NullMessage(lang.require("argv", "null_message").format(target=data))
         self.ndata = i
         self.bak_data = raw_data.copy()
         if self.message_cache:
             self.token = self.generate_token(raw_data)
         return self
 
-    def rebuild(self, *data: str | Any) -> Self:
+    def addon(self, *data: str | Any) -> Self:
         self.raw_data = self.bak_data.copy()
         for i, d in enumerate(data):
             if not d:
                 continue
             if isinstance(d, str) and i > 0 and isinstance(self.raw_data[-1], str):
                 self.raw_data[-1] += f"{self.separators[0]}{d}"
             else:
@@ -116,53 +123,53 @@
                 self.ndata += 1
         self.current_index = 0
         self.bak_data = self.raw_data.copy()
         if self.message_cache:
             self.token = self.generate_token(self.raw_data)
         return self
 
-    def popitem(self, separate: tuple[str, ...] | None = None, move: bool = True) -> tuple[str | Any, bool]:
+    def next(self, separate: tuple[str, ...] | None = None, move: bool = True) -> tuple[str | Any, bool]:
         """获取解析需要的下个数据"""
         if self._sep:
             self._sep = None
         if self.current_index == self.ndata:
             return "", True
         separate = separate or self.separators
         _current_data = self.raw_data[self.current_index]
-        if _current_data.__class__ == str:
+        if _current_data.__class__ is str:
             _text, _rest_text = split_once(_current_data, separate, self.filter_crlf)  # type: ignore
             if move:
                 if _rest_text:
                     self._sep = separate
                     self.raw_data[self.current_index] = _rest_text
                 else:
                     self.current_index += 1
             return _text, True
         if move:
             self.current_index += 1
         return _current_data, False
 
-    def pushback(self, data: str | Any, replace: bool = False):
+    def rollback(self, data: str | Any, replace: bool = False):
         """把 pop的数据放回 (实际只是‘指针’移动)"""
-        if data in ("", None):
+        if data == "" or data is None:
             return
         if self._sep:
             _current_data = self.raw_data[self.current_index]
             self.raw_data[self.current_index] = f"{data}{self._sep[0]}{_current_data}"
             return
         if self.current_index >= 1:
             self.current_index -= 1
         if replace:
             self.raw_data[self.current_index] = data
 
     def release(self, separate: tuple[str, ...] | None = None, recover: bool = False) -> list[str | Any]:
         _result = []
         data = self.bak_data if recover else self.raw_data[self.current_index:]
         for _data in data:
-            if isinstance(_data, str):
+            if _data.__class__ is str:
                 _result.extend(split(_data, separate or (' ',)))
             else:
                 _result.append(_data)
         return _result
 
     def data_set(self):
         return self.raw_data.copy(), self.current_index
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/arparma.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 from abc import ABCMeta, abstractmethod
 from contextlib import suppress
 from dataclasses import dataclass, field
 from functools import lru_cache
 from types import MappingProxyType
 from typing import Any, Callable, Generic, Mapping, TypeVar, overload
-from tarina import get_signature, generic_isinstance, Empty
-from tarina.lang import lang
+from tarina import get_signature, generic_isinstance, Empty, lang
 from typing_extensions import Self
 
 from .exceptions import BehaveCancelled, OutBoundsBehave
 from .model import HeadResult, OptionResult, SubcommandResult
-from .typing import TDataCollection
+from .typing import TDC
 
 T = TypeVar('T')
 D = TypeVar('D')
 
 
 def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
     if _pf == "options":
@@ -40,34 +39,34 @@
     elif not (__src := _subs.get(_pf)):
         return _subs, _pf
     if (_end := _parts.pop(0)) == "value":
         return __src, _end
     if _end == 'args':
         return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
     if _end == "options" and (_end in __src.options or not _parts):
-        raise RuntimeError(lang.arpamar.ambiguous_name.format(target=f"{_pf}.{_end}"))
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
     if _end == "options" or _end in __src.options:
         return _handle_opt(_end, _parts, __src.options)
     if _end == "subcommands" and (_end in __src.subcommands or not _parts):
-        raise RuntimeError(lang.arpamar.ambiguous_name.format(target=f"{_pf}.{_end}"))
+        raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=f"{_pf}.{_end}"))
     if _end == "subcommands" or _end in __src.subcommands:
         return _handle_sub(_end, _parts, __src.subcommands)
     return __src.args, _end
 
 
-class Arparma(Generic[TDataCollection]):
+class Arparma(Generic[TDC]):
     """承载解析结果与操作数据的接口类"""
     header_match: HeadResult
     options: dict[str, OptionResult]
     subcommands: dict[str, SubcommandResult]
 
     def __init__(
         self,
         source: str,
-        origin: TDataCollection,
+        origin: TDC,
         matched: bool = False,
         header_match: HeadResult | None = None,
         error_info: type[BaseException] | BaseException | str = '',
         error_data: list[str | Any] | None = None,
         main_args: dict[str, Any] | None = None,
         options: dict[str, OptionResult] | None = None,
         subcommands: dict[str, SubcommandResult] | None = None,
@@ -165,15 +164,15 @@
                     continue
                 except OutBoundsBehave as e:
                     return self.fail(e)
         return self
 
     def call(self, target: Callable[..., T], **additional):
         if self.matched:
-            names = tuple(p.name for p in get_signature(target))
+            names = {p.name for p in get_signature(target)}
             return target(**{k: v for k, v in {**self.all_matched_args, **additional}.items() if k in names})
         raise RuntimeError
 
     def fail(self, exc: type[BaseException] | BaseException | str):
         return Arparma(self._source, self.origin, False, self.header_match, error_info=exc)
 
     def __require__(self, parts: list[str]) -> tuple[dict[str, Any] | OptionResult | SubcommandResult | None, str]:
@@ -184,15 +183,15 @@
                 if part in src:
                     return src, part
             if part in {"options", "subcommands", "main_args", "other_args"}:
                 return getattr(self, part, {}), ''
             return (self.all_matched_args, '') if part == "args" else (None, part)
         prefix = parts.pop(0)  # parts[0]
         if prefix in {"options", "subcommands"} and prefix in self.components:
-            raise RuntimeError(lang.arpamar.ambiguous_name.format(target=prefix))
+            raise RuntimeError(lang.require("arparma", "ambiguous_name").format(target=prefix))
         if prefix == "options" or prefix in self.options:
             return _handle_opt(prefix, parts, self.options)
         if prefix == "subcommands" or prefix in self.subcommands:
             return _handle_sub(prefix, parts, self.subcommands)
         prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
         if prefix in {"main_args", "other_args"}:
             return getattr(self, prefix, {}), parts.pop(0)
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/base.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Alconna 的基础内容相关"""
 from __future__ import annotations
 
 from functools import reduce
 from typing import Callable, Iterable, Sequence, overload
 from typing_extensions import Self
-from tarina.lang import lang
+from tarina import lang
 
 from .action import ArgAction
 from .args import Arg, Args
 from .exceptions import InvalidParam
 
 
 class CommandNode:
@@ -35,15 +35,15 @@
             name(str): 命令节点名称
             args(Arg | Args): 命令节点参数
             action(ArgAction): 命令节点响应动作
             separators(str | Sequence[str] | Set[str]): 命令分隔符
             help_text(str): 命令帮助信息
         """
         if not name:
-            raise InvalidParam(lang.node.name_empty)
+            raise InvalidParam(lang.require("common", "name_empty"))
         _parts = name.split(" ")
         self.name = _parts[-1]
         self.requires = ([requires] if isinstance(requires, str) else list(requires)) if requires else []
         self.requires.extend(_parts[:-1])
         self.args = Args() + args
         self.action = ArgAction.__validator__(action, self.args)
         self.separators = (' ',) if separators is None else (
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, TYPE_CHECKING
-from tarina import ContextModel
-from tarina.lang import lang
+from tarina import ContextModel, lang
 
 from .exceptions import PauseTriggered
 from .manager import command_manager
 from .output import output_manager
 
 
 if TYPE_CHECKING:
@@ -17,20 +16,20 @@
 @dataclass(eq=True, frozen=True, unsafe_hash=True)
 class Prompt:
     text: str = field(hash=True)
     can_use: bool = field(default=True, hash=False)
     removal_prefix: str | None = field(default=None, hash=False)
 
 
-class CompInterface:
+class CompSession:
     """
     Examples:
-        >>> from arclet.alconna import Alconna, CompInterface
+        >>> from arclet.alconna import Alconna, CompSession
         >>> alc = Alconna(...)
-        >>> with CompInterface(alc) as comp:
+        >>> with CompSession(alc) as comp:
         ...     res = alc.parse("test")
         ...
         >>> if comp.available:
         ...     print(comp.current())
         ...     print(comp.tab())
         ...     with comp:
         ...         res = comp.enter()
@@ -62,28 +61,28 @@
         self.index += offset
         self.index %= len(self.prompts)
         return self.prompts[self.index].text
 
     def enter(self, content: Any | None = None):
         argv = command_manager.resolve(self.source.command)
         if content:
-            argv.rebuild(content)
+            argv.addon(content)
             self.clear()
             return self.source.process(argv)
         if not self.prompts:
             raise ValueError("No prompt available.")
         prompt = self.prompts[self.index]
         if not prompt.can_use:
             raise ValueError("This prompt cannot be used.")
         if prompt.removal_prefix:
             last = argv.bak_data[-1]
             argv.bak_data[-1] = last[
                 : last.rfind(prompt.removal_prefix)
             ]
-        argv.rebuild(prompt.text)
+        argv.addon(prompt.text)
         self.clear()
         return self.source.process(argv)
 
     def push(self, *suggests: Prompt):
         self.prompts.extend(suggests)
         return self
 
@@ -96,15 +95,15 @@
     def lines(self):
         return [
             f"{'>' if self.index == index else '*'} {sug.text}"
             for index, sug in enumerate(self.prompts)
         ]
 
     def __repr__(self):
-        return f"{lang.common.completion_node}\n" + "\n".join(self.lines())
+        return f"{lang.require('completion', 'node')}\n" + "\n".join(self.lines())
 
     def send_prompt(self):
         return output_manager.send(self.source.command.name, lambda: self.__repr__())
 
     def __enter__(self):
         self._token = comp_ctx.set(self)
         return self
@@ -114,8 +113,8 @@
             comp_ctx.reset(self._token)
         if exc_type is PauseTriggered:
             self.clear()
             self.push(*exc_val.args[0])
             return True
 
 
-comp_ctx: ContextModel[CompInterface] = ContextModel("comp_ctx")
+comp_ctx: ContextModel[CompSession] = ContextModel("comp_ctx")
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/config.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import ContextManager, TypedDict, Callable, Any, TYPE_CHECKING
-from tarina.lang import lang
+from tarina import lang
 from pathlib import Path
 
-from .typing import TPrefixes
+from .typing import TPrefixes, DataCollection
 
 if TYPE_CHECKING:
     from .formatter import TextFormatter
 
 
 class OptionNames(TypedDict):
     help: set[str]
@@ -30,14 +30,15 @@
         default_factory=lambda: {
             "help": {"--help", "-h"},
             "shortcut": {"--shortcut", "-sct"},
             "completion": {"--comp", "-cp", "?", "？"},
         }
     )
     to_text: Callable[[Any], str | None] = field(default=lambda x: x if isinstance(x, str) else None)
+    converter: Callable[[str | list], DataCollection[Any]] | None = field(default=lambda x: x)
 
     def __eq__(self, other):
         return isinstance(other, Namespace) and other.name == self.name
 
     def __hash__(self):
         return hash(self.name)
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,51 @@
 from __future__ import annotations
 
 import sys
 from dataclasses import InitVar, dataclass, field
 from functools import reduce, partial
 from typing import Any, Callable, Generic, Sequence, TypeVar, overload
 
-from tarina import init_spec
-from tarina.lang import lang
+from tarina import init_spec, lang
 from typing_extensions import Self
 
 from .action import ArgAction, exec_, exec_args
 from .analyser import TCompile, Analyser
 from .args import Arg, Args
 from .arparma import Arparma, ArparmaBehavior
 from .base import Option, Subcommand
 from .config import Namespace, config
 from .duplication import Duplication
-from .exceptions import NullMessage
-from .executor import ArparmaExecutor, T
+from .exceptions import NullMessage, ExecuteFailed
 from .formatter import TextFormatter
 from .manager import ShortcutArgs, command_manager
-from .typing import TDataCollection, TPrefixes
+from .typing import TDC, TPrefixes
 
 T_Duplication = TypeVar('T_Duplication', bound=Duplication)
+T = TypeVar("T")
+
+
+@dataclass(init=True, unsafe_hash=True)
+class ArparmaExecutor(Generic[T]):
+    target: Callable[..., T]
+    binding: Callable[..., list[Arparma]] = field(default=lambda: [], repr=False)
+
+    __call__ = lambda self, *args, **kwargs: self.target(*args, **kwargs)
+
+    @property
+    def result(self) -> T:
+        if not self.binding:
+            raise ExecuteFailed(None)
+        arps = self.binding()
+        if not arps or not arps[0].matched:
+            raise ExecuteFailed("Unmatched")
+        try:
+            return arps[0].call(self.target)
+        except Exception as e:
+            raise ExecuteFailed(e) from e
 
 
 @dataclass
 class ActionHandler(ArparmaBehavior):
     source: InitVar[Alconna]
     main_action: ArgAction | None = field(init=False, default=None)
     options: dict[str, ArgAction] = field(init=False, default_factory=dict)
@@ -62,15 +81,15 @@
     author: str | None = field(default=None)
     fuzzy_match: bool = field(default=False)
     raise_exception: bool = field(default=False)
     hide: bool = field(default=False)
     keep_crlf: bool = field(default=False)
 
 
-class Alconna(Subcommand, Generic[TDataCollection]):
+class Alconna(Subcommand, Generic[TDC]):
     """
     更加精确的命令解析
 
     Examples:
 
         >>> from arclet.alconna import Alconna
         >>> alc = Alconna(
@@ -93,15 +112,15 @@
     namespace: str
     meta: CommandMeta
     behaviors: list[ArparmaBehavior]
 
     global_analyser_type: type[Analyser] = Analyser
 
     @property
-    def compile(self) -> Callable[[TCompile | None], Analyser[TDataCollection]]:
+    def compile(self) -> Callable[[TCompile | None], Analyser[TDC]]:
         return partial(self.analyser_type, self)
 
     @classmethod
     def default_analyser(cls, __t: type[Analyser] | None = None):
         """配置 Alconna 的默认解析器"""
         if __t is not None:
             cls.global_analyser_type = __t
@@ -146,26 +165,27 @@
         self.analyser_type = analyser_type or self.__class__.global_analyser_type  # type: ignore
         self.formatter = (formatter_type or np_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
         self.meta.fuzzy_match = self.meta.fuzzy_match or np_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or np_config.raise_exception
         options = [i for i in args if isinstance(i, (Option, Subcommand))]
         options.append(
-            Option("|".join(np_config.builtin_option_name['help']), help_text=lang.builtin.option_help),
+            Option("|".join(np_config.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")),
         )
         options.append(
             Option(
                 "|".join(np_config.builtin_option_name['shortcut']),
                 Args["delete;?", "delete"]["name", str]["command", str, "_"],
-                help_text=lang.builtin.option_shortcut
+                help_text=lang.require("builtin", "option_shortcut")
             )
         )
         options.append(
             Option(
-                "|".join(np_config.builtin_option_name['completion']), help_text=lang.builtin.option_completion
+                "|".join(np_config.builtin_option_name['completion']),
+                help_text=lang.require("builtin", "option_completion")
             )
         )
         name = f"{self.command or self.prefixes[0]}".replace(command_manager.sign, "")  # type: ignore
         self.path = f"{self.namespace}::{name}"
         super().__init__(
             "ALCONNA::",
             reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
@@ -191,23 +211,24 @@
         if isinstance(namespace, str):
             namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
         self.namespace = namespace.name
         self.path = f"{self.namespace}::{self.name}"
         if header:
             self.prefixes = namespace.prefixes.copy()
         self.options[-3] = Option(
-            "|".join(namespace.builtin_option_name['help']), help_text=lang.builtin.option_help
+            "|".join(namespace.builtin_option_name['help']), help_text=lang.require("builtin", "option_help")
         )
         self.options[-2] = Option(
             "|".join(namespace.builtin_option_name['shortcut']),
             Args["delete;?", "delete"]["name", str]["command", str, "_"],
-            help_text=lang.builtin.option_shortcut
+            help_text=lang.require("builtin", "option_shortcut")
         )
         self.options[-1] = Option(
-            "|".join(namespace.builtin_option_name['completion']), help_text=lang.builtin.option_completion
+            "|".join(namespace.builtin_option_name['completion']),
+            help_text=lang.require("builtin", "option_completion")
         )
         self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
         self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
@@ -216,33 +237,34 @@
         self.behaviors[1:] = behaviors
         return self
 
     def get_help(self) -> str:
         """返回该命令的帮助信息"""
         return self.formatter.format_node()
 
-    def shortcut(self, key: str, args: ShortcutArgs[TDataCollection] | None = None, delete: bool = False):
+    def shortcut(self, key: str, args: ShortcutArgs[TDC] | None = None, delete: bool = False):
         """添加快捷命令"""
         try:
             if delete:
                 command_manager.delete_shortcut(self, key)
-                return lang.shortcut.delete_success.format(shortcut=key, target=self.path)
+                return lang.require("shortcut", "delete_success").format(shortcut=key, target=self.path)
             if args:
                 command_manager.add_shortcut(self, key, args)
-                return lang.shortcut.add_success.format(shortcut=key, target=self.path)
+                return lang.require("shortcut", "add_success").format(shortcut=key, target=self.path)
             elif cmd := command_manager.recent_message:
                 alc = command_manager.last_using
                 if alc and alc == self:
                     command_manager.add_shortcut(self, key, {"command": cmd})
-                    return lang.shortcut.add_success.format(shortcut=key, target=self.path)
+                    return lang.require("shortcut", "add_success").format(shortcut=key, target=self.path)
                 raise ValueError(
-                    lang.shortcut.recent_command_error.format(target=self.path, source=getattr(alc, "path", "Unknown"))
+                    lang.require("shortcut", "recent_command_error")
+                    .format(target=self.path, source=getattr(alc, "path", "Unknown"))
                 )
             else:
-                raise ValueError(lang.shortcut.no_recent_command)
+                raise ValueError(lang.require("shortcut", "no_recent_command"))
         except Exception as e:
             if self.meta.raise_exception:
                 raise e
             return str(e)
 
     def __repr__(self):
         return f"{self.namespace}::{self.name}(args={self.args}, options={self.options})"
@@ -259,53 +281,57 @@
     def option(self, opt: Option) -> Self:
         return self.add(opt)
 
     @init_spec(Subcommand, True)
     def subcommand(self, sub: Subcommand) -> Self:
         return self.add(sub)
 
-    def _parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
+    def _parse(self, message: TDC) -> Arparma[TDC]:
         if self.union:
             for ana, argv in command_manager.requires(*self.union):
-                argv.build(message)
-                if (res := ana.process(argv)).matched:
+                if (res := ana.process(argv.build(message))).matched:
                     return res
         analyser = command_manager.require(self)
         argv = command_manager.resolve(self)
         argv.build(message)
         return analyser.process(argv)
 
     @overload
-    def parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
+    def parse(self, message: TDC) -> Arparma[TDC]:
         ...
 
     @overload
     def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication:
         ...
 
     def parse(
-        self, message: TDataCollection, *, duplication: type[T_Duplication] | None = None
-    ) -> Arparma[TDataCollection] | T_Duplication:
+        self, message: TDC, *, duplication: type[T_Duplication] | None = None
+    ) -> Arparma[TDC] | T_Duplication:
         """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类"""
         try:
             arp = self._parse(message)
         except NullMessage as e:
             if self.meta.raise_exception:
                 raise e
             return Arparma(self.path, message, False, error_info=e)
         if arp.matched:
             self.behaviors[0].operate(arp)
             arp = arp.execute()
+            if self._executors:
+                for ext in self._executors:
+                    arp.call(ext.target)
         return duplication(arp) if duplication else arp
 
-    def bind(self, target: Callable[..., T]) -> ArparmaExecutor[T]:
-        ext = ArparmaExecutor(target)
-        ext.binding = lambda: command_manager.get_result(self)
-        self._executors.append(ext)
-        return self._executors[-1]
+    def bind(self, active: bool = True):
+        def wrapper(target: Callable[..., T]) -> ArparmaExecutor[T]:
+            ext = ArparmaExecutor(target, lambda: command_manager.get_result(self))
+            if active:
+                self._executors.append(ext)
+            return ext
+        return wrapper
 
     def __truediv__(self, other) -> Self:
         return self.reset_namespace(other)
 
     __rtruediv__ = __truediv__
 
     def __add__(self, other) -> Self:
@@ -325,16 +351,14 @@
         return self
 
     def __or__(self, other: Alconna) -> Self:
         self.union.add(other.path)
         return self
 
     def _calc_hash(self):
-        return hash(
-            (self.path + str(self.prefixes), self.meta, *self.options, *self.args.argument)
-        )
+        return hash((self.path + str(self.prefixes), self.meta, *self.options, *self.args))
 
     def __call__(self, *args, **kwargs):
         return self.parse(list(args)) if args else self.parse(sys.argv[1:])
 
 
 __all__ = ["Alconna", "CommandMeta"]
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
-from tarina import Empty
+from tarina import Empty, lang
 from nepattern import AllParam, BasePattern
 
 from .args import Arg, Args
 from .base import Option, Subcommand
 
 if TYPE_CHECKING:
     from .core import Alconna
@@ -176,54 +176,72 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n## 注释\n  " + "\n  ".join([f"{v[0]}: {v[1]}" for v in notice]) if notice else res
+        return (
+            f"{res}\n## {lang.require('format', 'notice')}\n  " +
+            "\n  ".join([f"{v[0]}: {v[1]}" for v in notice])
+        ) if notice else res
+
 
     def header(self, root: dict[str, Any], separators: tuple[str, ...]) -> str:
         """头部节点的描述"""
         help_string = f"\n{desc}" if (desc := root.get('description')) else ""
-        usage = f"\n用法:\n{usage}" if (usage := root.get('usage')) else ""
-        example = f"\n使用示例:\n{example}" if (example := root.get('example')) else ""
+        usage = f"\n{lang.require('format', 'usage')}:\n{usage}" if (usage := root.get('usage')) else ""
+        example = f"\n{lang.require('format', 'example')}:\n{example}" if (example := root.get('example')) else ""
         prefixs = f"[{''.join(map(str, prefixs))}]" if (prefixs := root.get('prefix', [])) != [] else ""
         cmd = f"{prefixs}{root.get('name', '')}"
         command_string = cmd or (root['name'] + separators[0])
-        return f"{command_string} %s{help_string}{usage}\n%s{example}"
+        return f"{command_string} %s{help_string}{usage}\n\n%s{example}"
 
-    def part(self, node: Subcommand | Option) -> str:
-        """每个子节点的描述"""
-        if isinstance(node, Subcommand):
-            name = " ".join(node.requires) + (' ' if node.requires else '') + node.name
-            option_string = "".join([self.part(i).replace("\n", "\n ") for i in node.options])
-            option_help = "## 该子命令内可用的选项有:\n " if option_string else ""
-            return (
-                f"# {node.help_text}\n"
-                f"  {name}{tuple(node.separators)[0]}"
-                f"{self.parameters(node.args)}\n"
-                f"{option_help}{option_string}"
-            )
-        elif isinstance(node, Option):
-            alias_text = " ".join(node.requires) + (' ' if node.requires else '') + ", ".join(node.aliases)
-            return (
-                f"# {node.help_text}\n"
-                f"  {alias_text}{tuple(node.separators)[0]}"
-                f"{self.parameters(node.args)}\n"
-            )
-        else:
-            raise TypeError(f"{node} is not a valid node")
+    def opt(self, node: Option) -> str:
+        """对单个选项的描述"""
+        alias_text = " ".join(node.requires) + (' ' if node.requires else '') + "|".join(node.aliases)
+        return (
+            f"* {node.help_text}\n"
+            f"  {alias_text}{node.separators[0]}{self.parameters(node.args)}\n"
+        )
+
+    def sub(self, node: Subcommand) -> str:
+        """对单个子命令的描述"""
+        name = " ".join(node.requires) + (' ' if node.requires else '') + node.name
+        opt_string = "".join(
+            [
+                self.opt(opt).replace("\n", "\n  ").replace("# ", "* ")
+                for opt in filter(lambda x: isinstance(x, Option), node.options)
+            ]
+        )
+        sub_string = "".join(
+            [
+                self.opt(sub).replace("\n", "\n  ").replace("# ", "* ")  # type: ignore
+                for sub in filter(lambda x: isinstance(x, Subcommand), node.options)
+            ]
+        )
+        opt_help = f"  {lang.require('format', 'subcommands.opts')}:\n  " if opt_string else ""
+        sub_help = f"  {lang.require('format', 'subcommands.subs')}:\n  " if sub_string else ""
+        return (
+            f"* {node.help_text}\n"
+            f"  {name}{tuple(node.separators)[0]}{self.parameters(node.args)}\n"
+            f"{sub_help}{sub_string}"
+            f"{opt_help}{opt_string}"
+        ).rstrip(' ')
 
     def body(self, parts: list[Option | Subcommand]) -> str:
         """子节点列表的描述"""
         option_string = "".join(
-            [self.part(opt) for opt in filter(lambda x: isinstance(x, Option), parts)
-            if opt.name not in self.ignore_names]
+            [
+                self.opt(opt) for opt in filter(lambda x: isinstance(x, Option), parts)
+                if opt.name not in self.ignore_names
+            ]
+        )
+        subcommand_string = "".join(
+            [self.sub(sub) for sub in filter(lambda x: isinstance(x, Subcommand), parts)]
         )
-        subcommand_string = "".join([self.part(sub) for sub in filter(lambda x: isinstance(x, Subcommand), parts)])
-        option_help = "可用的选项有:\n" if option_string else ""
-        subcommand_help = "可用的子命令有:\n" if subcommand_string else ""
+        option_help = f"{lang.require('format', 'options')}:\n" if option_string else ""
+        subcommand_help = f"{lang.require('format', 'subcommands')}:\n" if subcommand_string else ""
         return f"{subcommand_help}{subcommand_string}{option_help}{option_string}"
 
 
 __all__ = ["TextFormatter", "Trace"]
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/handlers.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
-from tarina import Empty, split_once
-from tarina.lang import lang
+from tarina import Empty, split_once, lang
 from nepattern import AllParam, BasePattern
 from nepattern.util import TPattern
 
 from .args import Arg, Args
 from .header import Double, Header
 from .base import Option, Subcommand
 from .config import config
@@ -33,50 +32,50 @@
     optional: bool,
     key: str | None = None,
     fuzzy: bool = False,
 ):
     if _kwarg := re.match(fr'^([^{value.sep}]+){value.sep}(.*?)$', may_arg):
         key = key or _kwarg[1]
         if (_key := _kwarg[1]) != key:
-            argv.pushback(may_arg)
+            argv.rollback(may_arg)
             if fuzzy and levenshtein_norm(_key, key) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_key, target=key))
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_key, target=key))
             if default_val is None:
-                raise ParamsUnmatched(lang.common.fuzzy_matched.format(source=_key, target=key))
+                raise ParamsUnmatched(lang.require("fuzzy", "matched").format(source=_key, target=key))
             result_dict[_key] = None if default_val is Empty else default_val
             return
         if not (_m_arg := _kwarg[2]):
-            _m_arg, _ = argv.popitem(seps)
-        res = value.base(_m_arg, default_val)
+            _m_arg, _ = argv.next(seps)
+        res = value.base.exec(_m_arg, default_val)
         if res.flag != 'valid':
-            argv.pushback(may_arg)
+            argv.rollback(may_arg)
         if res.flag == 'error':
             if optional:
                 return
             raise ParamsUnmatched(*res.error.args)
         result_dict[_kwarg[1]] = res._value  # type: ignore
         return
-    argv.pushback(may_arg)
-    raise ParamsUnmatched(lang.args.key_missing.format(target=may_arg, key=key))
+    argv.rollback(may_arg)
+    raise ParamsUnmatched(lang.require("args", "key_missing").format(target=may_arg, key=key))
 
 
 def _loop_kw(
     argv: Argv,
     _loop: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any
 ):
     result = {}
     for _ in range(_loop):
-        _m_arg, _m_str = argv.popitem(seps)
+        _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and _m_arg in argv.param_ids:
-            argv.pushback(_m_arg)
+            argv.rollback(_m_arg)
             break
         try:
             _handle_keyword(argv, value.base, _m_arg, seps, result, default, False)  # type: ignore
         except ParamsUnmatched:
             break
     if not result:
         if value.flag == '+':
@@ -92,25 +91,25 @@
     value: MultiVar,
     default: Any,
     args: Args
 ):
     kw = args[args.var_keyword].value.base if args.var_keyword else None
     result = []
     for _ in range(_loop):
-        _m_arg, _m_str = argv.popitem(seps)
+        _m_arg, _m_str = argv.next(seps)
         if not _m_arg:
             continue
         if _m_str and (
             _m_arg in argv.param_ids or
             (kw and re.match(fr'^([^{kw.sep}]+){kw.sep}(.*?)$', _m_arg))
         ):
-            argv.pushback(_m_arg)
+            argv.rollback(_m_arg)
             break
-        if (res := value.base(_m_arg)).flag != 'valid':
-            argv.pushback(_m_arg)
+        if (res := value.base.exec(_m_arg)).flag != 'valid':
+            argv.rollback(_m_arg)
             break
         result.append(res._value)  # type: ignore
     if not result:
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return tuple(result)
@@ -156,50 +155,48 @@
     """
     result: dict[str, Any] = {}
     for arg in args.argument:
         argv.context = arg
         key = arg.name
         value = arg.value
         default_val = arg.field.default_gen
-        optional = arg.optional
-        seps = arg.separators
-        may_arg, _str = argv.popitem(seps)
+        may_arg, _str = argv.next(arg.separators)
         if _str and may_arg in argv.special:
             raise SpecialOptionTriggered(argv.special[may_arg])
         if not may_arg or (_str and may_arg in argv.param_ids):
-            argv.pushback(may_arg)
+            argv.rollback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
             elif value.__class__ is MultiVar and value.flag == '*':
                 result[key] = ()
-            elif not optional:
-                raise ArgumentMissing(lang.args.missing.format(key=key))
+            elif not arg.optional:
+                raise ArgumentMissing(lang.require("args", "missing").format(key=key))
             continue
         if value.__class__ is MultiVar:
-            argv.pushback(may_arg)
+            argv.rollback(may_arg)
             multi_arg_handler(argv, args, arg, result)  # type: ignore
         elif value.__class__ is KeyWordVar:
             _handle_keyword(
-                argv, value, may_arg, seps, result, default_val, optional, key, argv.fuzzy_match  # type: ignore
+                argv, value, may_arg, arg.separators, result, default_val, arg.optional, key, argv.fuzzy_match  # type: ignore
             )
         elif value is AllParam:
-            argv.pushback(may_arg)
-            result[key] = argv.release(seps)
+            argv.rollback(may_arg)
+            result[key] = argv.converter(argv.release(arg.separators))
             argv.current_index = argv.ndata
             return result
         else:
             res = (
                 value.invalidate(may_arg, default_val)
                 if value.anti
                 else value.validate(may_arg, default_val)
             )
             if res.flag != 'valid':
-                argv.pushback(may_arg)
+                argv.rollback(may_arg)
             if res.flag == 'error':
-                if optional:
+                if arg.optional:
                     continue
                 raise ParamsUnmatched(*res.error.args)
             if not arg.anonymous:
                 result[key] = res._value  # type: ignore
     if args.var_keyword:
         kwargs = result[args.var_keyword]
         if not isinstance(kwargs, dict):
@@ -225,63 +222,72 @@
             for _o in _p:
                 _may_param, _ = split_once(text, _o.separators)
                 if _may_param in _o.aliases or any(map(_may_param.startswith, _o.aliases)):
                     analyser.compile_params.setdefault(text, res)
                     res.append(_o)
                     continue
                 if argv.fuzzy_match and levenshtein_norm(_may_param, _o.name) >= config.fuzzy_threshold:
-                    raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_o.name))
+                    raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_o.name))
             if res:
                 return res
+        elif isinstance(_p, Option):
+            _may_param, _ = split_once(text, _p.separators)
+            if _may_param in _p.aliases or any(map(_may_param.startswith, _p.aliases)):
+                analyser.compile_params.setdefault(text, _p)
+                return _p
+            if argv.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.name))
         elif isinstance(_p, Sentence):
             if (_may_param := split_once(text, _p.separators)[0]) == _p.name:
                 analyser.compile_params.setdefault(text, _p)
                 return _p
             if argv.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.name))
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.name))
         else:
             _may_param, _ = split_once(text, _p.command.separators)
             if _may_param == _p.command.name or _may_param.startswith(_p.command.name):
                 analyser.compile_params.setdefault(text, _p)
                 return _p
             if argv.fuzzy_match and levenshtein_norm(_may_param, _p.command.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.command.name))
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(source=_may_param, target=_p.command.name))
 
 
 def analyse_option(analyser: SubAnalyser, argv: Argv, param: Option) -> tuple[str, OptionResult]:
     """
     分析 Option 部分
 
     Args:
         analyser: 使用的分析器
+        argv: 使用的分析器
         param: 目标Option
     """
     argv.context = param
     if param.requires and analyser.sentences != param.requires:
         raise ParamsUnmatched(f"{param.name}'s required is not '{' '.join(analyser.sentences)}'")
     analyser.sentences = []
     if param.is_compact:
-        name, _ = argv.popitem()
+        name, _ = argv.next()
         for al in param.aliases:
             if mat := re.fullmatch(f"{al}(?P<rest>.*?)", name):
-                argv.pushback(mat.groupdict()['rest'], replace=True)
+                argv.rollback(mat.groupdict()['rest'], replace=True)
                 break
         else:
             raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
     else:
-        name, _ = argv.popitem(param.separators)
+        name, _ = argv.next(param.separators)
         if name not in param.aliases:  # 先匹配选项名称
             raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
     name = param.dest
     if param.nargs == 0:
         return name, OptionResult()
     return name, OptionResult(None, analyse_args(argv, param.args))
 
 
-def analyse_param(analyser: SubAnalyser, argv: Argv, _text: Any, _str: bool):
+def analyse_param(analyser: SubAnalyser, argv: Argv, seps: tuple[str, ...] | None = None):
+    _text, _str = argv.next(seps, move=False)
     if _str and _text in argv.special:
         if _text in argv.completion_names:
             if argv.current_index < argv.ndata:
                 argv.bak_data = argv.bak_data[:argv.current_index+1]
             last = argv.bak_data[-1]
             argv.bak_data[-1] = last[:last.rfind(_text)]
         raise SpecialOptionTriggered(argv.special[_text])
@@ -289,52 +295,55 @@
         _param = None
     elif _text in analyser.compile_params:
         _param = analyser.compile_params[_text]
     else:
         _param = None if analyser.default_separate else analyse_unmatch_params(analyser, argv, _text)
     if not _param and not analyser.args_result:
         analyser.args_result = analyse_args(argv, analyser.self_args)
-    elif isinstance(_param, list):
+    elif _param.__class__ is Option:
+        opt_n, opt_v = analyse_option(analyser, argv, _param)
+        analyser.options_result[opt_n] = opt_v
+    elif _param.__class__ is list:
         for opt in _param:
             _data, _index = argv.data_set()
             try:
                 opt_n, opt_v = analyse_option(analyser, argv, opt)
                 analyser.options_result[opt_n] = opt_v
                 _data.clear()
                 break
             except Exception as e:
                 exc = e
                 argv.data_reset(_data, _index)
                 continue
         else:
             raise exc  # type: ignore  # noqa
-    elif isinstance(_param, Sentence):
-        analyser.sentences.append(argv.popitem()[0])
-    elif _param:
+    elif _param.__class__ is Sentence:
+        analyser.sentences.append(argv.next()[0])
+    elif _param is not None:
         _param.process(argv)
         analyser.subcommands_result.setdefault(_param.command.dest, _param.result())
     argv.context = None
 
 
 def analyse_header(header: Header, argv: Argv) -> HeadResult:
     content = header.content
     mapping = header.mapping
-    head_text, _str = argv.popitem()
-    if isinstance(content, TPattern) and _str and (mat := content.fullmatch(head_text)):
+    head_text, _str = argv.next()
+    if content.__class__ is TPattern and _str and (mat := content.fullmatch(head_text)):
         return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
-    elif isinstance(content, BasePattern) and (val := content(head_text, Empty)).success:
+    elif isinstance(content, BasePattern) and (val := content.exec(head_text, Empty)).success:
         return HeadResult(head_text, val.value, True, fixes=mapping)
 
-    may_command, _m_str = argv.popitem()
-    if isinstance(content, list) and _m_str:
+    may_command, _m_str = argv.next()
+    if content.__class__ is list and _m_str:
         for pair in content:
             if res := pair.match(head_text, may_command):
                 return HeadResult(*res, fixes=mapping)
-    if isinstance(content, Double) and (
-        res := content.match(head_text, may_command, _str, _m_str, argv.pushback)
+    if content.__class__ is Double and (
+        res := content.match(head_text, may_command, _str, _m_str, argv.rollback)
     ):
         return HeadResult(*res, fixes=mapping)
 
     if _str and argv.fuzzy_match:
         command, prefixes = header.origin
         headers_text = []
         if prefixes and prefixes != [""]:
@@ -342,19 +351,19 @@
         elif command:
             headers_text.append(str(command))
         if isinstance(content, (TPattern, BasePattern)):
             source = head_text
         else:
             source = head_text + argv.separators[0] + str(may_command)
         if source == command:
-            raise ParamsUnmatched(lang.header.error.format(target=head_text))
+            raise ParamsUnmatched(lang.require("header", "error").format(target=head_text))
         for ht in headers_text:
             if levenshtein_norm(source, ht) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(target=source, source=ht))
-    raise ParamsUnmatched(lang.header.error.format(target=head_text))
+                raise FuzzyMatchSuccess(lang.require("fuzzy", "matched").format(target=source, source=ht))
+    raise ParamsUnmatched(lang.require("header", "error").format(target=head_text))
 
 
 def handle_help(analyser: Analyser, argv: Argv):
     _help_param = [str(i) for i in argv.release(recover=True) if str(i) not in argv.special]
     output_manager.send(
         analyser.command.name,
         lambda: analyser.command.formatter.format_node(_help_param),
@@ -362,20 +371,20 @@
     return analyser.export(argv, True)
 
 
 _args = Args["delete;?", "delete"]["name", str]["command", str, "_"]
 
 
 def handle_shortcut(analyser: Analyser, argv: Argv):
-    argv.popitem()
+    argv.next()
     opt_v = analyse_args(argv, _args)
     try:
         msg = analyser.command.shortcut(
             opt_v["name"],
-            None if opt_v["command"] == "_" else {"command": analyser.converter(opt_v["command"])},
+            None if opt_v["command"] == "_" else {"command": argv.converter(opt_v["command"])},
             bool(opt_v.get("delete"))
         )
         output_manager.send(analyser.command.name, lambda: msg)
     except Exception as e:
         output_manager.send(analyser.command.name, lambda: str(e))
     return analyser.export(argv, True)
 
@@ -456,10 +465,10 @@
 
 def handle_completion(analyser: Analyser, argv: Argv, trigger: str | None = None):
     if res := prompt(analyser, argv, trigger):
         if comp_ctx.get(None):
             raise PauseTriggered(res)
         output_manager.send(
             analyser.command.name,
-            lambda: f"{lang.common.completion_node}\n* " + "\n* ".join([i.text for i in res]),
+            lambda: f"{lang.require('completion', 'node')}\n* " + "\n* ".join([i.text for i in res]),
         )
     return analyser.export(argv, True, 'NoneType: None\n')  # type: ignore
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/header.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import re
 from copy import deepcopy
-from dataclasses import dataclass, field
 from inspect import isclass
 from typing import Any, Callable
 
 from nepattern import BasePattern, UnionPattern, all_patterns, type_parser
 from nepattern.util import TPattern
 from tarina import Empty
 
@@ -35,41 +34,42 @@
                 mapping[res[0]] = pattern_map[res[1]]
                 parts[i] = f"(?P<{res[0]}>{pattern_map[res[1]].pattern})"
             else:
                 parts[i] = f"(?P<{res[0]}>{res[1]})"
     return "".join(parts), mapping
 
 
-@dataclass
 class Pair:
-    prefix: Any
-    pattern: TPattern
-    is_prefix_pat: bool = field(default=False, init=False)
+    __slots__ = ("prefix", "pattern", "is_prefix_pat")
 
-    def __post_init__(self):
+    def __init__(self, prefix: Any, pattern: TPattern):
+        self.prefix = prefix
+        self.pattern = pattern
         self.is_prefix_pat = isinstance(self.prefix, BasePattern)
 
     def match(self, prefix: Any, command: str):
         if mat := self.pattern.fullmatch(command):
             if self.is_prefix_pat and (val := self.prefix(prefix, Empty)).success:
                 return (prefix, command), (val.value, command), True, mat.groupdict()
             if (
                 not isclass(prefix)
                 and prefix == self.prefix
                 or type(prefix) == self.prefix
             ):
                 return (prefix, command), (prefix, command), True, mat.groupdict()
 
 
-@dataclass
 class Double:
-    elements: list[Any]
-    patterns: UnionPattern | None
-    prefix: TPattern | None
-    command: BasePattern | TPattern
+    __slots__ = ("elements", "patterns", "prefix", "command")
+
+    def __init__(self, es: list, pats: UnionPattern | None, prefix: TPattern | None, command: BasePattern | TPattern):
+        self.elements = es
+        self.patterns = pats
+        self.prefix = prefix
+        self.command = command
 
     def match(
         self,
         prefix: Any,
         command: Any,
         prefix_str: bool,
         command_str: bool,
@@ -80,15 +80,15 @@
                 pat = re.compile(self.prefix.pattern + self.command.pattern)
                 if mat := pat.fullmatch(prefix):
                     pushback_fn(command)
                     return prefix, prefix, True, mat.groupdict()
                 elif mat := pat.fullmatch(name := (prefix + command)):
                     return name, name, True, mat.groupdict()
             if (mat := self.prefix.fullmatch(prefix)) and (
-                _val := self.command(command, Empty)
+                _val := self.command.exec(command, Empty)
             ).success:
                 return (prefix, command), (prefix, _val.value), True, mat.groupdict()
         if self.patterns and (val := self.patterns.validate(prefix, Empty)).success:
             _po, _pr = prefix, val.value
         elif (
             self.elements
             and not isclass(prefix)
@@ -101,24 +101,31 @@
             isinstance(self.command, TPattern)
             and command_str
             and (mat := self.command.fullmatch(command))
         ):
             return (_po, command), (_pr, command), True, mat.groupdict()
         elif (
             isinstance(self.command, BasePattern)
-            and (_val := self.command(command, Empty)).success
+            and (_val := self.command.exec(command, Empty)).success
         ):
             return (_po, command), (_pr, _val.value), True
 
 
-@dataclass
 class Header:
-    origin: tuple[str | type | BasePattern, TPrefixes]
-    content: TPattern | BasePattern | list[Pair] | Double
-    mapping: dict[str, BasePattern] = field(default_factory=dict)
+    __slots__ = ("origin", "content", "mapping")
+
+    def __init__(
+        self,
+        origin: tuple[str | type | BasePattern, TPrefixes],
+        content: TPattern | BasePattern | list[Pair] | Double,
+        mapping: dict[str, BasePattern] | None = None,
+    ):
+        self.origin = origin
+        self.content = content
+        self.mapping = mapping or {}
 
     @classmethod
     def generate(
         cls,
         command: str | type | BasePattern,
         prefixes: TPrefixes,
     ):
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/en-US.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5960526315789473%*

 * *Differences: {"'analyser'": "{delete: ['filter_missing', 'handle_null_message', 'handle_unexpect_type']}",*

 * * "'argv'": "OrderedDict([('null_message', 'You income a message without text: {target}')])",*

 * * "'arparma'": 'OrderedDict([(\'ambiguous_name\', "Name called  {target} is ambiguous\\nplease add '*

 * *              'prefix \'options.\' or \'subcommands.\'")])',*

 * * "'common'": "{'name_empty': 'You cannot give a empty name', delete: ['fuzzy_matched', "*

 * *             "'completion_node']}",*

 * * "'completion'": "OrderedDict([('node', […]*

```diff
@@ -2,67 +2,77 @@
     "action": {
         "args_empty": "The type of {target} cannot set to {source}",
         "args_error": "The type of {target} is not same as {source} of '{key}' in Args",
         "args_not_same": "The target type of {target} is not {source}",
         "length_error": "The count of arguments of this action must same as the given Args"
     },
     "analyser": {
-        "filter_missing": "The subclass of class Analyser must define its filter_out",
-        "handle_null_message": "You income a message without text: {target}",
-        "handle_unexpect_type": "You income a message with invalid element: {target}",
         "param_missing": "You need more data to analyse!",
         "param_unmatched": "Unmatched params: {target}"
     },
     "args": {
         "duplicate_kwargs": "You cannot set multiple kwargs at the same Args",
         "duplicate_varargs": "You cannot set multiple varargs at the same Args",
         "exclude_mutable_args": "This flag cannot be set when the Args is mutable",
         "key_missing": "{target} missing its key. Do you forget to add '{key}='?",
         "key_not_found": "Arg {name} not exists",
         "missing": "param {key} is required",
         "name_empty": "Name of arg cannot be empty",
         "name_error": "Name of arg must be a string",
         "value_error": "Value of {target} cannot be empty"
     },
-    "arpamar": {
+    "argv": {
+        "null_message": "You income a message without text: {target}"
+    },
+    "arparma": {
         "ambiguous_name": "Name called  {target} is ambiguous\nplease add prefix 'options.' or 'subcommands.'"
     },
     "behavior": {
         "cooldown_matched": "Your action is too frequent",
         "exclude_matched": "{target} and {other} cannot be both matched"
     },
     "builtin": {
         "option_completion": "give a next input suggestion of current command",
         "option_help": "show the help information",
         "option_shortcut": "set a shortcut command"
     },
     "common": {
-        "completion_node": "suggest input follows:",
         "custom_type_error": "The custom parameter type {target} can't be a type.",
-        "fuzzy_matched": "{target} is not matched. Do you mean \"{source}\"?"
+        "name_empty": "You cannot give a empty name"
+    },
+    "completion": {
+        "node": "suggest input follows:"
     },
     "duplication": {
         "stub_type_error": "{value} is not a valid stub"
     },
+    "format": {
+        "example": "Example",
+        "notice": "Notice",
+        "options": "General Options",
+        "subcommands": "Commands",
+        "subcommands.opts": "Options in above command",
+        "subcommands.subs": "Commands in above command",
+        "usage": "Usage"
+    },
+    "fuzzy": {
+        "matched": "{target} is not matched. Do you mean \"{source}\"?"
+    },
     "header": {
         "error": "{target} dose not matched"
     },
     "manager": {
         "help_footer": "# Invoke '$command {help}' to see syntax",
         "help_header": "# Following commands are available:",
         "help_pages": "Page {current} of {total}",
         "incorrect_shortcut": "Shortcut {target} cannot be used",
         "target_command_error": "The target command of {shortcut} is not {target}",
         "undefined_command": "Command {target} is not defined",
         "undefined_shortcut": "Shortcut {target} is not defined"
     },
-    "node": {
-        "name_empty": "You cannot give a empty name",
-        "name_error": "There is an invalid character in the name"
-    },
     "shortcut": {
         "add_success": "Add shortcut: \"{shortcut}\" for {target} successfully",
         "delete_success": "Delete shortcut: \"{shortcut}\" for {target} successfully",
         "no_recent_command": "get recent message failed",
         "recent_command_error": "command {target} is not same as recent message's command {source}"
     },
     "stub": {
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/i18n/zh-CN.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5960526315789473%*

 * *Differences: {"'analyser'": "{delete: ['filter_missing', 'handle_null_message', 'handle_unexpect_type']}",*

 * * "'argv'": "OrderedDict([('null_message', '传入了一个无法获取文本的消息: {target}')])",*

 * * "'arparma'": 'OrderedDict([(\'ambiguous_name\', "名称 {target} 存在歧义\\n请添加前缀 \'options.\' 或 '*

 * *              '\'subcommands.\'")])',*

 * * "'common'": "{'name_empty': '名字不能为空', delete: ['fuzzy_matched', 'completion_node']}",*

 * * "'completion'": "OrderedDict([('node', '以下是建议的输入：')])",*

 * * "'format'": "OrderedDict([('notice', '注释'), ('usage', '用法'), ('exampl […]*

```diff
@@ -2,67 +2,77 @@
     "action": {
         "args_empty": "{target} \u7684\u7c7b\u578b\u4e0d\u80fd\u6307\u5b9a\u4e3a {source}",
         "args_error": "{target} \u7684\u7c7b\u578b \u4e0e Args \u4e2d '{key}' \u63a5\u53d7\u7684\u7c7b\u578b {source} \u4e0d\u4e00\u81f4",
         "args_not_same": "{target} \u6307\u5b9a\u7684\u6d88\u606f\u5143\u7d20\u7c7b\u578b\u4e0d\u662f {source}",
         "length_error": "\u8be5 action \u63a5\u53d7\u7684\u53c2\u6570\u4e2a\u6570\u5fc5\u987b\u4e0e Args \u91cc\u7684\u4e00\u81f4"
     },
     "analyser": {
-        "filter_missing": "Analyser \u7684\u5b50\u7c7b\u5fc5\u987b\u5b9e\u73b0 filter_out \u5c5e\u6027",
-        "handle_null_message": "\u4f20\u5165\u4e86\u4e00\u4e2a\u65e0\u6cd5\u83b7\u53d6\u6587\u672c\u7684\u6d88\u606f: {target}",
-        "handle_unexpect_type": "\u4f20\u5165\u7684\u6d88\u606f\u4e2d\u6709\u975e\u6cd5\u7c7b\u578b\u7684\u5143\u7d20 {target}",
         "param_missing": "\u4f60\u5e94\u5f53\u4f20\u5165\u66f4\u591a\u7684\u53c2\u6570\u6765\u5b8c\u6210\u89e3\u6790!",
         "param_unmatched": "\u53c2\u6570 {target} \u5339\u914d\u5931\u8d25"
     },
     "args": {
         "duplicate_kwargs": "\u4e0d\u80fd\u540c\u65f6\u8bbe\u7f6e\u591a\u4e2a\u952e\u503c\u5bf9\u53ef\u53d8\u53c2\u6570",
         "duplicate_varargs": "\u4e0d\u80fd\u540c\u65f6\u8bbe\u7f6e\u591a\u4e2a\u975e\u952e\u503c\u5bf9\u53ef\u53d8\u53c2\u6570",
         "exclude_mutable_args": "\u8be5\u9009\u9879\u4e0d\u80fd\u4e0e\u53ef\u53d8\u53c2\u6570\u540c\u65f6\u4f7f\u7528",
         "key_missing": "{target} \u7f3a\u5c11\u952e. \u4f60\u662f\u4e0d\u662f\u5fd8\u4e86\u5e26\u4e0a '{key}=' ?",
         "key_not_found": "\u53c2\u6570 {name} \u4e0d\u5b58\u5728",
         "missing": "\u53c2\u6570 {key} \u4e22\u5931",
         "name_empty": "\u8be5\u53c2\u6570\u7684\u6307\u793a\u540d\u4e0d\u80fd\u4e3a\u7a7a",
         "name_error": "\u53c2\u6570\u7684\u540d\u5b57\u53ea\u80fd\u662f\u5b57\u7b26\u4e32",
         "value_error": "{target} \u7684\u53c2\u6570\u503c\u4e0d\u80fd\u4e3aEmpty"
     },
-    "arpamar": {
+    "argv": {
+        "null_message": "\u4f20\u5165\u4e86\u4e00\u4e2a\u65e0\u6cd5\u83b7\u53d6\u6587\u672c\u7684\u6d88\u606f: {target}"
+    },
+    "arparma": {
         "ambiguous_name": "\u540d\u79f0 {target} \u5b58\u5728\u6b67\u4e49\n\u8bf7\u6dfb\u52a0\u524d\u7f00 'options.' \u6216 'subcommands.'"
     },
     "behavior": {
         "cooldown_matched": "\u64cd\u4f5c\u8fc7\u4e8e\u9891\u7e41",
         "exclude_matched": "{target} \u4e0e {other} \u4e0d\u80fd\u540c\u65f6\u5b58\u5728"
     },
     "builtin": {
         "option_completion": "\u8865\u5168\u5f53\u524d\u547d\u4ee4",
         "option_help": "\u663e\u793a\u5e2e\u52a9\u4fe1\u606f",
         "option_shortcut": "\u8bbe\u7f6e\u5feb\u6377\u547d\u4ee4"
     },
     "common": {
-        "completion_node": "\u4ee5\u4e0b\u662f\u5efa\u8bae\u7684\u8f93\u5165\uff1a",
         "custom_type_error": "\u81ea\u5b9a\u4e49\u53c2\u6570\u7c7b\u578b\u4f20\u5165\u7684\u4e0d\u662f\u7c7b\u578b\u800c\u662f {target}, \u8fd9\u662f\u6709\u610f\u800c\u4e3a\u4e4b\u7684\u5417?",
-        "fuzzy_matched": "\u65e0\u6cd5\u89e3\u6790 {target}\u3002\u60a8\u60f3\u8981\u8f93\u5165\u7684\u662f\u4e0d\u662f \"{source}\" ?"
+        "name_empty": "\u540d\u5b57\u4e0d\u80fd\u4e3a\u7a7a"
+    },
+    "completion": {
+        "node": "\u4ee5\u4e0b\u662f\u5efa\u8bae\u7684\u8f93\u5165\uff1a"
     },
     "duplication": {
         "stub_type_error": "{value} \u4e0d\u662f\u4e00\u4e2a\u5408\u6cd5\u7684 Stub \u5b50\u7c7b"
     },
+    "format": {
+        "example": "\u4f7f\u7528\u793a\u4f8b",
+        "notice": "\u6ce8\u91ca",
+        "options": "\u53ef\u7528\u7684\u9009\u9879\u6709",
+        "subcommands": "\u53ef\u7528\u7684\u5b50\u547d\u4ee4\u6709",
+        "subcommands.opts": "\u8be5\u5b50\u547d\u4ee4\u5185\u53ef\u7528\u7684\u9009\u9879\u6709",
+        "subcommands.subs": "\u8be5\u5b50\u547d\u4ee4\u5185\u53ef\u7528\u7684\u5b50\u547d\u4ee4\u6709",
+        "usage": "\u7528\u6cd5"
+    },
+    "fuzzy": {
+        "matched": "\u65e0\u6cd5\u89e3\u6790 {target}\u3002\u60a8\u60f3\u8981\u8f93\u5165\u7684\u662f\u4e0d\u662f \"{source}\" ?"
+    },
     "header": {
         "error": "\u547d\u4ee4\u5934\u90e8 {target} \u5339\u914d\u5931\u8d25"
     },
     "manager": {
         "help_footer": "# \u8f93\u5165'\u547d\u4ee4\u540d {help}' \u67e5\u770b\u7279\u5b9a\u547d\u4ee4\u7684\u8bed\u6cd5",
         "help_header": "# \u5f53\u524d\u53ef\u7528\u7684\u547d\u4ee4\u6709:",
         "help_pages": "\u7b2c {current}/{total} \u9875",
         "incorrect_shortcut": "\u5feb\u6377\u547d\u4ee4 {target} \u65e0\u6cd5\u4f7f\u7528",
         "target_command_error": "{shortcut} \u7684\u76ee\u6807\u547d\u4ee4 {target} \u9519\u8bef",
         "undefined_command": "\u547d\u4ee4 {target} \u4e0d\u5b58\u5728",
         "undefined_shortcut": "\u5feb\u6377\u547d\u4ee4 {target} \u4e0d\u5b58\u5728"
     },
-    "node": {
-        "name_empty": "\u8be5\u6307\u4ee4\u7684\u540d\u5b57\u4e0d\u80fd\u4e3a\u7a7a",
-        "name_error": "\u8be5\u6307\u4ee4\u7684\u540d\u5b57\u542b\u6709\u975e\u6cd5\u5b57\u7b26"
-    },
     "shortcut": {
         "add_success": "{target} \u7684\u5feb\u622a\u6307\u4ee4: \"{shortcut}\" \u6dfb\u52a0\u6210\u529f",
         "delete_success": "{target} \u7684\u5feb\u622a\u6307\u4ee4: \"{shortcut}\" \u5220\u9664\u6210\u529f",
         "recent_command_error": "\u5386\u53f2\u8bb0\u5f55\u5bf9\u5e94\u7684\u547d\u4ee4 {source} \u4e0e \u672c\u547d\u4ee4 {target} \u4e0d\u4e00\u81f4"
     },
     "stub": {
         "key_error": "\u4e0d\u652f\u6301 {target}"
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,31 @@
 import re
 import shelve
 import weakref
 from copy import copy
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload, Generic
 from typing_extensions import NotRequired
-from tarina import LRU
-from tarina.lang import lang
+from tarina import LRU, lang
 from weakref import WeakKeyDictionary, WeakValueDictionary
 
 from .argv import Argv
 from .arparma import Arparma
 from .config import Namespace, config
 from .exceptions import ExceedMaxCount
-from .typing import DataCollection, TDataCollection
+from .typing import DataCollection, TDC
 
 
 if TYPE_CHECKING:
     from .analyser import Analyser
     from .core import Alconna, CommandMeta
 
 
-    class ShortcutArgs(TypedDict, Generic[TDataCollection]):
-        command: NotRequired[TDataCollection]
+    class ShortcutArgs(TypedDict, Generic[TDC]):
+        command: NotRequired[TDC]
         args: NotRequired[list[Any]]
         fuzzy: NotRequired[bool]
 else:
     class ShortcutArgs(TypedDict):
         command: NotRequired[DataCollection[Any]]
         args: NotRequired[list[Any]]
         fuzzy: NotRequired[bool]
@@ -115,14 +114,15 @@
         if self.current_count >= self.max_count:
             raise ExceedMaxCount
         self.__argv.pop(command, None)
         self.__argv[command] = Argv(
             command.namespace_config,
             fuzzy_match=command.meta.fuzzy_match,
             to_text=command.namespace_config.to_text,
+            converter=command.namespace_config.converter,
             separators=command.separators,
             message_cache=command.namespace_config.enable_message_cache,
             filter_crlf=not command.meta.keep_crlf,
         )
         self.__analysers.pop(command, None)
         self.__analysers[command] = command.compile(None)
         namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
@@ -132,29 +132,29 @@
             _cmd.formatter.add(command)
             command.formatter = _cmd.formatter
         else:
             command.formatter.add(command)
             namespace[command.name] = command
             self.current_count += 1
 
-    def resolve(self, command: Alconna[TDataCollection]) -> Argv[TDataCollection]:
+    def resolve(self, command: Alconna[TDC]) -> Argv[TDC]:
         """获取命令解析器的参数解析器"""
         try:
             return self.__argv[command]
         except KeyError as e:
             namespace, name = self._command_part(command.path)
-            raise ValueError(lang.manager.undefined_command.format(target=f"{namespace}.{name}")) from e
+            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
 
-    def require(self, command: Alconna[TDataCollection]) -> Analyser[TDataCollection]:
+    def require(self, command: Alconna[TDC]) -> Analyser[TDC]:
         """获取命令解析器"""
         try:
             return self.__analysers[command]  # type: ignore
         except KeyError as e:
             namespace, name = self._command_part(command.path)
-            raise ValueError(lang.manager.undefined_command.format(target=f"{namespace}.{name}")) from e
+            raise ValueError(lang.require("manager", "undefined_command").format(target=f"{namespace}.{name}")) from e
 
     def requires(self, *paths: str) -> zip[tuple[Analyser, Argv]]:  # type: ignore
         return zip(
             [v for k, v in self.__analysers.items() if k.path in paths],
             [v for k, v in self.__argv.items() if k.path in paths],
         )
 
@@ -191,40 +191,40 @@
         if isinstance(source, dict):
             source['command'] = source.get('command', target.command or target.name)
             source.setdefault('fuzzy', True)
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         elif source.matched:
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         else:
-            raise ValueError(lang.manager.incorrect_shortcut.format(target=f"{key}"))
+            raise ValueError(lang.require("manager", "incorrect_shortcut").format(target=f"{key}"))
 
     @overload
     def find_shortcut(
-        self, target: Alconna[TDataCollection]
-    ) -> list[Union[Arparma[TDataCollection], ShortcutArgs[TDataCollection]]]:
+        self, target: Alconna[TDC]
+    ) -> list[Union[Arparma[TDC], ShortcutArgs[TDC]]]:
         ...
 
     @overload
     def find_shortcut(
-        self, target: Alconna[TDataCollection], query: str
-    ) -> tuple[Arparma[TDataCollection] | ShortcutArgs[TDataCollection], Match[str] | None]:
+        self, target: Alconna[TDC], query: str
+    ) -> tuple[Arparma[TDC] | ShortcutArgs[TDC], Match[str] | None]:
         ...
 
-    def find_shortcut(self, target: Alconna[TDataCollection], query: str | None = None):
+    def find_shortcut(self, target: Alconna[TDC], query: str | None = None):
         """查找快捷命令"""
         namespace, name = self._command_part(target.path)
         if query:
             try:
                 return self.__shortcuts[f"{namespace}.{name}::{query}"], None
             except KeyError as e:
                 for k in self.__shortcuts.keys():
                     if mat := re.match(k.split("::")[1], query):
                         return self.__shortcuts[k], mat
                 raise ValueError(
-                    lang.manager.target_command_error.format(target=f"{namespace}.{name}", shortcut=query)
+                    lang.require("manager", "target_command_error").format(target=f"{namespace}.{name}", shortcut=query)
                 ) from e
         return [self.__shortcuts[k] for k in self.__shortcuts.keys() if f"{namespace}.{name}" in k]
 
     def delete_shortcut(self, target: Alconna, key: str | None = None):
         """删除快捷命令"""
         for res in [self.find_shortcut(target, key)[0]] if key else self.find_shortcut(target):
             with contextlib.suppress(StopIteration):
@@ -243,15 +243,15 @@
             return list(self.__analysers.keys())
         if isinstance(namespace, Namespace):
             namespace = Namespace.name
         if namespace not in self.__commands:
             return []
         return list(self.__commands[namespace].values())
 
-    def broadcast(self, message: TDataCollection, namespace: str | Namespace = '') -> Arparma[TDataCollection] | None:
+    def broadcast(self, message: TDC, namespace: str | Namespace = '') -> Arparma[TDC] | None:
         """将一段命令广播给当前空间内的所有命令"""
         for cmd in self.get_commands(namespace):
             if (res := cmd.parse(message)) and res.matched:
                 return res
 
     def all_command_help(
         self,
@@ -271,17 +271,17 @@
             namespace: 指定的命名空间, 如果为None则选择所有命令
             header: 帮助信息的页眉
             pages: 帮助信息的页码
             footer: 帮助信息的页脚
             max_length: 单个页面展示的最大长度
             page: 当前页码
         """
-        pages = pages or lang.manager.help_pages
+        pages = pages or lang.require("manager", "help_pages")
         cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
-        header = header or lang.manager.help_header
+        header = header or lang.require("manager", "help_header")
         if max_length < 1:
             command_string = "\n".join(
                 f" {str(index).rjust(len(str(len(cmds))), '0')} {slot.name} : {slot.meta.description}"
                 for index, slot in enumerate(cmds)
             ) if show_index else "\n".join(
                 f" - {cmd.name} : {cmd.meta.description}"
                 for cmd in cmds
@@ -299,15 +299,15 @@
             ) if show_index else "\n".join(
                 f" - {cmd.name} : {cmd.meta.description}"
                 for cmd in cmds[(page - 1) * max_length: page * max_length]
             )
         help_names = set()
         for i in cmds:
             help_names.update(i.namespace_config.builtin_option_name['help'])
-        footer = footer or lang.manager.help_footer.format(help="|".join(help_names))
+        footer = footer or lang.require("manager", "help_footer").format(help="|".join(help_names))
         return f"{header}\n{command_string}\n{footer}"
 
     def all_command_raw_help(self, namespace: str | Namespace | None = None) -> dict[str, CommandMeta]:
         """获取所有命令的原始帮助信息"""
         cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
         return {cmd.path: copy(cmd.meta) for cmd in cmds}
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class DataCollection(Protocol[DataUnit]):
     """数据集合协议"""
     def __repr__(self) -> str: ...
     def __iter__(self) -> Iterator[DataUnit]: ...
     def __len__(self) -> int: ...
 
 
-TDataCollection = TypeVar("TDataCollection", bound=DataCollection[Any])
+TDC = TypeVar("TDC", bound=DataCollection[Any])
 
 
 class KeyWordVar(BasePattern):
     """对具名参数的包装"""
     base: BasePattern
 
     def __init__(self, value: BasePattern | Any, sep: str = '='):
@@ -53,22 +53,22 @@
             alias = f"({self.base}{flag})"
             self.flag = flag
             self.length = -1
         elif flag > 1:
             alias = f"({self.base}+)[:{flag}]"
             self.flag = "+"
             self.length = flag
-        else:
+        else:  # pragma: no cover
             alias = str(self.base)
             self.flag = "+"
             self.length = 1
         origin = Dict[str, self.base.origin] if isinstance(self.base, KeyWordVar) else Tuple[self.base.origin, ...]
         super().__init__(r"(.+?)", MatchMode.KEEP, origin, alias=alias)
 
     def __repr__(self):
         return self.alias
 
 
 Nargs = MultiVar
 Kw = _Kw()
 
-__all__ = ["DataCollection", "TDataCollection", "MultiVar", "Nargs", "Kw", "KeyWordVar", "TPrefixes"]
+__all__ = ["DataCollection", "TDC", "MultiVar", "Nargs", "Kw", "KeyWordVar", "TPrefixes"]
```

### Comparing `arclet-alconna-1.7.0rc3/src/arclet/alconna/util.py` & `arclet-alconna-1.7.0rc4/src/arclet/alconna/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import sys
 import dataclasses
 
 
 def dataclass(*args, **kwargs):
-    if sys.version_info < (3, 10):
+    if sys.version_info < (3, 10):  # pragma: no cover
         kwargs.pop('slots')
     return dataclasses.dataclass(*args, **kwargs)
 
 
 def levenshtein_norm(source: str, target: str) -> float:
     """编辑距离算法, 计算源字符串与目标字符串的相似度, 取值范围[0, 1], 值越大越相似"""
     l_s, l_t = len(source), len(target)
```

### Comparing `arclet-alconna-1.7.0rc3/PKG-INFO` & `arclet-alconna-1.7.0rc4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc3
+Version: 1.7.0rc4
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
-Provides-Extra: all
-Provides-Extra: cli
 Provides-Extra: full
-Provides-Extra: graia
 Project-URL: documentation, https://arcletproject.github.io/docs/alconna/tutorial
 Project-URL: repository, https://github.com/ArcletProject/Alconna
 Description-Content-Type: text/markdown
 
 ![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
 <div align="center"> 
 
@@ -81,23 +78,49 @@
 
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
-* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py) 
-* Simple and Flexible Constructor 
+* High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
 * Powerful Automatic Type Parse and Conversion
-* Support Synchronous and Asynchronous Actions
-* Customizable Help Text Formatter, Command Analyser, etc.
-* Customizable Language File, Support i18n
+* Customizable Help Text Formatter and Control of Command Analyser
+* i18n Support
 * Cache of input command for quick response of repeated command
 * Easy-to-use Construct and Usage of Command Shortcut
-* Various Features (FuzzyMatch, Command Completion, etc.)
+* Can bind callback function to execute after command parsing
+* Can create command completion session to implement multi-round continuous completion prompt
+* Various Features (FuzzyMatch, Output Capture, etc.)
+
+Example of Callback Executor:
+
+```python
+# callback.py
+from arclet.alconna import Alconna, Args
+
+alc = Alconna("test", Args["foo", int]["bar", str])
+
+@alc.bind()
+def callback(foo: int, bar: str):
+    print(f"foo: {foo}")
+    print(f"bar: {bar}")
+    print(bar * foo)
+    
+if __name__ == "__main__":
+    alc()
+```
+
+```shell
+$ python callback.py test 3 hello
+foo: 3
+bar: hello
+hellohellohello
+```
+
 
 Example of Type Conversion:
 
 ```python
 from arclet.alconna import Alconna, Args
 from pathlib import Path
 
@@ -113,38 +136,52 @@
 '''
 <class 'bytes'>
 <class 'bytes'>
 <class 'bytes'>
 '''
 ```
 
-Example of FuzzyMatch:
-
+Example of Command Shortcut:
 ```python
-from arclet.alconna import Alconna, CommandMeta, Arg
+# shortcut.py
+from arclet.alconna import Alconna, Args
 
-alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
-alc.parse("！test_fuzy foo bar")
+alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
+alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
 
-'''
-！test_fuzy not matched. Are you mean "!test_fuzzy"?
-'''
+if __name__ == "__main__":
+    alc()
 ```
 
-Example of Command Shortcut:
+```shell
+$ python shortcut.py eval print(\"hello world\")
+hello world
+$ python shortcut.py echo hello world!
+hello world!
+```
+
+Example of Command Completion:
 ```python
-from arclet.alconna import Alconna, Args
+# completion.py
+from arclet.alconna import Alconna, Args, Option
 
-alc = Alconna("eval", Args["content", str], action=lambda x: eval(x, {}, {}))
-alc.shortcut("echo", {"command": "eval print(\\'{*}\\')"})
-alc.parse("echo Hello World!")
+alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
 
-'''
-Hello World!
-'''
+if __name__ == "__main__":
+    alc.completion()
+```
+
+```shell
+$ python completion.py test ?
+next input maybe:
+> foo
+> int
+> -h
+> --help
+> fool
 ```
 
 Example of `typing` Support:
 ```python
 from typing import Annotated  # or typing_extensions.Annotated
 from arclet.alconna import Alconna, Args
 
@@ -154,32 +191,37 @@
 
 '''
 'foo': 2
 ParamsUnmatched: param 3 is incorrect
 '''
 ```
 
+Example of FuzzyMatch:
 
-Example of Command Completion:
 ```python
-from arclet.alconna import Alconna, Args, Option
+# fuzzy.py
+from arclet.alconna import Alconna, CommandMeta, Arg
 
-alc = Alconna("test", Args["bar", int]) + Option("foo") + Option("fool")
-alc.parse("test --comp")
+alc = Alconna('!test_fuzzy', Arg("foo", str), meta=CommandMeta(fuzzy_match=True))
+
+if __name__ == "__main__":
+    alc()
 
-'''
-next input maybe:
-> foo
-> int
-> -h
-> --help
-> fool
-'''
 ```
 
+```shell
+$ python fuzzy.py /test_fuzzy foo bar
+/test_fuzy not matched. Are you mean "!test_fuzzy"?
+```
+
+
+
+
+
+
 ## License
 
 Alconna is licensed under the [MIT License](LICENSE).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FArcletProject%2FAlconna.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FArcletProject%2FAlconna?ref=badge_large)
 
 ## Acknowledgement
```

