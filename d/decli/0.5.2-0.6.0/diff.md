# Comparing `tmp/decli-0.5.2.tar.gz` & `tmp/decli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decli-0.5.2.tar", last modified: Sun Jul 26 08:29:21 2020, max compression
+gzip compressed data, was "decli-0.6.0.tar", max compression
```

## Comparing `decli-0.5.2.tar` & `decli-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2018-08-13 08:50:23.528219 decli-0.5.2/LICENSE
--rw-r--r--   0        0        0    17339 2018-08-19 09:00:29.925665 decli-0.5.2/README.rst
--rw-r--r--   0        0        0       72 2020-07-26 08:29:03.039834 decli-0.5.2/decli/__init__.py
--rw-r--r--   0        0        0     4581 2020-07-26 08:26:49.849334 decli-0.5.2/decli/application.py
--rw-r--r--   0        0        0      884 2020-07-26 08:29:03.063834 decli-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    18587 2020-07-26 08:29:21.203282 decli-0.5.2/setup.py
--rw-r--r--   0        0        0    17823 2020-07-26 08:29:21.204130 decli-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-28 09:49:27.803266 decli-0.6.0/LICENSE
+-rw-r--r--   0        0        0    17159 2023-04-28 09:49:27.803266 decli-0.6.0/README.rst
+-rw-r--r--   0        0        0       72 2023-04-28 09:49:27.803266 decli-0.6.0/decli/__init__.py
+-rw-r--r--   0        0        0     4607 2023-04-28 09:49:27.803266 decli-0.6.0/decli/application.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:49:27.803266 decli-0.6.0/decli/py.typed
+-rw-r--r--   0        0        0      750 2023-04-28 09:49:27.803266 decli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    17745 1970-01-01 00:00:00.000000 decli-0.6.0/PKG-INFO
```

### Comparing `decli-0.5.2/LICENSE` & `decli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decli-0.5.2/README.rst` & `decli-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 ======
 Decli
 ======
 
 Minimal declarative cli tool.
 
-.. image:: https://img.shields.io/travis/Woile/decli.svg?style=flat-square
-    :alt: Travis
-    :target: https://travis-ci.org/Woile/decli
-
 .. image:: https://img.shields.io/codecov/c/github/Woile/decli.svg?style=flat-square
     :alt: Codecov
     :target: https://codecov.io/gh/Woile/decli
 
 .. image:: https://img.shields.io/pypi/v/decli.svg?style=flat-square
     :alt: PyPI
     :target: https://pypi.org/project/decli/
@@ -678,28 +674,28 @@
 More Examples
 -------------
 
 Many examples from `argparse documentation <https://docs.python.org/3/library/argparse.html>`_
 are covered in test/examples.py
 
 
-Testing
-=======
+Contributing
+============
 
 1. Clone the repo
 2. Install dependencies
 
 ::
 
     poetry install
 
 3. Run tests
 
 ::
 
-    poetry run pytest -s --cov-report term-missing --cov=decli tests/
+    ./scripts/tests
 
 
 Contributing
 ============
 
 **PRs are welcome!**
```

### Comparing `decli-0.5.2/decli/application.py` & `decli-0.6.0/decli/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import logging
 from typing import Optional, Callable, Union
 from copy import deepcopy
 
 
-config = None
+config: dict = {}
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 def init_config():
     return {"prefix_chars": "-"}
 
@@ -60,27 +60,27 @@
     if group_parser is None:
         group_parser = parser.add_argument_group(title, description)
         groups.update({title: group_parser})
     return group_parser
 
 
 def get_or_create_exclusive_group(
-    parser, groups: dict, title: str = None, required=False
+    parser, groups: dict, title: Optional[str] = None, required=False
 ):
     group_parser = groups.get(title)
     if group_parser is None:
         group_parser = parser.add_mutually_exclusive_group(required=required)
         groups.update({title: group_parser})
 
     return group_parser
 
 
 def add_arguments(parser, args: list):
-    groups = {}
-    exclusive_groups = {}
+    groups: dict = {}
+    exclusive_groups: dict = {}
 
     for arg in validate_args(args):
         logger.debug("arg: %s", arg)
 
         name: list = arg.pop("name")
         group_title: Optional[str] = arg.pop("group", None)
         exclusive_group_title: Optional[str] = arg.pop("exclusive_group", None)
```

### Comparing `decli-0.5.2/setup.py` & `decli-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,719 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: decli
+Version: 0.6.0
+Summary: Minimal, easy-to-use, declarative cli tool
+License: MIT
+Author: Santiago Fraire
+Author-email: santiwilly@gmail.com
+Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
 
-packages = \
-['decli']
+======
+Decli
+======
 
