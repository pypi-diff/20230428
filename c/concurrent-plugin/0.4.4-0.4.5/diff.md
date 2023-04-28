# Comparing `tmp/concurrent_plugin-0.4.4-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,19 @@
-Zip file size: 30857 bytes, number of entries: 18
--rw-rw-r--  2.0 unx        2 b- defN 22-Nov-27 22:37 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    31832 b- defN 23-Apr-19 15:02 concurrent_plugin/concurrent_backend.py
--rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-17 04:51 concurrent_plugin/concurrent_core.py
--rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 23:54 concurrent_plugin/login.py
--rw-rw-r--  2.0 unx     3994 b- defN 22-Dec-20 19:35 concurrent_plugin/periodic_run.py
--rw-rw-r--  2.0 unx     1298 b- defN 23-Jan-19 23:36 concurrent_plugin/periodic_run_utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/__init__.py
--rw-rw-r--  2.0 unx      990 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_download.py
--rw-rw-r--  2.0 unx     1339 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_prefetch.py
--rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinfs.py
--rw-rw-r--  2.0 unx     5326 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinmount.py
--rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    15276 b- defN 23-Apr-09 17:20 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      205 b- defN 23-Apr-19 15:03 concurrent_plugin-0.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 15:03 concurrent_plugin-0.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx      182 b- defN 23-Apr-19 15:03 concurrent_plugin-0.4.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-19 15:03 concurrent_plugin-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-19 15:03 concurrent_plugin-0.4.4.dist-info/RECORD
-18 files, 106719 bytes uncompressed, 28069 bytes compressed:  73.7%
+Zip file size: 30346 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx        2 b- defN 22-Dec-14 21:27 concurrent_plugin/__init__.py
+-rw-rw-r--  2.0 unx    31832 b- defN 23-Apr-27 01:05 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-14 21:27 concurrent_plugin/concurrent_core.py
+-rw-rw-r--  2.0 unx    15759 b- defN 23-Apr-27 01:05 concurrent_plugin/login.py
+-rw-rw-r--  2.0 unx     3994 b- defN 23-Apr-27 01:05 concurrent_plugin/periodic_run.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/__init__.py
+-rw-rw-r--  2.0 unx      990 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_download.py
+-rw-rw-r--  2.0 unx     1339 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_prefetch.py
+-rw-rw-r--  2.0 unx    10783 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinfs.py
+-rw-rw-r--  2.0 unx     5326 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinmount.py
+-rw-rw-r--  2.0 unx     1140 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/mount_main.py
+-rw-rw-r--  2.0 unx    15402 b- defN 23-Apr-28 07:15 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      268 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      181 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1567 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/RECORD
+17 files, 105513 bytes uncompressed, 27712 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,17 +9,14 @@
 
 Filename: concurrent_plugin/login.py
 Comment: 
 
 Filename: concurrent_plugin/periodic_run.py
 Comment: 
 
-Filename: concurrent_plugin/periodic_run_utils.py
-Comment: 
-
 Filename: concurrent_plugin/infinfs/__init__.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_download.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_prefetch.py
@@ -33,23 +30,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.4.4.dist-info/METADATA
+Filename: concurrent_plugin-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.4.4.dist-info/WHEEL
+Filename: concurrent_plugin-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.4.4.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.4.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.4.dist-info/top_level.txt
+Filename: concurrent_plugin-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.4.dist-info/RECORD
+Filename: concurrent_plugin-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/infinfs/mount_service.py

```diff
@@ -278,14 +278,16 @@
     print_info("Starting..")
     HOST = "127.0.0.1"
     PORT = 7963
     last_upload_time = time.time()
     start_time = time.time()
     print("Environment #", os.environ)
     config.load_incluster_config()
+    print('Setting k8s client configuration item retries to 10', flush=True)
+    kubernetes.client.configuration.retries = 10
     k8s_client:client.CoreV1Api = client.CoreV1Api()
     run_id = os.getenv('MLFLOW_RUN_ID')
     pod_name = os.getenv('MY_POD_NAME')
     pod_namespace = os.getenv('MY_POD_NAMESPACE')
     dag_execution_id = os.getenv('DAG_EXECUTION_ID')
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.settimeout(15)
```

## Comparing `concurrent_plugin-0.4.4.dist-info/RECORD` & `concurrent_plugin-0.4.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
 concurrent_plugin/concurrent_backend.py,sha256=iIeT_QfncYXoIxuyD76M_kBCb1jUOXGRcK1ls57KtQE,31832
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
-concurrent_plugin/periodic_run_utils.py,sha256=MZuX9uSFEuA7B8UFDAchsrWhidXT5QyuOA-GDtzIPOo,1298
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
-concurrent_plugin/infinfs/mount_service.py,sha256=y2vNoDpEXLm95ch_GDhnVNF7oXf8I9fvQZhjc_JNcX4,15276
-concurrent_plugin-0.4.4.dist-info/METADATA,sha256=tD9iAbMMlDWz4cJcNMqEqgsCsEcOwv61t9nvO4cxBM4,205
-concurrent_plugin-0.4.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.4.4.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
-concurrent_plugin-0.4.4.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.4.4.dist-info/RECORD,,
+concurrent_plugin/infinfs/mount_service.py,sha256=6dCIqKUzlmR_kDWu67ax5Gbga503AD429RrueacIFOE,15402
+concurrent_plugin-0.4.5.dist-info/METADATA,sha256=ic_lXGzALGwSpAcG2f12-D7sAvIl2nBquNJmiP4kQd8,268
+concurrent_plugin-0.4.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.4.5.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
+concurrent_plugin-0.4.5.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.4.5.dist-info/RECORD,,
```

