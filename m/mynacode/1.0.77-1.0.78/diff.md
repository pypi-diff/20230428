# Comparing `tmp/mynacode-1.0.77-py3-none-any.whl.zip` & `tmp/mynacode-1.0.78-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 6768 bytes, number of entries: 8
+Zip file size: 8785 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
--rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Mar-20 01:12 mynacode-1.0.77.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-20 01:12 mynacode-1.0.77.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-20 01:12 mynacode-1.0.77.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      605 b- defN 23-Mar-20 01:12 mynacode-1.0.77.dist-info/RECORD
-8 files, 22976 bytes uncompressed, 5718 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
+-rw-rw-rw-  2.0 fat     5731 b- defN 23-Apr-28 02:49 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 02:50 mynacode-1.0.78.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 02:50 mynacode-1.0.78.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 02:50 mynacode-1.0.78.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 02:50 mynacode-1.0.78.dist-info/RECORD
+9 files, 28791 bytes uncompressed, 7605 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: mlauto/mlauto.py
 Comment: 
 
 Filename: mynacode/__init__.py
 Comment: 
 
+Filename: mynacode/mynacode - Copy.py
+Comment: 
+
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.77.dist-info/METADATA
+Filename: mynacode-1.0.78.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.77.dist-info/WHEEL
+Filename: mynacode-1.0.78.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.77.dist-info/top_level.txt
+Filename: mynacode-1.0.78.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.77.dist-info/RECORD
+Filename: mynacode-1.0.78.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -1,33 +1,26 @@
 import numpy as np
 import os, sys
 import json, requests, ast
 import pkg_resources
 import GPUtil, platform, psutil
 from datetime import datetime
+from sklearn import metrics
 
 #protocol = 'https'
 protocol = 'http'
 
 
 IP = '127.0.0.1:8000'
 #IP = 'mynacode.com'
 #prev_func_list = ['a1zqw_9_', 'b1zqw_9_']
 prev_func_list = []
 prev_node = -999
 username = ""
 key = ""
-run_id = -999
-
-
-def reset_os_variables():
-
-    os.environ["include_variables"] = 'False'
-    os.environ["variables_to_track"] = '[]'
-    os.environ["variables_to_not_track"] = '[]'
   
 
 def login(uname, ky):
   global username
   global key
   
   print("Logging in...")
@@ -39,16 +32,15 @@
     username = uname
     key = ky
     print("Successfully connected to mynacode!")
   else:
     print("Credentials could not be verified.")
 
 
-def project(project_name, project_id = -999):
-  global run_id
+def metadata(node_id = -999):
 
   installed_packages = pkg_resources.working_set #Save all installed packages for that project
   installed_packages_list = sorted(["%s = %s" % (i.key, i.version) for i in installed_packages])
 
   project_info_list = ['Codebase Python ' + platform.python_version()]
   
   project_info_list.append("    GPU    ")
@@ -70,175 +62,117 @@
   project_info_list.append("    CPU    ")
   project_info_list.append(platform.processor())
   project_info_list.append(platform.platform())
   project_info_list.append(platform.machine())
   project_info_list.append("    MEMORY    ")
   project_info_list.append("RAM " + str(round(psutil.virtual_memory().total / (1024.0 **3))) + " GB")
 
