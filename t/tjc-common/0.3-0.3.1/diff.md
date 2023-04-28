# Comparing `tmp/tjc_common-0.3-py3-none-any.whl.zip` & `tmp/tjc_common-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2937 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     2308 b- defN 22-Oct-18 05:52 tjc_common/__init__.py
--rw-rw-rw-  2.0 fat     1123 b- defN 22-Oct-18 06:34 tjc_common-0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      535 b- defN 22-Oct-18 06:34 tjc_common-0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Oct-18 06:34 tjc_common-0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Oct-18 06:34 tjc_common-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      469 b- defN 22-Oct-18 06:34 tjc_common-0.3.dist-info/RECORD
-6 files, 4538 bytes uncompressed, 2087 bytes compressed:  54.0%
+Zip file size: 3004 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2425 b- defN 23-Apr-19 11:22 tjc_common/__init__.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 23-Apr-20 05:43 tjc_common-0.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      554 b- defN 23-Apr-20 05:43 tjc_common-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 05:43 tjc_common-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 05:43 tjc_common-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      479 b- defN 23-Apr-20 05:43 tjc_common-0.3.1.dist-info/RECORD
+6 files, 4684 bytes uncompressed, 2134 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: tjc_common/__init__.py
 Comment: 
 
-Filename: tjc_common-0.3.dist-info/LICENSE
+Filename: tjc_common-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: tjc_common-0.3.dist-info/METADATA
+Filename: tjc_common-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: tjc_common-0.3.dist-info/WHEEL
+Filename: tjc_common-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: tjc_common-0.3.dist-info/top_level.txt
+Filename: tjc_common-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tjc_common-0.3.dist-info/RECORD
+Filename: tjc_common-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tjc_common/__init__.py

```diff
@@ -19,18 +19,21 @@
 def read_config():
     sysimage_path = ''
     need_use_sysimage = True
     need_print_time = True
     tjc_backend = ''  # 如'jnumpy'
 
     conn = ConfigParser()
-    if platform.system().lower() == 'windows':
-        file_path = "C:/Users/Public/TongYuan/syslab-python/tjc_common.ini"
-    else:
-        file_path = expanduser("~/TongYuan/syslab-python/tjc_common.ini")
+    ty_path = os.getenv("TONGYUAN_PATH")
+    file_path = ty_path + "/syslab-python/tjc_common.ini"
+    
+    # if platform.system().lower() == 'windows':
+    #     file_path = "C:/Users/Public/TongYuan/syslab-python/tjc_common.ini"
+    # else:
+    #     file_path = expanduser("~/TongYuan/syslab-python/tjc_common.ini")
 
     if os.path.exists(file_path):
         conn.read(file_path, encoding='utf-8')
         if conn.has_option('Config', 'sysimage_path'):
             sysimage_path = conn.get('Config', 'sysimage_path')
 
         if conn.has_option('Config', 'need_use_sysimage'):
@@ -52,19 +55,19 @@
     # 读配置文件
     sysimage_path, need_use_sysimage, need_print_time, tjc_backend = read_config()
 
     if tjc_backend != '':
         use_backend(tjc_backend)
 
     if sysimage_path == '':
+        ty_path = os.getenv("TONGYUAN_PATH")
         if platform.system().lower() == 'windows':
-            sysimage_path = "C:/Users/Public/TongYuan/.julia/environments/v1.7/JuliaSysimage.dll"
+            sysimage_path = ty_path + "/.julia/environments/v1.7/JuliaSysimage.dll"
         elif platform.system().lower() == 'linux':
-            sysimage_path = expanduser(
-                "~/TongYuan/.julia/environments/v1.7/JuliaSysimage.so")
+            sysimage_path = ty_path + "/.julia/environments/v1.7/JuliaSysimage.so"
 
     if need_use_sysimage:
         if os.path.exists(sysimage_path):
             use_sysimage(sysimage_path)
         else:
             print("%s 文件不存在！" % sysimage_path)
```

## Comparing `tjc_common-0.3.dist-info/LICENSE` & `tjc_common-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

