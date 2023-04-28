# Comparing `tmp/saspy-5.1.0.tar.gz` & `tmp/saspy-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.1.0.tar", last modified: Fri Apr 14 17:59:53 2023, max compression
+gzip compressed data, was "saspy-5.1.2.tar", last modified: Fri Apr 28 14:58:16 2023, max compression
```

## Comparing `saspy-5.1.0.tar` & `saspy-5.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.952901 saspy-5.1.0/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-04-14 17:59:34.000000 saspy-5.1.0/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-04-14 17:59:34.000000 saspy-5.1.0/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-14 17:59:53.951901 saspy-5.1.0/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-04-14 17:59:34.000000 saspy-5.1.0/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-04-14 17:59:34.000000 saspy-5.1.0/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.923900 saspy-5.1.0/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.925900 saspy-5.1.0/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.938901 saspy-5.1.0/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.942901 saspy-5.1.0/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.950901 saspy-5.1.0/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   130256 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    84218 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    99383 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.951901 saspy-5.1.0/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-04-14 17:59:34.000000 saspy-5.1.0/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-14 17:59:53.925900 saspy-5.1.0/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-04-14 17:59:53.000000 saspy-5.1.0/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-04-14 17:59:53.952901 saspy-5.1.0/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-04-14 17:59:34.000000 saspy-5.1.0/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.845075 saspy-5.1.2/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-04-28 14:58:04.000000 saspy-5.1.2/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-04-28 14:58:04.000000 saspy-5.1.2/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-28 14:58:16.845075 saspy-5.1.2/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-04-28 14:58:04.000000 saspy-5.1.2/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-04-28 14:58:04.000000 saspy-5.1.2/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.819074 saspy-5.1.2/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.821074 saspy-5.1.2/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.832074 saspy-5.1.2/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.836075 saspy-5.1.2/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.844076 saspy-5.1.2/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   130256 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    84218 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    87068 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    99701 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.844076 saspy-5.1.2/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-04-28 14:58:04.000000 saspy-5.1.2/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-04-28 14:58:16.820073 saspy-5.1.2/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-04-28 14:58:16.000000 saspy-5.1.2/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-04-28 14:58:16.845075 saspy-5.1.2/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-04-28 14:58:04.000000 saspy-5.1.2/setup.py
```

### Comparing `saspy-5.1.0/LICENSE.md` & `saspy-5.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/PKG-INFO` & `saspy-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.1.0
+Version: 5.1.2
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.1.0/README.md` & `saspy-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/SASLogLexer.py` & `saspy-5.1.2/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/__init__.py` & `saspy-5.1.2/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/autocfg.py` & `saspy-5.1.2/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.1.2/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/sas.core.jar` & `saspy-5.1.2/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.1.2/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.1.2/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/pyiom/saspy2j.class` & `saspy-5.1.2/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/pyiom/saspy2j.java` & `saspy-5.1.2/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/saspyiom.jar` & `saspy-5.1.2/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/NOTICE.md` & `saspy-5.1.2/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.1.2/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.1.2/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.1.2/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/libname_gen.sas` & `saspy-5.1.2/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasViyaML.py` & `saspy-5.1.2/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sas_magic.py` & `saspy-5.1.2/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasbase.py` & `saspy-5.1.2/saspy/sasbase.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sascfg.py` & `saspy-5.1.2/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasdata.py` & `saspy-5.1.2/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasdecorator.py` & `saspy-5.1.2/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasets.py` & `saspy-5.1.2/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasexceptions.py` & `saspy-5.1.2/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasiocom.py` & `saspy-5.1.2/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasiohttp.py` & `saspy-5.1.2/saspy/sasiohttp.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasioiom.py` & `saspy-5.1.2/saspy/sasioiom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasiostdio.py` & `saspy-5.1.2/saspy/sasiostdio.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,16 @@
 
 try:
    import pandas as pd
    import numpy  as np
 except ImportError:
    pass
 
-if os.name == 'nt':
-   from queue     import Queue, Empty
-   from threading import Thread
+from queue     import Queue, Empty
+from threading import Thread
 
 class SASconfigSTDIO:
    """
    This object is not intended to be used directly. Instantiate a SASsession object instead
    """
    def __init__(self, session, **kwargs):
       self._kernel  = kwargs.get('kernel', None)
@@ -438,28 +437,39 @@
             self.te = Thread(target=self._read_err, args=())
             self.to.daemon = True
             self.te.daemon = True
             self.to.start()
             self.te.start()
             self.stdin  = self.pid.stdin
       else:
-         self.pid    = pidpty[0]
-         self.stdin  = os.fdopen(pin[PIPE_WRITE], mode='wb')
-         self.stderr = os.fdopen(perr[PIPE_READ], mode='rb')
-         self.stdout = os.fdopen(pout[PIPE_READ], mode='rb')
-
-         fcntl.fcntl(self.stdout, fcntl.F_SETFL, os.O_NONBLOCK)
-         fcntl.fcntl(self.stderr, fcntl.F_SETFL, os.O_NONBLOCK)
+         self.pid     = pidpty[0]
+         self.stdin   = os.fdopen(pin[PIPE_WRITE], mode='wb')
+         self.stdoutp = os.fdopen(pout[PIPE_READ], mode='rb')
+         self.stderrp = os.fdopen(perr[PIPE_READ], mode='rb')
+
+         # to fix deadlock when submitting a huge amount of code, which is written to stderr and blocks
+         # stdin, so we deadlock, use the queue's and read/write threads to asynch read so we don't block
+         #fcntl.fcntl(self.stdoutp, fcntl.F_SETFL, os.O_NONBLOCK)
+         #fcntl.fcntl(self.stderrp, fcntl.F_SETFL, os.O_NONBLOCK)
 
          rc = os.waitpid(self.pid, os.WNOHANG)
          if rc[0] != 0:
             self.pid = None
             self._sb.SASpid = None
-            lst = self.stdout.read1(4096)
+            lst = self.stdoutp.read1(4096000)
             logger.error("stdout from subprocess is:\n"+lst.decode())
+         else:
+            self.stdout = Queue()
+            self.stderr = Queue()
+            self.to = Thread(target=self._read_out, args=())
+            self.te = Thread(target=self._read_err, args=())
+            self.to.daemon = True
+            self.te.daemon = True
+            self.to.start()
+            self.te.start()
 
       if self.pid is None:
          msg  = "SAS Connection failed. No connection established. Double check your settings in sascfg_personal.py file.\n"
          msg += "Attempted to run program "+pgm+" with the following parameters:"+str(parms)+"\n"
          msg += "Try running the following command (where saspy is running) manually to see if you can get more information on what went wrong:\n"+s+"\n"
          logger.error(msg)
          return None
@@ -480,26 +490,41 @@
          pid = self.pid if os.name != 'nt' else self.pid.pid
          logger.info("SAS Connection established. Subprocess id is "+str(pid)+"\n")
       return self.pid
 
    if os.name == 'nt':
       def _read_out(self):
          while True:
-            lst = self.pid.stdout.read(4096)
+            lst = self.pid.stdout.read(4096000)
+            if lst == b'':
+               break
+            self.stdout.put(lst)
+
+      def _read_err(self):
+         while True:
+            log = self.pid.stderr.read(4096000)
+            if log == b'':
+               break
+            self.stderr.put(log)
+   else:
+      def _read_out(self):
+         while True:
+            lst = self.stdoutp.read1(4096000)
             if lst == b'':
                break
             self.stdout.put(lst)
 
       def _read_err(self):
          while True:
-            log = self.pid.stderr.read(4096)
+            log = self.stderrp.read1(4096000)
             if log == b'':
                break
             self.stderr.put(log)
 
+
    def _endsas(self):
       rc  = 0
       ret = None
       if self.pid:
          if os.name == 'nt':
             pid = self.pid.pid
          else:
@@ -508,14 +533,19 @@
          code = b";*\';*\";*/;\n;quit;endsas;\n"
          self._getlog(wait=1)
          if self.pid:
             out = self.stdin.write(code)
             self.stdin.flush()
          sleep(1)
 
+         try:
+            self._log += self.stderr.get_nowait().decode(self.sascfg.encoding, errors='replace').replace(chr(12), chr(10))
+         except Empty:
+            pass
+
          if self.pid:
             if os.name == 'nt':
                self.pid.stdin.close()
                self.pid.stdout.close()
                self.pid.stderr.close()
                try:
                   rc = self.pid.wait(5)
@@ -538,14 +568,16 @@
 
                if rc[0] != 0:
                   pass
                else:
                   if self.sascfg.verbose:
                      logger.warning("SAS didn't shutdown w/in 5 seconds; killing it to be sure")
                   os.kill(self.pid, signal.SIGKILL)
+               self.to.join(5)
+               self.te.join(5)
 
          if self.sascfg.verbose:
             logger.info("SAS Connection terminated. Subprocess id was "+str(pid))
          self.pid        = None
          self._sb.SASpid = None
       return ret
 
