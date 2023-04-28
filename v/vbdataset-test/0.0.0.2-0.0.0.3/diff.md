# Comparing `tmp/vbdataset_test-0.0.0.2-py3-none-any.whl.zip` & `tmp/vbdataset_test-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2333 bytes, number of entries: 6
+Zip file size: 2816 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-28 05:36 vbdataset/__init__.py
--rw-rw-rw-  2.0 fat     1848 b- defN 23-Apr-28 05:19 vbdataset/fetch.py
--rw-rw-rw-  2.0 fat      275 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      485 b- defN 23-Apr-28 06:33 vbdataset_test-0.0.0.2.dist-info/RECORD
-6 files, 2833 bytes uncompressed, 1449 bytes compressed:  48.9%
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-Apr-28 10:40 vbdataset/fetch.py
+-rw-rw-rw-  2.0 fat      296 b- defN 23-Apr-28 10:42 vbdataset_test-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 10:42 vbdataset_test-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-28 10:42 vbdataset_test-0.0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      485 b- defN 23-Apr-28 10:42 vbdataset_test-0.0.0.3.dist-info/RECORD
+6 files, 4621 bytes uncompressed, 1932 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vbdataset/__init__.py
 Comment: 
 
 Filename: vbdataset/fetch.py
 Comment: 
 
-Filename: vbdataset_test-0.0.0.2.dist-info/METADATA
+Filename: vbdataset_test-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: vbdataset_test-0.0.0.2.dist-info/WHEEL
+Filename: vbdataset_test-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: vbdataset_test-0.0.0.2.dist-info/top_level.txt
+Filename: vbdataset_test-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: vbdataset_test-0.0.0.2.dist-info/RECORD
+Filename: vbdataset_test-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vbdataset/fetch.py

```diff
@@ -1,51 +1,93 @@
+import json
 import os
 from datetime import datetime
 from pathlib import Path
+from re import search
+from typing import List
 
 import boto3
 import pymongo
 from botocore.client import Config
+from tqdm import tqdm
 
 S3 = boto3.resource('s3',
                     endpoint_url='http://172.19.221.184:9000',
                     aws_access_key_id='grai_user',
                     aws_secret_access_key='grailab12#',
                     config=Config(signature_version='s3v4'))
 S3_BUCKET = S3.Bucket('vaai-body')
 
+MONGO = pymongo.MongoClient(host='172.19.195.104')   
+GESTURE_DB = MONGO['gestureDB'] 
 
 
-def download_test():
-    print('download')
 
+def fetch_db(fetch_path: str,
+             actors: List[str] = ['all'], 
+             gesture_types: List[str] = ['all'], 
+             isTalk: bool = False,
+             gesture_styles: List[str] = ['all']):
+    '''
+    
+    Fetching data by defined conditions.
+
+    Args:
+        fetch_path (str): decide path to fetch data
+        actors (List[str]): decide which actor's data to fetch.
+        gesture_types (List[str]): decide which gesture type to fetch. 
+        isTalk (boolean): decide whether talk or non-talk data to fetch.
+        gesture_styles (List[str]): decide which gesture style to fecth.
 
-def create_db_by_condition(db, search_type="or", **kwargs):
-    assert search_type in ['or', 'and'], "Wrong search type"
+    '''
+
+    assert type(isTalk) == bool, "'isTalk' argument type must be boolean"
 
     now = datetime.now()
     dt_string = now.strftime("%Y-%m-%d-%H-%M-%S")
 
-    filter_list = []
-    for (filter_type, values) in kwargs.items():
-        assert filter_type in ['file_name', 'actor', 'status', 'subject', 'is_talk'], "Wrong filtering option"
-        if filter_type == 'file_name':
-            filter_type = 'fileName'
-        if filter_type == 'is_talk':
-            filter_type = 'isTalk'
-        for v in values:
-            if type(v) is not str:
-                pass
-            filter_list.append({filter_type: v})
+    conditions = '{}'
+    condition_json = json.loads(conditions)
+
+    if actors != ['all'] and len(actors) > 0:
+        condition_json.update({"actor" : {"$in": actors}})
 
-    bvh_download_path = Path(__file__).resolve().parent.parent.parent / 'data' / dt_string / 'bvh'
-    wav_download_path = Path(__file__).resolve().parent.parent.parent / 'data' / dt_string / 'wav'
+    if gesture_types != ['all'] and len(gesture_types) > 0:
+        for g_type in gesture_types:
+            assert g_type in ['emblem', 'manipulator', 'illustrator', 'affect display', 'regulator', 'all'], \
+                        "Gesture type must be 'emblem', 'manipulator', 'illustrator', 'affect display', 'regulator' or 'all'"
+        condition_json.update({"status" : {"$in": gesture_types}})
+
+    if gesture_styles != ['all'] and len(gesture_styles) > 0:
+        for g_style in gesture_styles:
+            assert g_style in ['introvert', 'extrovert', 'light', 'heavy', 'slow', 'hurry', 'all'], \
+                            "Gesture style must be 'introvert', 'extrovert', 'light', 'heavy', 'slow', 'hurry' or 'all'"
+        condition_json.update({"style" : {"$in": gesture_styles}})
+
+    bvh_download_path = Path(fetch_path) / dt_string / 'bvh'
+    wav_download_path = Path(fetch_path) / dt_string / 'wav'
     os.makedirs(bvh_download_path)
     os.makedirs(wav_download_path)
 
-    search_type = "$" + search_type
-    for x in db.gestures.find({search_type: filter_list}):
-        bvh_file_name = x['fileName'] + '.bvh'
-        S3_BUCKET.download_file(x['bvhFile'], bvh_download_path / bvh_file_name)
+    total_data_cnt = 0
+    for x in GESTURE_DB.gestures.find({'$and': [
+                                                {'isTalk': isTalk}, 
+                                                condition_json
+                                                ]
+                                      }):
+        bvh_file_name = x['fileName'] + str(x['_id']) + '.bvh'
+        try:
+            S3_BUCKET.download_file(x['bvhFile'], bvh_download_path / bvh_file_name)
+        except Exception:
+            print(f"[Error] {x['bvhFile']} is not exist")
+            continue
+        
         if x['audioFile'] is not None:
-            wav_file_name = x['fileName'] + '.wav'
-            S3_BUCKET.download_file(x['audioFile'], wav_download_path / wav_file_name)
+            wav_file_name = x['fileName'] + str(x['_id']) + '.wav'
+            try:
+                S3_BUCKET.download_file(x['audioFile'], wav_download_path / wav_file_name)
+            except Exception:
+                print(f"[Error] {x['audioFile']} is not exist")
+                pass
+        total_data_cnt += 1
+
+    print(f'Data fetching complete. number of data: {total_data_cnt}')
```