-  data = {'project_id' : project_id, 'project_name': project_name, 'installed_packages': str(installed_packages_list),
+  data = {'run_id' : project_id, 'installed_packages': str(installed_packages_list),
           'username': username, 'key': key, 'run_information': str(project_info_list)}
   
-  response = requests.post(protocol+'://'+IP+'/api/create_project', data=data)
+  response = requests.post(protocol+'://'+IP+'/api/add_metadata', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
-    response_dict = ast.literal_eval(response.text)
-    
-    if response_dict['exists'] == 0:
-      print("Created a new project.")
-    else:
-      print("Project exists. Created a new run")
-      
-  run_id = response_dict['run_id']
-  reset_os_variables()    
-  
-def node(node_name = "", filename = "", lineno = 0, node_description="", library_function = 0):
-  global prev_node
-  
-  if prev_node == -999:
-    data = {'current_node_name': node_name, 'node_description': node_description,
-            'username': username, 'key': key, 'run_id': run_id,
-            'filepath': filename, 'line_number': lineno, 'library_function': library_function}
-  else:
-    data = {'current_node_name': node_name, 'connect_with':  prev_node, 'node_description': node_description,
-            'username': username, 'key': key, 'run_id': run_id,
-            'filepath': filename, 'line_number': lineno, 'library_function': library_function}
+    print("Metadata saved")
+   
 
-  response = requests.post(protocol+'://'+IP+'/api/create_node', data=data)
 
-  if response.text == '-1':
-    print("Authentication failed")
 
-      
-  prev_node = response.text #Store previous node
+def datasets(train, test, val):
 
+  train = np.array(train)
+  test = np.array(test)
+  val = np.array(val)
 
-def node_log(variables, main_function = False):
-  global prev_node
-  if len(variables) == 0:
-    return 0
-  
-  for var_key in variables:
-      if len(str(variables[var_key]))>40:
-          variables[var_key] = 'Large value'
-      else:
-          variables[var_key] = str(variables[var_key])
+  train_shape = train.shape
+  test_shape = test.shape
+  val_shape = val.shape
 
-  if main_function == True:
-      data = {'run_id':run_id, '_id': prev_node, 'type':'node', 'variables': str(variables), 'username': username, 'key': key, 'main_function':1}
-  else:
-      data = {'_id': prev_node, 'type':'node', 'variables': str(variables), 'username': username, 'key': key, 'main_function':0}
 
-  response = requests.post(protocol+'://'+IP+'/api/set_variables', data=data)
+  data = {'train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
+          'username': username, 'key': key}
+  
+  response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
+  
+  if response.text == '0':
+    print("Authentication failed")
+  else:
+    print("Datasets Information saved.")
 
+def csv_data(dataframe):
+    columns_list = dataframe.columns.values.tolist()
+    isnull_list = dataframe.isnull().sum().values.tolist()
+    isunique_list = dataframe.nunique().values.tolist()
+    dtypes_list = dataframe.dtypes.tolist()
 
-def include_variables(status = False, include_only = [], exclude_only = []):
-  if status == False:
-    return
-  elif status == True:
-    os.environ["include_variables"] = 'True'
-    
-    if len(include_only) != 0:
-      variables_to_track = []
-      for var in include_only:
-        variables_to_track.append(var)
-      os.environ["variables_to_track"] = str(variables_to_track)
-      print(os.environ["variables_to_track"])
-      
-    elif len(exclude_only) != 0:
-      variables_to_not_track = []
-      for var in exclude_only:
-        variables_to_not_track.append(var)
-      os.environ["variables_to_not_track"] = str(variables_to_not_track)
-      print(os.environ["variables_to_not_track"])
-      
-    else:
-      pass
+    data = ['columns_list': columns_list, 'isnull_list': isnull_list, 'isunique_list': isunique_list, 'dtypes_list': dtypes_list}
 
+    response = requests.post(protocol+'://'+IP+'/api/add_csv', data=data)
 
-def tracefunc(frame, event, arg):
-    save_function = False
-    library_function = False
-    global prev_func_list
-    
-    if '__autograph_generated' in frame.f_code.co_filename:
-        pass
-    elif 'Attributes' in frame.f_code.co_filename or 'Attributes' in frame.f_code.co_name:
-        pass
-    elif "Python" in frame.f_code.co_filename:
-        pass
-    elif "<module" in frame.f_code.co_name:
-        pass
-    elif ("<" in frame.f_code.co_name or "<" in frame.f_code.co_filename) and ("<ipython-input" not in frame.f_code.co_filename):
-        pass
-    elif "site-packages" in frame.f_code.co_filename:
-        pass
-    elif "dist-packages" in frame.f_code.co_filename:
-        pass
-    elif "lib/python" in frame.f_code.co_filename:
-        pass
-    elif "_init_" in frame.f_code.co_name:
-        pass
+    if response.text == '0':
+      print("Authentication failed")
     else:
-        save_function = True
-        
-    if save_function:
-        
-        if event == "call":
-            if not library_function:
-              if frame.f_code.co_name in prev_func_list:
-                return
-              else:
-                prev_func_list.pop(0)
-                prev_func_list.append(frame.f_code.co_name)
-
-            if library_function == True:
-                node(frame.f_code.co_filename.rsplit('/', 1)[1], frame.f_code.co_filename, frame.f_code.co_firstlineno,"", 1)
-            else:
-              if 'ipykernel' not in frame.f_code.co_filename:
-                  node(frame.f_code.co_name, frame.f_code.co_filename, frame.f_code.co_firstlineno,"", 0)
-              else:
-                  node(frame.f_code.co_name, 'Jupyter notebook', 0,"", 0)
-                  
-        if event == "return":
-            variables_to_log = {}
-            include_variables = os.environ.get("include_variables") == 'True'
-            
-            if include_variables:
-              variables_to_track = set(ast.literal_eval(os.environ.get("variables_to_track")))
-              variables_to_not_track = set(ast.literal_eval(os.environ.get("variables_to_not_track")))
-
-              if len(variables_to_track) != 0:
-                variables_to_log.update({key: frame.f_locals[key] for key in variables_to_track if key in frame.f_locals})
-                    
-              elif len(variables_to_not_track) != 0:
-                for key in frame.f_locals:
-                  if key not in variables_to_not_track:
-                    variables_to_log[key] = frame.f_locals[key]
-                    
-              else:
-                for key in frame.f_locals:
-                  variables_to_log[key] = frame.f_locals[key]
-                          
-
-              if frame.f_code.co_name == 'main': #code ends here
-                  node_log(variables_to_log, True)
-              else:
-                  node_log(variables_to_log, False)
+      print("CSV Information saved.")
 
-        return tracefunc
     
+
+def specificity(y_true, y_pred):
+    y_correct = np.isnan(np.divide(y_pred, y_true)) #0/0 -> nan, 1/0 -> inf
+    y_correct = np.sum(y_correct)
+    y_truth = np.count_nonzero(y_true == 0)
    
-def settrace(state=True, library_function=False, repitition = 2):
-  global prev_func_list
-  prev_func_list = ['f'] * repitition
-    
-  if state==True: 
-      sys.setprofile(tracefunc)
-  else:
-      sys.setprofile(None)
+    return float(y_correct/y_truth)
 
+def npv(y_true, y_pred): #Negative Predicted Value
+    y_correct = np.isnan(np.divide(y_pred, y_true)) #0/0 -> nan, 1/0 -> inf
+    y_correct = np.sum(y_correct)
+    y_predicted = np.count_nonzero(y_pred == 0)
+   
+    return float(y_correct/y_predicted)
 
+def get_roc_auc(y_true, y_pred):
+    fpr, tpr, threshold = roc_curve(y_true, y_pred)
+    roc_auc = auc(fpr, tpr)
+    gmeans = np.sqrt(tpr * (1 - fpr))
+    index = np.argmax(gmeans) #Returns index of max value
+    best_threshold = threshold[index]
+   
+    return fpr, tpr, roc_auc, gmeans, best_threshold, index
+
+def get_metrics(y_true, y_pred, threshold):
+    y_pred_binary = (y_pred > threshold).astype('float')
+   
+    prec = metrics.precision_score(y_true, y_pred_binary)
+    rec = metrics.recall_score(y_true, y_pred_binary)
+    spec = specificity(y_true, y_pred_binary)
+    f1 = metrics.f1_score(y_true, y_pred_binary)
+    acc = metrics.accuracy_score(y_true, y_pred_binary)
+    npv_val = npv(y_true, y_pred_binary)
+   
+    c_matrix = confusion_matrix(y_true, y_pred_binary, labels=[0,1])
+   
+    return prec, rec, spec, f1, acc, npv_val, c_matrix
+
+
+
+def results(predicted_values, test_labels, problem_type = 'binary classification', threshold = 0.5):
+    prec, rec, spec, f1, acc, npv_val, c_matrix = get_metrics(y_true, y_pred, threshold)
+    #t_cmatrix = PrettyTable(['', 'No Disease', 'Disease'])
+    #t_cmatrix.add_row(["No Disease", c_matrix[0][0], c_matrix[0][1]])
+    #t_cmatrix.add_row(["Disease", c_matrix[1][0], c_matrix[1][1]])                
+    #print(t_cmatrix)
+
+    data = {'node_id' : node_id, 'precision': prec, 'recall': recall, 'specificity': spec, 'f1': f1, 'accuracy': acc, 'npv': npv, 'c_matrix': c_matrix,
+            'username': username, 'key': key}
+
+    response = requests.post(protocol+'://'+IP+'/api/add_results', data=data)
+  
+    if response.text == '0':
+      print("Authentication failed")
+    else:
+      print("Results saved")
+
```

## Comparing `mynacode-1.0.77.dist-info/RECORD` & `mynacode-1.0.78.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
-mynacode/mynacode.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode-1.0.77.dist-info/METADATA,sha256=QNYwV31FTjg6Y6w0g6_IDE6wV--ERdQ2ODBmiJpZh4w,352
-mynacode-1.0.77.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.77.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.77.dist-info/RECORD,,
+mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
+mynacode/mynacode.py,sha256=02TM3b9jBmLEpFtHiNRbV8-DWrE2YAcySfh7RMnNXh8,5731
+mynacode-1.0.78.dist-info/METADATA,sha256=cAMLFLHiceeLV8McLt6sCFlaOHBdx-zudwo6YGOWaLI,352
+mynacode-1.0.78.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.78.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.78.dist-info/RECORD,,
```

