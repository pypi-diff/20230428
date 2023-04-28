# Comparing `tmp/cf_speedtest-0.1.6.tar.gz` & `tmp/cf_speedtest-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cf_speedtest-0.1.6.tar", last modified: Sun Jan  3 08:32:28 2021, max compression
+gzip compressed data, was "cf_speedtest-0.1.7.tar", last modified: Fri Apr 28 10:35:22 2023, max compression
```

## Comparing `cf_speedtest-0.1.6.tar` & `cf_speedtest-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/
--rw-rw-rw-   0        0        0      632 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2021-01-03 03:15:12.000000 cf_speedtest-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest/
--rw-rw-rw-   0        0        0      107 2021-01-01 09:49:59.000000 cf_speedtest-0.1.6/cf_speedtest/__init__.py
--rw-rw-rw-   0        0        0     9400 2021-01-03 08:30:54.000000 cf_speedtest-0.1.6/cf_speedtest/cf_speedtest.py
--rw-rw-rw-   0        0        0    26343 2020-12-28 14:33:15.000000 cf_speedtest-0.1.6/cf_speedtest/locations.py
--rw-rw-rw-   0        0        0     1718 2021-01-01 14:51:49.000000 cf_speedtest-0.1.6/cf_speedtest/options.py
-drwxrwxrwx   0        0        0        0 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/
--rw-rw-rw-   0        0        0      632 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/cf_speedtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      939 2021-01-03 08:32:28.000000 cf_speedtest-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0       37 2020-12-26 13:23:35.000000 cf_speedtest-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:35:22.544106 cf_speedtest-0.1.7/
+-rw-rw-rw-   0        0        0     1069 2020-12-05 14:07:24.000000 cf_speedtest-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      729 2023-04-28 10:35:22.544106 cf_speedtest-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2021-01-03 08:52:32.000000 cf_speedtest-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 10:35:22.538105 cf_speedtest-0.1.7/cf_speedtest/
+-rw-rw-rw-   0        0        0      107 2021-01-01 09:49:58.000000 cf_speedtest-0.1.7/cf_speedtest/__init__.py
+-rw-rw-rw-   0        0        0       99 2023-04-28 10:20:42.000000 cf_speedtest-0.1.7/cf_speedtest/__main__.py
+-rw-rw-rw-   0        0        0    37239 2023-04-28 10:16:10.000000 cf_speedtest-0.1.7/cf_speedtest/locations.py
+-rw-rw-rw-   0        0        0     1718 2023-04-28 10:16:03.000000 cf_speedtest-0.1.7/cf_speedtest/options.py
+-rw-rw-rw-   0        0        0     9698 2023-04-28 10:21:28.000000 cf_speedtest-0.1.7/cf_speedtest/speedtest.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:35:22.543108 cf_speedtest-0.1.7/cf_speedtest.egg-info/
+-rw-rw-rw-   0        0        0      729 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 10:35:22.000000 cf_speedtest-0.1.7/cf_speedtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1007 2023-04-28 10:35:22.545105 cf_speedtest-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       37 2020-12-26 13:17:33.000000 cf_speedtest-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:35:22.543108 cf_speedtest-0.1.7/tests/
+-rw-rw-rw-   0        0        0      357 2023-04-28 10:20:42.000000 cf_speedtest-0.1.7/tests/test_all.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cf_speedtest-0.1.6/README.md` & `cf_speedtest-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 ## A simple internet speed test tool/library, which uses https://speed.cloudflare.com (provided by Cloudflare)
 
 [![PyPI version](https://img.shields.io/pypi/v/cf-speedtest.svg)](https://pypi.python.org/pypi/cf-speedtest)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/cf-speedtest.svg)](https://pypi.python.org/pypi/cf-speedtest)
 [![PyPI status](https://img.shields.io/pypi/status/cf-speedtest.svg)](https://pypi.python.org/pypi/cf-speedtest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cf-speedtest.svg)](https://pypi.python.org/pypi/cf-speedtest)
 
+## Installation:
+```bash
+$ pip install -U cf-speedtest
+```
+
 ## Basic CLI usage:
 
 - ### Running a normal speedtest:
 	- `cf_speedtest`
 
 - ### Without verifying SSL:
 	- `cf_speedtest --verifyssl=false`
```

### Comparing `cf_speedtest-0.1.6/cf_speedtest/cf_speedtest.py` & `cf_speedtest-0.1.7/cf_speedtest/speedtest.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import math
 import time
 import statistics
 from timeit import default_timer as timer
 from typing import Union
 import urllib3
 
-from . import options
-from . import locations
+import cf_speedtest.locations as locations
+import cf_speedtest.options as options
 
 REQ_SESSION = requests.Session()
 
 CGI_ENDPOINT 		= "https://speed.cloudflare.com/cdn-cgi/trace"
 DOWNLOAD_ENDPOINT 	= "https://speed.cloudflare.com/__down?measId=0&bytes={}"
 UPLOAD_ENDPOINT		= "https://speed.cloudflare.com/__up?measId=0"
 
@@ -105,17 +105,17 @@
 
 	return cgi_dict.get('loc') or "Unknown"
 
 def preamble() -> str:
 	r = REQ_SESSION.get(DOWNLOAD_ENDPOINT.format(0), verify=VERIFY_SSL,  proxies=PROXY_DICT)
 	r.raise_for_status()
 
-	our_ip 		= r.headers['cf-meta-ip']
-	colo 		= r.headers['cf-meta-colo']
-	server_city = r.headers.get('cf-meta-city') or colo #doesn't exist sometimes?
+	our_ip 		= r.headers.get('cf-meta-ip')
+	colo 		= r.headers.get('cf-meta-colo')
+	server_city = colo
 	server_country = next((loc.get('cca2') or "Unknown" for loc in locations.SERVER_LOCATIONS if loc["iata"] == colo.upper()), "Unknown")
 	preamble_str = f"Your IP:\t{our_ip} ({get_our_country()})\nServer loc:\t{server_city} ({colo}) - ({server_country})"
 
 	return preamble_str
 
 # runs x amount of y-byte tests, given a test_type ("down" or "up")
 # returns a list of measurements in bits per second
@@ -139,64 +139,68 @@
 # simulates what is ran on speed.cloudflare.com
 def run_standard_test(measurement_sizes: list, measurement_percentile: int = 90, verbose: bool = False, test_patience: int = 15) -> dict:
 	LATENCY_MEASUREMENTS 	= []
 	DOWNLOAD_MEASUREMENTS 	= []
 	UPLOAD_MEASUREMENTS 	= []
 
 	if verbose:
-		print(preamble())
+		print(preamble(), '\n')
 
 	latency_test()  # ignore first request as it contains http connection setup
 	for i in range(0, 20):
 		LATENCY_MEASUREMENTS.append(latency_test() * 1000)
 
 	# Assume the median latency is our latency (just like the website)
 	latency = percentile(LATENCY_MEASUREMENTS, 50)
 	jitter = statistics.stdev(LATENCY_MEASUREMENTS)
 	if verbose:
-		print(f"Latency: {latency:.2f} ms")
-		print(f"Jitter: {jitter:.2f} ms")
-		print("Running tests...")
+		print(f"{'Latency:':<16} {latency:.2f} ms")
+		print(f"{'Jitter:':<16} {jitter:.2f} ms")
+		print("Running speed tests...\n")
 	
 	first_dl_test, first_ul_test = True, True
 	continue_dl_test, continue_ul_test = True, True
+	current_up_speed_mbps = 0
+	current_down_speed_mbps = 0
 
 	# The SLOWEST test should take no longer than 30 seconds
 	for i in range(0, len(measurement_sizes)):
 		measurement = measurement_sizes[i]
 		download_test_count = (-2 * i + 12) 	# this is how the website does it
-		upload_test_count = (-2 * i + 10) 	# this is how the website does it
+		upload_test_count = (-2 * i + 10) 		# this is how the website does it
 		total_download_bytes = measurement * download_test_count
 		total_upload_bytes = measurement * upload_test_count
 
 		if not first_dl_test:
 			if current_down_speed_mbps * test_patience < total_download_bytes / 125000:
 				continue_dl_test = False
 		else:
 			first_dl_test = False
 		
 		if continue_dl_test:
 			#print(f"Testing download ({measurement / 1_000_000:.2f}MiB) ({download_test_count} time(s))")
 			DOWNLOAD_MEASUREMENTS += run_tests("down", measurement, download_test_count)
 			current_down_speed_mbps = percentile(DOWNLOAD_MEASUREMENTS, measurement_percentile) / 1_000_000
 			if verbose:
-				print(f"Current down: {current_down_speed_mbps:.2f} Mbit/sec")
+				# print(f"Current down: {current_down_speed_mbps:.2f} Mbit/sec")
+				print(f"{'Current speeds:':<24} {'Down: '}{current_down_speed_mbps:.2f} Mbit/sec\t{'Up: '}{current_up_speed_mbps:.2f} Mbit/sec")
 
 		if not first_ul_test:
 			if current_up_speed_mbps * test_patience < total_upload_bytes / 125000:
 				continue_ul_test = False
 		else:
 			first_ul_test = False
 
 		if continue_ul_test:
 			#print(f"Testing upload ({measurement / 1_000_000:.2f}MiB) ({upload_test_count} time(s))")
 			UPLOAD_MEASUREMENTS += run_tests("up", measurement, upload_test_count)
 			current_up_speed_mbps = percentile(UPLOAD_MEASUREMENTS, measurement_percentile) / 1_000_000
 			if verbose:
-				print(f"Current up: {current_up_speed_mbps:.2f} Mbit/sec")
+				# print(f"Current up: {current_up_speed_mbps:.2f} Mbit/sec")
+				print(f"{'Current speeds:':<24} {'Down: '}{current_down_speed_mbps:.2f} Mbit/sec\t{'Up: '}{current_up_speed_mbps:.2f} Mbit/sec")
 
 	# all raw measurements are in bits per second
 	pctile_download	= percentile(DOWNLOAD_MEASUREMENTS, measurement_percentile)
 	pctile_upload	= percentile(UPLOAD_MEASUREMENTS, measurement_percentile)
 	download_stdev 	= statistics.stdev(DOWNLOAD_MEASUREMENTS)
 	upload_stdev	= statistics.stdev(UPLOAD_MEASUREMENTS)
 
@@ -206,15 +210,14 @@
 		"latency_measurements"	: LATENCY_MEASUREMENTS,
 		'download_speed'		: pctile_download,
 		'upload_speed'			: pctile_upload,
 		'download_stdev'		: download_stdev,
 		'upload_stdev'			: upload_stdev,
 	}
 
-import pprint
 def main(argv=None) -> int:
 	global PROXY_DICT, VERIFY_SSL, OUTPUT_FILE
 	# disable annoying warning when using verify=False in requests.get("x", verify=False)
 	urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 	parser = argparse.ArgumentParser()
 	parser_with_args = options.add_run_options(parser)
@@ -256,14 +259,13 @@
 	speeds = run_standard_test(measurement_sizes, percentile, True, patience)
 
 	d = speeds['download_speed']
 	u = speeds['upload_speed']
 	d_s = speeds['download_stdev']
 	u_s = speeds['upload_stdev']
 
-	print(f"{args.percentile}th percentile download speed: {d/1_000_000:.2f} Mbit/sec")
-	print(f"{args.percentile}th percentile upload speed: {u/1_000_000:.2f} Mbit/sec")
+	print(f"{args.percentile}{'th percentile results:':<24} Down: {d/1_000_000:.2f} Mbit/sec\tUp: {u/1_000_000:.2f} Mbit/sec")
 
 	return 0
 
 if __name__ == '__main__':
-	exit(main())
+	raise SystemExit(main())
```

### Comparing `cf_speedtest-0.1.6/cf_speedtest/options.py` & `cf_speedtest-0.1.7/cf_speedtest/options.py`

 * *Files identical despite different names*

### Comparing `cf_speedtest-0.1.6/setup.cfg` & `cf_speedtest-0.1.7/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 665f 7370 6565 6474 6573 740d   = cf_speedtest.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e36  .version = 0.1.6
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e37  .version = 0.1.7
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 436f 6d6d 616e 642d 6c69 6e65 2069 6e74  Command-line int
 00000050: 6572 6e65 7420 7370 6565 6420 7465 7374  ernet speed test
 00000060: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000070: 6f6e 203d 2052 4541 444d 452e 6d64 0d0a  on = README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
@@ -27,33 +27,37 @@
 000001a0: 3a20 332e 360d 0a09 5072 6f67 7261 6d6d  : 3.6...Programm
 000001b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 000001c0: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
 000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 000001f0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
 00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000210: 5079 7468 6f6e 203a 3a20 332e 390d 0a0d  Python :: 3.9...
-00000220: 0a5b 6f70 7469 6f6e 735d 0d0a 7079 7468  .[options]..pyth
-00000230: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000240: 332e 362e 300d 0a70 6163 6b61 6765 7320  3.6.0..packages 
-00000250: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
-00000260: 5f72 6571 7569 7265 7320 3d20 7265 7175  _requires = requ
-00000270: 6573 7473 5b73 6f63 6b73 5d3e 3d32 2e32  ests[socks]>=2.2
-00000280: 322e 300d 0a69 6e63 6c75 6465 5f70 6163  2.0..include_pac
-00000290: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-000002a0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000002b0: 6b61 6765 732e 6669 6e64 5d0d 0a65 7863  kages.find]..exc
-000002c0: 6c75 6465 203d 200d 0a09 7465 7374 730d  lude = ...tests.
-000002d0: 0a09 2a2e 7465 7374 730d 0a09 2a2e 7465  ..*.tests...*.te
-000002e0: 7374 732e 2a0d 0a09 7465 7374 732e 2a0d  sts.*...tests.*.
-000002f0: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
-00000300: 795f 706f 696e 7473 5d0d 0a63 6f6e 736f  y_points]..conso
-00000310: 6c65 5f73 6372 6970 7473 203d 200d 0a09  le_scripts = ...
-00000320: 6366 2d73 7065 6564 7465 7374 203d 2063  cf-speedtest = c
-00000330: 665f 7370 6565 6474 6573 742e 6366 5f73  f_speedtest.cf_s
-00000340: 7065 6564 7465 7374 3a6d 6169 6e0d 0a09  peedtest:main...
-00000350: 6366 5f73 7065 6564 7465 7374 203d 2063  cf_speedtest = c
-00000360: 665f 7370 6565 6474 6573 742e 6366 5f73  f_speedtest.cf_s
-00000370: 7065 6564 7465 7374 3a6d 6169 6e0d 0a0d  peedtest:main...
-00000380: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000390: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000003a0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000210: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000230: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000240: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
+00000250: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000260: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
+00000270: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
+00000280: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000290: 3e3d 332e 362e 300d 0a70 6163 6b61 6765  >=3.6.0..package
+000002a0: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
+000002b0: 6c6c 5f72 6571 7569 7265 7320 3d20 7265  ll_requires = re
+000002c0: 7175 6573 7473 5b73 6f63 6b73 5d0d 0a69  quests[socks]..i
+000002d0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+000002e0: 6174 6120 3d20 5472 7565 0d0a 0d0a 5b6f  ata = True....[o
+000002f0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000300: 6669 6e64 5d0d 0a65 7863 6c75 6465 203d  find]..exclude =
+00000310: 200d 0a09 7465 7374 730d 0a09 2a2e 7465   ...tests...*.te
+00000320: 7374 730d 0a09 2a2e 7465 7374 732e 2a0d  sts...*.tests.*.
+00000330: 0a09 7465 7374 732e 2a0d 0a0d 0a5b 6f70  ..tests.*....[op
+00000340: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+00000350: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+00000360: 6970 7473 203d 200d 0a09 6366 2d73 7065  ipts = ...cf-spe
+00000370: 6564 7465 7374 203d 2063 665f 7370 6565  edtest = cf_spee
+00000380: 6474 6573 742e 7370 6565 6474 6573 743a  dtest.speedtest:
+00000390: 6d61 696e 0d0a 0963 665f 7370 6565 6474  main...cf_speedt
+000003a0: 6573 7420 3d20 6366 5f73 7065 6564 7465  est = cf_speedte
+000003b0: 7374 2e73 7065 6564 7465 7374 3a6d 6169  st.speedtest:mai
+000003c0: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
+000003d0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000003e0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

