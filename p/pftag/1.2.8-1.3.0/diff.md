# Comparing `tmp/pftag-1.2.8.tar.gz` & `tmp/pftag-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pftag-1.2.8.tar", last modified: Mon Mar 13 22:00:19 2023, max compression
+gzip compressed data, was "pftag-1.3.0.tar", last modified: Thu Apr 27 22:18:17 2023, max compression
```

## Comparing `pftag-1.2.8.tar` & `pftag-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-13 22:00:19.821119 pftag-1.2.8/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2023-03-08 20:28:33.000000 pftag-1.2.8/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    10934 2023-03-13 22:00:19.821119 pftag-1.2.8/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    10396 2023-03-12 21:32:10.000000 pftag-1.2.8/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-13 22:00:19.820119 pftag-1.2.8/pftag/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-08 20:28:33.000000 pftag-1.2.8/pftag/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    12404 2023-03-12 21:24:55.000000 pftag-1.2.8/pftag/__main__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4794 2023-03-08 20:57:30.000000 pftag-1.2.8/pftag/data.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    21172 2023-03-13 21:59:12.000000 pftag-1.2.8/pftag/pftag.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-13 22:00:19.821119 pftag-1.2.8/pftag.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    10934 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      268 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       46 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       62 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        6 2023-03-13 22:00:19.000000 pftag-1.2.8/pftag.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-03-13 22:00:19.821119 pftag-1.2.8/setup.cfg
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1774 2023-03-10 18:27:12.000000 pftag-1.2.8/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-04-27 22:18:17.465396 pftag-1.3.0/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2023-03-21 20:06:55.000000 pftag-1.3.0/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11681 2023-04-27 22:18:17.465396 pftag-1.3.0/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11163 2023-04-27 22:13:00.000000 pftag-1.3.0/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-04-27 22:18:17.465396 pftag-1.3.0/pftag/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-21 20:06:55.000000 pftag-1.3.0/pftag/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    13165 2023-04-27 22:02:51.000000 pftag-1.3.0/pftag/__main__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4833 2023-03-21 20:06:55.000000 pftag-1.3.0/pftag/data.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    23459 2023-04-27 21:57:13.000000 pftag-1.3.0/pftag/pftag.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-04-27 22:18:17.465396 pftag-1.3.0/pftag.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11681 2023-04-27 22:18:16.000000 pftag-1.3.0/pftag.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      268 2023-04-27 22:18:17.000000 pftag-1.3.0/pftag.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-04-27 22:18:16.000000 pftag-1.3.0/pftag.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       46 2023-04-27 22:18:17.000000 pftag-1.3.0/pftag.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       62 2023-04-27 22:18:17.000000 pftag-1.3.0/pftag.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        6 2023-04-27 22:18:17.000000 pftag-1.3.0/pftag.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-04-27 22:18:17.465396 pftag-1.3.0/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1774 2023-03-21 20:06:55.000000 pftag-1.3.0/setup.py
```

### Comparing `pftag-1.2.8/LICENSE` & `pftag-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pftag-1.2.8/PKG-INFO` & `pftag-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pftag
-Version: 1.2.8
+Version: 1.3.0
 Summary: A tag parser with optional functional support
 Home-page: https://github.com/FNNDSC/pftag
 Author: FNNDSC
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Provides-Extra: none
 Provides-Extra: dev
 License-File: LICENSE
@@ -59,32 +58,32 @@
 
 Runnning
 --------
 
 Script mode
 ~~~~~~~~~~~
 
-To use ``pftag`` in script mode you simply call the script with
-appropriate arguments
+To use ``pftag`` in script mode simply call the script with appropriate
+CLI arguments
 
 .. code:: bash
 
 
    pftag --tag "run-%timestamp-on-%platform-%arch.log"
 
    run-2023-03-10T13:41:58.921660-05:00-on-Linux-64bit-ELF.log
 
 Module mode
 ~~~~~~~~~~~
 
 There are several ways to use ``pftag`` in python module mode. Perhaps
 the simplest is just to declare an object and instantiate with an empty
-dictionary. Then call the object with the ``tag`` to process.
+dictionary, and then call the object with the ``tag`` to process.
 
-If you wanted to set any other values in the declaration, use an
+If additional values need to be set in the declaration, use an
 appropriate dictionary. The dictionary keys are *identical* to the
 script CLI keys (*sans* the leading ``--``):
 
 .. code:: python
 
    from pftag import pftag
 
@@ -109,14 +108,18 @@
    }
 
 .. code:: html
 
           --tag <tagString>
            The tag string to process.
 
+           [--lookupDictAdd <listOfDictionaryString>]
+           A string list of additional named lookup dictionary tags and values to
+           add.
+
            [--tagMarker <mark>]
            The marker string that identifies a tag (default "%")
 
            [--funcMarker <mark>]
            The marker string that pre- and post marks a function (default "_").
 
            [--funcArgMarker <mark>]
@@ -154,30 +157,46 @@
            [--debugPort <7900>]
            Debugging is via telnet session. This specifies the port on which the telnet
            session is listening.
 
 Available tags and functions
 ----------------------------
 
+Tags
+~~~~
+
+Additional tag lookup structures can be added with either the CLI or
+directory using the python API, for example:
+
 ::
 
-           TAGS
+   --lookupDictAdd '[{"secrets": {"CUBEuser": "rudolph", "CUBEpassword": "rudolph1234"}}]'
+
+The following tags are internal/reserved:
+
+::
 
                %literal   : simply replace the tag with the word 'literal'.
