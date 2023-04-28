# Comparing `tmp/mynacode-1.0.80-py3-none-any.whl.zip` & `tmp/mynacode-1.0.81-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8766 bytes, number of entries: 9
+Zip file size: 8768 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5689 b- defN 23-Apr-28 04:57 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 04:57 mynacode-1.0.80.dist-info/RECORD
-9 files, 28749 bytes uncompressed, 7586 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat     5678 b- defN 23-Apr-28 05:01 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/RECORD
+9 files, 28738 bytes uncompressed, 7588 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.80.dist-info/METADATA
+Filename: mynacode-1.0.81.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.80.dist-info/WHEEL
+Filename: mynacode-1.0.81.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.80.dist-info/top_level.txt
+Filename: mynacode-1.0.81.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.80.dist-info/RECORD
+Filename: mynacode-1.0.81.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -36,40 +36,40 @@
 
 
 def metadata(run_id = -999):
 
   installed_packages = pkg_resources.working_set #Save all installed packages for that project
   installed_packages_list = sorted(["%s = %s" % (i.key, i.version) for i in installed_packages])
 
-  project_info_list = ['Codebase Python ' + platform.python_version()]
+  system_info_list = ['Codebase Python ' + platform.python_version()]
   
-  project_info_list.append("    GPU    ")
+  system_info_list.append("    GPU    ")
   try:
       gpus = GPUtil.getGPUs()
       if len(gpus) == 0:
-          project_info_list.append("No NVIDIA GPU found")
+          system_info_list.append("No NVIDIA GPU found")
       else:
           for gpu in gpus:
             gpu_id = gpu.id
             gpu_name = gpu.name
             gpu_memory = gpu.memoryTotal
-            project_info_list.append("GPU ID " + str(gpu_id))
-            project_info_list.append(gpu_name)
-            project_info_list.append(str(gpu_memory) + " MB")
+            system_info_list.append("GPU ID " + str(gpu_id))
+            system_info_list.append(gpu_name)
+            system_info_list.append(str(gpu_memory) + " MB")
   except:
-      project_info_list.append("No NVIDIA Driver found")
+      system_info_list.append("No NVIDIA Driver found")
 
-  project_info_list.append("    CPU    ")
-  project_info_list.append(platform.processor())
-  project_info_list.append(platform.platform())
-  project_info_list.append(platform.machine())
-  project_info_list.append("    MEMORY    ")
-  project_info_list.append("RAM " + str(round(psutil.virtual_memory().total / (1024.0 **3))) + " GB")
+  system_info_list.append("    CPU    ")
+  system_info_list.append(platform.processor())
+  system_info_list.append(platform.platform())
+  system_info_list.append(platform.machine())
+  system_info_list.append("    MEMORY    ")
+  system_info_list.append("RAM " + str(round(psutil.virtual_memory().total / (1024.0 **3))) + " GB")
 
-  data = {'run_id' : run_id, 'installed_packages': str(installed_packages_list), 'username': username, 'key': key, 'run_information': str(project_info_list)}
+  data = {'run_id' : run_id, 'installed_packages': str(installed_packages_list), 'username': username, 'key': key, 'system_information': str(system_info_list)}
   
   response = requests.post(protocol+'://'+IP+'/api/add_metadata', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
     print("Metadata saved")
```

