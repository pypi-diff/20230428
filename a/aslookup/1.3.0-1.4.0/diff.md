# Comparing `tmp/aslookup-1.3.0.tar.gz` & `tmp/aslookup-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aslookup-1.3.0.tar", last modified: Sun Apr 10 08:37:17 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aslookup-1.3.0.tar` & `aslookup-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxr-xr-x   0 dspruell   (501) staff       (20)        0 2022-04-10 08:37:17.393614 aslookup-1.3.0/
--rw-r--r--   0 dspruell   (501) staff       (20)      759 2019-02-24 01:44:43.000000 aslookup-1.3.0/LICENSE
--rwx------   0 dspruell   (501) staff       (20)       27 2019-02-24 01:28:15.000000 aslookup-1.3.0/MANIFEST.in
--rw-r--r--   0 dspruell   (501) staff       (20)     2688 2022-04-10 08:37:17.393268 aslookup-1.3.0/PKG-INFO
--rw-r--r--   0 dspruell   (501) staff       (20)     2236 2022-04-10 08:36:15.000000 aslookup-1.3.0/README.md
-drwxr-xr-x   0 dspruell   (501) staff       (20)        0 2022-04-10 08:37:17.390706 aslookup-1.3.0/aslookup/
--rw-r--r--   0 dspruell   (501) staff       (20)      277 2020-10-11 07:38:41.000000 aslookup-1.3.0/aslookup/__init__.py
--rwxr-xr-x   0 dspruell   (501) staff       (20)     3632 2022-04-10 08:34:03.000000 aslookup-1.3.0/aslookup/cli.py
--rw-r--r--   0 dspruell   (501) staff       (20)      452 2020-10-11 07:42:28.000000 aslookup-1.3.0/aslookup/exceptions.py
--rwxr-xr-x   0 dspruell   (501) staff       (20)     7803 2021-04-21 05:55:44.000000 aslookup-1.3.0/aslookup/lookup.py
-drwxr-xr-x   0 dspruell   (501) staff       (20)        0 2022-04-10 08:37:17.392837 aslookup-1.3.0/aslookup.egg-info/
--rw-r--r--   0 dspruell   (501) staff       (20)     2688 2022-04-10 08:37:16.000000 aslookup-1.3.0/aslookup.egg-info/PKG-INFO
--rw-r--r--   0 dspruell   (501) staff       (20)      326 2022-04-10 08:37:17.000000 aslookup-1.3.0/aslookup.egg-info/SOURCES.txt
--rw-r--r--   0 dspruell   (501) staff       (20)        1 2022-04-10 08:37:16.000000 aslookup-1.3.0/aslookup.egg-info/dependency_links.txt
--rw-r--r--   0 dspruell   (501) staff       (20)       48 2022-04-10 08:37:17.000000 aslookup-1.3.0/aslookup.egg-info/entry_points.txt
--rw-r--r--   0 dspruell   (501) staff       (20)       19 2022-04-10 08:37:17.000000 aslookup-1.3.0/aslookup.egg-info/requires.txt
--rw-r--r--   0 dspruell   (501) staff       (20)        9 2022-04-10 08:37:17.000000 aslookup-1.3.0/aslookup.egg-info/top_level.txt
--rw-r--r--   0 dspruell   (501) staff       (20)       38 2022-04-10 08:37:17.393717 aslookup-1.3.0/setup.cfg
--rw-r--r--   0 dspruell   (501) staff       (20)      987 2022-04-10 08:31:01.000000 aslookup-1.3.0/setup.py
--rw-r--r--   0 dspruell   (501) staff       (20)      124 2021-03-21 02:50:21.000000 aslookup-1.3.0/test_input.txt
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 aslookup-1.4.0/tox.ini
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/__init__.py
+-rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/exceptions.py
+-rwxr-xr-x   0        0        0     7887 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/lookup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/.keep
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/test_input.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/test_nop.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aslookup-1.4.0/.gitignore
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aslookup-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 aslookup-1.4.0/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 aslookup-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 aslookup-1.4.0/PKG-INFO
```

### Comparing `aslookup-1.3.0/LICENSE` & `aslookup-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aslookup-1.3.0/PKG-INFO` & `aslookup-1.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: aslookup
-Version: 1.3.0
-Summary: IP to AS routing data query script
-Home-page: https://github.com/dspruell/aslookup
-Author: Darren Spruell
-Author-email: dspruell@sancho2k.net
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.4.0
+Summary: IP to ASN routing data query script
+Project-URL: Homepage, https://github.com/dspruell/aslookup/
+Author-email: Darren Spruell <phatbuckett@gmail.com>
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: dnspython
+Requires-Dist: pytricia
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # aslookup
 Python client for IP to ASN lookup services
 
 aslookup is a client utility for two of the public IP/AS query services
 operated by the following organizations:
 
