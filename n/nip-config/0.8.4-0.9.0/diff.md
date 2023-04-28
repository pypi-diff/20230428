# Comparing `tmp/nip-config-0.8.4.tar.gz` & `tmp/nip-config-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nip-config-0.8.4.tar", last modified: Wed Mar 29 19:49:00 2023, max compression
+gzip compressed data, was "nip-config-0.9.0.tar", last modified: Fri Apr 28 08:22:55 2023, max compression
```

## Comparing `nip-config-0.8.4.tar` & `nip-config-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 19:49:00.529356 nip-config-0.8.4/
--rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.8.4/LICENSE
--rw-rw-rw-   0        0        0      740 2023-03-29 19:49:00.529356 nip-config-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 19:49:00.510006 nip-config-0.8.4/nip/
--rw-rw-rw-   0        0        0      140 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/__init__.py
--rw-rw-rw-   0        0        0     6053 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/constructor.py
--rw-rw-rw-   0        0        0     3078 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/convertor.py
--rw-rw-rw-   0        0        0     1107 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/directives.py
--rw-rw-rw-   0        0        0      835 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/dumper.py
--rw-rw-rw-   0        0        0    19350 2023-03-29 19:48:35.000000 nip-config-0.8.4/nip/elements.py
--rw-rw-rw-   0        0        0     1672 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/iter_parser.py
--rw-rw-rw-   0        0        0     9016 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/main.py
--rw-rw-rw-   0        0        0     2532 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/non_seq_constructor.py
--rw-rw-rw-   0        0        0     1578 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/parser.py
--rw-rw-rw-   0        0        0     2562 2022-10-04 13:30:14.000000 nip-config-0.8.4/nip/stream.py
--rw-rw-rw-   0        0        0     7084 2023-03-29 19:48:35.000000 nip-config-0.8.4/nip/tokens.py
--rw-rw-rw-   0        0        0     1517 2023-03-29 17:47:22.000000 nip-config-0.8.4/nip/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 19:49:00.525295 nip-config-0.8.4/nip_config.egg-info/
--rw-rw-rw-   0        0        0      740 2023-03-29 19:49:00.000000 nip-config-0.8.4/nip_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-03-29 19:49:00.000000 nip-config-0.8.4/nip_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 19:49:00.000000 nip-config-0.8.4/nip_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-03-29 19:49:00.000000 nip-config-0.8.4/nip_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-29 19:49:00.000000 nip-config-0.8.4/nip_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.8.4/pyproject.toml
--rw-rw-rw-   0        0        0      841 2023-03-29 19:49:00.530866 nip-config-0.8.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 19:49:00.527618 nip-config-0.8.4/tests/
--rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.8.4/tests/test_multi.py
--rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.8.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.557201 nip-config-0.9.0/
+-rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-04-28 08:22:55.558469 nip-config-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.540770 nip-config-0.9.0/nip/
+-rw-rw-rw-   0        0        0      137 2023-04-28 07:36:18.000000 nip-config-0.9.0/nip/__init__.py
+-rw-rw-rw-   0        0        0     5869 2023-04-28 07:37:49.000000 nip-config-0.9.0/nip/constructor.py
+-rw-rw-rw-   0        0        0     3078 2023-04-28 08:21:33.000000 nip-config-0.9.0/nip/convertor.py
+-rw-rw-rw-   0        0        0     1581 2023-04-28 08:19:13.000000 nip-config-0.9.0/nip/directives.py
+-rw-rw-rw-   0        0        0      807 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/dumper.py
+-rw-rw-rw-   0        0        0    19040 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/elements.py
+-rw-rw-rw-   0        0        0     1632 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/iter_parser.py
+-rw-rw-rw-   0        0        0     8749 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/main.py
+-rw-rw-rw-   0        0        0     2453 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/non_seq_constructor.py
+-rw-rw-rw-   0        0        0     1603 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/parser.py
+-rw-rw-rw-   0        0        0     2478 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/stream.py
+-rw-rw-rw-   0        0        0     6848 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/tokens.py
+-rw-rw-rw-   0        0        0     1462 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.556112 nip-config-0.9.0/nip_config.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2023-04-28 08:22:55.559897 nip-config-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.557201 nip-config-0.9.0/tests/
+-rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.9.0/tests/test_multi.py
+-rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.9.0/tests/test_utils.py
```

### Comparing `nip-config-0.8.4/LICENSE` & `nip-config-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nip-config-0.8.4/PKG-INFO` & `nip-config-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.8.4
+Version: 0.9.0
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 NIP is a yaml-like config files parser for convenient python object construction and experiment holding.
 Short guide can be found here: https://github.com/spairet/nip/tree/main/doc