-package_data = \
-{'': ['*']}
+Minimal declarative cli tool.
 
-setup_kwargs = {
-    'name': 'decli',
-    'version': '0.5.2',
-    'description': 'Minimal, easy-to-use, declarative cli tool',
-    'long_description': '======\nDecli\n======\n\nMinimal declarative cli tool.\n\n.. image:: https://img.shields.io/travis/Woile/decli.svg?style=flat-square\n    :alt: Travis\n    :target: https://travis-ci.org/Woile/decli\n\n.. image:: https://img.shields.io/codecov/c/github/Woile/decli.svg?style=flat-square\n    :alt: Codecov\n    :target: https://codecov.io/gh/Woile/decli\n\n.. image:: https://img.shields.io/pypi/v/decli.svg?style=flat-square\n    :alt: PyPI\n    :target: https://pypi.org/project/decli/\n\n.. image:: https://img.shields.io/pypi/pyversions/decli.svg?style=flat-square\n    :alt: PyPI - Python Version\n    :target: https://pypi.org/project/decli/\n\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "prog": "myapp",\n        "description": "Process some integers.",\n        "arguments": [\n            {\n                "name": "integers",\n                "metavar": "N",\n                "type": int,\n                "nargs": "+",\n                "help": "an integer for the accumulator",\n            },\n            {\n                "name": "--sum",\n                "dest": "accumulate",\n                "action": "store_const",\n                "const": sum,\n                "default": max,\n                "help": "sum the integers (default: find the max)",\n            },\n        ],\n    }\n    parser = cli(data)\n    parser.parse_args()\n\n\n::\n\n    >> parser.print_help()\n    usage: myapp [-h] [--sum] N [N ...]\n\n    Process some integers.\n\n    positional arguments:\n    N           an integer for the accumulator\n\n    optional arguments:\n    -h, --help  show this help message and exit\n    --sum       sum the integers (default: find the max)\n\n\n::\n\n    In [4]: args = parser.parse_args("--sum 3 2 1".split())\n\n    In [5]: args.accumulate(args.integers)\n    Out[5]: 6\n\n\n.. contents::\n    :depth: 2\n\n\nAbout\n=====\n\nDecli is minimal wrapper around **argparse**.\n\nIt\'s useful when writing big applications that have many arguments and subcommands, this way it\'ll be more clear.\n\nIt\'s a minimal library to rapidly create an interface separated from your app.\n\nIt\'s possible to use any argument from **argparse** and it works really well with it.\n\nForget about copy pasting the argparse functions, if you are lazy like me, this library should be really handy!\n\nMany cases were tested, but it\'s possible that not everything was covered, so if you find anything, please report it.\n\n\nInstallation\n============\n\n::\n\n    pip install -U decli\n\nor alternatively:\n\n::\n\n    poetry add decli\n\n\nUsage\n======\n\nMain cli\n--------\n\nCreate the dictionary in which the cli tool is declared.\n\nThe same arguments argparse use are accepted, except parents, which is ignored.\n\n- prog - The name of the program (default: sys.argv[0])\n- usage - The string describing the program usage (default: generated from arguments added to parser)\n- description - Text to display before the argument help (default: none)\n- epilog - Text to display after the argument help (default: none)\n- formatter_class - A class for customizing the help output\n- prefix_chars - The set of characters that prefix optional arguments (default: ‘-‘)\n- fromfile_prefix_chars - The set of characters that prefix files from which additional arguments should be read (default: None)\n- argument_default - The global default value for arguments (default: None)\n- conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)\n- add_help - Add a -h/--help option to the parser (default: True)\n- allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)\n\nMore info in the `argparse page <https://docs.python.org/3/library/argparse.html#argumentparser-objects>`_\n\nExample:\n\n.. code-block:: python\n\n    data = {\n        "prog": "myapp",\n        "description": "This app does something cool",\n        "epilog": "And that\'s it"\n    }\n\n\nArguments\n---------\n\nIt\'s just a list with dictionaries. To add aliases just use a list instead of a string.\n\nAccepted values:\n\n\n- name: - Either a name or a list of option strings, e.g. foo or -f, --foo.\n- action - The basic type of action to be taken when this argument is encountered at the command line.\n- nargs - The number of command-line arguments that should be consumed.\n- const - A constant value required by some action and nargs selections.\n- default - The value produced if the argument is absent from the command line.\n- type - The type to which the command-line argument should be converted.\n- choices - A container of the allowable values for the argument.\n- required - Whether or not the command-line option may be omitted (optionals only).\n- help - A brief description of what the argument does.\n- metavar - A name for the argument in usage messages.\n- dest - The name of the attribute to be added to the object returned by parse_args().\n\n\nMore info about `arguments <https://docs.python.org/3/library/argparse.html#the-add-argument-method>`_\n\nExample:\n\n.. code-block:: python\n\n    data = {\n        "prog": "myapp",\n        "description": "This app does something cool",\n        "epilog": "And that\'s it",\n        "arguments": [\n            {\n                "name": "--foo"\n            },\n            {\n                "name": ["-b", "--bar"]\n            }\n        ]\n    }\n\n\nSubcommands\n-----------\n\nJust a dictionary where the most important key is **commands** which is a list of the commands.\n\n\nAccepted values:\n\n\n- title - title for the sub-parser group in help output; by default “subcommands” if description is provided, otherwise uses title for positional arguments\n- description - description for the sub-parser group in help output, by default None\n- commands - list of dicts describing the commands. Same arguments as the **main cli** are supported. And **func** which is really important.\n- prog - usage information that will be displayed with sub-command help, by default the name of the program and any positional arguments before the subparser argument\n- action - the basic type of action to be taken when this argument is encountered at the command line\n- dest - name of the attribute under which sub-command name will be stored; by default None and no value is stored\n- required - Whether or not a subcommand must be provided, by default False.\n- help - help for sub-parser group in help output, by default None\n- metavar - string presenting available sub-commands in help; by default it is None and presents sub-commands in form {cmd1, cmd2, ..}\n\n\nMore info about `subcommands <https://docs.python.org/3/library/argparse.html#sub-commands>`_\n\nFunc\n~~~~\n\nUsually in a sub-command it\'s useful to specify to which function are they pointing to. That\'s why each command should have this parameter.\n\n\nWhen you are building an app which does multiple things, each function should be mapped to a command this way, using the **func** argument.\n\nExample:\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "prog": "myapp",\n        "description": "This app does something cool",\n        "epilog": "And that\'s it",\n        "subcommands": {\n            "title": "main",\n            "commands": [\n                {\n                    "name": "sum",\n                    "help": "new project",\n                    "func": sum,\n                    "arguments": [\n                        {\n                            "name": "integers",\n                            "metavar": "N",\n                            "type": int,\n                            "nargs": "+",\n                            "help": "an integer for the accumulator",\n                        },\n                        {"name": "--name", "nargs": "?"},\n                    ],\n                }\n            ]\n        }\n    }\n\n    parser = cli(data)\n    args = parser.parse_args(["sum 1 2 3".split()])\n    args.func(args.integers)  # Runs the sum of the integers\n\nGroups\n------\n\nUsed to group the arguments based on conceptual groups. This only affects the shown **help**, nothing else.\n\nExample:\n\n.. code-block:: python\n\n    data = {\n        "prog": "app",\n        "arguments": [\n            {"name": "foo", "help": "foo help", "group": "group1"},\n            {"name": "choo", "help": "choo help", "group": "group1"},\n            {"name": "--bar", "help": "bar help", "group": "group2"},\n        ]\n    }\n    parser = cli(data)\n    parser.print_help()\n\n::\n\n    usage: app [-h] [--bar BAR] foo choo\n\n    optional arguments:\n    -h, --help  show this help message and exit\n\n    group1:\n    foo         foo help\n    choo        choo help\n\n    group2:\n    --bar BAR   bar help\n\n\nExclusive Groups\n----------------\n\nA mutually exclusive group allows to execute only one **optional** argument (starting with :code:`--`) from the group.\nIf the condition is not met, it will show an error.\n\nExample:\n\n.. code-block:: python\n\n    data = {\n        "prog": "app",\n        "arguments": [\n            {"name": "--foo", "help": "foo help", "exclusive_group": "group1"},\n            {"name": "--choo", "help": "choo help", "exclusive_group": "group1"},\n            {"name": "--bar", "help": "bar help", "exclusive_group": "group1"},\n        ]\n    }\n    parser = cli(data)\n    parser.print_help()\n\n::\n\n    usage: app [-h] [--foo FOO | --choo CHOO | --bar BAR]\n\n    optional arguments:\n    -h, --help   show this help message and exit\n    --foo FOO    foo help\n    --choo CHOO  choo help\n    --bar BAR    bar help\n\n::\n\n    In [1]: parser.parse_args("--foo 1 --choo 2".split())\n\n    usage: app [-h] [--foo FOO | --choo CHOO | --bar BAR]\n    app: error: argument --choo: not allowed with argument --foo\n\n\nGroups and Exclusive groups\n---------------------------\n\nIt is not possible to have groups inside exclusive groups with **decli**.\n\n**Decli** will prevent from doing this by raising a :code:`ValueError`.\n\nIt is possible to accomplish it with argparse, but the help message generated will be broken and the\nexclusion won\'t work.\n\nParents\n-------\n\nSometimes, several cli share a common set of arguments.\n\nRather than repeating the definitions of these arguments,\none or more parent clis with all the shared arguments can be passed\nto :code:`parents=argument` to cli.\n\nMore info about `parents <https://docs.python.org/3/library/argparse.html#parents>`_\n\nExample:\n\n.. code-block:: python\n\n    parent_foo_data = {\n        "add_help": False,\n        "arguments": [{"name": "--foo-parent", "type": int}],\n    }\n    parent_bar_data = {\n        "add_help": False,\n        "arguments": [{"name": "--bar-parent", "type": int}],\n    }\n    parent_foo_cli = cli(parent_foo_data)\n    parent_bar_cli = cli(parent_bar_data)\n\n    parents = [parent_foo_cli, parent_bar_cli]\n\n    data = {\n        "prog": "app",\n        "arguments": [\n            {"name": "foo"}\n        ]\n    }\n    parser = cli(data, parents=parents)\n    parser.print_help()\n\n::\n\n    usage: app [-h] [--foo-parent FOO_PARENT] [--bar-parent BAR_PARENT] foo\n\n    positional arguments:\n    foo\n\n    optional arguments:\n    -h, --help            show this help message and exit\n    --foo-parent FOO_PARENT\n    --bar-parent BAR_PARENT\n\n\nRecipes\n=======\n\nSubcommands\n-----------------\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "prog": "myapp",\n        "formatter_class": argparse.RawDescriptionHelpFormatter,\n        "description": "The software has subcommands which you can use",\n        "subcommands": {\n            "title": "main",\n            "description": "main commands",\n            "commands": [\n                {\n                    "name": "all",\n                    "help": "check every values is true",\n                    "func": all\n                },\n                {\n                    "name": ["s", "sum"],\n                    "help": "new project",\n                    "func": sum,\n                    "arguments": [\n                        {\n                            "name": "integers",\n                            "metavar": "N",\n                            "type": int,\n                            "nargs": "+",\n                            "help": "an integer for the accumulator",\n                        },\n                        {"name": "--name", "nargs": "?"},\n                    ],\n                }\n            ],\n        },\n    }\n    parser = cli(data)\n    args = parser.parse_args(["sum 1 2 3".split()])\n    args.func(args.integers)  # Runs the sum of the integers\n\n\nMinimal\n-------\n\nThis app does nothing, but it\'s the min we can have:\n\n.. code-block:: python\n\n    from decli import cli\n\n    parser = cli({})\n    parser.print_help()\n\n::\n\n    usage: ipython [-h]\n\n    optional arguments:\n    -h, --help  show this help message and exit\n\n\nPositional arguments\n--------------------\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "arguments": [\n            {\n                "name": "echo"\n            }\n        ]\n    }\n    parser = cli(data)\n    args = parser.parse_args(["foo"])\n\n::\n\n    In [11]: print(args.echo)\n    foo\n\n\nPositional arguments with type\n------------------------------\n\nWhen a type is specified, the argument will be treated as that type, otherwise it\'ll fail.\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "arguments": [\n            {\n                "name": "square",\n                "type": int\n            }\n        ]\n    }\n    parser = cli(data)\n    args = parser.parse_args(["1"])\n\n::\n\n    In [11]: print(args.echo)\n    1\n\nOptional arguments\n------------------\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "arguments": [\n            {\n                "name": "--verbose",\n                "help": "increase output verbosity"\n            }\n        ]\n    }\n    parser = cli(data)\n    args = parser.parse_args(["--verbosity 1"])\n\n::\n\n    In [11]: print(args.verbosity)\n    1\n\n    In [15]: args = parser.parse_args([])\n\n    In [16]: args\n    Out[16]: Namespace(verbose=None)\n\n\nFlags\n-----\n\nFlags are a boolean only (True/False) subset of options.\n\n.. code-block:: python\n\n    from decli import cli\n\n    data = {\n        "arguments": [\n            {\n                "name": "--verbose",\n                "action": "store_true",  # defaults to False\n            },\n            {\n                "name": "--noisy",\n                "action": "store_false",  # defaults to True\n            }\n        ]\n    }\n    parser = cli(data)\n\n\n\n\nShort options\n-------------\n\nUsed to add short versions of the options.\n\n.. code-block:: python\n\n    data = {\n        "arguments": [\n            {\n                "name": ["-v", "--verbose"],\n                "help": "increase output verbosity"\n            }\n        ]\n    }\n\n\nGrouping\n--------\n\nThis is only possible using **arguments**.\n\nOnly affect the way the help gets displayed. You might be looking for subcommands.\n\n\n.. code-block:: python\n\n    data = {\n        "prog": "mycli",\n        "arguments": [\n            {\n                "name": "--save",\n                "group": "main",\n                "help": "This save belongs to the main group",\n            },\n            {\n                "name": "--remove",\n                "group": "main",\n                "help": "This remove belongs to the main group",\n            },\n        ],\n    }\n    parser = cli(data)\n    parser.print_help()\n\n::\n\n    usage: mycli [-h] [--save SAVE] [--remove REMOVE]\n\n    optional arguments:\n    -h, --help       show this help message and exit\n\n    main:\n    --save SAVE      This save belongs to the main group\n    --remove REMOVE  This remove belongs to the main group\n\n\nExclusive group\n---------------\n\nThis is only possible using **optional arguments**.\n\n\n.. code-block:: python\n\n    data = {\n        "prog": "mycli",\n        "arguments": [\n            {\n                "name": "--save",\n                "exclusive_group": "main",\n                "help": "This save belongs to the main group",\n            },\n            {\n                "name": "--remove",\n                "exclusive_group": "main",\n                "help": "This remove belongs to the main group",\n            },\n        ],\n    }\n    parser = cli(data)\n    parser.print_help()\n\n::\n\n    usage: mycli [-h] [--save SAVE | --remove REMOVE]\n\n    optional arguments:\n    -h, --help       show this help message and exit\n    --save SAVE      This save belongs to the main group\n    --remove REMOVE  This remove belongs to the main group\n\n\nCombining Positional and Optional arguments\n-------------------------------------------\n\n.. code-block:: python\n\n    data = {\n        "arguments": [\n            {\n                "name": "square",\n                "type": int,\n                "help": "display a square of a given number"\n            },\n            {\n                "name": ["-v", "--verbose"],\n                "action": "store_true",\n                "help": "increase output verbosity"\n            }\n        ]\n    }\n    parser = cli(data)\n\n    args = parser.parse_args()\n    answer = args.square**2\n    if args.verbose:\n        print(f"the square of {args.square} equals {answer}")\n    else:\n        print(answer)\n\n\nMore Examples\n-------------\n\nMany examples from `argparse documentation <https://docs.python.org/3/library/argparse.html>`_\nare covered in test/examples.py\n\n\nTesting\n=======\n\n1. Clone the repo\n2. Install dependencies\n\n::\n\n    poetry install\n\n3. Run tests\n\n::\n\n    poetry run pytest -s --cov-report term-missing --cov=decli tests/\n\n\nContributing\n============\n\n**PRs are welcome!**\n',
-    'author': 'Santiago Fraire',
-    'author_email': 'santiwilly@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.6',
-}
+.. image:: https://img.shields.io/codecov/c/github/Woile/decli.svg?style=flat-square
+    :alt: Codecov
+    :target: https://codecov.io/gh/Woile/decli
 