@@ -31,23 +30,26 @@
 listing of IP networks which are unroutable internet addresses, typically
 special use ranges in RFCs. In this way it can both filter out addresses from
 queries which are a waste of time, as well as provide context to the user on
 the address.
 
 ## Installation
 
-The app has been tested on Python 3. The script requires the *dnspython*
-package. If missing, it will be installed automatically.
+The app has been tested on Python 3.
 
-It's best to install the program into a Python virtualenv.
+It's best to install the program into a Python virtualenv. If you will only use
+the command line interface, the recommended way to install it is using
+[pipx](https://pypa.github.io/pipx/):
 
-Recommended installation from PyPI using pip (make sure to use the pip or
-python command from your target Python 3 environment)!
+    pipx install aslookup
 
-    pip3 install aslookup
+If you will use aslookup as a library, you'll instead want to install it using
+`pip` in your target Python environment:
+
+    python3 -m pip install aslookup
 
 ## Usage
 
 ### Python module
 
 The Python module defaults to querying the Team Cymru data service. The
 desired service may be specified by passing the *service* parameter to
@@ -64,19 +66,21 @@
 It is possible to provide multiple IP addresses as arguments to the script, or 
 to send them as a list on standard input, in which cases the script loops over 
 them and returns output on separate lines. When providing invalid IPv4 
 addresses as arguments, the script reports the problem on standard error and 
 exits with an error. When providing input on stdin, the error is reported on 
 standard output but execution is not aborted.
 
-    as-lookup 8.8.8.8 11.22.33.44
+    as-lookup 8.8.8.8 9.9.9.9
+
+or:
+
+    as-lookup < ipaddrs.txt
 
 ### Test data
 
-A list of test values for the script is included in the file `test_input.txt`.
+A list of test values for the script is included in the file `tests/test_input.txt`.
 This can be useful to validate included IP prefix classifications and see the
 output format.
 
-    as-lookup < test_input.txt
-
-
+    as-lookup < tests/test_input.txt
```

### Comparing `aslookup-1.3.0/README.md` & `aslookup-1.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 listing of IP networks which are unroutable internet addresses, typically
 special use ranges in RFCs. In this way it can both filter out addresses from
 queries which are a waste of time, as well as provide context to the user on
 the address.
 
 ## Installation
 
-The app has been tested on Python 3. The script requires the *dnspython*
-package. If missing, it will be installed automatically.
+The app has been tested on Python 3.
 
-It's best to install the program into a Python virtualenv.
+It's best to install the program into a Python virtualenv. If you will only use
+the command line interface, the recommended way to install it is using
+[pipx](https://pypa.github.io/pipx/):
 
-Recommended installation from PyPI using pip (make sure to use the pip or
-python command from your target Python 3 environment)!
+    pipx install aslookup
 
-    pip3 install aslookup
+If you will use aslookup as a library, you'll instead want to install it using
+`pip` in your target Python environment:
+
+    python3 -m pip install aslookup
 
 ## Usage
 
 ### Python module
 
 The Python module defaults to querying the Team Cymru data service. The
 desired service may be specified by passing the *service* parameter to
@@ -49,17 +52,21 @@
 It is possible to provide multiple IP addresses as arguments to the script, or 
 to send them as a list on standard input, in which cases the script loops over 
 them and returns output on separate lines. When providing invalid IPv4 
 addresses as arguments, the script reports the problem on standard error and 
 exits with an error. When providing input on stdin, the error is reported on 
 standard output but execution is not aborted.
 
-    as-lookup 8.8.8.8 11.22.33.44
+    as-lookup 8.8.8.8 9.9.9.9
+
+or:
+
+    as-lookup < ipaddrs.txt
 
 ### Test data
 
-A list of test values for the script is included in the file `test_input.txt`.
+A list of test values for the script is included in the file `tests/test_input.txt`.
 This can be useful to validate included IP prefix classifications and see the
 output format.
 
-    as-lookup < test_input.txt
+    as-lookup < tests/test_input.txt
```

### Comparing `aslookup-1.3.0/aslookup/cli.py` & `aslookup-1.4.0/aslookup/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,99 @@
-'CLI module'
+"""aslookup CLI module."""
 
-from os import linesep
-import sys
-import logging
 import argparse
+import logging
+import sys
+from os import linesep
 from time import sleep
 
 from . import __full_version__
 from .exceptions import AddressFormatError, LookupError
 from .lookup import get_as_data
 
-
 DEFAULT_LOOKUP_SOURCE = "cymru"
 
 logging.basicConfig(
-    level=logging.DEBUG,
-    format='[%(levelname)s] %(message)s'
+    level=logging.DEBUG, format="[%(levelname)s] %(message)s"
 )
 logger = logging.getLogger(__name__)
 
 
 def main():
-    description = ('Client to return autonomous system information for '
-                   'IPv4 addresses')
-    epilog = ('One or more IP addresses may be passed as arguments on the '
-              'command line. A list of IP addresses (newline-separated) may '
-              'also be passed on standard input.')
+    """Run main CLI."""
+    description = (
+        "Client to return autonomous system information for "
+        "IPv4 addresses"
+    )
+    epilog = (
+        "One or more IP addresses may be passed as arguments on the "
+        "command line. A list of IP addresses (newline-separated) may "
+        "also be passed on standard input."
+    )
     parser = argparse.ArgumentParser(description=description, epilog=epilog)
-    parser.add_argument('-s', '--service', choices=['shadowserver', 'cymru'],
-                        default=DEFAULT_LOOKUP_SOURCE,
-                        help='service to query (default: %(default)s)')
-    parser.add_argument('-H', '--header', action='store_true',
-                        help='print descriptive header before output')
-    parser.add_argument('-p', '--pause', action='store_true',
-                        help='pause for one second between each query on '
-                             'address list input')
-    parser.add_argument('-r', '--raw', action='store_true',
-                        help='display internal ASData object showing the '
-                             'value of each known field in the AS data')
-    parser.add_argument('-V', '--version', action='store_true',
-                        help='display package version')
-    parser.add_argument('-v', '--verbose', dest='loglevel',
-                        action='store_const', const=logging.DEBUG,
-                        default=logging.WARNING, help='show verbose output')
-    parser.add_argument('address', nargs='*',
-                        help='IPv4 address(es) on which to perform AS lookup')
+    parser.add_argument(
+        "-s",
+        "--service",
+        choices=["shadowserver", "cymru"],
+        default=DEFAULT_LOOKUP_SOURCE,
+        help="service to query (default: %(default)s)",
+    )
+    parser.add_argument(
+        "-H",
+        "--header",
+        action="store_true",
+        help="print descriptive header before output",
+    )
+    parser.add_argument(
+        "-p",
+        "--pause",
+        action="store_true",
+        help="pause for one second between each query on "
+        "address list input",
+    )
+    parser.add_argument(
+        "-r",
+        "--raw",
+        action="store_true",
+        help="display internal ASData object showing the "
+        "value of each known field in the AS data",
+    )
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="store_true",
+        help="display package version",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        dest="loglevel",
+        action="store_const",
+        const=logging.DEBUG,
+        default=logging.WARNING,
+        help="show verbose output",
+    )
+    parser.add_argument(
+        "address",
+        nargs="*",
+        help="IPv4 address(es) on which to perform AS lookup",
+    )
     args = parser.parse_args()
 
     logging.getLogger().setLevel(args.loglevel)
 
     # Print software version
     if args.version:
         parser.exit(status=0, message=__full_version__ + linesep)
 
     # Print header lines if specified
     if args.header:
-        print('-' * 50)
-        print('%-15s  %s' % ('IP Address', 'AS Information'))
-        print('-' * 50)
+        print("-" * 50)
+        print("%-15s  %s" % ("IP Address", "AS Information"))
+        print("-" * 50)
 
     # Process addresses given as parameters or fed on stdin.
     # - Input as parameters: In this mode, invalid IP addresses result in
     #   script exiting with an error. Non-routable addresses result in
     #   message to stderr.
     # - Input on stdin: In this mode, invalid IP addresses result in script
     #   proceeding without exiting, in order to make it so that address lists
@@ -69,26 +101,27 @@
     in_src = args.address if args.address else sys.stdin
     for addr in in_src:
         addr = addr.strip()
         try:
             data = get_as_data(addr, service=args.service)
         except AddressFormatError as e:
             if args.address:
-                parser.error('[{}] {}'.format(addr, e))
+                parser.error("[{}] {}".format(addr, e))
             else:
                 stream = sys.stderr
                 out_str = e
         except LookupError as e:
             stream = sys.stderr
             out_str = e
         else:
             stream = sys.stdout
             if not args.raw:
-                out_str = '{0} | {1} | {2}'.format(
-                    data.handle, data.cc, data.as_name)
+                out_str = "{0} | {1} | {2}".format(
+                    data.handle, data.cc, data.as_name
+                )
             else:
                 print(data)
                 continue
 
-        print('%-15s  %s' % (addr, out_str), file=stream)
+        print("%-15s  %s" % (addr, out_str), file=stream)
         if args.pause:
             sleep(1)
```

### Comparing `aslookup-1.3.0/aslookup/lookup.py` & `aslookup-1.4.0/aslookup/lookup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,238 @@
-'Lookup routines'
+"""Lookup routines."""
 
 import re
 import logging
 from collections import namedtuple
 
 import pytricia
 import dns.resolver
 import dns.reversename
 
-from .exceptions import (NoASDataError, NonroutableAddressError,
-                         AddressFormatError)
+from .exceptions import (
+    NoASDataError,
+    NonroutableAddressError,
+    AddressFormatError,
+)
 
 
 logger = logging.getLogger(__name__)
 
 AS_SERVICES = {
-    'shadowserver': {
-        'origin_suffix': 'origin.asn.shadowserver.org',
+    "shadowserver": {
+        "origin_suffix": "origin.asn.shadowserver.org",
     },
-    'cymru': {
-        'origin_suffix': 'origin.asn.cymru.com',
-        'as_description_suffix': 'asn.cymru.com',
+    "cymru": {
+        "origin_suffix": "origin.asn.cymru.com",
+        "as_description_suffix": "asn.cymru.com",
     },
 }
 
 # IPs with these prefixes aren't routable on Internet and need not be sent
 # to lookup service. Ref. RFC 5735.
 IP_NOLOOKUP_NETS = {
-    '0.0.0.0/8':       'RFC 1122 IPv4 any',
-    '127.0.0.0/8':     'RFC 1122 loopback',
-    '10.0.0.0/8':      'RFC 1918 range',
-    '100.64.0.0/10':   'RFC 6598 shared transition space',
-    '169.254.0.0/16':  'RFC 3927 link local range',
-    '172.16.0.0/12':   'RFC 1918 range',
-    '192.0.0.0/24':    'RFC 5736 protocol assignment range',
-    '192.0.2.0/24':    'RFC 5737 TEST-NET-1 range',
-    '192.88.99.0/24':  'RFC 3068 6to4 relay anycast range',
-    '192.168.0.0/16':  'RFC 1918 range',
-    '198.18.0.0/15':   'RFC 2544 network device benchmark range',
-    '198.51.100.0/24': 'RFC 5737 TEST-NET-2 range',
-    '203.0.113.0/24':  'RFC 5737 TEST-NET-3 range',
-    '224.0.0.0/4':     'RFC 5771 multicast range',
-    '240.0.0.0/4':     'RFC 1112 IANA future use reserved range',
-    '255.0.0.0/8':     'RFC 1112 IPv4 limited broadcast',
+    "0.0.0.0/8": "RFC 1122 IPv4 any",
+    "127.0.0.0/8": "RFC 1122 loopback",
+    "10.0.0.0/8": "RFC 1918 range",
+    "100.64.0.0/10": "RFC 6598 shared transition space",
+    "169.254.0.0/16": "RFC 3927 link local range",
+    "172.16.0.0/12": "RFC 1918 range",
+    "192.0.0.0/24": "RFC 5736 protocol assignment range",
+    "192.0.2.0/24": "RFC 5737 TEST-NET-1 range",
+    "192.88.99.0/24": "RFC 3068 6to4 relay anycast range",
+    "192.168.0.0/16": "RFC 1918 range",
+    "198.18.0.0/15": "RFC 2544 network device benchmark range",
+    "198.51.100.0/24": "RFC 5737 TEST-NET-2 range",
+    "203.0.113.0/24": "RFC 5737 TEST-NET-3 range",
+    "224.0.0.0/4": "RFC 5771 multicast range",
+    "240.0.0.0/4": "RFC 1112 IANA future use reserved range",
+    "255.0.0.0/8": "RFC 1112 IPv4 limited broadcast",
 }
 
 # Build the patricia tree
 pyt = pytricia.PyTricia()
 for net, descr in IP_NOLOOKUP_NETS.items():
     pyt[net] = descr
-logger.debug('created exception network tree with %d networks', len(pyt))
+logger.debug("created exception network tree with %d networks", len(pyt))
 
-IPV4_FMT = re.compile(r'^(?:\d{1,3}\.){3}\d{1,3}$')
-PREFIX_FMT = re.compile(r'(?:\d{1,3}\.){3}\d{1,3}/\d{1,2}\b')
+IPV4_FMT = re.compile(r"^(?:\d{1,3}\.){3}\d{1,3}$")
+PREFIX_FMT = re.compile(r"(?:\d{1,3}\.){3}\d{1,3}/\d{1,2}\b")
 
 # Structured record tuple
-ASData = namedtuple('ASData', ['handle', 'asn', 'as_name', 'rir', 'reg_date',
-                    'prefix', 'cc', 'domain', 'isp', 'data_source'])
+ASData = namedtuple(
+    "ASData",
+    [
+        "handle",
+        "asn",
+        "as_name",
+        "rir",
+        "reg_date",
+        "prefix",
+        "cc",
+        "domain",
+        "isp",
+        "data_source",
+    ],
+)
 
 
 def validate_ipv4(addr):
-    'Validate that input is an IPv4 address.'
-
+    """Validate that input is an IPv4 address."""
     # Check that it's a valid IPv4 address
     if not re.match(IPV4_FMT, addr):
-        raise AddressFormatError('Invalid format for IPv4 address')
-    for octet in addr.split('.'):
+        raise AddressFormatError("Invalid format for IPv4 address")
+    for octet in addr.split("."):
         if not 0 <= int(octet) <= 255:
-            raise AddressFormatError('Invalid octet value for IPv4 address')
+            raise AddressFormatError("Invalid octet value for IPv4 address")
 
     # Verify address not in reserved/non-routable prefixes.
     if addr in pyt:
         raise NonroutableAddressError(pyt.get(addr))
     return
 
 
 def get_cymru_data(s, extra={}):
-    '''
+    """
     Parse Team Cymru AS data query and return structured record tuple.
 
     `extra` is a dict of additional fields that can be passed in, typically
     consisting of data from the origin DNS query.
 
     DNS answer format received, first query (2020-09-11):
         "15133 | 93.184.216.0/24 | EU | ripencc | 2008-06-02"
     DNS answer format received, second query (handled here) (2020-09-11):
         "15133 | US | arin | 2007-03-19 | EDGECAST, US"
 
-    '''
+    """
     s = s.strip('"')
     # Cymru results began to append a comma and country code to the end of the
     # AS name, polluting the data. Strip it off.
-    s = re.sub(r', [A-Z]{2}$', '', s)
-    fields = s.split(' | ')
+    s = re.sub(r", [A-Z]{2}$", "", s)
+    fields = s.split(" | ")
     fields = [x.strip() for x in fields]
     as_data = ASData(
         asn=fields[0],
-        handle=f'AS{fields[0]}',
+        handle=f"AS{fields[0]}",
         as_name=fields[4],
-        prefix=extra.get('ip_prefix'),
+        prefix=extra.get("ip_prefix"),
         domain=None,
         cc=fields[1],
         rir=fields[2],
         reg_date=fields[3],
         isp=None,
-        data_source='cymru'
+        data_source="cymru",
     )
     return as_data
 
 
 def get_shadowserver_data(s):
-    '''
+    """
     Parse Shadowserver AS data query and return structured record tuple.
 
     DNS answer format received (2020-09-11):
         "15133 | 93.184.216.0/24 | EDGECAST | US | EDGECAST"
     DNS answer format received (2021-03-20):
         "12876 | 212.129.0.0/18 |  | FR | Online SAS"
 
-    '''
+    """
     s = s.strip('"')
     # Shadowserver results at one point appended a comma and country code to
     # the end of the AS name, polluting the data. Strip it off.
-    s = re.sub(r', [A-Z]{2}$', '', s)
-    fields = s.split(' | ')
+    s = re.sub(r", [A-Z]{2}$", "", s)
+    fields = s.split(" | ")
     fields = [x.strip() for x in fields]
     # For any response that returned AS data but no AS name, alert user.
     if fields[0] and not fields[2]:
-        logger.warning('no value for AS name; overriding with ISP')
+        logger.warning("no value for AS name; overriding with ISP")
 
     as_data = ASData(
         asn=fields[0],
-        handle=f'AS{fields[0]}',
+        handle=f"AS{fields[0]}",
         # If the AS Name field is blank, toss the ISP in and mark it as
         # an ISP override.
         as_name=fields[4] or fields[2],
         prefix=fields[1],
         domain=None,
         cc=fields[3],
         rir=None,
         reg_date=None,
         isp=fields[4],
-        data_source='shadowserver'
+        data_source="shadowserver",
     )
     return as_data
 
 
-def get_as_data(addr, service='shadowserver'):
-    '''
+def get_as_data(addr, service="shadowserver"):
+    """
     Query and return AS information for supplied IP address.
 
     Each IP-ASN service operates differently and returns slightly different
     fields in their responses.
 
     Return string containing formatted AS information for a given IP address,
     unless the address falls into these categories: it is not a valid IPv4
     address, there is no current AS data for that address, (i.e. not part of an
     announced prefix), or it is known to be a non-routable or reserved IP
     address. In these cases, an appropriate exception is raised.
 
-    '''
+    """
     addr = addr.strip()
     try:
         validate_ipv4(addr)
     except AddressFormatError:
         raise
     except LookupError as e:
-        raise LookupError('Ignoring: %s' % e)
+        raise LookupError("Ignoring: %s" % e)
 
     # Format IP to reversed-octet structure and issue origin lookup.
-    rev_addr = '.'.join(reversed(addr.split('.')))
-    origin_addr = '.'.join([rev_addr, AS_SERVICES[service]['origin_suffix']])
+    rev_addr = ".".join(reversed(addr.split(".")))
+    origin_addr = ".".join(
+        [rev_addr, AS_SERVICES[service]["origin_suffix"]]
+    )
     try:
-        answers = dns.resolver.query(origin_addr, 'TXT')
+        answers = dns.resolver.query(origin_addr, "TXT")
     except dns.resolver.NXDOMAIN:
-        raise NoASDataError('No routing origin data for address')
+        raise NoASDataError("No routing origin data for address")
 
     if answers:
         for a in answers:
-            logger.debug('raw DNS record response: %s', a)
-        if service == 'shadowserver':
+            logger.debug("raw DNS record response: %s", a)
+        if service == "shadowserver":
             # Shadowserver origin lookup response includes AS name information
             asdata_text = answers[0].to_text()
             asdata = get_shadowserver_data(asdata_text)
             # Shadowserver will still output information in cases that no ASN
             # is identified, so raise exception when this occurs
             if not asdata.asn:
-                raise NoASDataError('No routing origin data for address')
+                raise NoASDataError("No routing origin data for address")
         else:
             extra_data = {}
 
             # Team Cymru origin lookup response returns only ASN and requires
             # second lookup to return AS name information
             origin_data = answers[0].to_text().strip('"')
-            m1 = re.match(r'^\d+', origin_data)
+            m1 = re.match(r"^\d+", origin_data)
             if m1 is None:
-                msg = (f'Error in lookup from service {service} for IP {addr} '
-                       f'(origin_data response: {origin_data})')
+                msg = (
+                    f"Error in lookup from service {service} for IP {addr} "
+                    f"(origin_data response: {origin_data})"
+                )
                 raise NoASDataError(msg)
 
             # Capture prefix from the origin data response
             m2 = PREFIX_FMT.search(origin_data)
             if m2 is not None:
                 extra_data.update(ip_prefix=m2.group(0))
 
             # Run second query for AS name/description info
-            _sfx = AS_SERVICES[service]['as_description_suffix']
-            as_data_addr = f'AS{m1.group(0)}.{_sfx}'
+            _sfx = AS_SERVICES[service]["as_description_suffix"]
+            as_data_addr = f"AS{m1.group(0)}.{_sfx}"
             try:
-                answers = dns.resolver.query(as_data_addr, 'TXT')
+                answers = dns.resolver.query(as_data_addr, "TXT")
             except dns.resolver.NXDOMAIN:
-                raise NoASDataError('No routing origin data for address')
+                raise NoASDataError("No routing origin data for address")
             if answers:
                 for a in answers:
-                    logger.debug('raw DNS record response: %s', a)
+                    logger.debug("raw DNS record response: %s", a)
                 asdata_text = answers[0].to_text()
                 asdata = get_cymru_data(asdata_text, extra=extra_data)
         return asdata
```