@@ -573,30 +605,27 @@
          rc = os.waitpid(self.pid, os.WNOHANG)
          if rc[0] != 0:
             self.pid = None
             self._sb.SASpid = None
             return 'SAS process has terminated unexpectedly. Pid State= '+str(rc)
 
       while True:
-         if os.name == 'nt':
-            try:
-               log = self.stderr.get_nowait()
-            except Empty:
-               log = b''
-         else:
-            log = self.stderr.read1(4096)
+         try:
+            log = self.stderr.get_nowait()
+         except Empty:
+            log = b''
          if len(log) > 0:
             logf += log
          else:
             quit -= 1
             if quit < 0 or len(logf) > 0:
                break
             sleep(0.5)
 
-      x = logf.decode(self.sascfg.encoding, errors='replace').replace(code1, " ")
+      x = logf.decode(self.sascfg.encoding, errors='replace').replace(code1, " ").replace(chr(12), chr(10))
       self._log += x
 
       if self._checkLogForError(x):
          warnings.warn("Noticed 'ERROR:' in LOG, you ought to take a look and see if there was a problem")
          self._sb.check_error_log = True
 
       if self.pid == None:
@@ -622,21 +651,18 @@
       lstf = b''
       quit = wait * 2
       eof = 0
       bof = False
       lenf = 0
 
       while True:
-         if os.name == 'nt':
-            try:
-               lst = self.stdout.get_nowait()
-            except Empty:
-               lst = b''
-         else:
-            lst = self.stdout.read1(4096)
+         try:
+            lst = self.stdout.get_nowait()
+         except Empty:
+            lst = b''
          if len(lst) > 0:
             lstf += lst
 
             if ((not bof) and lst.count(b"<!DOCTYPE html>", 0, 20) > 0):
                bof = True
          else:
             lenf = len(lstf)
@@ -680,21 +706,18 @@
       f2 = [None]
       lstf = b''
       quit = wait * 2
       eof = 0
       self._asubmit("data _null_;file print;put 'Tom was here';run;", "text")
 
       while True:
-         if os.name == 'nt':
-            try:
-               lst = self.stdout.get_nowait()
-            except Empty:
-               lst = b''
-         else:
-            lst = self.stdout.read1(4096)
+         try:
+            lst = self.stdout.get_nowait()
+         except Empty:
+            lst = b''
          if len(lst) > 0:
             lstf += lst
 
             lenf = len(lstf)
             eof = lstf.find(b"Tom was here", lenf - 25, lenf)
 
             if (eof != -1):
@@ -885,15 +908,15 @@
                   except:
                      pass
                else:
                   rc = os.waitpid(self.pid, os.WNOHANG)
                   if rc[0] != 0:
                      log = b''
                      try:
-                        log = self.stderr.read1(4096)
+                        log = self.stderr.get_nowait()
                         if len(log) > 0:
                             logf += log
                         self._log += logf.decode(self.sascfg.encoding, errors='replace')
                      except:
                         pass
                      self.pid = None
                      self._sb.SASpid = None
@@ -907,38 +930,32 @@
 
                if bail:
                   eof -= 1
                if eof < 0:
                   break
 
                while True:
-                  if os.name == 'nt':
-                     try:
-                        lst = self.stdout.get_nowait()
-                     except Empty:
-                        lst = b''
-                  else:
-                     lst = self.stdout.read1(4096000)
+                  try:
+                     lst = self.stdout.get_nowait()
+                  except Empty:
+                     lst = b''
 
                   if len(lst) > 0:
                      wait = False
                      lstf += lst
                      if ods and not bof and lstf.count(b"<!DOCTYPE html>") > 0:
                         bof = True
                   else:
                      break
 
                while True:
-                  if os.name == 'nt':
-                     try:
-                        log = self.stderr.get_nowait()
-                     except Empty:
-                        log = b''
-                  else:
-                     log = self.stderr.read1(4096000)
+                  try:
+                     log = self.stderr.get_nowait()
+                  except Empty:
+                     log = b''
 
                   if len(log) > 0:
                      wait = False
                      logf += log
 
                   if not (pos < end):
                      if not bail and logf.count(logcodeo) >= 1:
@@ -984,27 +1001,23 @@
                end += len(undo+odsclose+logcodei.encode(self.sascfg.encoding)+b'\n')
             else:
                self.stdin.write(undo+odsclose+logcodei.encode(self.sascfg.encoding)+b'\n')
                self.stdin.flush()
 
          except (ConnectionResetError):
             log = ''
