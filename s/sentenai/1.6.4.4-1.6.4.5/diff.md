# Comparing `tmp/sentenai-1.6.4.4.tar.gz` & `tmp/sentenai-1.6.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentenai-1.6.4.4.tar", last modified: Thu Apr 27 15:20:31 2023, max compression
+gzip compressed data, was "sentenai-1.6.4.5.tar", last modified: Fri Apr 28 20:33:56 2023, max compression
```

## Comparing `sentenai-1.6.4.4.tar` & `sentenai-1.6.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.803426 sentenai-1.6.4.4/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.4/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-27 15:20:31.803482 sentenai-1.6.4.4/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.4/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.801980 sentenai-1.6.4.4/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9160 2023-04-27 15:19:47.000000 sentenai-1.6.4.4/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.4/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.803315 sentenai-1.6.4.4/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.4/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.4/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.4/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24090 2023-04-27 15:19:50.000000 sentenai-1.6.4.4/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-27 15:20:31.802581 sentenai-1.6.4.4/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-27 15:20:31.000000 sentenai-1.6.4.4/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-27 15:20:31.803689 sentenai-1.6.4.4/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-27 15:20:11.000000 sentenai-1.6.4.4/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.869784 sentenai-1.6.4.5/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.5/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-28 20:33:56.869864 sentenai-1.6.4.5/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.5/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.868024 sentenai-1.6.4.5/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9160 2023-04-27 15:19:47.000000 sentenai-1.6.4.5/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.5/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.869585 sentenai-1.6.4.5/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.5/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.5/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.5/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24241 2023-04-28 20:33:48.000000 sentenai-1.6.4.5/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.868715 sentenai-1.6.4.5/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-28 20:33:56.870080 sentenai-1.6.4.5/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-28 20:33:48.000000 sentenai-1.6.4.5/setup.py
```

### Comparing `sentenai-1.6.4.4/LICENSE` & `sentenai-1.6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/PKG-INFO` & `sentenai-1.6.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.4
+Version: 1.6.4.5
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.4/README.md` & `sentenai-1.6.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/sentenai/__init__.py` & `sentenai-1.6.4.5/sentenai/__init__.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/sentenai/api.py` & `sentenai-1.6.4.5/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/sentenai/stream/events.py` & `sentenai-1.6.4.5/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/sentenai/stream/metadata.py` & `sentenai-1.6.4.5/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.4/sentenai/stream/streams.py` & `sentenai-1.6.4.5/sentenai/stream/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 
 from queue import Queue
 from threading import Thread
 from concurrent.futures import ThreadPoolExecutor
 
 Update = namedtuple('Update', ['id', 'start', 'end', 'data'])
 
