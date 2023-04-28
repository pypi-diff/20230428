# Comparing `tmp/mynacode-1.0.79-py3-none-any.whl.zip` & `tmp/mynacode-1.0.80-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8781 bytes, number of entries: 9
+Zip file size: 8766 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5715 b- defN 23-Apr-28 04:55 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 04:55 mynacode-1.0.79.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 04:55 mynacode-1.0.79.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 04:55 mynacode-1.0.79.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 04:55 mynacode-1.0.79.dist-info/RECORD
-9 files, 28775 bytes uncompressed, 7601 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat     5689 b- defN 23-Apr-28 04:57 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/RECORD
+9 files, 28749 bytes uncompressed, 7586 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.79.dist-info/METADATA
+Filename: mynacode-1.0.80.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.79.dist-info/WHEEL
+Filename: mynacode-1.0.80.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.79.dist-info/top_level.txt
+Filename: mynacode-1.0.80.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.79.dist-info/RECORD
+Filename: mynacode-1.0.80.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -24,15 +24,14 @@
   global key
   
   print("Logging in...")
   credentials = {'username':uname, 'key':ky, 'task':'login'}
   response = requests.post(protocol+'://'+IP+'/api/python_login', data=credentials)
   
   if response.text == '1':
-    reset_os_variables()
     username = uname
     key = ky
     print("Successfully connected to mynacode!")
   else:
     print("Credentials could not be verified.")
```