-            if os.name == 'nt':
-               try:
-                  log = self.stderr.get_nowait()
-               except Empty:
-                  log = b''
-            else:
-               try:
-                  log = self.stderr.read1(4096)
-                  if len(log) > 0:
-                     logf += log
-                  self._log += logf.decode(self.sascfg.encoding, errors='replace')
-               except:
-                  pass
+            try:
+               log = self.stderr.get_nowait()
+            except Empty:
+               log = b''
+
+            if len(log) > 0:
+               logf += log
+               self._log += logf.decode(self.sascfg.encoding, errors='replace')
+
             rc = 0
             if os.name == 'nt':
                try:
                   rc = self.pid.wait(0)
                except:
                   pass
             else:
@@ -1088,15 +1101,15 @@
                rc = os.waitpid(self.pid, os.WNOHANG)
                if rc[0] != 0:
                   self.pid = None
                   self._sb.SASpid = None
                   outrc = str(rc)
                   return dict(LOG='SAS process has terminated unexpectedly. Pid State= '+outrc, LST='',ABORT=True)
 
-            lst = self.stdout.read1(4096)
+            lst = self.stdout.get_nowait()
             if len(lst) > 0:
                 lsts = lst.rpartition(b'Select:')
                 if lsts[0] != b'' and lsts[1] != b'':
                     found = True
                     query = lsts[1] + lsts[2].rsplit(b'\n?')[0] + b'\n'
                     print('Processing interrupt\nAttn handler Query is\n\n' + query.decode(self.sascfg.encoding, errors='replace'))
                     response = None
@@ -1131,15 +1144,15 @@
                         else:
                            lstf += lst
                         bc = True
                         break
             else:
                 if bc:
                    break
-                log = self.stderr.read1(4096)
+                log = self.stderr.get_nowait()
                 logf += log
                 self._log += log.decode(self.sascfg.encoding, errors='replace')
 
                 if log.count(eos) >= 1:
                     print("******************Found end of step. No interrupt processed")
                     found = True
 
@@ -1202,30 +1215,30 @@
                   print("'Press' Response="+response+'\n')
                   self._asubmit(response+'\n','text')
                else:
                   #print("******************No 'Select' or 'Press' found in lst=")
                   pass
 
             sleep(.25)
-            lst = self.stdout.read1(4096).decode(self.sascfg.encoding, errors='replace')
+            lst = self.stdout.get_nowait().decode(self.sascfg.encoding, errors='replace')
          else:
-            log = self.stderr.read1(4096).decode(self.sascfg.encoding, errors='replace')
+            log = self.stderr.get_nowait().decode(self.sascfg.encoding, errors='replace')
             self._log += log
             logn = self._logcnt(False)
 
             if log.count("E3969440A681A24088859985"+logn+"\n") >= 1:
                print("******************Found end of step. No interupt processed")
                found = True
 
             if found:
                ll = self.submit("ods "+self.sascfg.output+" (id=saspy_internal) close;ods listing close;ods listing;libname work list;\n",'text')
                break
 
             sleep(.25)
-            lst = self.stdout.read1(4096).decode(self.sascfg.encoding, errors='replace')
+            lst = self.stdout.get_nowait().decode(self.sascfg.encoding, errors='replace')
 
       return log
 
    def saslog(self):
       """
       this method is used to get the current, full contents of the SASLOG
       """
@@ -2033,21 +2046,18 @@
                      sock.connect((host, port))
                      ssock = sock
                      sleep(1)
                   pass
                send -= sent
             code = ""
 
-            if os.name == 'nt':
-               try:
-                  log = self.stderr.get_nowait()
-               except Empty:
-                  log = b''
-            else:
-               log = self.stderr.read1(4096)
+            try:
+               log = self.stderr.get_nowait()
+            except Empty:
+               log = b''
 
             if len(log) > 0:
                logf += log
 
       logd = logf.decode(self.sascfg.encoding, errors='replace')
       self._log += logd
       if self._checkLogForError(logd):
```

### Comparing `saspy-5.1.0/saspy/sasml.py` & `saspy-5.1.2/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasproccommons.py` & `saspy-5.1.2/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasqc.py` & `saspy-5.1.2/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasresults.py` & `saspy-5.1.2/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasstat.py` & `saspy-5.1.2/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sastabulate.py` & `saspy-5.1.2/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/sasutil.py` & `saspy-5.1.2/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy/scripts/run_sas.py` & `saspy-5.1.2/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/saspy.egg-info/PKG-INFO` & `saspy-5.1.2/saspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.1.0
+Version: 5.1.2
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.1.0/saspy.egg-info/SOURCES.txt` & `saspy-5.1.2/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.1.0/setup.py` & `saspy-5.1.2/setup.py`

 * *Files identical despite different names*