+.. image:: https://img.shields.io/pypi/v/decli.svg?style=flat-square
+    :alt: PyPI
+    :target: https://pypi.org/project/decli/
+
+.. image:: https://img.shields.io/pypi/pyversions/decli.svg?style=flat-square
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/decli/
+
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "prog": "myapp",
+        "description": "Process some integers.",
+        "arguments": [
+            {
+                "name": "integers",
+                "metavar": "N",
+                "type": int,
+                "nargs": "+",
+                "help": "an integer for the accumulator",
+            },
+            {
+                "name": "--sum",
+                "dest": "accumulate",
+                "action": "store_const",
+                "const": sum,
+                "default": max,
+                "help": "sum the integers (default: find the max)",
+            },
+        ],
+    }
+    parser = cli(data)
+    parser.parse_args()
+
+
+::
+
+    >> parser.print_help()
+    usage: myapp [-h] [--sum] N [N ...]
+
+    Process some integers.
+
+    positional arguments:
+    N           an integer for the accumulator
+
+    optional arguments:
+    -h, --help  show this help message and exit
+    --sum       sum the integers (default: find the max)
+
+
+::
+
+    In [4]: args = parser.parse_args("--sum 3 2 1".split())
+
+    In [5]: args.accumulate(args.integers)
+    Out[5]: 6
+
+
+.. contents::
+    :depth: 2
+
+
+About
+=====
+
+Decli is minimal wrapper around **argparse**.
+
+It's useful when writing big applications that have many arguments and subcommands, this way it'll be more clear.
+
+It's a minimal library to rapidly create an interface separated from your app.
+
+It's possible to use any argument from **argparse** and it works really well with it.
+
+Forget about copy pasting the argparse functions, if you are lazy like me, this library should be really handy!
+
+Many cases were tested, but it's possible that not everything was covered, so if you find anything, please report it.
+
+
+Installation
+============
+
+::
+
+    pip install -U decli
+
+or alternatively:
+
+::
+
+    poetry add decli
+
+
+Usage
+======
+
+Main cli
+--------
+
+Create the dictionary in which the cli tool is declared.
+
+The same arguments argparse use are accepted, except parents, which is ignored.
+
+- prog - The name of the program (default: sys.argv[0])
+- usage - The string describing the program usage (default: generated from arguments added to parser)
+- description - Text to display before the argument help (default: none)
+- epilog - Text to display after the argument help (default: none)
+- formatter_class - A class for customizing the help output
+- prefix_chars - The set of characters that prefix optional arguments (default: ‘-‘)
+- fromfile_prefix_chars - The set of characters that prefix files from which additional arguments should be read (default: None)
+- argument_default - The global default value for arguments (default: None)
+- conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)
+- add_help - Add a -h/--help option to the parser (default: True)
+- allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)
+
+More info in the `argparse page <https://docs.python.org/3/library/argparse.html#argumentparser-objects>`_
+
+Example:
+
+.. code-block:: python
+
+    data = {
+        "prog": "myapp",
+        "description": "This app does something cool",
+        "epilog": "And that's it"
+    }
+
+
+Arguments
+---------
+
+It's just a list with dictionaries. To add aliases just use a list instead of a string.
+
+Accepted values:
+
+
+- name: - Either a name or a list of option strings, e.g. foo or -f, --foo.
+- action - The basic type of action to be taken when this argument is encountered at the command line.
+- nargs - The number of command-line arguments that should be consumed.
+- const - A constant value required by some action and nargs selections.
+- default - The value produced if the argument is absent from the command line.
+- type - The type to which the command-line argument should be converted.
+- choices - A container of the allowable values for the argument.
+- required - Whether or not the command-line option may be omitted (optionals only).
+- help - A brief description of what the argument does.
+- metavar - A name for the argument in usage messages.
+- dest - The name of the attribute to be added to the object returned by parse_args().
+
+
+More info about `arguments <https://docs.python.org/3/library/argparse.html#the-add-argument-method>`_
+
+Example:
+
+.. code-block:: python
+
+    data = {
+        "prog": "myapp",
+        "description": "This app does something cool",
+        "epilog": "And that's it",
+        "arguments": [
+            {
+                "name": "--foo"
+            },
+            {
+                "name": ["-b", "--bar"]
+            }
+        ]
+    }
+
+
+Subcommands
+-----------
+
+Just a dictionary where the most important key is **commands** which is a list of the commands.
+
+
+Accepted values:
+
+
+- title - title for the sub-parser group in help output; by default “subcommands” if description is provided, otherwise uses title for positional arguments
+- description - description for the sub-parser group in help output, by default None
+- commands - list of dicts describing the commands. Same arguments as the **main cli** are supported. And **func** which is really important.
+- prog - usage information that will be displayed with sub-command help, by default the name of the program and any positional arguments before the subparser argument
+- action - the basic type of action to be taken when this argument is encountered at the command line
+- dest - name of the attribute under which sub-command name will be stored; by default None and no value is stored
+- required - Whether or not a subcommand must be provided, by default False.
+- help - help for sub-parser group in help output, by default None
+- metavar - string presenting available sub-commands in help; by default it is None and presents sub-commands in form {cmd1, cmd2, ..}
+
+
+More info about `subcommands <https://docs.python.org/3/library/argparse.html#sub-commands>`_
+
+Func
+~~~~
+
+Usually in a sub-command it's useful to specify to which function are they pointing to. That's why each command should have this parameter.
+
+
+When you are building an app which does multiple things, each function should be mapped to a command this way, using the **func** argument.
+
+Example:
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "prog": "myapp",
+        "description": "This app does something cool",
+        "epilog": "And that's it",
+        "subcommands": {
+            "title": "main",
+            "commands": [
+                {
+                    "name": "sum",
+                    "help": "new project",
+                    "func": sum,
+                    "arguments": [
+                        {
+                            "name": "integers",
+                            "metavar": "N",
+                            "type": int,
+                            "nargs": "+",
+                            "help": "an integer for the accumulator",
+                        },
+                        {"name": "--name", "nargs": "?"},
+                    ],
+                }
+            ]
+        }
+    }
+
+    parser = cli(data)
+    args = parser.parse_args(["sum 1 2 3".split()])
+    args.func(args.integers)  # Runs the sum of the integers
+
+Groups
+------
+
+Used to group the arguments based on conceptual groups. This only affects the shown **help**, nothing else.
+
+Example:
+
+.. code-block:: python
+
+    data = {
+        "prog": "app",
+        "arguments": [
+            {"name": "foo", "help": "foo help", "group": "group1"},
+            {"name": "choo", "help": "choo help", "group": "group1"},
+            {"name": "--bar", "help": "bar help", "group": "group2"},
+        ]
+    }
+    parser = cli(data)
+    parser.print_help()
+
+::
+
+    usage: app [-h] [--bar BAR] foo choo
+
+    optional arguments:
+    -h, --help  show this help message and exit
+
+    group1:
+    foo         foo help
+    choo        choo help
+
+    group2:
+    --bar BAR   bar help
+
+
+Exclusive Groups
+----------------
+
+A mutually exclusive group allows to execute only one **optional** argument (starting with :code:`--`) from the group.
+If the condition is not met, it will show an error.
+
+Example:
+
+.. code-block:: python
+
+    data = {
+        "prog": "app",
+        "arguments": [
+            {"name": "--foo", "help": "foo help", "exclusive_group": "group1"},
+            {"name": "--choo", "help": "choo help", "exclusive_group": "group1"},
+            {"name": "--bar", "help": "bar help", "exclusive_group": "group1"},
+        ]
+    }
+    parser = cli(data)
+    parser.print_help()
+
+::
+
+    usage: app [-h] [--foo FOO | --choo CHOO | --bar BAR]
+
+    optional arguments:
+    -h, --help   show this help message and exit
+    --foo FOO    foo help
+    --choo CHOO  choo help
+    --bar BAR    bar help
+
+::
+
+    In [1]: parser.parse_args("--foo 1 --choo 2".split())
+
+    usage: app [-h] [--foo FOO | --choo CHOO | --bar BAR]
+    app: error: argument --choo: not allowed with argument --foo
+
+
+Groups and Exclusive groups
+---------------------------
+
+It is not possible to have groups inside exclusive groups with **decli**.
+
+**Decli** will prevent from doing this by raising a :code:`ValueError`.
+
+It is possible to accomplish it with argparse, but the help message generated will be broken and the
+exclusion won't work.
+
+Parents
+-------
+
+Sometimes, several cli share a common set of arguments.
+
+Rather than repeating the definitions of these arguments,
+one or more parent clis with all the shared arguments can be passed
+to :code:`parents=argument` to cli.
+
+More info about `parents <https://docs.python.org/3/library/argparse.html#parents>`_
+
+Example:
+
+.. code-block:: python
+
+    parent_foo_data = {
+        "add_help": False,
+        "arguments": [{"name": "--foo-parent", "type": int}],
+    }
+    parent_bar_data = {
+        "add_help": False,
+        "arguments": [{"name": "--bar-parent", "type": int}],
+    }
+    parent_foo_cli = cli(parent_foo_data)
+    parent_bar_cli = cli(parent_bar_data)
+
+    parents = [parent_foo_cli, parent_bar_cli]
+
+    data = {
+        "prog": "app",
+        "arguments": [
+            {"name": "foo"}
+        ]
+    }
+    parser = cli(data, parents=parents)
+    parser.print_help()
+
+::
+
+    usage: app [-h] [--foo-parent FOO_PARENT] [--bar-parent BAR_PARENT] foo
+
+    positional arguments:
+    foo
+
+    optional arguments:
+    -h, --help            show this help message and exit
+    --foo-parent FOO_PARENT
+    --bar-parent BAR_PARENT
+
+
+Recipes
+=======
+
+Subcommands
+-----------------
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "prog": "myapp",
+        "formatter_class": argparse.RawDescriptionHelpFormatter,
+        "description": "The software has subcommands which you can use",
+        "subcommands": {
+            "title": "main",
+            "description": "main commands",
+            "commands": [
+                {
+                    "name": "all",
+                    "help": "check every values is true",
+                    "func": all
+                },
+                {
+                    "name": ["s", "sum"],
+                    "help": "new project",
+                    "func": sum,
+                    "arguments": [
+                        {
+                            "name": "integers",
+                            "metavar": "N",
+                            "type": int,
+                            "nargs": "+",
+                            "help": "an integer for the accumulator",
+                        },
+                        {"name": "--name", "nargs": "?"},
+                    ],
+                }
+            ],
+        },
+    }
+    parser = cli(data)
+    args = parser.parse_args(["sum 1 2 3".split()])
+    args.func(args.integers)  # Runs the sum of the integers
+
+
+Minimal
+-------
+
+This app does nothing, but it's the min we can have:
+
+.. code-block:: python
+
+    from decli import cli
+
+    parser = cli({})
+    parser.print_help()
+
+::
+
+    usage: ipython [-h]
+
+    optional arguments:
+    -h, --help  show this help message and exit
+
+
+Positional arguments
+--------------------
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "arguments": [
+            {
+                "name": "echo"
+            }
+        ]
+    }
+    parser = cli(data)
+    args = parser.parse_args(["foo"])
+
+::
+
+    In [11]: print(args.echo)
+    foo
+
+
+Positional arguments with type
+------------------------------
+
+When a type is specified, the argument will be treated as that type, otherwise it'll fail.
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "arguments": [
+            {
+                "name": "square",
+                "type": int
+            }
+        ]
+    }
+    parser = cli(data)
+    args = parser.parse_args(["1"])
+
+::
+
+    In [11]: print(args.echo)
+    1
+
+Optional arguments
+------------------
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "arguments": [
+            {
+                "name": "--verbose",
+                "help": "increase output verbosity"
+            }
+        ]
+    }
+    parser = cli(data)
+    args = parser.parse_args(["--verbosity 1"])
+
+::
+
+    In [11]: print(args.verbosity)
+    1
+
+    In [15]: args = parser.parse_args([])
+
+    In [16]: args
+    Out[16]: Namespace(verbose=None)
+
+
+Flags
+-----
+
+Flags are a boolean only (True/False) subset of options.
+
+.. code-block:: python
+
+    from decli import cli
+
+    data = {
+        "arguments": [
+            {
+                "name": "--verbose",
+                "action": "store_true",  # defaults to False
+            },
+            {
+                "name": "--noisy",
+                "action": "store_false",  # defaults to True
+            }
+        ]
+    }
+    parser = cli(data)
+
+
+
+
+Short options
+-------------
+
+Used to add short versions of the options.
+
+.. code-block:: python
+
+    data = {
+        "arguments": [
+            {
+                "name": ["-v", "--verbose"],
+                "help": "increase output verbosity"
+            }
+        ]
+    }
+
+
+Grouping
+--------
+
+This is only possible using **arguments**.
+
+Only affect the way the help gets displayed. You might be looking for subcommands.
+
+
+.. code-block:: python
+
+    data = {
+        "prog": "mycli",
+        "arguments": [
+            {
+                "name": "--save",
+                "group": "main",
+                "help": "This save belongs to the main group",
+            },
+            {
+                "name": "--remove",
+                "group": "main",
+                "help": "This remove belongs to the main group",
+            },
+        ],
+    }
+    parser = cli(data)
+    parser.print_help()
+
+::
+
+    usage: mycli [-h] [--save SAVE] [--remove REMOVE]
+
+    optional arguments:
+    -h, --help       show this help message and exit
+
+    main:
+    --save SAVE      This save belongs to the main group
+    --remove REMOVE  This remove belongs to the main group
+
+
+Exclusive group
+---------------
+
+This is only possible using **optional arguments**.
+
+
+.. code-block:: python
+
+    data = {
+        "prog": "mycli",
+        "arguments": [
+            {
+                "name": "--save",
+                "exclusive_group": "main",
+                "help": "This save belongs to the main group",
+            },
+            {
+                "name": "--remove",
+                "exclusive_group": "main",
+                "help": "This remove belongs to the main group",
+            },
+        ],
+    }
+    parser = cli(data)
+    parser.print_help()
+
+::
+
+    usage: mycli [-h] [--save SAVE | --remove REMOVE]
+
+    optional arguments:
+    -h, --help       show this help message and exit
+    --save SAVE      This save belongs to the main group
+    --remove REMOVE  This remove belongs to the main group
+
+
+Combining Positional and Optional arguments
+-------------------------------------------
+
+.. code-block:: python
+
+    data = {
+        "arguments": [
+            {
+                "name": "square",
+                "type": int,
+                "help": "display a square of a given number"
+            },
+            {
+                "name": ["-v", "--verbose"],
+                "action": "store_true",
+                "help": "increase output verbosity"
+            }
+        ]
+    }
+    parser = cli(data)
+
+    args = parser.parse_args()
+    answer = args.square**2
+    if args.verbose:
+        print(f"the square of {args.square} equals {answer}")
+    else:
+        print(answer)
+
+
+More Examples
+-------------
+
+Many examples from `argparse documentation <https://docs.python.org/3/library/argparse.html>`_
+are covered in test/examples.py
+
+
+Contributing
+============
+
+1. Clone the repo
+2. Install dependencies
+
+::
+
+    poetry install
+
+3. Run tests
+
+::
+
+    ./scripts/tests
+
+
+Contributing
+============
+
+**PRs are welcome!**
 
-setup(**setup_kwargs)
```