-                             This tag is only useful in conjunction with the
-                             'echo' function and together they provide a means
-                             to inject arbitary text typically for md5 hashing.
+                            This tag is only useful in conjunction with the
+                            'echo' function and together they provide a means
+                            to inject arbitary text typically for md5 hashing.
                %name      : return the os.name
                %platform  : return the platform.system()
                %release   : return the platform.release()
                %machine   : return the platform.machine()
                %arch      : return the '%s' % platform.architecture()
                %timestamp :  return the a timestamp
 
-           FUNCTIONS
+Functions
+~~~~~~~~~
+
+The lookup from any tagged string can be further processed by the
+following functions
+
+::
 
            md5|<chars>         : perform an md5hash on the upstream, limit result
                                  to <chars> characters
 
                                    eg: "%timestamp_md5|4_"
 
                                  replace the %timestamp in the input string with
@@ -187,107 +206,109 @@
 
                                    eg: "%timestamp_chrplc|:|-_"
 
                                  replace the %timestamp in the input string with
                                  the actual timestamp where all ":" are replaced with
                                  "-".
 
-           strmsk|<mask>       : for each '*' in mask pattern use upstream char
-                                 otherwise replace with <mask> char.
+           strmsk|<mask>       : for each '*' in mask pattern use ups tream char
+                                 otherwise replace with <mask> char .
 
                                    eg: "%platform_strmsk|l****_"
 
                                  replace the %platform in the input string with
                                  a string that starts with an 'l' and don't change
                                  the subsequent 4 characters. If the %platform
                                  has more than 4 characters, only return the 5
                                  chars as masked.
 
-           dcmname|<s>|<tail> : replace any upstream %VAR with a DICOM formatted
+           dcmname|<s>|<tail>  : replace any upstream %VAR with a DICOM formatted
                                  name. If <s> is passed, the seed the faker module
                                  with <s> (any string) -- this guarantees that calls
                                  with that same <s> result in the same name. If
                                  <tail> is passed, then append <tail> to the name.
 
                                    eg: %NAME_dcmname_
 
-                                may produce "BROOKS^JOHN". Each call will have
-                                a different name. However,
+                                 may produce "BROOKS^JOHN". Each call will have
+                                 a different name. However,
 
                                    %NAME_dcmname|foobar_
 
-                               will always generate "SCHWARTZ^THOMAS". While
+                                 will always generate "SCHWARTZ^THOMAS". While
 
                                    %NAME_dcmname|foobar|^ANON
 
-                               will generate "SCHWARTZ^THOMAS^ANON"
+                                 will generate "SCHWARTZ^THOMAS^ANON"
 
-           echo|<something> :  Best used with the %literal tag for legibility, will
-                               replace the tag with <something>. Be careful of commas
-                               in the <something>. If they are to be preserved you
-                               will need to set --funcSep to something other than a
-                               comma.
+           echo|<something>    : Best used with the %literal tag for legibility, will
+                                 replace the tag with <something>. Be careful of commas
+                                 in the <something>. If they are to be preserved you
+                                 will need to set --funcSep to something other than a
+                                 comma.
 
                                    %literal_echo|why-are-we-here?_
 
-                               will replace the %literal with "why-are-we-here".
-                               This is most useful when literal data is to obscured
-                               in a template. For instance:
+                                 will replace the %literal with "why-are-we-here".
+                                 This is most useful when literal data is to obscured
+                                 in a template. For instance:
 
                                    %literal_echo|Subject12345,md5|5_
 
-                               where say "Subject12345" is privileged information but
-                               important to add to the string. In this case, we can
-                               add and then hash that literal string. In future,
-                               if we know all the privileged strings, we can easily
-                               hash and then and lookup in any `pftag` generated
-                               strings to resolve which hashes belong to which
-                               subjects.
+                                 where say "Subject12345" is privileged information but
+                                 important to add to the string. In this case, we can
+                                 add and then hash that literal string. In future,
+                                 if we know all the privileged strings, we can easily
+                                 hash and then and lookup in any `pftag` generated
+                                 strings to resolve which hashes belong to which
+                                 subjects.
 
-Functions
----------
+Function detail
+---------------
 
 ::
 
        OVERVIEW
        In addition to performing a lookup on a template string token, this
        package can also process the lookup value in various ways. These
        process functions follow a Reverse Polish Notation (RPN) schema of
 
-           tag func1 func2 func3 ...
+           tag func1(args1) func2(args2) func3(args3) ...
 
        where first the <tag> is looked up, then this lookup is processed by
        <func1>. The result is then processed by <func2>, and so on and
-       so forth.
+       so forth, each functional optionally with a set a arguments.
 
        This RPN approach also mirrors the standard UNIX piping schema.
 
-       A function that is to be applied to a <tag> should be connected
-       to the tag with a <funcMarker> string, usually '_'. The final
-       function should end with the same <funcMarker>, so
-
-           %tag_func_
-
-       will apply the function called "func" to the tag called "tag".
+       A function (or function list) that is to be applied to a <tag> should
+       be connected to the tag with a <funcMarker> string, usually '_'. The
+       final function should end with the same <funcMarker>, so
+
+           %tag_func1,func2,...,funcN_
+
+       will apply the function list in order to the tag value lookup called
+       "tag"; each successive evaluation consuming the result of its
+       predecessor as input.
 
        Some functions can accept arguments. Arguments are passed to a function
        with a <funcArgMarker> string, typically '|', that also separates
        arguments:
 
            %tag_func|a1|a2|a3_
 
        will pass 'a1', 'a2', and 'a3' as parameters to "func".
 
        Finally, several functions can be chained within the '_'...'_' by
-       separating the <func>|<argList> constructs with commas, so
+       separating the <func>|<argList> constructs with commas, so pedantically
 