```

### Comparing `nip-config-0.8.4/README.md` & `nip-config-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nip-config-0.8.4/nip/convertor.py` & `nip-config-0.9.0/nip/convertor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.8.4/nip/elements.py` & `nip-config-0.9.0/nip/elements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,536 +1,540 @@
-"""Contains all the elements of nip config files"""
-from __future__ import annotations
-
-import logging
-
-import nip.constructor  # This import pattern because of cycle imports
-import nip.directives
-import nip.dumper
-import nip.non_seq_constructor as nsc
-import nip.parser
-import nip.stream
-import nip.tokens as tokens
-import nip.utils
-
-from abc import abstractmethod, ABC
-from typing import Any, Union, Tuple, Dict
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class Element(ABC):
-    """Base token for nip file"""
-    def __init__(self, name: str = '', value: Any = None):
-        self.name = name
-        self.value = value
-
-    @classmethod
-    @abstractmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Element, None]:
-        pass
-
-    def __str__(self):
-        return f"{self.__class__.__name__}('{self.name}', {self.value})"
-
-    def __getitem__(self, item):
-        return self.value[item]
-
-    def __setitem__(self, key, value):
-        self.value[key] = value
-
-    def to_python(self):
-        return self.value.to_python()
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        return self.value.construct(constructor)
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return self.value.dump(dumper)
-
-    def __eq__(self, other):
-        return self.name == other.name and self.value == other.value
-
-    def flatten(self, delimiter='.') -> Dict:
-        return nip.utils.flatten(self.to_python(), delimiter)
-
-
-class Document(Element):  # ToDo: add multi document support
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Document:
-        doc_name = cls._read_name(stream)
-        content = RightValue.read(stream, parser)
-        return Document(doc_name, content)
-
-    @classmethod
-    def _read_name(cls, stream: nip.stream.Stream):
-        read_tokens = stream.peek(tokens.Operator('---'), tokens.Name) or \
-                      stream.peek(tokens.Operator('---'))
-        if read_tokens is not None:
-            stream.step()
-            if len(read_tokens) == 2:
-                return read_tokens[1].value
-        return ''
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        string = "---"
-        if self.name:
-            string += " " + self.name + " "
-        return string + self.value.dump(dumper)
-
-
-class RightValue(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Element:
-        value = Directive.read(stream, parser) or \
-                LinkCreation.read(stream, parser) or \
-                Link.read(stream, parser) or \
-                Class.read(stream, parser) or \
-                Tag.read(stream, parser) or \
-                Iter.read(stream, parser) or \
-                Args.read(stream, parser) or \
-                FString.read(stream, parser) or \
-                Nothing.read(stream, parser) or \
-                InlinePython.read(stream, parser) or \
-                Value.read(stream, parser)
-
-        if value is None:
-            raise nip.parser.ParserError(stream, "Wrong right value")
-
-        return value
-
-
-class Value(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[None, Value]:
-        tokens_list = [
-            tokens.Number,
-            tokens.Bool,
-            tokens.String,
-            tokens.List,
-            tokens.TupleToken,
-            tokens.Dict
-        ]
-        for token in tokens_list:
-            read_tokens = stream.peek(token)
-            if read_tokens is not None:
-                stream.step()
-                return Value(read_tokens[0].name, read_tokens[0].value)
-
-        return None
-
-    def to_python(self):
-        return self.value
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        return self.value
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        if isinstance(self.value, str):
-            return f'"{self.value}"'
-        return str(self.value)
-
-    def __len__(self):
-        return len(self.value)
-
-
-class LinkCreation(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Element, None]:
-        read_tokens = stream.peek(tokens.Operator('&'), tokens.Name)
-        if read_tokens is None:
-            # if stream.peek(tokens.Operator('&')):  # mb: do it more certainly: peak operator
-            #     raise nip.parser.ParserError(      # mb: firstly and then choose class to read)
-            #         stream, "Found variable creation operator '&' but name is not specified")
-            return None
-
-        name = read_tokens[1].value
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-        if name in parser.links:
-            raise nip.parser.ParserError(stream, f"Redefining of link '{name}'")
-        parser.links.append(name)
-
-        return LinkCreation(name, value)
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        constructor.vars[self.name] = self.value.construct(constructor)
-        return constructor.vars[self.name]
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"&{self.name} {self.value.dump(dumper)}"
-
-
-class Link(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Element, None]:
-        read_tokens = stream.peek(tokens.Operator('*'), tokens.Name)
-        if read_tokens is None:
-            return None
-
-        name = read_tokens[1].value
-        if parser.sequential_links and name not in parser.links:
-            nip.parser.ParserError(stream, "Link usage before assignment")
-        stream.step()
-
-        return Link(name)
-
-    def to_python(self):
-        return "nil"  # something that means that object is not constructed yet.
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        return constructor.vars[self.name]
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"*{self.name}"
-
-
-class Tag(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Tag, None]:
-        read_tokens = stream.peek(tokens.Operator('!'), tokens.Name)
-        if read_tokens is None:
-            return None
-        name = read_tokens[1].value
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-
-        return Tag(name, value)
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        if isinstance(self.value, Args):
-            args, kwargs = self.value.construct(constructor, always_pair=True)
-        else:
-            value = self.value.construct(constructor)
-            if isinstance(value,  Nothing):  # mb: Add IS_NOTHING method
-                return constructor.builders[self.name]()
-            else:
-                args, kwargs = [value], {}
-
-        if self.name not in constructor.builders:
-            raise nip.constructor.ConstructorError(
-                self, args, kwargs, f"Constructor for Tag '{self.name}' is not registered.")
-
-        messages = nip.constructor.check_typing(constructor.builders[self.name], args, kwargs)
-        if len(messages) > 0:
-            if constructor.strict_typing:
-                raise nip.constructor.ConstructorError(self, args, kwargs, "\n".join(messages))
-            else:
-                _LOGGER.warning(f"Typing mismatch while constructing {self.name}:\n" +
-                                "\n".join(messages))
-
-        try:  # Try to construct
-            return constructor.builders[self.name](*args, **kwargs)
-        except Exception as e:
-            raise nip.constructor.ConstructorError(self, args, kwargs, e)
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"!{self.name} " + self.value.dump(dumper)
-
-
-class Class(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Class, None]:
-        read_tokens = stream.peek(tokens.Operator('!&'), tokens.Name)
-        if read_tokens is None:
-            return None
-        name = read_tokens[1].value
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-        if not isinstance(value, Nothing):
-            raise nip.parser.ParserError(stream, "Class should be created with nothing to the right.")
-
-        return Class(name, value)
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        value = self.value.construct(constructor)
-        assert isinstance(value, Nothing), "Unexpected right value while constructing Class"
-
-        return constructor.builders[self.name]
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"!&{self.name} " + self.value.dump(dumper)
-
-
-class Args(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Args, None]:
-        start_indent = stream.pos
-        if start_indent <= parser.last_indent:
-            return None
-
-        args = []
-        kwargs = {}  # mb: just dict with integer and string keys
-        read_kwarg = False
-        while stream and stream.pos == start_indent:
-            parser.last_indent = start_indent
-
-            item = cls._read_list_item(stream, parser)
-            if item is not None:
-                if parser.strict and read_kwarg:
-                    raise nip.parser.ParserError(stream,
-                                                 "Positional argument after keyword argument "
-                                                 "is forbiddent in `strict` mode.")
-                args.append(item)
-                continue
-
-            key, value = cls._read_dict_pair(stream, parser, kwargs.keys())
-            if key is not None:
-                read_kwarg = True
-                kwargs[key] = value
-                continue
-
-            break
-
-        if stream.pos > start_indent:
-            raise nip.parser.ParserError(stream, "Unexpected indent")
-
-        if not args and not kwargs:
-            return None
-        return Args("args", (args, kwargs))
-
-    @classmethod
-    def _read_list_item(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) \
-            -> Union[Element, None]:
-        read_tokens = stream.peek(tokens.Operator('- '))
-        if read_tokens is None:
-            return None
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-
-        return value
-
-    @classmethod
-    def _read_dict_pair(cls, stream: nip.stream.Stream, parser: nip.parser.Parser, kwargs_keys) \
-            -> Union[Tuple[str, Element], Tuple[None, None]]:
-        # mb: read String instead of Name for keys with spaces,
-        # mb: but this leads to the case that
-        read_tokens = stream.peek(tokens.Name, tokens.Operator(': '))
-        if read_tokens is None:
-            return None, None
-
-        key = read_tokens[0].value
-        if parser.strict and key in kwargs_keys:
-            raise nip.parser.ParserError(stream,
-                                         f"Dict key overwriting is forbidden in `strict` "
-                                         f"mode. Overwritten key: '{key}'.")
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-
-        return key, value
-
-    def __str__(self):
-        args_repr = "[" + ", ".join([str(item) for item in self.value[0]]) + "]"
-        kwargs_repr = \
-            "{" + ", ".join([f"{key}: {str(value)}" for key, value in self.value[1].items()]) + "}"
-
-        return f"{self.__class__.__name__}('{self.name}', {args_repr}, {kwargs_repr})"
-
-    def __bool__(self):
-        return bool(self.value[0]) or bool(self.value[1])
-
-    def __getitem__(self, item):
-        try:
-            return self.value[0][item]
-        except TypeError:
-            return self.value[1][item]
-
-    def __setitem__(self, key, value):
-        if isinstance(key, int):
-            self.value[0][key] = nip.convert(value)
-        else:
-            self.value[1][key] = nip.convert(value)
-
-    def append(self, value):
-        self.value[0].append(nip.convert(value))
-
-    def __len__(self):
-        return len(self.value[0]) + len(self.value[1])
-
-    def __iter__(self):
-        for item in self.value[0]:
-            yield item
-        for key, item in self.value[1].items():
-            yield item
-
-    def to_python(self):
-        args = list(item.to_python() for item in self.value[0])
-        kwargs = {key: value.to_python() for key, value in self.value[1].items()}
-        assert args or kwargs, "Error converting Args node to python"  # This should never happen
-        if args and kwargs:
-            result = {}
-            result.update(nip.utils.iterate_items(args))
-            result.update(nip.utils.iterate_items(kwargs))
-            return result
-        return args or kwargs
-
-    def construct(self, constructor: nip.constructor.Constructor, always_pair=False):
-        args = list(item.construct(constructor) for item in self.value[0])
-        kwargs = {key: value.construct(constructor) for key, value in self.value[1].items()}
-        assert args or kwargs, "Error converting Args node to python"  # This should never happen
-        if args and kwargs or always_pair:
-            return args, kwargs
-        return args or kwargs
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        dumped_args = '\n'.join([
-            " "*dumper.indent + f"- {item.dump(dumper + dumper.default_shift)}"
-            for item in self.value[0]
-        ])
-        string = ('\n' if dumped_args else '') + dumped_args
-
-        dumped_kwargs = '\n'.join([
-            " "*dumper.indent + f"{key}: {value.dump(dumper + dumper.default_shift)}"
-            for key, value in self.value[1].items()
-        ])
-        string += ('\n' if dumped_kwargs else '') + dumped_kwargs
-
-        return string
-
-
-class Iter(Element):
-    def __init__(self, name: str = '', value: Any = None):
-        super(Iter, self).__init__(name, value)
-        self.return_index = -1
-        # mb: name all the iterators and get the value from constructor rather then use this index
-
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Iter, None]:
-        read_tokens = stream.peek(tokens.Operator('@'), tokens.Name) or \
-                      stream.peek(tokens.Operator('@'))
-        if read_tokens is None:
-            return None
-        stream.step()
-        value = RightValue.read(stream, parser)
-        if isinstance(value, Value) and isinstance(value.value, list):
-            value = value.value
-        elif isinstance(value, Args) and len(value.value[1]) == 0:
-            value = value
-        else:
-            raise nip.parser.ParserError(stream, "List is expected as a value for Iterable node")
-        if len(read_tokens) == 1:
-            iterator = Iter('', value)
-        else:
-            iterator = Iter(read_tokens[1].value, value)
-
-        parser.iterators.append(iterator)
-        return iterator
-
-    def to_python(self):
-        if self.return_index == -1:
-            raise iter(self.value)
-        if isinstance(self.value[self.return_index], Element):
-            return self.value[self.return_index].to_python()
-        return self.value[self.return_index]
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        if self.return_index == -1:
-            raise Exception("Iterator index was not specified by IterParser")
-        if isinstance(self.value, list):
-            return self.value[self.return_index]
-        elif isinstance(self.value, Args):
-            return self.value[self.return_index].construct(constructor)
-        else:
-            raise nip.constructor.ConstructorError(self, (), {}, "Unexpected iter value type")
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        if self.return_index == -1:
-            raise nip.dumper.DumpError(
-                "Dumping an iterator but index was not specified by IterParser"
-            )
-        if isinstance(self.value, list):
-            return str(self.value[self.return_index])
-        elif isinstance(self.value, Args):
-            return self.value[self.return_index].dump(dumper)
-        else:
-            raise nip.dumper.DumpError("Unable to dump Iterable node: unexpected value type")
-
-
-class InlinePython(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> \
-            Union[InlinePython, None]:
-        read_tokens = stream.peek(tokens.InlinePython)
-        if read_tokens is None:
-            return None
-        stream.step()
-        exec_string = read_tokens[0].value
-        return InlinePython(value=exec_string)
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        nsc.preload_vars(self.value, constructor)
-        locals().update(constructor.vars)
-        return eval(self.value)
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"`{self.value}`"
-
-    def to_python(self):
-        return f"`{self.value}`"
-
-
-class Nothing(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> Union[Nothing, None]:
-        if not stream:
-            return Nothing()
-
-        indent = stream.pos
-        if stream.pos == 0 or (
-                stream.lines[stream.n][:stream.pos].isspace()
-                and indent <= parser.last_indent):
-            return Nothing()
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        return self
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return ""
-
-    def to_python(self):
-        return None
-
-
-class FString(Element):  # Includes f-string and r-string
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> \
-            Union[FString, None]:
-        read_tokens = stream.peek(tokens.PythonString)
-        if read_tokens is None:
-            return None
-        stream.step()
-        string, t = read_tokens[0].value
-        if t == 'r':
-            print("Warning: all strings in NIP are already python r-string. "
-                  "You don't have to explicitly specify it.")
-        return FString(value=string)
-
-    def construct(self, constructor: nip.constructor.Constructor):
-        nsc.preload_vars(f"f{self.value}", constructor)
-        locals().update(constructor.vars)
-        return eval(f"f{self.value}")
-
-    def dump(self, dumper: nip.dumper.Dumper):
-        return f"f{self.value}"
-
-    def to_python(self):
-        return f"f{self.value}"
-
-
-class Directive(Element):
-    @classmethod
-    def read(cls, stream: nip.stream.Stream, parser: nip.parser.Parser) -> \
-            Union[FString, None]:
-        read_tokens = stream.peek(tokens.Operator('!!'), tokens.Name)
-        if read_tokens is None:
-            return None
-        name = read_tokens[1].value
-        stream.step()
-
-        value = RightValue.read(stream, parser)
-
-        return nip.directives.call_directive(name, value, stream)
+"""Contains all the elements of nip config files"""
+# from __future__ import annotations
+
+import logging
+
+import nip.constructor  # This import pattern because of cycle imports
+import nip.directives
+import nip.dumper
+import nip.non_seq_constructor as nsc
+import nip.parser
+import nip.stream
+import nip.tokens as tokens
+import nip.utils
+
+from abc import abstractmethod, ABC
+from typing import Any, Union, Tuple, Dict
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class Element(ABC):
+    """Base token for nip file"""
+    def __init__(self, name: str = '', value: Any = None):
+        self.name = name
+        self.value = value
+
+    @classmethod
+    @abstractmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Element", None]:
+        pass
+
+    def __str__(self):
+        return f"{self.__class__.__name__}('{self.name}', {self.value})"
+
+    def __getitem__(self, item):
+        return self.value[item]
+
+    def __setitem__(self, key, value):
+        self.value[key] = value
+
+    def to_python(self):
+        return self.value.to_python()
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        return self.value.construct(constructor)
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return self.value.dump(dumper)
+
+    def __eq__(self, other):
+        return self.name == other.name and self.value == other.value
+
+    def flatten(self, delimiter='.') -> Dict:
+        return nip.utils.flatten(self.to_python(), delimiter)
+
+
+class Document(Element):  # ToDo: add multi document support
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> "Document":
+        doc_name = cls._read_name(stream)
+        content = RightValue.read(stream, parser)
+        return Document(doc_name, content)
+
+    @classmethod
+    def _read_name(cls, stream: "nip.stream.Stream"):
+        read_tokens = stream.peek(tokens.Operator('---'), tokens.Name) or \
+                      stream.peek(tokens.Operator('---'))
+        if read_tokens is not None:
+            stream.step()
+            if len(read_tokens) == 2:
+                return read_tokens[1].value
+        return ''
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        string = "---"
+        if self.name:
+            string += " " + self.name + " "
+        return string + self.value.dump(dumper)
+
+
+class RightValue(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Element:
+        value = Directive.read(stream, parser) or \
+                LinkCreation.read(stream, parser) or \
+                Link.read(stream, parser) or \
+                Class.read(stream, parser) or \
+                Tag.read(stream, parser) or \
+                Iter.read(stream, parser) or \
+                Args.read(stream, parser) or \
+                FString.read(stream, parser) or \
+                Nothing.read(stream, parser) or \
+                InlinePython.read(stream, parser) or \
+                Value.read(stream, parser)
+
+        if value is None:
+            raise nip.parser.ParserError(stream, "Wrong right value")
+
+        return value
+
+
+class Value(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[None, "Value"]:
+        tokens_list = [
+            tokens.Number,
+            tokens.Bool,
+            tokens.String,
+            tokens.List,
+            tokens.TupleToken,
+            tokens.Dict
+        ]
+        for token in tokens_list:
+            read_tokens = stream.peek(token)
+            if read_tokens is not None:
+                stream.step()
+                return Value(read_tokens[0].name, read_tokens[0].value)
+
+        return None
+
+    def to_python(self):
+        return self.value
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        return self.value
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        if isinstance(self.value, str):
+            return f'"{self.value}"'
+        return str(self.value)
+
+    def __len__(self):
+        return len(self.value)
+
+
+class LinkCreation(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[Element, None]:
+        read_tokens = stream.peek(tokens.Operator('&'), tokens.Name)
+        if read_tokens is None:
+            # if stream.peek(tokens.Operator('&')):  # mb: do it more certainly: peak operator
+            #     raise "nip.parser.Parser"Error(      # mb: firstly and then choose class to read)
+            #         stream, "Found variable creation operator '&' but name is not specified")
+            return None
+
+        name = read_tokens[1].value
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+        if name in parser.link_names:
+            raise nip.parser.ParserError(stream, f"Redefining of link '{name}'")
+        parser.link_names.append(name)
+
+        return LinkCreation(name, value)
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        constructor.vars[self.name] = self.value.construct(constructor)
+        return constructor.vars[self.name]
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"&{self.name} {self.value.dump(dumper)}"
+
+
+class Link(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union[Element, None]:
+        read_tokens = stream.peek(tokens.Operator('*'), tokens.Name)
+        if read_tokens is None:
+            return None
+
+        name = read_tokens[1].value
+        stream.step()
+
+        if name in parser.link_replacements:
+            return parser.link_replacements[name]
+
+        if parser.sequential_links and name not in parser.link_names:
+            nip.parser.ParserError(stream, "Link usage before assignment")
+
+        return Link(name)
+
+    def to_python(self):
+        return "nil"  # something that means that object is not constructed yet.
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        return constructor.vars[self.name]
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"*{self.name}"
+
+
+class Tag(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Tag", None]:
+        read_tokens = stream.peek(tokens.Operator('!'), tokens.Name)
+        if read_tokens is None:
+            return None
+        name = read_tokens[1].value
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+
+        return Tag(name, value)
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        if isinstance(self.value, Args):
+            args, kwargs = self.value.construct(constructor, always_pair=True)
+        else:
+            value = self.value.construct(constructor)
+            if isinstance(value,  Nothing):  # mb: Add IS_NOTHING method
+                return constructor.builders[self.name]()
+            else:
+                args, kwargs = [value], {}
+
+        if self.name not in constructor.builders:
+            raise nip.constructor.ConstructorError(
+                self, args, kwargs, f"Constructor for Tag '{self.name}' is not registered.")
+
+        messages = nip.constructor.check_typing(constructor.builders[self.name], args, kwargs)
+        if len(messages) > 0:
+            if constructor.strict_typing:
+                raise nip.constructor.ConstructorError(self, args, kwargs, "\n".join(messages))
+            else:
+                _LOGGER.warning(f"Typing mismatch while constructing {self.name}:\n" +
+                                "\n".join(messages))
+
+        try:  # Try to construct
+            return constructor.builders[self.name](*args, **kwargs)
+        except Exception as e:
+            raise nip.constructor.ConstructorError(self, args, kwargs, e)
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"!{self.name} " + self.value.dump(dumper)
+
+
+class Class(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Class", None]:
+        read_tokens = stream.peek(tokens.Operator('!&'), tokens.Name)
+        if read_tokens is None:
+            return None
+        name = read_tokens[1].value
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+        if not isinstance(value, Nothing):
+            raise nip.parser.ParserError(stream, "Class should be created with nothing to the right.")
+
+        return Class(name, value)
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        value = self.value.construct(constructor)
+        assert isinstance(value, Nothing), "Unexpected right value while constructing Class"
+
+        return constructor.builders[self.name]
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"!&{self.name} " + self.value.dump(dumper)
+
+
+class Args(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Args", None]:
+        start_indent = stream.pos
+        if start_indent <= parser.last_indent:
+            return None
+
+        args = []
+        kwargs = {}  # mb: just dict with integer and string keys
+        read_kwarg = False
+        while stream and stream.pos == start_indent:
+            parser.last_indent = start_indent
+
+            item = cls._read_list_item(stream, parser)
+            if item is not None:
+                if parser.strict and read_kwarg:
+                    raise nip.parser.ParserError(stream,
+                                                 "Positional argument after keyword argument "
+                                                 "is forbiddent in `strict` mode.")
+                args.append(item)
+                continue
+
+            key, value = cls._read_dict_pair(stream, parser, kwargs.keys())
+            if key is not None:
+                read_kwarg = True
+                kwargs[key] = value
+                continue
+
+            break
+
+        if stream.pos > start_indent:
+            raise nip.parser.ParserError(stream, "Unexpected indent")
+
+        if not args and not kwargs:
+            return None
+        return Args("args", (args, kwargs))
+
+    @classmethod
+    def _read_list_item(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") \
+            -> Union[Element, None]:
+        read_tokens = stream.peek(tokens.Operator('- '))
+        if read_tokens is None:
+            return None
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+
+        return value
+
+    @classmethod
+    def _read_dict_pair(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser", kwargs_keys) \
+            -> Union[Tuple[str, Element], Tuple[None, None]]:
+        # mb: read String instead of Name for keys with spaces,
+        # mb: but this leads to the case that
+        read_tokens = stream.peek(tokens.Name, tokens.Operator(': '))
+        if read_tokens is None:
+            return None, None
+
+        key = read_tokens[0].value
+        if parser.strict and key in kwargs_keys:
+            raise nip.parser.ParserError(stream,
+                                         f"Dict key overwriting is forbidden in `strict` "
+                                         f"mode. Overwritten key: '{key}'.")
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+
+        return key, value
+
+    def __str__(self):
+        args_repr = "[" + ", ".join([str(item) for item in self.value[0]]) + "]"
+        kwargs_repr = \
+            "{" + ", ".join([f"{key}: {str(value)}" for key, value in self.value[1].items()]) + "}"
+
+        return f"{self.__class__.__name__}('{self.name}', {args_repr}, {kwargs_repr})"
+
+    def __bool__(self):
+        return bool(self.value[0]) or bool(self.value[1])
+
+    def __getitem__(self, item):
+        try:
+            return self.value[0][item]
+        except TypeError:
+            return self.value[1][item]
+
+    def __setitem__(self, key, value):
+        if isinstance(key, int):
+            self.value[0][key] = nip.convert(value)
+        else:
+            self.value[1][key] = nip.convert(value)
+
+    def append(self, value):
+        self.value[0].append(nip.convert(value))
+
+    def __len__(self):
+        return len(self.value[0]) + len(self.value[1])
+
+    def __iter__(self):
+        for item in self.value[0]:
+            yield item
+        for key, item in self.value[1].items():
+            yield item
+
+    def to_python(self):
+        args = list(item.to_python() for item in self.value[0])
+        kwargs = {key: value.to_python() for key, value in self.value[1].items()}
+        assert args or kwargs, "Error converting Args node to python"  # This should never happen
+        if args and kwargs:
+            result = {}
+            result.update(nip.utils.iterate_items(args))
+            result.update(nip.utils.iterate_items(kwargs))
+            return result
+        return args or kwargs
+
+    def construct(self, constructor: "nip.constructor.Constructor", always_pair=False):
+        args = list(item.construct(constructor) for item in self.value[0])
+        kwargs = {key: value.construct(constructor) for key, value in self.value[1].items()}
+        assert args or kwargs, "Error converting Args node to python"  # This should never happen
+        if args and kwargs or always_pair:
+            return args, kwargs
+        return args or kwargs
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        dumped_args = '\n'.join([
+            " "*dumper.indent + f"- {item.dump(dumper + dumper.default_shift)}"
+            for item in self.value[0]
+        ])
+        string = ('\n' if dumped_args else '') + dumped_args
+
+        dumped_kwargs = '\n'.join([
+            " "*dumper.indent + f"{key}: {value.dump(dumper + dumper.default_shift)}"
+            for key, value in self.value[1].items()
+        ])
+        string += ('\n' if dumped_kwargs else '') + dumped_kwargs
+
+        return string
+
+
+class Iter(Element):
+    def __init__(self, name: str = '', value: Any = None):
+        super(Iter, self).__init__(name, value)
+        self.return_index = -1
+        # mb: name all the iterators and get the value from constructor rather then use this index
+
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Iter", None]:
+        read_tokens = stream.peek(tokens.Operator('@'), tokens.Name) or \
+                      stream.peek(tokens.Operator('@'))
+        if read_tokens is None:
+            return None
+        stream.step()
+        value = RightValue.read(stream, parser)
+        if isinstance(value, Value) and isinstance(value.value, list):
+            value = value.value
+        elif isinstance(value, Args) and len(value.value[1]) == 0:
+            value = value
+        else:
+            raise nip.parser.ParserError(stream, "List is expected as a value for Iterable node")
+        if len(read_tokens) == 1:
+            iterator = Iter('', value)
+        else:
+            iterator = Iter(read_tokens[1].value, value)
+
+        parser.iterators.append(iterator)
+        return iterator
+
+    def to_python(self):
+        if self.return_index == -1:
+            raise iter(self.value)
+        if isinstance(self.value[self.return_index], Element):
+            return self.value[self.return_index].to_python()
+        return self.value[self.return_index]
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        if self.return_index == -1:
+            raise Exception("Iterator index was not specified by IterParser")
+        if isinstance(self.value, list):
+            return self.value[self.return_index]
+        elif isinstance(self.value, Args):
+            return self.value[self.return_index].construct(constructor)
+        else:
+            raise nip.constructor.ConstructorError(self, (), {}, "Unexpected iter value type")
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        if self.return_index == -1:
+            raise nip.dumper.DumpError(
+                "Dumping an iterator but index was not specified by IterParser"
+            )
+        if isinstance(self.value, list):
+            return str(self.value[self.return_index])
+        elif isinstance(self.value, Args):
+            return self.value[self.return_index].dump(dumper)
+        else:
+            raise nip.dumper.DumpError("Unable to dump Iterable node: unexpected value type")
+
+
+class InlinePython(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+            Union["InlinePython", None]:
+        read_tokens = stream.peek(tokens.InlinePython)
+        if read_tokens is None:
+            return None
+        stream.step()
+        exec_string = read_tokens[0].value
+        return InlinePython(value=exec_string)
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        nsc.preload_vars(self.value, constructor)
+        locals().update(constructor.vars)
+        return eval(self.value)
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"`{self.value}`"
+
+    def to_python(self):
+        return f"`{self.value}`"
+
+
+class Nothing(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> Union["Nothing", None]:
+        if not stream:
+            return Nothing()
+
+        indent = stream.pos
+        if stream.pos == 0 or (
+                stream.lines[stream.n][:stream.pos].isspace()
+                and indent <= parser.last_indent):
+            return Nothing()
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        return self
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return ""
+
+    def to_python(self):
+        return None
+
+
+class FString(Element):  # Includes f-string and r-string
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+            Union["FString", None]:
+        read_tokens = stream.peek(tokens.PythonString)
+        if read_tokens is None:
+            return None
+        stream.step()
+        string, t = read_tokens[0].value
+        if t == 'r':
+            print("Warning: all strings in NIP are already python r-string. "
+                  "You don't have to explicitly specify it.")
+        return FString(value=string)
+
+    def construct(self, constructor: "nip.constructor.Constructor"):
+        nsc.preload_vars(f"f{self.value}", constructor)
+        locals().update(constructor.vars)
+        return eval(f"f{self.value}")
+
+    def dump(self, dumper: nip.dumper.Dumper):
+        return f"f{self.value}"
+
+    def to_python(self):
+        return f"f{self.value}"
+
+
+class Directive(Element):
+    @classmethod
+    def read(cls, stream: "nip.stream.Stream", parser: "nip.parser.Parser") -> \
+            Union["FString", None]:
+        read_tokens = stream.peek(tokens.Operator('!!'), tokens.Name)
+        if read_tokens is None:
+            return None
+        name = read_tokens[1].value
+        stream.step()
+
+        value = RightValue.read(stream, parser)
+
+        return nip.directives.call_directive(name, value, stream)
```

### Comparing `nip-config-0.8.4/nip/iter_parser.py` & `nip-config-0.9.0/nip/iter_parser.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from collections import defaultdict
-from itertools import product
-from typing import Iterable
-
-from .parser import Parser
-from .elements import Element
-
-
-class IterParser:  # mb: insert this functionality into Parser (save parsed tree in Parser)
-    def __init__(self, parser: Parser, element: Element = None):
-        self.iterators = parser.iterators
-        self.element = element
-
-    def iter_configs(self, element: Element) -> Iterable[Element]:
-        iter_groups = defaultdict(list)
-        for i, iterator in enumerate(self.iterators):
-            name = iterator.name if iterator.name else f'_{i}'
-            iter_groups[name].append(iterator)
-        for group_name, group in iter_groups.items():
-            iter_len = len(group[0].value)
-            for iterator in group:
-                if len(iterator.value) != iter_len:
-                    raise IterParserError(f"Iterators of group '{group_name}' have different lengths")
-
-        group_names = sorted(iter_groups.keys())
-        group_lengths = [len(iter_groups[name][0].value) for name in group_names]
-        index_sets = product(*(range(length) for length in group_lengths))
-
-        for indexes in index_sets:
-            for index, group_name in zip(indexes, group_names):
-                for iterator in iter_groups[group_name]:
-                    iterator.return_index = index
-            yield element
-
-    def __iter__(self):
-        if self.element is None:
-            raise IterParserError("config element to iterate through was not defined in __init__")
-        return self.iter_configs(self.element)
-
-
-class IterParserError(Exception):
-    pass
+from collections import defaultdict
+from itertools import product
+from typing import Iterable
+
+from .parser import Parser
+from .elements import Element
+
+
+class IterParser:  # mb: insert this functionality into Parser (save parsed tree in Parser)
+    def __init__(self, parser: Parser, element: Element = None):
+        self.iterators = parser.iterators
+        self.element = element
+
+    def iter_configs(self, element: Element) -> Iterable[Element]:
+        iter_groups = defaultdict(list)
+        for i, iterator in enumerate(self.iterators):
+            name = iterator.name if iterator.name else f'_{i}'
+            iter_groups[name].append(iterator)
+        for group_name, group in iter_groups.items():
+            iter_len = len(group[0].value)
+            for iterator in group:
+                if len(iterator.value) != iter_len:
+                    raise IterParserError(f"Iterators of group '{group_name}' have different lengths")
+
+        group_names = sorted(iter_groups.keys())
+        group_lengths = [len(iter_groups[name][0].value) for name in group_names]
+        index_sets = product(*(range(length) for length in group_lengths))
+
+        for indexes in index_sets:
+            for index, group_name in zip(indexes, group_names):
+                for iterator in iter_groups[group_name]:
+                    iterator.return_index = index
+            yield element
+
+    def __iter__(self):
+        if self.element is None:
+            raise IterParserError("config element to iterate through was not defined in __init__")
+        return self.iter_configs(self.element)
+
+
+class IterParserError(Exception):
+    pass
```

### Comparing `nip-config-0.8.4/nip/main.py` & `nip-config-0.9.0/nip/main.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-from typing import Union, Any, Iterable, Callable, Optional
-from pathlib import Path
-
-
-from .parser import Parser
-from .constructor import Constructor, ConstructorError
-from .non_seq_constructor import NonSequentialConstructor
-from .iter_parser import IterParser
-from .dumper import Dumper
-from .convertor import Convertor
-from . import elements
-
-
-def parse(path: Union[str, Path], always_iter: bool = False,
-          implicit_fstrings: bool = True,
-          strict: bool = False) -> \
-        Union[elements.Element, Iterable[elements.Element]]:
-    """Parses config providing Element tree
-
-    Parameters
-    ----------
-    path: str or Path
-        path to config file
-    always_iter: bool
-        If True will always return iterator over configs.
-    implicit_fstrings: boot, default: True
-        If True, all quoted strings will be treated as python f-strings.
-    strict:
-        It True, checks overwriting dict keys and positioning (`args` before `kwargs`).
-
-    Returns
-    -------
-    tree: Element or Iterable[Element]
-    """
-    parser = Parser(implicit_fstrings=implicit_fstrings, strict=strict)
-    tree = parser.parse(path)
-    if parser.has_iterators() or always_iter:
-        return IterParser(parser).iter_configs(tree)
-    return tree
-
-
-def construct(tree: elements.Element,
-              strict_typing: bool = False,
-              nonsequential: bool = False) -> Any:
-    """Constructs python object based on config and known nip-objects
-
-    Parameters
-    ----------
-    tree: Element
-        Read config tree.
-    strict_typing:
-        If True, raises Exception when typing mismatch.
-    nonsequential:
-        If True, allows to use links before creation.
-
-    Returns
-    -------
-    obj: Any
-    """
-    if nonsequential:
-        constructor = NonSequentialConstructor(tree, strict_typing=strict_typing)
-    else:
-        constructor = Constructor(strict_typing=strict_typing)
-    return constructor.construct(tree)
-
-
-def _iter_load(configs, strict_typing, nonsequential):  # Otherwise load() will always be an iterator
-    for config in configs:
-        yield construct(config, strict_typing, nonsequential)
-
-
-def load(path: Union[str, Path],
-         always_iter: bool = False,
-         strict: bool = False,
-         nonsequential: bool = False) -> Union[Any, Iterable[Any]]:
-    """Parses config and constructs python object
-    Parameters
-    ----------
-    path: str or Path
-        Path to config file
-    always_iter: bool
-        If True will always return iterator over configs.
-    strict:
-        If True, raises Exception when typing mismatch or overwriting dict key.
-    nonsequential:
-        If True, allows to use links before creation.
-
-    Returns
-    -------
-    obj: Any or Iterable[Any]
-    """
-    config = parse(path, always_iter, strict=strict)
-
-    if isinstance(config, Iterable):
-        return _iter_load(config, strict, nonsequential)
-
-    return construct(config, strict, nonsequential)
-
-
-def dump(path: Union[str, Path], obj: Union[elements.Element, object]):
-    """Dumps config tree to file.
-
-    Parameters
-    ----------
-    path: str or Path
-        Path to save the config.
-    obj: Element or object
-        Read or generated config if Element. In case of any other object `convert` will be called.
-    """
-    if not isinstance(obj, elements.Element):
-        obj = convert(obj)
-    dumper = Dumper()
-    dumper.dump(path, obj)
-
-
-def dumps(obj: Union[elements.Element, object]) -> str:
-    """Dumps config tree to file.
-
-    Parameters
-    ----------
-    obj: Element
-        Read or generated config tree.
-
-    Returns
-    -------
-    string: str
-        Dumped element as a string.
-    """
-    if not isinstance(obj, elements.Element):
-        obj = convert(obj)
-    dumper = Dumper()
-    return dumper.dumps(obj)
-
-
-def convert(obj):
-    """Converts object to nip.Element
-
-    Parameters
-    ----------
-    obj: nip-serializable object.
-
-    Returns
-    -------
-    Element:
-        Object representation as Nip.Element
-
-    Notes
-    -----
-    Any standard python objects that can be casted to and from nip are supported.
-    For custom classes method `__nip__` that casts them to the standard object are needed.
-    Anything that is returned from `__nip__` method will be recursively converted.
-    `__nip__` method is expected to return everything needed for object construction with __init__
-    or any other used constructor.
-    By default, tag specified in @nip or default class name otherwise will be used as a tag.
-    """
-    convertor = Convertor()
-    return convertor.convert(obj)
-
-
-def _run_return(value, config, return_values, return_configs):
-    return_tuple = []
-    if return_values:
-        return_tuple.append(value)
-    if return_configs:
-        return_tuple.append(config)
-    if len(return_tuple) == 0:
-        return None
-    if len(return_tuple) == 1:
-        return return_tuple[0]
-    return tuple(return_tuple)
-
-
-def _single_run(config, func, verbose, return_values, return_configs, config_parameter,
-                strict, nonsequential):
-    if verbose:
-        print("=" * 20)
-        print("Running config:")
-        print(dumps(config))
-        print("----")
-
-    value = construct(config, strict, nonsequential)
-    if func is not None:
-        if isinstance(value, tuple) and isinstance(value[0], list) and isinstance(value[1], dict):
-            args, kwargs = value
-        elif isinstance(value, list):
-            args, kwargs = value, {}
-        elif isinstance(value, dict):
-            args, kwargs = [], value
-        else:
-            raise RuntimeError("Value constructed by the config cant be parsed as args and kwargs")
-
-        if config_parameter:
-            if config_parameter in kwargs:
-                raise RuntimeWarning(
-                    f"nip.run() was asked to add config parameter '{config_parameter}', "
-                    f"but it is already specified by the config. It will be overwritten.")
-            kwargs[config_parameter] = config
-
-        value = func(*args, **kwargs)
-
-    if verbose:
-        print("----")
-        print("Run value:")
-        print(value)
-
-    return _run_return(value, config, return_values, return_configs)
-
-
-def _iter_run(configs, func, verbose, return_values, return_configs, config_parameter,
-              strict, nonsequential):
-    for config in configs:
-        run_return = _single_run(config, func, verbose, return_values, return_configs,
-                                 config_parameter, strict, nonsequential)
-        if run_return:
-            yield run_return
-
-
-def run(path: Union[str, Path],
-        func: Optional[Callable] = None,
-        verbose: bool = True,
-        strict: bool = False,
-        nonsequential: bool = False,
-        return_values: bool = True,
-        return_configs: bool = False,
-        always_iter: bool = False,
-        config_parameter: Optional[str] = None,):
-    """Runs config. Config should be declared with function to run as a tag for the Document.
-    In case of iterable configs we will iterate over and run each of them.
-
-    Parameters
-    ----------
-    path: str or Path
-        path to config to run.
-    func:
-        Function to be called with loaded configs.
-        If not specified, config will be constructed as is.
-    verbose: bool, optional
-        Whether to print information about currently running experiment or not.
-    strict:
-        If True, raises Exception when typing mismatch or overwriting dict key.
-    nonsequential:
-        If True, allows to use links before creation.
-    return_values: bool, optional
-        Whether to return values of ran functions or not.
-    return_configs: bool, optional
-        Whether to return config for ran function or not.
-    always_iter: bool, optional
-        Result will always be iterable.
-    config_parameter: str, optional
-        If specified, parsed config will be passed to called function as a parameter with this name.
-        `func` parameter must be specified.
-
-    Returns
-    -------
-    Iterator or single value depending on whether the config is iterable
-    value or config or (value, config): Any or str or (Any, str)
-        returned values and configs of runs
-    """
-    assert config_parameter is None or config_parameter is not None and func is not None, \
-        "`config_parameter` can be used only with specified `func`"
-    config = parse(path, always_iter=always_iter, strict=strict)
-    if isinstance(config, Iterable):
-        return list(_iter_run(config, func, verbose, return_values, return_configs,
-                              config_parameter, strict, nonsequential))  # mb iter?
-
-    return _single_run(config, func, verbose, return_values, return_configs, config_parameter,
-                       strict, nonsequential)
+from typing import Union, Any, Iterable, Callable, Optional
+from pathlib import Path
+
+
+from .parser import Parser
+from .constructor import Constructor, ConstructorError
+from .non_seq_constructor import NonSequentialConstructor
+from .iter_parser import IterParser
+from .dumper import Dumper
+from .convertor import Convertor
+from . import elements
+
+
+def parse(path: Union[str, Path], always_iter: bool = False,
+          implicit_fstrings: bool = True,
+          strict: bool = False) -> \
+        Union[elements.Element, Iterable[elements.Element]]:
+    """Parses config providing Element tree
+
+    Parameters
+    ----------
+    path: str or Path
+        path to config file
+    always_iter: bool
+        If True will always return iterator over configs.
+    implicit_fstrings: boot, default: True
+        If True, all quoted strings will be treated as python f-strings.
+    strict:
+        It True, checks overwriting dict keys and positioning (`args` before `kwargs`).
+
+    Returns
+    -------
+    tree: Element or Iterable[Element]
+    """
+    parser = Parser(implicit_fstrings=implicit_fstrings, strict=strict)
+    tree = parser.parse(path)
+    if parser.has_iterators() or always_iter:
+        return IterParser(parser).iter_configs(tree)
+    return tree
+
+
+def construct(tree: elements.Element,
+              strict_typing: bool = False,
+              nonsequential: bool = False) -> Any:
+    """Constructs python object based on config and known nip-objects
+
+    Parameters
+    ----------
+    tree: Element
+        Read config tree.
+    strict_typing:
+        If True, raises Exception when typing mismatch.
+    nonsequential:
+        If True, allows to use links before creation.
+
+    Returns
+    -------
+    obj: Any
+    """
+    if nonsequential:
+        constructor = NonSequentialConstructor(tree, strict_typing=strict_typing)
+    else:
+        constructor = Constructor(strict_typing=strict_typing)
+    return constructor.construct(tree)
+
+
+def _iter_load(configs, strict_typing, nonsequential):  # Otherwise load() will always be an iterator
+    for config in configs:
+        yield construct(config, strict_typing, nonsequential)
+
+
+def load(path: Union[str, Path],
+         always_iter: bool = False,
+         strict: bool = False,
+         nonsequential: bool = False) -> Union[Any, Iterable[Any]]:
+    """Parses config and constructs python object
+    Parameters
+    ----------
+    path: str or Path
+        Path to config file
+    always_iter: bool
+        If True will always return iterator over configs.
+    strict:
+        If True, raises Exception when typing mismatch or overwriting dict key.
+    nonsequential:
+        If True, allows to use links before creation.
+
+    Returns
+    -------
+    obj: Any or Iterable[Any]
+    """
+    config = parse(path, always_iter, strict=strict)
+
+    if isinstance(config, Iterable):
+        return _iter_load(config, strict, nonsequential)
+
+    return construct(config, strict, nonsequential)
+
+
+def dump(path: Union[str, Path], obj: Union[elements.Element, object]):
+    """Dumps config tree to file.
+
+    Parameters
+    ----------
+    path: str or Path
+        Path to save the config.
+    obj: Element or object
+        Read or generated config if Element. In case of any other object `convert` will be called.
+    """
+    if not isinstance(obj, elements.Element):
+        obj = convert(obj)
+    dumper = Dumper()
+    dumper.dump(path, obj)
+
+
+def dumps(obj: Union[elements.Element, object]) -> str:
+    """Dumps config tree to file.
+
+    Parameters
+    ----------
+    obj: Element
+        Read or generated config tree.
+
+    Returns
+    -------
+    string: str
+        Dumped element as a string.
+    """
+    if not isinstance(obj, elements.Element):
+        obj = convert(obj)
+    dumper = Dumper()
+    return dumper.dumps(obj)
+
+
+def convert(obj):
+    """Converts object to nip.Element
+
+    Parameters
+    ----------
+    obj: nip-serializable object.
+
+    Returns
+    -------
+    Element:
+        Object representation as Nip.Element
+
+    Notes
+    -----
+    Any standard python objects that can be casted to and from nip are supported.
+    For custom classes method `__nip__` that casts them to the standard object are needed.
+    Anything that is returned from `__nip__` method will be recursively converted.
+    `__nip__` method is expected to return everything needed for object construction with __init__
+    or any other used constructor.
+    By default, tag specified in @nip or default class name otherwise will be used as a tag.
+    """
+    convertor = Convertor()
+    return convertor.convert(obj)
+
+
+def _run_return(value, config, return_values, return_configs):
+    return_tuple = []
+    if return_values:
+        return_tuple.append(value)
+    if return_configs:
+        return_tuple.append(config)
+    if len(return_tuple) == 0:
+        return None
+    if len(return_tuple) == 1:
+        return return_tuple[0]
+    return tuple(return_tuple)
+
+
+def _single_run(config, func, verbose, return_values, return_configs, config_parameter,
+                strict, nonsequential):
+    if verbose:
+        print("=" * 20)
+        print("Running config:")
+        print(dumps(config))
+        print("----")
+
+    value = construct(config, strict, nonsequential)
+    if func is not None:
+        if isinstance(value, tuple) and isinstance(value[0], list) and isinstance(value[1], dict):
+            args, kwargs = value
+        elif isinstance(value, list):
+            args, kwargs = value, {}
+        elif isinstance(value, dict):
+            args, kwargs = [], value
+        else:
+            raise RuntimeError("Value constructed by the config cant be parsed as args and kwargs")
+
+        if config_parameter:
+            if config_parameter in kwargs:
+                raise RuntimeWarning(
+                    f"nip.run() was asked to add config parameter '{config_parameter}', "
+                    f"but it is already specified by the config. It will be overwritten.")
+            kwargs[config_parameter] = config
+
+        value = func(*args, **kwargs)
+
+    if verbose:
+        print("----")
+        print("Run value:")
+        print(value)
+
+    return _run_return(value, config, return_values, return_configs)
+
+
+def _iter_run(configs, func, verbose, return_values, return_configs, config_parameter,
+              strict, nonsequential):
+    for config in configs:
+        run_return = _single_run(config, func, verbose, return_values, return_configs,
+                                 config_parameter, strict, nonsequential)
+        if run_return:
+            yield run_return
+
+
+def run(path: Union[str, Path],
+        func: Optional[Callable] = None,
+        verbose: bool = True,
+        strict: bool = False,
+        nonsequential: bool = False,
+        return_values: bool = True,
+        return_configs: bool = False,
+        always_iter: bool = False,
+        config_parameter: Optional[str] = None,):
+    """Runs config. Config should be declared with function to run as a tag for the Document.
+    In case of iterable configs we will iterate over and run each of them.
+
+    Parameters
+    ----------
+    path: str or Path
+        path to config to run.
+    func:
+        Function to be called with loaded configs.
+        If not specified, config will be constructed as is.
+    verbose: bool, optional
+        Whether to print information about currently running experiment or not.
+    strict:
+        If True, raises Exception when typing mismatch or overwriting dict key.
+    nonsequential:
+        If True, allows to use links before creation.
+    return_values: bool, optional
+        Whether to return values of ran functions or not.
+    return_configs: bool, optional
+        Whether to return config for ran function or not.
+    always_iter: bool, optional
+        Result will always be iterable.
+    config_parameter: str, optional
+        If specified, parsed config will be passed to called function as a parameter with this name.
+        `func` parameter must be specified.
+
+    Returns
+    -------
+    Iterator or single value depending on whether the config is iterable
+    value or config or (value, config): Any or str or (Any, str)
+        returned values and configs of runs
+    """
+    assert config_parameter is None or config_parameter is not None and func is not None, \
+        "`config_parameter` can be used only with specified `func`"
+    config = parse(path, always_iter=always_iter, strict=strict)
+    if isinstance(config, Iterable):
+        return list(_iter_run(config, func, verbose, return_values, return_configs,
+                              config_parameter, strict, nonsequential))  # mb iter?
+
+    return _single_run(config, func, verbose, return_values, return_configs, config_parameter,
+                       strict, nonsequential)
```

### Comparing `nip-config-0.8.4/nip/tokens.py` & `nip-config-0.9.0/nip/tokens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,235 +1,233 @@
-from __future__ import annotations
-
-from abc import abstractmethod, ABC
-from typing import Tuple, Any, Union
-
-import nip.parser as parser
-
-
-class Token(ABC):
-    """Abstract of token reader"""
-    def __init__(self, value: Any = None):
-        self.value = value
-
-    @staticmethod
-    @abstractmethod
-    def read(stream: str) -> Tuple[int, Union[None, Token]]:
-        pass
-
-    def set_position(self, line, pos):
-        self.line = line
-        self.pos = pos
-
-    def __eq__(self, other: Token):
-        return self.__class__ == other.__class__ and self.value == other.value
-
-    @property
-    def name(self):
-        return self.__class__.__name__
-
-
-class TokenError(Exception):
-    def __init__(self, msg: str):
-        self.msg = msg
-
-    def __str__(self):
-        return f"{self.msg}"
-
-
-class Number(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Number]]:
-        string = Number._read_number_string(stream)
-        value = None
-        for t in (int, float):
-            try:
-                value = t(string)
-                break
-            except:
-                pass
-        if value is not None:
-            return len(string), Number(value)
-        else:
-            return 0, None
-
-    @staticmethod
-    def _read_number_string(stream: str):
-        string_number = ""
-        for c in stream[:].strip():
-            if c.isnumeric():
-                string_number += c
-                continue
-            if c == '-' and (len(string_number) == 0 or string_number[-1] == 'e'):
-                string_number += c
-                continue
-            if c in ['e', '.'] and c not in string_number:
-                string_number += c
-                continue
-            break
-        return string_number
-
-
-class Bool(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Bool]]:
-        string = stream[:].strip()
-        if string in ['true', 'True', 'yes']:
-            return len(string), Bool(True)
-        if string in ["false", 'False', 'no']:
-            return len(string), Bool(False)
-        return 0, None
-
-
-# class NoneType(Token):
-#     @staticmethod
-#     def read(stream: str) -> Tuple[int, Any]:
-#         string = stream[:strip]
-
-class String(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, String]]:
-        for op in Operator.operators:
-            if stream.startswith(op):
-                return 0, None
-        pos = 0
-        if stream[pos] in "\'\"":
-            start_char = stream[pos]
-            pos += 1
-            while stream[pos] and stream[pos] != start_char:
-                pos += 1
-            if stream[pos] != start_char:
-                raise TokenError("Not closed string expression")
-            pos += 1
-            return pos, String(stream[1:pos - 1])
-
-        pos = len(stream)
-        for op in ['#']:  # mb: other operators stops string. (hard to raise good exception)
-            found_pos = stream.find(op)
-            if found_pos >= 0:
-                pos = min(pos, found_pos)
-
-        if pos == 0:
-            return 0, None
-        return pos, String(stream[:pos].strip())
-
-
-class Name(String):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Name]]:
-        pos = 0
-        if not stream[pos].isalpha():
-            return 0, None
-
-        while pos < len(stream) and (
-                stream[pos].isalnum() or stream[pos] == '_' or stream[pos] == '.'):
-            pos += 1
-
-        return pos, Name(stream[:pos])
-
-
-class Operator(Token):
-    operators = ['---', '@', '#', '&', '!&', '!!', '!', '- ', ': ', '*', '{', '}', '[', ']', '(', ')']
-
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Operator]]:
-        for op in Operator.operators:
-            if stream.startswith(op):
-                return len(op), Operator(op)
-        return 0, None
-
-
-class Indent(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Indent]]:
-        indent = 0
-        pos = 0
-        while stream[pos].isspace():
-            if stream[pos] == ' ':
-                indent += 1
-            elif stream[pos] == '\t':
-                indent += 4
-            else:
-                raise TokenError("Unknown indent symbol")
-            pos += 1
-
-        return pos, Indent(indent)
-
-
-class List(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, List]]:
-        pos = 0
-        if stream[pos] != '[':
-            return pos, None
-        while stream and stream[pos] != ']':
-            pos += 1
-        if stream[pos] != ']':
-            raise TokenError('List was not closed')
-        pos += 1
-        read_list = eval(stream[:pos])
-        return pos, List(read_list)
-
-
-class TupleToken(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, List]]:
-        pos = 0
-        if stream[pos] != '(':
-            return pos, None
-        while stream and stream[pos] != ')':
-            pos += 1
-        if stream[pos] != ')':
-            raise TokenError('Tuple was not closed')
-        pos += 1
-        read_list = eval(stream[:pos])
-        return pos, List(read_list)
-
-
-class Dict(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, Dict]]:
-        pos = 0
-        if stream[pos] != '{':
-            return pos, None
-        while stream and stream[pos] != '}':
-            pos += 1
-        if stream[pos] != '}':
-            raise TokenError('Dict was not closed')
-        pos += 1
-        read_dict = eval(stream[:pos])
-        return pos, Dict(read_dict)
-
-
-class InlinePython(Token):
-    @staticmethod
-    def read(stream: str) -> Tuple[int, Union[None, InlinePython]]:
-        pos = 0
-        if stream[pos] != '`':
-            return pos, None
-        pos += 1
-        while stream and stream[pos] != '`':
-            pos += 1
-        if stream[pos] != '`':
-            raise TokenError('Inline python string was not clothed')
-        pos += 1
-        return pos, InlinePython(stream[1:pos - 1])
-
-
-class PythonString(Token):
-    @classmethod
-    def read(cls, stream: str, implicit_fstrings: bool = False) -> \
-            Tuple[int, Union[None, PythonString]]:
-        string = stream[:].strip()
-        if implicit_fstrings and string[0] in "\"\'":
-            if string[-1] != string[0]:
-                raise TokenError("Not closed f-string")
-            return len(string), PythonString((string, 'f'))
-        if string[0] == 'f' and string[1] in "\"\'":
-            if string[-1] != string[1]:
-                raise TokenError("Not closed f-string")
-            return len(string), PythonString((string[1:], 'f'))
-        if string[0] == 'r' and string[1] in "\"\'":
-            if string[-1] != string[1]:
-                raise TokenError("Not closed r-string")
-            return len(string), PythonString((string[1:], 'r'))
-        return 0, None
+# from __future__ import annotations
+
+from abc import abstractmethod, ABC
+from typing import Tuple, Any, Union
+
+
+class Token(ABC):
+    """Abstract of token reader"""
+    def __init__(self, value: Any = None):
+        self.value = value
+
+    @staticmethod
+    @abstractmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Token"]]:
+        pass
+
+    def set_position(self, line, pos):
+        self.line = line
+        self.pos = pos
+
+    def __eq__(self, other: "Token"):
+        return self.__class__ == other.__class__ and self.value == other.value
+
+    @property
+    def name(self):
+        return self.__class__.__name__
+
+
+class TokenError(Exception):
+    def __init__(self, msg: str):
+        self.msg = msg
+
+    def __str__(self):
+        return f"{self.msg}"
+
+
+class Number(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Number"]]:
+        string = Number._read_number_string(stream)
+        value = None
+        for t in (int, float):
+            try:
+                value = t(string)
+                break
+            except:
+                pass
+        if value is not None:
+            return len(string), Number(value)
+        else:
+            return 0, None
+
+    @staticmethod
+    def _read_number_string(stream: str):
+        string_number = ""
+        for c in stream[:].strip():
+            if c.isnumeric():
+                string_number += c
+                continue
+            if c == '-' and (len(string_number) == 0 or string_number[-1] == 'e'):
+                string_number += c
+                continue
+            if c in ['e', '.'] and c not in string_number:
+                string_number += c
+                continue
+            break
+        return string_number
+
+
+class Bool(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Bool"]]:
+        string = stream[:].strip()
+        if string in ['true', 'True', 'yes']:
+            return len(string), Bool(True)
+        if string in ["false", 'False', 'no']:
+            return len(string), Bool(False)
+        return 0, None
+
+
+# class NoneType(Token):
+#     @staticmethod
+#     def read(stream: str) -> Tuple[int, Any]:
+#         string = stream[:strip]
+
+class String(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "String"]]:
+        for op in Operator.operators:
+            if stream.startswith(op):
+                return 0, None
+        pos = 0
+        if stream[pos] in "\'\"":
+            start_char = stream[pos]
+            pos += 1
+            while stream[pos] and stream[pos] != start_char:
+                pos += 1
+            if stream[pos] != start_char:
+                raise TokenError("Not closed string expression")
+            pos += 1
+            return pos, String(stream[1:pos - 1])
+
+        pos = len(stream)
+        for op in ['#']:  # mb: other operators stops string. (hard to raise good exception)
+            found_pos = stream.find(op)
+            if found_pos >= 0:
+                pos = min(pos, found_pos)
+
+        if pos == 0:
+            return 0, None
+        return pos, String(stream[:pos].strip())
+
+
+class Name(String):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Name"]]:
+        pos = 0
+        if not stream[pos].isalpha():
+            return 0, None
+
+        while pos < len(stream) and (
+                stream[pos].isalnum() or stream[pos] == '_' or stream[pos] == '.'):
+            pos += 1
+
+        return pos, Name(stream[:pos])
+
+
+class Operator(Token):
+    operators = ['---', '@', '#', '&', '!&', '!!', '!', '- ', ': ', '*', '{', '}', '[', ']', '(', ')']
+
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Operator"]]:
+        for op in Operator.operators:
+            if stream.startswith(op):
+                return len(op), Operator(op)
+        return 0, None
+
+
+class Indent(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Indent"]]:
+        indent = 0
+        pos = 0
+        while stream[pos].isspace():
+            if stream[pos] == ' ':
+                indent += 1
+            elif stream[pos] == '\t':
+                indent += 4
+            else:
+                raise TokenError("Unknown indent symbol")
+            pos += 1
+
+        return pos, Indent(indent)
+
+
+class List(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "List"]]:
+        pos = 0
+        if stream[pos] != '[':
+            return pos, None
+        while stream and stream[pos] != ']':
+            pos += 1
+        if stream[pos] != ']':
+            raise TokenError('List was not closed')
+        pos += 1
+        read_list = eval(stream[:pos])
+        return pos, List(read_list)
+
+
+class TupleToken(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "List"]]:
+        pos = 0
+        if stream[pos] != '(':
+            return pos, None
+        while stream and stream[pos] != ')':
+            pos += 1
+        if stream[pos] != ')':
+            raise TokenError('Tuple was not closed')
+        pos += 1
+        read_list = eval(stream[:pos])
+        return pos, List(read_list)
+
+
+class Dict(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "Dict"]]:
+        pos = 0
+        if stream[pos] != '{':
+            return pos, None
+        while stream and stream[pos] != '}':
+            pos += 1
+        if stream[pos] != '}':
+            raise TokenError('Dict was not closed')
+        pos += 1
+        read_dict = eval(stream[:pos])
+        return pos, Dict(read_dict)
+
+
+class InlinePython(Token):
+    @staticmethod
+    def read(stream: str) -> Tuple[int, Union[None, "InlinePython"]]:
+        pos = 0
+        if stream[pos] != '`':
+            return pos, None
+        pos += 1
+        while stream and stream[pos] != '`':
+            pos += 1
+        if stream[pos] != '`':
+            raise TokenError('Inline python string was not clothed')
+        pos += 1
+        return pos, InlinePython(stream[1:pos - 1])
+
+
+class PythonString(Token):
+    @classmethod
+    def read(cls, stream: str, implicit_fstrings: bool = False) -> \
+            Tuple[int, Union[None, "PythonString"]]:
+        string = stream[:].strip()
+        if implicit_fstrings and string[0] in "\"\'":
+            if string[-1] != string[0]:
+                raise TokenError("Not closed f-string")
+            return len(string), PythonString((string, 'f'))
+        if string[0] == 'f' and string[1] in "\"\'":
+            if string[-1] != string[1]:
+                raise TokenError("Not closed f-string")
+            return len(string), PythonString((string[1:], 'f'))
+        if string[0] == 'r' and string[1] in "\"\'":
+            if string[-1] != string[1]:
+                raise TokenError("Not closed r-string")
+            return len(string), PythonString((string[1:], 'r'))
+        return 0, None
```

### Comparing `nip-config-0.8.4/nip/utils.py` & `nip-config-0.9.0/nip/utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import ast
-import inspect
-import typeguard
-
-from typing import List, Dict, Union, Any
-
-
-def get_subclasses(cls):
-    return set(cls.__subclasses__()).union(
-        [s for c in cls.__subclasses__() for s in get_subclasses(c)])
-
-
-def get_sub_dict(base_cls):
-    return {cls.__name__: cls for cls in get_subclasses(base_cls)}
-
-
-def deep_equals(first: Union[Dict, List, Any], second: Union[Dict, List, Any]):
-    if type(first) != type(second):
-        return False
-    if isinstance(first, dict):
-        for key in first:
-            if key not in second:
-                return False
-            if not deep_equals(first[key], second[key]):
-                return False
-    elif isinstance(first, list):
-        if len(first) != len(second):
-            return False
-        for i, j in zip(first, second):
-            if not deep_equals(i, j):
-                return False
-    else:
-        return first == second
-    return True
-
-
-def iterate_items(obj):
-    if isinstance(obj, (list, tuple)):
-        for i, value in enumerate(obj):
-            yield i, value
-    if isinstance(obj, dict):
-        for key, value in obj.items():
-            yield key, value
-
-
-def flatten(obj, delimiter='.', keys=()):
-    if not isinstance(obj, (list, tuple, dict)):
-        return {delimiter.join(keys): obj}
-
-    result = {}
-    for key, value in iterate_items(obj):
-        result.update(
-            flatten(value, delimiter, keys=keys + (str(key),)))
-    return result
-
+import ast
+import inspect
+import typeguard
+
+from typing import List, Dict, Union, Any
+
+
+def get_subclasses(cls):
+    return set(cls.__subclasses__()).union(
+        [s for c in cls.__subclasses__() for s in get_subclasses(c)])
+
+
+def get_sub_dict(base_cls):
+    return {cls.__name__: cls for cls in get_subclasses(base_cls)}
+
+
+def deep_equals(first: Union[Dict, List, Any], second: Union[Dict, List, Any]):
+    if type(first) != type(second):
+        return False
+    if isinstance(first, dict):
+        for key in first:
+            if key not in second:
+                return False
+            if not deep_equals(first[key], second[key]):
+                return False
+    elif isinstance(first, list):
+        if len(first) != len(second):
+            return False
+        for i, j in zip(first, second):
+            if not deep_equals(i, j):
+                return False
+    else:
+        return first == second
+    return True
+
+
+def iterate_items(obj):
+    if isinstance(obj, (list, tuple)):
+        for i, value in enumerate(obj):
+            yield i, value
+    if isinstance(obj, dict):
+        for key, value in obj.items():
+            yield key, value
+
+
+def flatten(obj, delimiter='.', keys=()):
+    if not isinstance(obj, (list, tuple, dict)):
+        return {delimiter.join(keys): obj}
+
+    result = {}
+    for key, value in iterate_items(obj):
+        result.update(
+            flatten(value, delimiter, keys=keys + (str(key),)))
+    return result
+
```

### Comparing `nip-config-0.8.4/nip_config.egg-info/PKG-INFO` & `nip-config-0.9.0/nip_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.8.4
+Version: 0.9.0
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 NIP is a yaml-like config files parser for convenient python object construction and experiment holding.
 Short guide can be found here: https://github.com/spairet/nip/tree/main/doc
```

### Comparing `nip-config-0.8.4/setup.cfg` & `nip-config-0.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6970 2d63 6f6e 6669 670d 0a76   = nip-config..v
-00000020: 6572 7369 6f6e 203d 2030 2e38 2e34 0d0a  ersion = 0.8.4..
+00000020: 6572 7369 6f6e 203d 2030 2e39 2e30 0d0a  ersion = 0.9.0..
 00000030: 6175 7468 6f72 203d 2049 6c79 6120 5661  author = Ilya Va
 00000040: 7369 6c69 6576 0d0a 6175 7468 6f72 5f65  siliev..author_e
 00000050: 6d61 696c 203d 2073 7061 6972 6574 4062  mail = spairet@b
 00000060: 6b2e 7275 0d0a 6465 7363 7269 7074 696f  k.ru..descriptio
 00000070: 6e20 3d20 4164 7661 6e63 6564 2063 6f6e  n = Advanced con
 00000080: 6669 6773 2066 6f72 2070 7974 686f 6e0d  figs for python.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
@@ -40,14 +40,14 @@
 00000270: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
 00000280: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
 00000290: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 000002a0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
 000002b0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
 000002c0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 000002d0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-000002e0: 3d20 3e3d 332e 370d 0a69 6e73 7461 6c6c  = >=3.7..install
+000002e0: 3d20 3e3d 332e 360d 0a69 6e73 7461 6c6c  = >=3.6..install
 000002f0: 5f72 6571 7569 7265 7320 3d20 0d0a 096d  _requires = ...m
 00000300: 756c 7469 706c 6564 6973 7061 7463 680d  ultipledispatch.
 00000310: 0a09 7479 7065 6775 6172 640d 0a0d 0a5b  ..typeguard....[
 00000320: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
 00000330: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
 00000340: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `nip-config-0.8.4/tests/test_utils.py` & `nip-config-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

