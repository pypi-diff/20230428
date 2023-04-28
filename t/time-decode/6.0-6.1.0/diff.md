# Comparing `tmp/time_decode-6.0.tar.gz` & `tmp/time_decode-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_decode-6.0.tar", last modified: Thu Apr 27 20:52:15 2023, max compression
+gzip compressed data, was "time_decode-6.1.0.tar", last modified: Fri Apr 28 15:09:00 2023, max compression
```

## Comparing `time_decode-6.0.tar` & `time_decode-6.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0     1024 users      (100)        0 2023-04-27 20:52:15.619438 time_decode-6.0/
--rwxrwxrwx   0     1024 users      (100)     1069 2021-03-18 17:28:16.000000 time_decode-6.0/LICENSE
--rwxrwxrwx   0     1024 users      (100)     3631 2023-04-27 20:52:15.618438 time_decode-6.0/PKG-INFO
--rw-rw-r--   0     1024 users      (100)     3232 2023-04-27 20:46:51.000000 time_decode-6.0/README.md
--rwxrwxrwx   0     1024 users      (100)       38 2023-04-27 20:52:15.619438 time_decode-6.0/setup.cfg
--rw-rw-r--   0     1024 users      (100)      902 2023-04-27 20:45:32.000000 time_decode-6.0/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2023-04-27 20:52:15.606438 time_decode-6.0/time_decode/
--rwxrwxrwx   0     1024 users      (100)        0 2021-03-18 17:39:28.000000 time_decode-6.0/time_decode/__init__.py
--rwxrwxr-x   0     1024 users      (100)   126883 2023-04-27 20:51:37.000000 time_decode-6.0/time_decode/time_decode.py
-drwxrwxrwx   0     1024 users      (100)        0 2023-04-27 20:52:15.616438 time_decode-6.0/time_decode.egg-info/
--rwxrwxrwx   0     1024 users      (100)     3631 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      289 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       61 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       25 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       12 2023-04-27 20:52:15.000000 time_decode-6.0/time_decode.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2023-04-28 15:09:00.237938 time_decode-6.1.0/
+-rwxrwxrwx   0     1024 users      (100)     1069 2023-04-28 02:15:43.000000 time_decode-6.1.0/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     3633 2023-04-28 15:09:00.236938 time_decode-6.1.0/PKG-INFO
+-rw-rw-r--   0     1024 users      (100)     3232 2023-04-27 21:23:19.000000 time_decode-6.1.0/README.md
+-rwxrwxrwx   0     1024 users      (100)       38 2023-04-28 15:09:00.237938 time_decode-6.1.0/setup.cfg
+-rw-rw-r--   0     1024 users      (100)      904 2023-04-28 15:05:48.000000 time_decode-6.1.0/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2023-04-28 15:09:00.225938 time_decode-6.1.0/time_decode/
+-rwxrwxrwx   0     1024 users      (100)        0 2021-03-18 17:39:28.000000 time_decode-6.1.0/time_decode/__init__.py
+-rwxrwxr-x   0     1024 users      (100)   127482 2023-04-28 15:06:09.000000 time_decode-6.1.0/time_decode/time_decode.py
+drwxrwxrwx   0     1024 users      (100)        0 2023-04-28 15:09:00.235938 time_decode-6.1.0/time_decode.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     3633 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      289 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       61 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       25 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       12 2023-04-28 15:09:00.000000 time_decode-6.1.0/time_decode.egg-info/top_level.txt
```

### Comparing `time_decode-6.0/LICENSE` & `time_decode-6.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Corey Forman
+Copyright (c) 2023 Corey Forman
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `time_decode-6.0/PKG-INFO` & `time_decode-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_decode
-Version: 6.0
+Version: 6.1.0
 Summary: Python 3 timestamp decode/encode tool
 Home-page: https://github.com/digitalsleuth/time_decode
 Author: Corey Forman
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,16 +28,16 @@
 `python3 -m pip install time-decode` or `python3 -m pip install git+https://github.com/digitalsleuth/time_decode`
 
 This python script provides the following conversions from existing timestamps:
 
 - 128-bit SYSTEMTIME
 - 32-bit MS-DOS time, result is Local
 - Active Directory value
-- Apple Biome hex format
 - Apple Biome 64-bit decimal format