-           %tag_func|a1|a2|a3,func2|b1|b2|b3_
+           %tag_func1|a1|a2|a3,func2|b1|b2|b3_
 
        All these special characters (tag marker, function pre- and post,
-       arg separation, fand unction separation can be overriden. For instance,
+       arg separation, function separation can be overriden. For instance,
        with a selection of
 
        --tagMarker "@" --funcMarker "[" --funcArgMarker "," --funcSep "|"
 
        strings can be specified as
 
            @tag[func,a1,a2,a3|func2,b1,b2,b3[
@@ -305,24 +326,22 @@
 ``Env.set_trace()`` calls where appropriate. These can remain in the
 codebase (i.e. you don’t need to delete/comment them out) since they are
 only *live* when a ``--debug`` flag is passed.
 
 Testing
 ~~~~~~~
 
-Run unit tests using ``pytest``
+Run unit tests using ``pytest``.
 
 .. code:: bash
 
    # In repo root dir:
    pytest
 
 *-30-*
 
 .. |Version| image:: https://img.shields.io/docker/v/fnndsc/pftag?sort=semver
    :target: https://hub.docker.com/r/fnndsc/pftag
 .. |MIT License| image:: https://img.shields.io/github/license/fnndsc/pftag
    :target: https://github.com/FNNDSC/pftag/blob/main/LICENSE
-.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/ci.yml/badge.svg
+.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/build.yml/badge.svg
    :target: https://github.com/FNNDSC/pftag/actions/workflows/build.yml
-
-
```

### Comparing `pftag-1.2.8/README.rst` & `pftag-1.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,32 +42,32 @@
 
 Runnning
 --------
 
 Script mode
 ~~~~~~~~~~~
 
-To use ``pftag`` in script mode you simply call the script with
-appropriate arguments
+To use ``pftag`` in script mode simply call the script with appropriate
+CLI arguments
 
 .. code:: bash
 
 
    pftag --tag "run-%timestamp-on-%platform-%arch.log"
 
    run-2023-03-10T13:41:58.921660-05:00-on-Linux-64bit-ELF.log
 
 Module mode
 ~~~~~~~~~~~
 
 There are several ways to use ``pftag`` in python module mode. Perhaps
 the simplest is just to declare an object and instantiate with an empty
-dictionary. Then call the object with the ``tag`` to process.
+dictionary, and then call the object with the ``tag`` to process.
 
-If you wanted to set any other values in the declaration, use an
+If additional values need to be set in the declaration, use an
 appropriate dictionary. The dictionary keys are *identical* to the
 script CLI keys (*sans* the leading ``--``):
 
 .. code:: python
 
    from pftag import pftag
 
@@ -92,14 +92,18 @@
    }
 
 .. code:: html
 
           --tag <tagString>
            The tag string to process.
 
+           [--lookupDictAdd <listOfDictionaryString>]
+           A string list of additional named lookup dictionary tags and values to
+           add.
+
            [--tagMarker <mark>]
            The marker string that identifies a tag (default "%")
 
            [--funcMarker <mark>]
            The marker string that pre- and post marks a function (default "_").
 
            [--funcArgMarker <mark>]
@@ -137,30 +141,46 @@
            [--debugPort <7900>]
            Debugging is via telnet session. This specifies the port on which the telnet
            session is listening.
 
 Available tags and functions
 ----------------------------
 
+Tags
+~~~~
+
+Additional tag lookup structures can be added with either the CLI or
+directory using the python API, for example:
+
 ::
 
-           TAGS
+   --lookupDictAdd '[{"secrets": {"CUBEuser": "rudolph", "CUBEpassword": "rudolph1234"}}]'
+
+The following tags are internal/reserved:
+
+::
 
                %literal   : simply replace the tag with the word 'literal'.
-                             This tag is only useful in conjunction with the
-                             'echo' function and together they provide a means
-                             to inject arbitary text typically for md5 hashing.
+                            This tag is only useful in conjunction with the
+                            'echo' function and together they provide a means
+                            to inject arbitary text typically for md5 hashing.
                %name      : return the os.name
                %platform  : return the platform.system()
                %release   : return the platform.release()
                %machine   : return the platform.machine()
                %arch      : return the '%s' % platform.architecture()
                %timestamp :  return the a timestamp
 
-           FUNCTIONS
+Functions
+~~~~~~~~~
+
+The lookup from any tagged string can be further processed by the
+following functions
+
+::
 
            md5|<chars>         : perform an md5hash on the upstream, limit result
                                  to <chars> characters
 
                                    eg: "%timestamp_md5|4_"
 
                                  replace the %timestamp in the input string with
@@ -170,107 +190,109 @@
 
                                    eg: "%timestamp_chrplc|:|-_"
 
                                  replace the %timestamp in the input string with
                                  the actual timestamp where all ":" are replaced with
                                  "-".
 
-           strmsk|<mask>       : for each '*' in mask pattern use upstream char
-                                 otherwise replace with <mask> char.
+           strmsk|<mask>       : for each '*' in mask pattern use ups tream char
+                                 otherwise replace with <mask> char .
 
                                    eg: "%platform_strmsk|l****_"
 
                                  replace the %platform in the input string with
                                  a string that starts with an 'l' and don't change
                                  the subsequent 4 characters. If the %platform
                                  has more than 4 characters, only return the 5
                                  chars as masked.
 
-           dcmname|<s>|<tail> : replace any upstream %VAR with a DICOM formatted
+           dcmname|<s>|<tail>  : replace any upstream %VAR with a DICOM formatted
                                  name. If <s> is passed, the seed the faker module
                                  with <s> (any string) -- this guarantees that calls
                                  with that same <s> result in the same name. If
                                  <tail> is passed, then append <tail> to the name.
 
                                    eg: %NAME_dcmname_
 
-                                may produce "BROOKS^JOHN". Each call will have
-                                a different name. However,
+                                 may produce "BROOKS^JOHN". Each call will have
+                                 a different name. However,
 
                                    %NAME_dcmname|foobar_
 
-                               will always generate "SCHWARTZ^THOMAS". While
+                                 will always generate "SCHWARTZ^THOMAS". While
 
                                    %NAME_dcmname|foobar|^ANON
 
-                               will generate "SCHWARTZ^THOMAS^ANON"
+                                 will generate "SCHWARTZ^THOMAS^ANON"
 
-           echo|<something> :  Best used with the %literal tag for legibility, will
-                               replace the tag with <something>. Be careful of commas
-                               in the <something>. If they are to be preserved you
-                               will need to set --funcSep to something other than a
-                               comma.
+           echo|<something>    : Best used with the %literal tag for legibility, will
+                                 replace the tag with <something>. Be careful of commas
+                                 in the <something>. If they are to be preserved you
+                                 will need to set --funcSep to something other than a
+                                 comma.
 
                                    %literal_echo|why-are-we-here?_
 
-                               will replace the %literal with "why-are-we-here".
-                               This is most useful when literal data is to obscured
-                               in a template. For instance:
+                                 will replace the %literal with "why-are-we-here".
+                                 This is most useful when literal data is to obscured
+                                 in a template. For instance:
 
                                    %literal_echo|Subject12345,md5|5_
 
-                               where say "Subject12345" is privileged information but
-                               important to add to the string. In this case, we can
-                               add and then hash that literal string. In future,
-                               if we know all the privileged strings, we can easily
-                               hash and then and lookup in any `pftag` generated
-                               strings to resolve which hashes belong to which
-                               subjects.
+                                 where say "Subject12345" is privileged information but
+                                 important to add to the string. In this case, we can
+                                 add and then hash that literal string. In future,
+                                 if we know all the privileged strings, we can easily
+                                 hash and then and lookup in any `pftag` generated
+                                 strings to resolve which hashes belong to which
+                                 subjects.
 
-Functions
----------
+Function detail
+---------------
 
 ::
 
        OVERVIEW
        In addition to performing a lookup on a template string token, this
        package can also process the lookup value in various ways. These
        process functions follow a Reverse Polish Notation (RPN) schema of
 
-           tag func1 func2 func3 ...
+           tag func1(args1) func2(args2) func3(args3) ...
 
        where first the <tag> is looked up, then this lookup is processed by
        <func1>. The result is then processed by <func2>, and so on and
-       so forth.
+       so forth, each functional optionally with a set a arguments.
 
        This RPN approach also mirrors the standard UNIX piping schema.
 
-       A function that is to be applied to a <tag> should be connected
-       to the tag with a <funcMarker> string, usually '_'. The final
-       function should end with the same <funcMarker>, so
-
-           %tag_func_
-
-       will apply the function called "func" to the tag called "tag".
+       A function (or function list) that is to be applied to a <tag> should
+       be connected to the tag with a <funcMarker> string, usually '_'. The
+       final function should end with the same <funcMarker>, so
+
+           %tag_func1,func2,...,funcN_
+
+       will apply the function list in order to the tag value lookup called
+       "tag"; each successive evaluation consuming the result of its
+       predecessor as input.
 
        Some functions can accept arguments. Arguments are passed to a function
        with a <funcArgMarker> string, typically '|', that also separates
        arguments:
 
            %tag_func|a1|a2|a3_
 
        will pass 'a1', 'a2', and 'a3' as parameters to "func".
 
        Finally, several functions can be chained within the '_'...'_' by
-       separating the <func>|<argList> constructs with commas, so
+       separating the <func>|<argList> constructs with commas, so pedantically
 
-           %tag_func|a1|a2|a3,func2|b1|b2|b3_
+           %tag_func1|a1|a2|a3,func2|b1|b2|b3_
 
        All these special characters (tag marker, function pre- and post,
-       arg separation, fand unction separation can be overriden. For instance,
+       arg separation, function separation can be overriden. For instance,
        with a selection of
 
        --tagMarker "@" --funcMarker "[" --funcArgMarker "," --funcSep "|"
 
        strings can be specified as
 
            @tag[func,a1,a2,a3|func2,b1,b2,b3[
@@ -288,22 +310,22 @@
 ``Env.set_trace()`` calls where appropriate. These can remain in the
 codebase (i.e. you don’t need to delete/comment them out) since they are
 only *live* when a ``--debug`` flag is passed.
 
 Testing
 ~~~~~~~
 
-Run unit tests using ``pytest``
+Run unit tests using ``pytest``.
 
 .. code:: bash
 
    # In repo root dir:
    pytest
 
 *-30-*
 
 .. |Version| image:: https://img.shields.io/docker/v/fnndsc/pftag?sort=semver
    :target: https://hub.docker.com/r/fnndsc/pftag
 .. |MIT License| image:: https://img.shields.io/github/license/fnndsc/pftag
    :target: https://github.com/FNNDSC/pftag/blob/main/LICENSE
-.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/ci.yml/badge.svg
+.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/build.yml/badge.svg
    :target: https://github.com/FNNDSC/pftag/actions/workflows/build.yml
```

### Comparing `pftag-1.2.8/pftag/__main__.py` & `pftag-1.3.0/pftag/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from importlib.metadata import Distribution
 
 __pkg       = Distribution.from_name(__package__)
 __version__ = __pkg.version
 
 import  os, sys, json
+os.environ['XDG_CONFIG_HOME'] = '/tmp'
 import  pudb
 from    pudb.remote             import set_trace
 from    pftag.pftag             import parser_setup, parser_interpret, parser_JSONinterpret
 
 
 DISPLAY_TITLE = r"""
 
@@ -42,14 +43,15 @@
         package provides both a CLI client as well as a python module.
 
 
 """
 
 package_CLIself:str         = """
         --tag <tagString>                                                       \\
+        [--lookupDictAdd <listOfDictionaryString>]                              \\
         [--tagMarker <mark>]                                                    \\
         [--funcMarker <mark>]                                                   \\
         [--funcArgMarker <mark>]                                                \\
         [--funcSep <mark>]                                                      \\
         [--inputdir <inputdir>]                                                 \\
         [--outputdir <outputdir>]                                               \\
         [--man]                                                                 \\
@@ -61,14 +63,18 @@
 
 package_CLIsynpsisArgs:str  = """
     ARGUMENTS
 
         --tag <tagString>
         The tag string to process.
 
+        [--lookupDictAdd <listOfDictionaryString>]
+        A string list of additional named lookup dictionary tags and values to
+        add.
+
         [--tagMarker <mark>]
         The marker string that identifies a tag (default "%")
 
         [--funcMarker <mark>]
         The marker string that pre- and post marks a function (default "_").
 
         [--funcArgMarker <mark>]
@@ -163,28 +169,38 @@
 """
 
 
 package_CLItagsFuncs:str = r"""
 
         AVAILABLE TAGS AND FUNCTIONS
 
+        Additional tag lookup structures can be added with either the CLI
+        or directory using the python API:
+
+        --lookupDictAdd '[{"secrets": {"CUBEuser": "rudolph", "CUBEpassword": "rudolph1234"}}]'
+
+        will add a new named lookup group called 'secrets' with tags %CUBEuser
+        and %CUBEpassword, substituted in string tags with the values as
+        shown. Any of these new tag lookups can be further processed by
+        internal functions.
+
         The following tags are available:
 
             %literal   : simply replace the tag with the word 'literal'.
                           This tag is only useful in conjunction with the
                           'echo' function and together they provide a means
                           to inject arbitary text typically for md5 hashing.
             %name      : return the os.name
             %platform  : return the platform.system()
             %release   : return the platform.release()
             %machine   : return the platform.machine()
             %arch      : return the '%s' % platform.architecture()
             %timestamp :  return the a timestamp
 
-        The following tags are available:
+        The following functions are available:
 
         md5|<chars>         : perform an md5hash on the upstream, limit result
                               to <chars> characters
 
                                 eg: "%timestamp_md5|4_"
 
                               replace the %timestamp in the input string with
@@ -328,13 +344,13 @@
 
     # any reason we should not continue?
     if earlyExit_check(options): return 1
 
     # set_trace(term_size=(253, 62), host = '0.0.0.0', port = 7900)
     tag:pftag.Pftag         = pftag.Pftag(options)
     d_pftag:dict            = tag.run(options.tag)
-    print(d_pftag['result'])
+    if d_pftag['status']: print(d_pftag['result'])
 
     return 0 if d_pftag['status'] else 2
 
 if __name__ == '__main__':
     sys.exit(main(sys.argv))
```

### Comparing `pftag-1.2.8/pftag/data.py` & `pftag-1.3.0/pftag/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 str_about = '''
     This module is responsible for handling some state related information
     which is mostly information about the pftel server.
 
     Core data includes information on the server (address) as well as
     possible future WIP for authentication/etc
 '''
+import  os
+os.environ['XDG_CONFIG_HOME'] = '/tmp'
 
 from    pudb.remote             import set_trace
 from    curses                  import meta
 from    pathlib                 import Path
 from    argparse                import Namespace
 from    loguru                  import logger
 import  pudb
 import  json
-import  os
 import  inspect
 import  sys
 
 logger_format = (
     "<green>{time:YYYY-MM-DD HH:mm:ss}</green> │ "
     "<level>{level: <5}</level> │ "
     "<yellow>{name: >28}</yellow>::"
```

### Comparing `pftag-1.2.8/pftag/pftag.py` & `pftag-1.3.0/pftag/pftag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
-__version__ = '1.2.8'
-
+__version__ = '1.3.0'
 from    pathlib                 import Path
 
 import  os, sys, json, platform, re
+os.environ['XDG_CONFIG_HOME'] = '/tmp'
+
 import  pudb
 from    pudb.remote             import set_trace
 
 from    concurrent.futures      import ThreadPoolExecutor
 from    threading               import current_thread
 
 from    datetime                import datetime, timezone
@@ -69,14 +70,19 @@
     )
     parser.add_argument(
                 '--outputdir',
                 default = './',
                 help    = 'optional directory specifying location of any output data'
     )
     parser.add_argument(
+                '--lookupDictAdd',
+                default = '',
+                help    = 'simple named dictionary lookups'
+    )
+    parser.add_argument(
                 '--tag',
                 default = '',
                 help    = 'tag string to process'
     )
     parser.add_argument(
                 '--tagMarker',
                 default = '%',
@@ -169,17 +175,14 @@
         self.env.outputdir      = options.outputdir
         self.env.debug_setup(
                     debug       = options.debug,
                     termsize    = options.debugTermSize,
                     port        = options.debugPort,
                     host        = options.debugHost
         )
-        # if not len(options.tag):
-        #     self.env.ERROR("The '--tag <tag>' CLI MUST be specified!")
-        #     status              = False
         return status
 
     def __init__(self, options, *args, **kwargs):
         """
         constructor
 
         Responsible primarily for setting up the client connection
@@ -196,14 +199,25 @@
                            'platform',
                            'release',
                            'machine',
                            'arch',
                            'timestamp']
         }
 
+        # Simple lookup structures/handling. These two dictionaries
+        # house "simple" lookup tag structures. A "simple" lookup is
+        # a named dictionary whose keys are the tags, and whose values
+        # are the lookup results.
+        #
+        # Typically, these are passed in the CLI --lookupDictAdd value.
+        self.d_tagSimpleLookupKeys:dict[str, list[str]]         = {
+        }
+        self.d_tagSimpleLookupData:dict[str, dict]              = {
+        }
+
         # If the <options> is a dictionary, then we interpret this as if
         # it were the CLI (instead of the real CLI) and convert to a
         # namespace
         if type(options) is dict:
             parser:ArgumentParser           = parser_setup('Setup client using dict')
             options:Namespace               = parser_JSONinterpret(parser, options)
         if type(options) is Namespace:
@@ -214,14 +228,24 @@
             self.env.ERROR("Env setup failure, exiting...")
             self.envOK                  = False
         self.str_tagMarker:str              = options.tagMarker     # '%
         self.str_funcMarker:str             = options.funcMarker    # '_'
         self.str_funcArgSep:str             = options.funcArgMarker # '|'
         self.str_funcSep:str                = options.funcSep       # ','
 
+        # Check for successful addition of possible external lists of dictionary
+        # tags
+        if self.options.lookupDictAdd:
+            self.envOK = all([list(x.values())[0] \
+                                for x in \
+                                    list(self.newLookupDictionary_add(
+                                        self.options.lookupDictAdd)
+                                    )
+                            ])
+
         self.env_show()
 
     def env_show(self) -> None:
         """
         Perform some setup
 
         Args:
@@ -240,17 +264,45 @@
 
         if self.options.osenv:
             self.self.env.DEBUG("base environment...")
             for k,v in os.environ.items():
                 self.self.env.DEBUG("%25s:  [%s]" % (k, v), level = 3)
             self.self.env.DEBUG("")
 
+    def newLookupDictionary_add(self, ld_data:list[dict]) -> list[bool]:
+        """
+        Add new "named" lookup tag dictionary values
+
+        Args:
+            ld_data (list[dict]): a list of named dictionaries with
+                                  lookup key/value tags
+
+        Returns:
+            bool (list[bool]): for each group, a bool status dictionary
+        """
+        try:
+            ld_data = json.loads(ld_data)
+        except:
+            pass
+        lb_status:list[dict]    = []
+        l_keys:list     = [list(x.keys())[0]    for x in ld_data]
+        l_lookups:list  = [list(x.values())[0]  for x in ld_data]
+        l_tags:list     = [list(y.keys())       for y in l_lookups]
+        for group,tags,data in zip(l_keys, l_tags, l_lookups):
+            try:
+                self.d_tagSimpleLookupKeys[group] = tags
+                self.d_tagSimpleLookupData[group] = data
+                lb_status.append({group: True})
+            except:
+                lb_status.append({group: False})
+        return lb_status
+
     def tag_findDict(self, tag:str) -> List[Tuple]:
         """
-        For a given <tag> superstring, determine if any reserved dictionaries
+        For a given <tag> superstring, determine if any internal dictionaries
         contain a token within the <tag>. If found, add the dictionary name and
         token to a tuple list, and eventually return a list of tuples of
         (<dict>, <tag>) containing hits.
 
         For example, imagine that the string to analyze is
 
                 %platform-name-os
@@ -271,19 +323,20 @@
             and tag within that dictionary
         """
         T:str                   = self.str_tagMarker
         l_tagPossibilities:list = []    # Is the tag in one of the possible dictionaries?
         l_tagHit:list           = []    # Which tag, *exactly*, is sought in the possibilities?
         tagHit:str              = ''    # This is it!
         l_tagDict:list          = []    # A list of tuples of (<dict>, <tag>)
-        for d in list(self.d_tagReserved.keys()):
-            l_tagPossibilities:list     = [i for i in self.d_tagReserved[d] if i in tag]
-            l_tagHit:list               = [i for i in l_tagPossibilities if f'{T}'+i in f'{T}'+tag]
-            tagHit:str                  = l_tagHit[0] if len(l_tagHit) else ''
-            if tagHit:                  l_tagDict.append( (d, tagHit) )
+        for group in [self.d_tagReserved, self.d_tagSimpleLookupKeys]:
+            for d in list(group.keys()):
+                l_tagPossibilities:list     = [i for i in group[d] if i in tag]
+                l_tagHit:list               = [i for i in l_tagPossibilities if f'{T}'+i in f'{T}'+tag]
+                tagHit:str                  = l_tagHit[0] if len(l_tagHit) else ''
+                if tagHit:                  l_tagDict.append( (d, tagHit) )
         return l_tagDict
 
     def tag_lookupCore(self, tag:str) -> str:
         """Lookup a tag in the "core" dictionary.
 
         Args:
             tag (str): the tag to lookup
@@ -313,18 +366,18 @@
         Args:
             tagTuple (tuple): a tuple of <dictionaryName> and <tag> to lookup
 
         Returns:
             str: the lookup value for the <tag>
         """
         lookup:str  = ""
-        if 'core' in tagTuple[0]: lookup = self.tag_lookupCore(tagTuple[1])
-        # match tagTuple[0]:
-        #     case 'core':
-        #         lookup  = self.tag_lookupCore(tagTuple[1])
+        if 'core' in tagTuple[0]:
+            lookup = self.tag_lookupCore(tagTuple[1])
+        if tagTuple[0] in list(self.d_tagSimpleLookupKeys.keys()):
+            lookup  = self.d_tagSimpleLookupData[tagTuple[0]][tagTuple[1]]
         return lookup
 
     def tag_process(self, astr:str, *args, **kwargs):
         """
         This method processes a string that contains "%<tag>" tokens in a
         variety of ways. Various %<tags> are understood, for example:
 
@@ -477,15 +530,15 @@
         tag:str                 = ''        # the tag in the funcTag combo
         result:str              = ''        # result of any applied function
         prevResult:str          = ''        # previous function stack result
         tagLookup:str           = ''        # the lookup value for the tag
         d_ret:dict[str, Any]    = {
             'status':           False,
             'funcApplied':      [],
-            'result':           ""
+            'result':           astr
         }
         T:str                   = self.str_tagMarker
         F:str                   = self.str_funcMarker
         S:str                   = self.str_funcSep
 
         if not f'{T}' in astr: return d_ret
         d_ret['status']     = True
@@ -548,8 +601,14 @@
 
     Args:
         str_datetime (str): a string generated by %timestamp
 
     Returns:
         datetime: a datetime object of the input
     """
-    return datetime.strptime(str_datetime, '%Y-%m-%dT%H:%M:%S.%f%z')
+    dt:datetime     = None
+    try:
+        dt = datetime.strptime(str_datetime, '%Y-%m-%dT%H:%M:%S.%f%z')
+    except:
+        # py36 backwards compatibility
+        dt = datetime.strptime(str_datetime[:-6], '%Y-%m-%dT%H:%M:%S.%f')
+    return dt
```

### Comparing `pftag-1.2.8/pftag.egg-info/PKG-INFO` & `pftag-1.3.0/pftag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pftag
-Version: 1.2.8
+Version: 1.3.0
 Summary: A tag parser with optional functional support
 Home-page: https://github.com/FNNDSC/pftag
 Author: FNNDSC
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Provides-Extra: none
 Provides-Extra: dev
 License-File: LICENSE
@@ -59,32 +58,32 @@
 
 Runnning
 --------
 
 Script mode
 ~~~~~~~~~~~
 
-To use ``pftag`` in script mode you simply call the script with
-appropriate arguments
+To use ``pftag`` in script mode simply call the script with appropriate
+CLI arguments
 
 .. code:: bash
 
 
    pftag --tag "run-%timestamp-on-%platform-%arch.log"
 
    run-2023-03-10T13:41:58.921660-05:00-on-Linux-64bit-ELF.log
 
 Module mode
 ~~~~~~~~~~~
 
 There are several ways to use ``pftag`` in python module mode. Perhaps
 the simplest is just to declare an object and instantiate with an empty
-dictionary. Then call the object with the ``tag`` to process.
+dictionary, and then call the object with the ``tag`` to process.
 
-If you wanted to set any other values in the declaration, use an
+If additional values need to be set in the declaration, use an
 appropriate dictionary. The dictionary keys are *identical* to the
 script CLI keys (*sans* the leading ``--``):
 
 .. code:: python
 
    from pftag import pftag
 
@@ -109,14 +108,18 @@
    }
 
 .. code:: html
 
           --tag <tagString>
            The tag string to process.
 
+           [--lookupDictAdd <listOfDictionaryString>]
+           A string list of additional named lookup dictionary tags and values to
+           add.
+
            [--tagMarker <mark>]
            The marker string that identifies a tag (default "%")
 
            [--funcMarker <mark>]
            The marker string that pre- and post marks a function (default "_").
 
            [--funcArgMarker <mark>]
@@ -154,30 +157,46 @@
            [--debugPort <7900>]
            Debugging is via telnet session. This specifies the port on which the telnet
            session is listening.
 
 Available tags and functions
 ----------------------------
 
+Tags
+~~~~
+
+Additional tag lookup structures can be added with either the CLI or
+directory using the python API, for example:
+
 ::
 
-           TAGS
+   --lookupDictAdd '[{"secrets": {"CUBEuser": "rudolph", "CUBEpassword": "rudolph1234"}}]'
+
+The following tags are internal/reserved:
+
+::
 
                %literal   : simply replace the tag with the word 'literal'.
-                             This tag is only useful in conjunction with the
-                             'echo' function and together they provide a means
-                             to inject arbitary text typically for md5 hashing.
+                            This tag is only useful in conjunction with the
+                            'echo' function and together they provide a means
+                            to inject arbitary text typically for md5 hashing.
                %name      : return the os.name
                %platform  : return the platform.system()
                %release   : return the platform.release()
                %machine   : return the platform.machine()
                %arch      : return the '%s' % platform.architecture()
                %timestamp :  return the a timestamp
 
-           FUNCTIONS
+Functions
+~~~~~~~~~
+
+The lookup from any tagged string can be further processed by the
+following functions
+
+::
 
            md5|<chars>         : perform an md5hash on the upstream, limit result
                                  to <chars> characters
 
                                    eg: "%timestamp_md5|4_"
 
                                  replace the %timestamp in the input string with
@@ -187,107 +206,109 @@
 
                                    eg: "%timestamp_chrplc|:|-_"
 
                                  replace the %timestamp in the input string with
                                  the actual timestamp where all ":" are replaced with
                                  "-".
 
-           strmsk|<mask>       : for each '*' in mask pattern use upstream char
-                                 otherwise replace with <mask> char.
+           strmsk|<mask>       : for each '*' in mask pattern use ups tream char
+                                 otherwise replace with <mask> char .
 
                                    eg: "%platform_strmsk|l****_"
 
                                  replace the %platform in the input string with
                                  a string that starts with an 'l' and don't change
                                  the subsequent 4 characters. If the %platform
                                  has more than 4 characters, only return the 5
                                  chars as masked.
 
-           dcmname|<s>|<tail> : replace any upstream %VAR with a DICOM formatted
+           dcmname|<s>|<tail>  : replace any upstream %VAR with a DICOM formatted
                                  name. If <s> is passed, the seed the faker module
                                  with <s> (any string) -- this guarantees that calls
                                  with that same <s> result in the same name. If
                                  <tail> is passed, then append <tail> to the name.
 
                                    eg: %NAME_dcmname_
 
-                                may produce "BROOKS^JOHN". Each call will have
-                                a different name. However,
+                                 may produce "BROOKS^JOHN". Each call will have
+                                 a different name. However,
 
                                    %NAME_dcmname|foobar_
 
-                               will always generate "SCHWARTZ^THOMAS". While
+                                 will always generate "SCHWARTZ^THOMAS". While
 
                                    %NAME_dcmname|foobar|^ANON
 
-                               will generate "SCHWARTZ^THOMAS^ANON"
+                                 will generate "SCHWARTZ^THOMAS^ANON"
 
-           echo|<something> :  Best used with the %literal tag for legibility, will
-                               replace the tag with <something>. Be careful of commas
-                               in the <something>. If they are to be preserved you
-                               will need to set --funcSep to something other than a
-                               comma.
+           echo|<something>    : Best used with the %literal tag for legibility, will
+                                 replace the tag with <something>. Be careful of commas
+                                 in the <something>. If they are to be preserved you
+                                 will need to set --funcSep to something other than a
+                                 comma.
 
                                    %literal_echo|why-are-we-here?_
 
-                               will replace the %literal with "why-are-we-here".
-                               This is most useful when literal data is to obscured
-                               in a template. For instance:
+                                 will replace the %literal with "why-are-we-here".
+                                 This is most useful when literal data is to obscured
+                                 in a template. For instance:
 
                                    %literal_echo|Subject12345,md5|5_
 
-                               where say "Subject12345" is privileged information but
-                               important to add to the string. In this case, we can
-                               add and then hash that literal string. In future,
-                               if we know all the privileged strings, we can easily
-                               hash and then and lookup in any `pftag` generated
-                               strings to resolve which hashes belong to which
-                               subjects.
+                                 where say "Subject12345" is privileged information but
+                                 important to add to the string. In this case, we can
+                                 add and then hash that literal string. In future,
+                                 if we know all the privileged strings, we can easily
+                                 hash and then and lookup in any `pftag` generated
+                                 strings to resolve which hashes belong to which
+                                 subjects.
 
-Functions
----------
+Function detail
+---------------
 
 ::
 
        OVERVIEW
        In addition to performing a lookup on a template string token, this
        package can also process the lookup value in various ways. These
        process functions follow a Reverse Polish Notation (RPN) schema of
 
-           tag func1 func2 func3 ...
+           tag func1(args1) func2(args2) func3(args3) ...
 
        where first the <tag> is looked up, then this lookup is processed by
        <func1>. The result is then processed by <func2>, and so on and
-       so forth.
+       so forth, each functional optionally with a set a arguments.
 
        This RPN approach also mirrors the standard UNIX piping schema.
 
-       A function that is to be applied to a <tag> should be connected
-       to the tag with a <funcMarker> string, usually '_'. The final
-       function should end with the same <funcMarker>, so
-
-           %tag_func_
-
-       will apply the function called "func" to the tag called "tag".
+       A function (or function list) that is to be applied to a <tag> should
+       be connected to the tag with a <funcMarker> string, usually '_'. The
+       final function should end with the same <funcMarker>, so
+
+           %tag_func1,func2,...,funcN_
+
+       will apply the function list in order to the tag value lookup called
+       "tag"; each successive evaluation consuming the result of its
+       predecessor as input.
 
        Some functions can accept arguments. Arguments are passed to a function
        with a <funcArgMarker> string, typically '|', that also separates
        arguments:
 
            %tag_func|a1|a2|a3_
 
        will pass 'a1', 'a2', and 'a3' as parameters to "func".
 
        Finally, several functions can be chained within the '_'...'_' by
-       separating the <func>|<argList> constructs with commas, so
+       separating the <func>|<argList> constructs with commas, so pedantically
 
-           %tag_func|a1|a2|a3,func2|b1|b2|b3_
+           %tag_func1|a1|a2|a3,func2|b1|b2|b3_
 
        All these special characters (tag marker, function pre- and post,
-       arg separation, fand unction separation can be overriden. For instance,
+       arg separation, function separation can be overriden. For instance,
        with a selection of
 
        --tagMarker "@" --funcMarker "[" --funcArgMarker "," --funcSep "|"
 
        strings can be specified as
 
            @tag[func,a1,a2,a3|func2,b1,b2,b3[
@@ -305,24 +326,22 @@
 ``Env.set_trace()`` calls where appropriate. These can remain in the
 codebase (i.e. you don’t need to delete/comment them out) since they are
 only *live* when a ``--debug`` flag is passed.
 
 Testing
 ~~~~~~~
 
-Run unit tests using ``pytest``
+Run unit tests using ``pytest``.
 
 .. code:: bash
 
    # In repo root dir:
    pytest
 
 *-30-*
 
 .. |Version| image:: https://img.shields.io/docker/v/fnndsc/pftag?sort=semver
    :target: https://hub.docker.com/r/fnndsc/pftag
 .. |MIT License| image:: https://img.shields.io/github/license/fnndsc/pftag
    :target: https://github.com/FNNDSC/pftag/blob/main/LICENSE
-.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/ci.yml/badge.svg
+.. |ci| image:: https://github.com/FNNDSC/pftag/actions/workflows/build.yml/badge.svg
    :target: https://github.com/FNNDSC/pftag/actions/workflows/build.yml
-
-
```

### Comparing `pftag-1.2.8/setup.py` & `pftag-1.3.0/setup.py`

 * *Files identical despite different names*