+
+def worker(q, workers, total):
+    with ThreadPoolExecutor(max_workers=workers) as pool:
+        v = 0
+        with tqdm(total=total, unit=" values") as pbar:
+            while True:
+                data = q.get()
+                if not data:
+                    pbar.update(total - v)
+                    break # exit on empty list
+                list(pool.map(index_data, data))
+                n = sum([len(v) for d, n, i, v in data])
+                v += n
+                pbar.update(n)
+
+
 def index_data(args):
     db, node, index, v = args
     counter = 0
     while counter < 10:
         data = cbor2.dumps(v)
         try:
             resp = db._post('nodes', node, 'types', index,
@@ -247,23 +263,26 @@
         if isinstance(key, tuple):
             return Stream(self, *key)
         else:
             return Stream(self, key)
 
     def __setitem__(self, key, content):
         workers = 32
+        chunksize = 4096
         if isinstance(key, tuple):
             if isinstance(key[-1], slice):
                 path = key[:-1]
                 path += key[-1].start
                 workers = key[-1].stop
+                chunksize = key.step or chunksize
             else:
                 path = key
         elif isinstance(key, slice):
             workers = key.stop
+            chunksize = key.step or chunksize
             path = key.start
         else:
             path = (key,)
 
         del self[path]
 
         if content is None:
@@ -331,78 +350,78 @@
 
                 self._put('nodes', nid, 'types', tmap[cname])
                 cmap[cname] = nid
                 dmap[cname] = []
 
             origin = self.origin
             res = []
-            with ThreadPoolExecutor(max_workers=workers) as pool:
-                for i, row in tqdm(df.iterrows(), total=len(df), unit='values', unit_scale=len(df.columns) - 1):
-                    if origin is not None:
-                        ts = (row['start'] - origin) // np.timedelta64(1, 'ns')
+            q = Queue()
+            Thread(target=worker, args=(q, workers, len(df) * (len(df.columns) - 1))).start()
+
+            for i, row in df.iterrows():
+                if origin is not None:
+                    ts = (row['start'] - origin) // np.timedelta64(1, 'ns')
+                else:
+                    ts = row['start'] // np.timedelta64(1, 'ns')
+                try:
+                    if 'end' in row and origin is not None:
+                        dur = (row['end'] - row['start']) // np.timedelta64(1, 'ns')
+                    elif origin is not None:
+                        dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
+                    elif 'end' in row:
+                        dur = (row['end'] - row['start']) // np.timedelta64(1, 'ns')
+                    else:
+                        dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
+                except IndexError:
+                    dur = 1
+
+                if dur <= 0: continue
+                for col, val in dict(row).items():
+                    if col == 'start' and 'start' in dmap:
+                        dmap[col].append((ts, dur))
+                    elif type(val) == float and math.isnan(val): # skip nans
+                        pass
+                    elif val is pd.NaT or val is None:
+                        pass
+                    elif col not in tmap:
+                        pass
+                    elif tmap[col] == 'point3':
+                        dmap[col].append((ts, dur, (val.x, val.y, val.z)))
+                    elif tmap[col] == 'point':
+                        dmap[col].append((ts, dur, (val.x, val.y)))
+                    elif tmap[col] == 'date':
+                        dmap[col].append((ts, dur, val.isoformat()))
+                    elif tmap[col] == 'time':
+                        dmap[col].append((ts, dur, val.isoformat()))
+                    elif tmap[col] == 'datetime':
+                        dmap[col].append((ts, dur, iso8601(val)))
+                    elif tmap[col] == 'timedelta':
+                        dmap[col].append((ts, dur, val // np.timedelta64(1, 'ns')))
                     else:
-                        ts = row['start'] // np.timedelta64(1, 'ns')
-                    try:
-                        if 'end' in row and origin is not None:
-                            dur = (row['end'] - row['start']) // np.timedelta64(1, 'ns')
-                        elif origin is not None:
-                            dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
-                        elif 'end' in row:
-                            dur = (row['end'] - row['start']) // np.timedelta64(1, 'ns')
-                        else:
-                            dur = (df['start'].iloc[i+1] - row['start']) // np.timedelta64(1, 'ns')
-                    except IndexError:
-                        dur = 1
-
-                    if dur <= 0: continue
-                    for col, val in dict(row).items():
-                        if col == 'start' and 'start' in dmap:
-                            dmap[col].append((ts, dur))
-                        elif type(val) == float and math.isnan(val): # skip nans
-                            pass
-                        elif val is pd.NaT or val is None:
-                            pass
-                        elif col not in tmap:
-                            pass
-                        elif tmap[col] == 'point3':
-                            dmap[col].append((ts, dur, (val.x, val.y, val.z)))
-                        elif tmap[col] == 'point':
-                            dmap[col].append((ts, dur, (val.x, val.y)))
-                        elif tmap[col] == 'date':
-                            dmap[col].append((ts, dur, val.isoformat()))
-                        elif tmap[col] == 'time':
-                            dmap[col].append((ts, dur, val.isoformat()))
-                        elif tmap[col] == 'datetime':
-                            dmap[col].append((ts, dur, iso8601(val)))
-                        elif tmap[col] == 'timedelta':
-                            dmap[col].append((ts, dur, val // np.timedelta64(1, 'ns')))
-                        else:
-                            dmap[col].append((ts, dur, val))
-
-                    if 'start' in dmap and len(dmap['start']) >= 4096:
-                        list(res) # force result
-                        res = pool.map(index_data, [(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
-                        for k, v in dmap.items():
-                            dmap[k] = []
-                    elif len(list(dmap.values())[0]) >= 4096:
-                        list(res) # force result
-                        res = pool.map(index_data, [(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
-                        for k, v in dmap.items():
-                            dmap[k] = []
+                        dmap[col].append((ts, dur, val))
 
-                if 'start' in dmap and len(dmap['start']) > 0:
-                    res = pool.map(index_data, [(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
+                if 'start' in dmap and len(dmap['start']) >= chunksize:
+                    q.put([(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
                     for k, v in dmap.items():
                         dmap[k] = []
-                    list(res) # force result
-                elif len(list(dmap.values())[0]) > 0:
-                    res = pool.map(index_data, [(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
+                elif len(list(dmap.values())[0]) >= chunksize:
+                    q.put([(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
                     for k, v in dmap.items():
                         dmap[k] = []
-                    list(res) # force result
+
+            if 'start' in dmap and len(dmap['start']) > 0:
+                q.put([(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
+                for k, v in dmap.items():
+                    dmap[k] = []
+            elif len(list(dmap.values())[0]) > 0:
+                q.put([(self, cmap[k], tmap[k], dmap[k]) for k, v in dmap.items()])
+                for k, v in dmap.items():
+                    dmap[k] = []
+            q.put([])
+            
                 
 
 
     def __delitem__(self, key):
         if isinstance(key, tuple):
             self._delete('paths', *key)
         else:
```

### Comparing `sentenai-1.6.4.4/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.5/sentenai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.4
+Version: 1.6.4.5
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.4/setup.py` & `sentenai-1.6.4.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.4',
+    version='1.6.4.5',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