+- Apple Biome hex format
 - Bitwise decimal 10-digit
 - BPlist (as NSDate)
 - Cocoa Core (as NSDate)
 - DHCP6 DUID
 - Discord URL
 - exFAT
 - FAT Date + Time (wFat)
```

### Comparing `time_decode-6.0/README.md` & `time_decode-6.1.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 `python3 -m pip install time-decode` or `python3 -m pip install git+https://github.com/digitalsleuth/time_decode`
 
 This python script provides the following conversions from existing timestamps:
 
 - 128-bit SYSTEMTIME
 - 32-bit MS-DOS time, result is Local
 - Active Directory value
-- Apple Biome hex format
 - Apple Biome 64-bit decimal format
+- Apple Biome hex format
 - Bitwise decimal 10-digit
 - BPlist (as NSDate)
 - Cocoa Core (as NSDate)
 - DHCP6 DUID
 - Discord URL
 - exFAT
 - FAT Date + Time (wFat)
```

### Comparing `time_decode-6.0/setup.py` & `time_decode-6.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding='utf8') as readme:
     long_description = readme.read()
 
 setup(
     name="time_decode",
-    version="6.0",
+    version="6.1.0",
     author="Corey Forman",
     license="MIT",
     url="https://github.com/digitalsleuth/time_decode",
     description=("Python 3 timestamp decode/encode tool"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `time_decode-6.0/time_decode/time_decode.py` & `time_decode-6.1.0/time_decode/time_decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 from calendar import monthrange
 from dateutil import parser as duparser
 from colorama import init
 
 init(autoreset=True)
 
 __author__ = "Corey Forman"
-__date__ = "27 Apr 2023"
-__version__ = "6.0"
+__date__ = "28 Apr 2023"
+__version__ = "6.1.0"
 __description__ = "Python 3 CLI Date Time Conversion Tool"
 __fmt__ = "%Y-%m-%d %H:%M:%S.%f"
 __red__ = "\033[1;31m"
 __clr__ = "\033[1;m"
 
 ts_types = {
     "unix_sec": ["Unix Seconds", "Unix seconds timestamp is 10 digits in length"],
@@ -314,15 +314,16 @@
     try:
         if args.guess:
             full_list = from_all(args.guess)
             if len(full_list) == 0:
                 print("[!] No valid dates found. Check your input and try again")
             else:
                 print(
-                    "[+] Outputs which do NOT result in a date/time value are NOT displayed\r"
+                    f"[+] Guessing timestamp format for {args.guess}\n"
+                    f"[+] Outputs which do NOT result in a date/time value are NOT displayed\r"
                 )
                 if len(full_list) == 1:
                     dt_text = "date"
                 else:
                     dt_text = "dates"
                 print(f"[+] Displaying {len(full_list)} potential {dt_text}\r")
                 print(
@@ -2254,14 +2255,15 @@
             in_uuid = indiv_output = combined_output = False
         else:
             u_data = uuid.UUID(uuid_lower)
             if u_data.version == 1:
                 unix_ts = int((u_data.time / 10000) - 12219292800000)
                 in_uuid = dt.utcfromtimestamp(float(unix_ts) / 1000.0).strftime(__fmt__)
             else:
+                in_uuid = indiv_output = combined_output = False
                 pass
             indiv_output = str(f"{ts_type}: {in_uuid}")
             combined_output = str(f"{__red__}{ts_type}:\t\t\t{in_uuid} UTC{__clr__}")
     except Exception:
         handle(sys.exc_info())
         in_uuid = indiv_output = combined_output = False
     return in_uuid, indiv_output, combined_output, reason
@@ -2496,19 +2498,20 @@
             in_nokia = indiv_output = combined_output = False
         else:
             to_int = int(timestamp, 16)
             int_diff = to_int ^ 4294967295
             int_diff = ~int_diff + 1
             unix_ts = int_diff + (epochs[2050] - epochs[1970]).total_seconds()
             if unix_ts < 0:
+                in_nokia = indiv_output = combined_output = False
                 pass
             else:
                 in_nokia = dt.utcfromtimestamp(unix_ts).strftime(__fmt__)
-            indiv_output = str(f"{ts_type}: {in_nokia}")
-            combined_output = str(f"{__red__}{ts_type}:\t\t\t{in_nokia} UTC{__clr__}")
+                indiv_output = str(f"{ts_type}: {in_nokia}")
+                combined_output = str(f"{__red__}{ts_type}:\t\t\t{in_nokia} UTC{__clr__}")
     except Exception:
         handle(sys.exc_info())
         in_nokia = indiv_output = combined_output = False
     return in_nokia, indiv_output, combined_output, reason
 
 
 def to_nokia(dt_val):
@@ -2544,19 +2547,20 @@
                 [timestamp[i : i + 2] for i in range(0, len(timestamp), 2)][::-1]
             )
             to_int = int(to_be, 16)
             int_diff = to_int ^ 4294967295
             int_diff = ~int_diff + 1
             unix_ts = int_diff + (epochs[2050] - epochs[1970]).total_seconds()
             if unix_ts < 0:
+                in_nokiale = indiv_output = combined_output = False
                 pass
             else:
                 in_nokiale = dt.utcfromtimestamp(unix_ts).strftime(__fmt__)
-            indiv_output = str(f"{ts_type}: {in_nokiale}")
-            combined_output = str(f"{__red__}{ts_type}:\t\t\t{in_nokiale} UTC{__clr__}")
+                indiv_output = str(f"{ts_type}: {in_nokiale}")
+                combined_output = str(f"{__red__}{ts_type}:\t\t\t{in_nokiale} UTC{__clr__}")
     except Exception:
         handle(sys.exc_info())
         in_nokiale = indiv_output = combined_output = False
     return in_nokiale, indiv_output, combined_output, reason
 
 
 def to_nokiale(dt_val):
@@ -2787,14 +2791,15 @@
             bitdate_hr = int(to_binary[21:26], 2)
             bitdate_min = int(to_binary[26:32], 2)
             try:
                 in_bitdate = dt(
                     bitdate_yr, bitdate_mon, bitdate_day, bitdate_hr, bitdate_min
                 ).strftime(__fmt__)
             except ValueError:
+                in_bitdate = indiv_output = combined_output = False
                 pass
             indiv_output = str(f"{ts_type}: {in_bitdate}")
             combined_output = str(
                 f"{__red__}{ts_type}:\t\t\t{in_bitdate} Local{__clr__}"
             )
     except Exception:
         handle(sys.exc_info())
@@ -3205,26 +3210,30 @@
 
 def main():
     """Parse all passed arguments"""
     now = dt.now().strftime(__fmt__)
     arg_parse = argparse.ArgumentParser(
         description=f"Time Decoder and Converter v"
         f"{str(__version__)} - supporting "
-        f"{str(__types__)} timestamps!",
+        f"{str(__types__)} timestamps!\n\n"
+        f"Some timestamps are only part of the entire value, and as such, full\n"
+        f"timestamps may not be generated based on only the date/time portion.",
         formatter_class=argparse.RawTextHelpFormatter,
     )
     arg_parse.add_argument(
-        "--guess", metavar="", help="guess format and output possibilities"
+        "--guess",
+        metavar="TIMESTAMP",
+        help="guess the timestamp format and output possibilities"
     )
     arg_parse.add_argument(
         "--timestamp",
         metavar="DATE",
         help="convert date to every timestamp\n"
-        'enter date as "YYYY-MM-DD HH:MM:SS.f" in 24h fmt.\n'
-        "Without argument gives current date/time\n",
+        'enter date as "YYYY-MM-DD HH:MM:SS.f" in 24h fmt\n'
+        "Without DATE argument, will convert current date/time\n",
         nargs="?",
         const=now,
     )
     arg_parse.add_argument(
         "--active", metavar="", help="convert from Active Directory value"
     )
     arg_parse.add_argument(
@@ -3265,34 +3274,34 @@
     )
     arg_parse.add_argument(
         "--exfat", metavar="", help="convert from an exFAT 4-byte value"
     )
     arg_parse.add_argument(
         "--fat", metavar="", help="convert from FAT Date + Time (wFat)"
     )
-    arg_parse.add_argument("--ft", metavar="", help="convert from FILETIME value")
+    arg_parse.add_argument("--ft", metavar="", help="convert from a FILETIME value")
     arg_parse.add_argument(
         "--gbound", metavar="", help="convert from a GMail Boundary value"
     )
     arg_parse.add_argument(
         "--gmsgid", metavar="", help="convert from a GMail Message ID value"
     )
     arg_parse.add_argument("--gps", metavar="", help="convert from a GPS value")
     arg_parse.add_argument("--gsm", metavar="", help="convert from a GSM value")
     arg_parse.add_argument(
-        "--hfsbe", metavar="", help="convert from HFS(+) BE, HFS Local, HFS+ UTC"
+        "--hfsbe", metavar="", help="convert from HFS(+) BE (HFS=Local, HFS+=UTC)"
     )
     arg_parse.add_argument(
-        "--hfsle", metavar="", help="convert from HFS(+) LE, HFS Local, HFS+ UTC"
+        "--hfsle", metavar="", help="convert from HFS(+) LE (HFS=Local, HFS+=UTC)"
     )
     arg_parse.add_argument(
-        "--hfsdec", metavar="", help="convert from Mac OS/HFS+ Decimal Time"
+        "--hfsdec", metavar="", help="convert from a Mac OS/HFS+ Decimal value"
     )
     arg_parse.add_argument("--hotmail", metavar="", help="convert from a Hotmail value")
-    arg_parse.add_argument("--ios", metavar="", help="convert from iOS 11 value")
+    arg_parse.add_argument("--ios", metavar="", help="convert from an iOS 11 value")
     arg_parse.add_argument(
         "--kstime", metavar="", help="convert from a KSUID 9-digit value"
     )
     arg_parse.add_argument(
         "--ksuid", metavar="", help="convert from a KSUID 27-character value"
     )
     arg_parse.add_argument("--mac", metavar="", help="convert from Mac Absolute Time")
@@ -3327,32 +3336,32 @@
         "--nsdate",
         metavar="",
         help="convert from an Apple NSDate (iOS, BPList, Cocoa, Mac Absolute)",
     )
     arg_parse.add_argument(
         "--oleb",
         metavar="",
-        help="convert from Windows OLE 64-bit BE, remove 0x & space\n"
+        help="convert from a Windows OLE 64-bit BE value, remove 0x & space\n"
         "- example from SRUM: 0x40e33f5d 0x97dfe8fb should be 40e33f5d97dfe8fb",
     )
     arg_parse.add_argument(
-        "--olel", metavar="", help="convert from Windows OLE 64-bit LE"
+        "--olel", metavar="", help="convert from a Windows OLE 64-bit LE value"
     )
     arg_parse.add_argument("--pr", metavar="", help="convert from Mozilla's PRTime")
     arg_parse.add_argument(
-        "--s32", metavar="", help="convert from an S32-encoded timestamp"
+        "--s32", metavar="", help="convert from an S32-encoded value"
     )
     arg_parse.add_argument(
         "--sony", metavar="", help="convert from a Sonyflake URL value"
     )
     arg_parse.add_argument(
         "--sym", metavar="", help="convert from Symantec's 6-byte AV value"
     )
     arg_parse.add_argument(
-        "--systime", metavar="", help="convert from 128-bit SYSTEMTIME value"
+        "--systime", metavar="", help="convert from a 128-bit SYSTEMTIME value"
     )
     arg_parse.add_argument(
         "--tiktok", metavar="", help="convert from a TikTok URL value"
     )
     arg_parse.add_argument(
         "--twitter", metavar="", help="convert from a Twitter URL value"
     )
```

### Comparing `time_decode-6.0/time_decode.egg-info/PKG-INFO` & `time_decode-6.1.0/time_decode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-decode
-Version: 6.0
+Version: 6.1.0
 Summary: Python 3 timestamp decode/encode tool
 Home-page: https://github.com/digitalsleuth/time_decode
 Author: Corey Forman
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,16 +28,16 @@
 `python3 -m pip install time-decode` or `python3 -m pip install git+https://github.com/digitalsleuth/time_decode`
 
 This python script provides the following conversions from existing timestamps:
 
 - 128-bit SYSTEMTIME
 - 32-bit MS-DOS time, result is Local
 - Active Directory value
-- Apple Biome hex format
 - Apple Biome 64-bit decimal format
+- Apple Biome hex format
 - Bitwise decimal 10-digit
 - BPlist (as NSDate)
 - Cocoa Core (as NSDate)
 - DHCP6 DUID
 - Discord URL
 - exFAT
 - FAT Date + Time (wFat)
```

