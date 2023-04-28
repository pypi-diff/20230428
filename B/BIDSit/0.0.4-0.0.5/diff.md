# Comparing `tmp/BIDSit-0.0.4.tar.gz` & `tmp/BIDSit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.4.tar", last modified: Tue Apr 25 22:30:08 2023, max compression
+gzip compressed data, was "BIDSit-0.0.5.tar", last modified: Fri Apr 28 21:50:18 2023, max compression
```

## Comparing `BIDSit-0.0.4.tar` & `BIDSit-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.945249 BIDSit-0.0.4/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-25 22:30:08.944880 BIDSit-0.0.4/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.4/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-25 22:30:08.945356 BIDSit-0.0.4/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2447 2023-04-25 20:42:57.000000 BIDSit-0.0.4/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.938160 BIDSit-0.0.4/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.941739 BIDSit-0.0.4/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)    25705 2023-04-25 21:38:02.000000 BIDSit-0.0.4/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.4/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-04-19 23:11:33.000000 BIDSit-0.0.4/src/BIDSit/__main__ .py
--rw-r--r--   0 labmanager   (501) staff       (20)    49871 2023-04-25 22:29:01.000000 BIDSit-0.0.4/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-25 20:54:59.000000 BIDSit-0.0.4/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.944275 BIDSit-0.0.4/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      300 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.366238 BIDSit-0.0.5/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-28 21:50:18.365973 BIDSit-0.0.5/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.5/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-28 21:50:18.366325 BIDSit-0.0.5/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2447 2023-04-25 20:42:57.000000 BIDSit-0.0.5/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.360793 BIDSit-0.0.5/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.363938 BIDSit-0.0.5/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)     4701 2023-04-28 21:36:44.000000 BIDSit-0.0.5/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.5/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-04-19 23:11:33.000000 BIDSit-0.0.5/src/BIDSit/__main__ .py
+-rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.5/src/BIDSit/dicom_to_bids2.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    53467 2023-04-28 21:31:25.000000 BIDSit-0.0.5/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-28 21:37:08.000000 BIDSit-0.0.5/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.365573 BIDSit-0.0.5/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      329 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.4/PKG-INFO` & `BIDSit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BIDSit-0.0.4/README.rst` & `BIDSit-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.4/setup.py` & `BIDSit-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.4/src/BIDSit/go.py` & `BIDSit-0.0.5/src/BIDSit/go.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,21 +88,22 @@
                         else:
                             sub_list.append(os.path.join(entry,file))
             else:
                 if os.path.isdir(os.path.join(WDIR,entry)):
                     continue
                 else:
                     sub_list.remove(entry)
-                    
+        for sub in sub_list:
+            BIDSit(sub, user_info)
         # - multiprocessing - #
-        pool = Pool() # Create a multiprocessing Pool
-        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # BIDSit for each participant or time point
-        # - Close the pool, keep the kids safe - #
-        pool.close()
-        pool.join()
+#        pool = Pool() # Create a multiprocessing Pool
+#        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # BIDSit for each participant or time point
+#        # - Close the pool, keep the kids safe - #
+#        pool.close()
+#        pool.join()
         
         ### --- make all the other files --- ###
         if out_dir != WDIR:
             WDIR = out_dir
         dir = listdir(WDIR)
         for fld in dir:
             if 'tempdata' in fld:
@@ -570,23 +571,26 @@
     col3 = [drop for drop in dropdown.values()]
 
     # - get list of scans - #
     scan_list = []
     scan_key = []
     type_list = []
     for key, value in user_info.items():
-        if "fmap_task_num" in key or "anat_task_num" in key:
+        if "func_scan_num" in key:
+            scan_list.append(int(value))
+            scan_key.append(key.split('_')[0])
+        if "fmap_task_num" in key or "anat_task_num" in key or "func_task_num" in key:
             continue
         elif "task_num" in key:
             scan_list.append(int(value))
             scan_key.append(key.split('_')[0])
     for i, type in enumerate(scan_key):
         if type == 'func':
             for i in range(scan_list[i]):
-                type_list.append(type + ' task ' + str(i+1))
+                type_list.append(type + ' scan ' + str(i+1))
         else:
             for i in range(scan_list[i]):
                 type_list.append(type + ' scan type ' + str(i+1))
     layout_2 = [
         [[[text_element(f"What kind of fmap image is scan type {num}?"), menu(files, num)], [text_element(f"What images is scan type {num} intended for? (select all that apply)"), sg.Push(), list_element(type_list, num)]] for num in range(1, int(task_num)+1)],
         [sg.Button('Info', key='-info-')],
         [sg.vbottom(sg.Column([[text_element(f"Order for scan type {task_num}")] for task_num in range(1, int(task_num)+1)],
@@ -672,25 +676,33 @@
 #----------------------------#
 #       Main Functions       #
 #----------------------------#
 ### --- convert DICOMs and PAR/RECs to NIFTIs --- ###
 def dcm2niix(in_dir, WDIR, ses=False):
     WDIR = WDIR + '/tempdata'
     if ses:
-        WDIR = WDIR + '/' + in_dir.split('/')[-3] + '/' + in_dir.split('/')[-2]
+        WDIR = WDIR + '/' + in_dir.split('/')[-2] + '/' + in_dir.split('/')[-1]
     else:
-        WDIR = WDIR + '/' + in_dir.split('/')[-2]
+        WDIR = WDIR + '/' + in_dir.split('/')[-1]
     mkdir(WDIR)
     subprocess.call(['dcm2niix', '-b', 'y', '-ba', 'y', '-z', 'y', '-f', '%x_%p_%t_%s', '-o', WDIR, in_dir]) # (%a=antenna (coil) name, %b=basename, %c=comments, %d=description, %e=echo number, %f=folder name, %i=ID of patient, %j=seriesInstanceUID, %k=studyInstanceUID, %m=manufacturer, %n=name of patient, %o=mediaObjectInstanceUID, %p=protocol, %r=instance number, %s=series number, %t=time, %u=acquisition number, %v=vendor, %x=study ID; %z=sequence name; default '%f_%p_%t_%s')
 
 ### --- organize NIFTIs into BIDS --- ###
-def BIDSit(sub, user_info):
+def BIDSit(sub, user_info, *types):
+    print(user_info)
     # - define variables in use - #
-    in_dir = user_info['WDIR'] # file input
     WDIR = user_info['out_dir'] # file output (where the work is done)
+    mkdir(WDIR, 'rawdata')
+    in_dir = user_info['WDIR'] # file input
+    in_dir_og = in_dir
+    if not 'tempdata' in in_dir:
+        new_indir = in_dir.rsplit('/', 1)[0] + "/tempdata"
+        if not dir_exists(new_indir):
+            shutil.copytree(in_dir, new_indir)
+        in_dir = new_indir
 
     og_sub = sub
     if user_info['ses'] =='Yes':
         sub = 'sub-'+''.join(re.findall(r'\d+',sub.split('/')[0]))+ '_ses-'+''.join(re.findall(r'\d+',sub.split('/')[1]))
         f_sub = sub.split('_')[0]+'/'+sub.split('_')[1]
         sub_solo = sub.split('_')[0]
     else:
@@ -709,17 +721,20 @@
         if key in user_info:
             if not user_info[key]:
                 continue
             else:
                 process.append(key)
     
     ### --- organize in BIDS --- ###
-    variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task'], 'exts': ['.json']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['T1','T2','FLAIR','PD','UNIT1','angio'], 'exts': ['.json']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['dwi', 'dti', 'hardi', 'sbref'], 'exts': ['.json', '.bvec', '.bval']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['rev', 'epi','EPI', 'fieldmap', 'mag', 'ph', 'MAG', 'PH'], 'exts': ['.json']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2'], 'exts': ['.json', '.tsv']}}
+    variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task'], 'exts': ['.json']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['T1','T2','FLAIR','PD','UNIT1','angio'], 'exts': ['.json']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['dwi', 'DWI', 'dti', 'DTI', 'hardi', 'HARDI', 'sbref', 'SBREF'], 'exts': ['.json', '.bvec', '.bval']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['rev', 'epi','EPI', 'fieldmap', 'mag', 'ph', 'MAG', 'PH'], 'exts': ['.json']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2'], 'exts': ['.json', '.tsv']}}
     map_dict = {}
     for file_type in process:
+        if types:
+            file_type = types[0]
+            
         file_log = {"Scan type": file_type, 'changes':{}}
         task_num = int(user_info[f"{file_type}_task_num"])
         scan_num = int(user_info[f"{file_type}_scan_num"])
         
         task_ord, task_names, menu, ents, ent_list, entsc_list= [],[],[],[],[],[]
         for ent in variables[file_type]['ents'].keys():
             ent_list.append(variables[file_type]['ents'][ent]['names'])
@@ -759,62 +774,71 @@
                 tity_list.append(ents)
         scans = dict_it(ent_scan, tity_list) # mapping for user_input
         user_info['scans'] = scans
         
         if not scans: #if no mapping is required
             for scan in range(1,scan_num+1):
                 scans[f"Scan {scan}"] = []
-        
+        scans['general'] = {'task_order': task_ord}
         # - get dir and ending for fmap files - #
         if file_type == 'fmap':
             for i, type in enumerate(task_ord):
                 if menu[type] == 'epi (rev-b0)':
                     if not 'dir' in scans[f"Scan {i+1}"]:
-                        scans[f"Scan {i+1}"].append(f"dir-{user_info['fmap']['rev-b0']}")
+                        scans[f"Scan {i+1}"].append(f"dir-{user_info['fmap']['rev-b0']['rev-dir']}")
                     for j, entry in enumerate(scans[f"Scan {i+1}"]):
                         if 'acq' in entry:
-                            scans[f"Scan {i+1}"][j] = entry+'-rev-b0'
+                            scans[f"Scan {i+1}"][j] = entry+'-revb0'
+                            acq = True
                             break
                         else:
-                            scans[f"Scan {i+1}"].append('acq-rev-b0')
+                            acq = False
+                    if not acq:
+                        scans[f"Scan {i+1}"].append('acq-revb0')
                 else:
                     scans[f"Scan {i+1}"].append('dir-'+menu[type].split('(')[-1].split(')')[0])
             menu = [menu[i].split(' ')[0] for i in range(task_num)]
-        
+                
         # - get endings for files - #
         endings = []
         for i, (key, val) in enumerate(scans.items()):
             for value in val:
                 if 'echo' in value:
-                    endings.append(value)
+                    endings.append('_' + value)
                     val.remove(value)
             if len(endings)-1 != i:
                 endings.append('')
     
         # - Rename files - #
         exts = variables[file_type]['key_words']
         tasksLookedAt=[]
-        map_dict = {f"file_type": {'task_ord': task_ord, 'scans': scans}, 'WDIR': WDIR, 'f_sub':f_sub}
+        map_dict = {f"{file_type}": {'task_ord': task_ord, 'scans': scans}, 'WDIR': WDIR, 'f_sub': f_sub}
         for i in range(scan_num):
             files =[]
             file = ''
-            for ext in exts:
-                files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
+            if types:
+                i = types[1]
+                for ext in exts:
+                    files.append(glob.glob(f"{in_dir.split('tempdata')[0] + in_dir_og.rsplit('/',1)[1]}/{og_sub}/*{ext}*.nii*"))
+            else:
+                for ext in exts:
+                    files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
             files = natsorted([item for sub_list in files for item in sub_list])
             if not files:
                 print(f"No {file_type} files were found in {in_dir}/{og_sub}")
                 break
             file_list = []
             for f in files:
                 if 'AX' in f and 'REF' in f:
                     continue
                 else:
                     file_list.append(f)
+                    
             if file_type != 'func':
-                if (scan_num - i) != len(file_list):
+                if (scan_num - i) != len([item for sublist in file_list for item in sublist]):
                     for end in user_info[file_type][f"menu_{i+1}"].split('w')[0].split('('):
                         end = end.split(')')[0]
                         end = end.split()[0]
                         for f in file_list:
                             f_full = f
                             f = f.rsplit('/')[-1].lower()
                             if end in f:
@@ -828,17 +852,32 @@
                                 break
                             else:
                                 file = ''
                         break
                 else:
                     file = file_list[0]
             else:
-                file = file_list[0]
+                if (scan_num - i) != len([item for sublist in file_list for item in sublist]):
+                    file_list_full = file_list
+                    file_list = []
+                    for file in file_list_full:
+                        if not 'EPI' in file:
+                            file_list.append(file)
+                if not file_list:
+                    file = ''
+                else:
+                    file = file_list[0]
+            
             if not file:
-                print(f"No files for {og_sub} matching", user_info[file_type][f"menu_{i+1}"])
+                if types:
+                    return
+                if file_type == 'func':
+                    print(f"No more func files for {og_sub}")
+                else:
+                    print(f"No files for {og_sub} matching", user_info[file_type][f"menu_{i+1}"])
                 continue
             mkdir(WDIR, f"rawdata/{f_sub}/{file_type}")
             task_cat = task_ord[i] # task number (-1)
             f_type = menu[task_cat] # type of file
             endings[i] = endings[i] + '_' + f_type # adds file type to ending
             fill_it = '_'+'_'.join(scans[f"Scan {i+1}"])
             if fill_it == '_':
@@ -846,70 +885,100 @@
             # - counting - #
             occur = tasksLookedAt.count(task_cat) # counts occurance of task
             run_num = occur + 1 # run number based on how many times that task occured
             tasksLookedAt.append(task_cat) # add current occurance to task list
             # - naming - #
             if file_type == 'func':
                 task_name = ''.join(task_names[task_cat].split()) # task name
-                new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run_{run_num}{endings[i]}.nii.gz" # new name for file
+                new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run-{run_num}{endings[i]}.nii.gz" # new name for file
                 file_log['changes'][f"scan {i+1} old"] = file
                 file_log['changes'][f"scan {i+1} new"] = new
                 print("file:", file)
                 print("new:", new)
-                os.rename(file, new) # rename file
+                if types:
+                    shutil.copy(file, new)
+                else:
+                    os.rename(file, new) # rename file
                 json_file = file.replace('.nii.gz','.json') # get .json file assocated
-                json_new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run_{run_num}{endings[i]}.json" # new name for .json file
-                os.rename(json_file, json_new) # rename file
+                json_new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run-{run_num}{endings[i]}.json" # new name for .json file
+                if types:
+                    shutil.copy(json_file, json_new)
+                else:
+                    os.rename(json_file, json_new) # rename file
+                json_edit(json_new, file_type, f_sub, og_sub, user_info)
             else:
                 new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}.nii.gz" # new name for file
                 file_log['changes'][f"scan {i+1} old"] = file
                 file_log['changes'][f"scan {i+1} new"] = new
                 print("file:", file)
                 print("new:", new)
-                os.rename(file, new) # rename file
+                if types:
+                    shutil.copy(file, new)
+                else:
+                    os.rename(file, new) # rename file
+                if file_type == 'fmap':
+                    add_dict = {user_info['fmap'][f"menu_{i+1}"]: user_info['fmap'][f"-list_{i+1}-"]}
+                else:
+                    add_dict = {}
                 for ext in variables[file_type]['exts']:
                     if 'nii.gz' in file:
                         file = file.rsplit('.',2)[0] + ext
                     else:
                         file = file.rsplit('.',1)[0] + ext
                     new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}{ext}" # new name for file
-                    os.rename(file, new) # rename file
+                    if types:
+                        shutil.copy(file, new)
+                    else:
+                        os.rename(file, new) # rename file
                     if ext == '.json':
-                        json_edit(new, file_type, map_dict)
+                        json_edit(new, file_type, f_sub, og_sub, user_info, add_dict)
+            if types:
+                if dir_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}"):
+                    if file_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json"):
+                        with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'r') as file:
+                            data_add = json.load(file)
+                            file_log['changes'] = {**data_add['changes'], **file_log['changes']}
+                    with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'w') as file:
+                        json.dump(file_log, file, indent=4)
+                return new
         if dir_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}"):
+            if file_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json"):
+                with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'r') as file:
+                    data_add = json.load(file)
+                    file_log['changes'] = {**data_add['changes'], **file_log['changes']}
             with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'w') as file:
                 json.dump(file_log, file, indent=4)
-        
+                
 # - Edit json files - #
-def json_edit(json_f, file_type, m_dict, *dicts):
+def json_edit(json_f, file_type, f_sub, og_sub, info, *dicts):
+    sub_solo = f_sub.split('/')[0]
     dic = {}
     for dict in dicts:
         dic = {**dic, **dict}
-    with open(json_f) as file:
+    with open(json_f, 'r') as file:
         data = json.load(file)
-        for l_no, line in enumerate(file):
-            if 'WaterFatShift' in line:
-                WaterFatShift = float(re.sub(",", "", line.split()[1]))
-            elif 'ImagingFrequency' in line:
-                ImagingFrequency = float(re.sub(",", "", line.split()[1]))
-            elif 'ReconMatrixPE' in line:
-                ReconMatrixPE = int(re.sub(",", "", line.split()[1]))
-            elif 'EPI_Factor' in line:
-                EPI_Factor = int(re.sub(",", "", line.split()[1]))
-            elif 'EchoTrainLength' in line:
-                EchoTrainLength = int(re.sub(",", "", line.split()[1]))
-            elif 'EstimatedEffectiveEchoSpacing' in line:
-                EstimatedEffectiveEchoSpacing = int(re.sub(",", "", line.split()[1]))
-            elif 'EstimatedTotalReadoutTime' in line:
-                EstimatedTotalReadoutTime = int(re.sub(",", "", line.split()[1]))
+        for value in data.keys():
+            if 'WaterFatShift' in value:
+                WaterFatShift = data[value]
+            elif 'ImagingFrequency' in value:
+                ImagingFrequency = data[value]
+            elif 'ReconMatrixPE' in value:
+                ReconMatrixPE = data[value]
+            elif 'EchoTrainLength' in value:
+                EchoTrainLength = data[value]
+            elif 'EstimatedEffectiveEchoSpacing' in value:
+                EstimatedEffectiveEchoSpacing = data[value]
+            elif 'EstimatedTotalReadoutTime' in value:
+                EstimatedTotalReadoutTime = data[value]
+            elif 'PhaseEncodingDirection' == value:
+                PhaseEncodingDirection = data[value]
         try :
             WaterFatShift
             ImagingFrequency
             ReconMatrixPE
-            EPI_Factor
             EchoTrainLength
         except NameError:
             add_dict = {}
         else:
             ActualEchoSpacing = WaterFatShift / (ImagingFrequency * 3.4 * (EchoTrainLength + 1))
             TotalReadoutTime = ActualEchoSpacing * EchoTrainLength
             EffectiveEchoSpacing = TotalReadoutTime / (ReconMatrixPE - 1)
@@ -919,59 +988,72 @@
                 EstimatedEffectiveEchoSpacing
                 EstimatedTotalReadoutTime
             except NameError:
                 add_dict = {}
             else:
                 add_dict = {'subject_id': sub_solo, 'EffectiveEchoSpacing': EstimatedEffectiveEchoSpacing, 'TotalReadoutTime': EstimatedTotalReadoutTime}
         data = {**data, **add_dict}
-        if 'dir-AP' in file:
-            data['PhaseEncodingDirection'] = "j-" # Anterior to Posterior Phase Encoding Direction
-        elif 'dir-PA' in file:
-             data['PhaseEncodingDirection'] = "j" # Posterior to Anterior Phase Encoding Direction
-        if 'dir-LR' in file:
-            data['PhaseEncodingDirection'] = "i-" # Anterior to Posterior Phase Encoding Direction
-        elif 'dir-RL' in file:
-             data['PhaseEncodingDirection'] = "i" # Posterior to Anterior Phase Encoding Direction
+        try:
+            PhaseEncodingDirection
+        except NameError:
+            data['PhaseEncodingDirection'] = "Unknown: j- (AP), j (PA), i- (LR), i (RL)"
+            if 'dir-AP' in json_f:
+                data['PhaseEncodingDirection'] = "j-" # Anterior to Posterior Phase Encoding Direction
+            elif 'dir-PA' in json_f:
+                 data['PhaseEncodingDirection'] = "j" # Posterior to Anterior Phase Encoding Direction
+            if 'dir-LR' in json_f:
+                data['PhaseEncodingDirection'] = "i-" # Left to Right Phase Encoding Direction
+            elif 'dir-RL' in json_f:
+                 data['PhaseEncodingDirection'] = "i" # Right to Left Phase Encoding Direction
         if file_type == 'fmap':
             if 'rev' in json_f: # rev has to happen before in order to catch correctly
                 for key in dic:
                     if 'rev' in key:
                         f_list = dic[key] #AP
                         files = []
                         for item in f_list:
                             file_t = item.split()[0] # file type to look at
                             t_num = int(item.split()[-1])-1 # scan to look at
-                            if file_t in m_dict:
-                                task_ord = m_dict[file_t]['task_ord']
-                                scans = m_dict[file_t]['scans']
-                                idx = [i for i, x in enumerate(task_ord) if x == t_num]
-                                for i in idx:
-                                    search = '_*'.join(scans[f"Scan {i+1}"])
-                                    files.append(glob.glob(f"{m_dict['WDIR']}/rawdata/{m_dict['f_sub']}/{file_t}/*{search}*.nii.gz"))
+                            if file_t in info:
+                                print(f"running BIDSit for on {file_t} for {og_sub}")
+                                files.append(BIDSit(og_sub, info, file_t, t_num))
                         data['IntendedFor'] = files
+                        print(data['IntendedFor'])
+                        break
             else:
                 for key in dic:
-                    if key in json_f:
-                        f_list = dic[key] #AP
-                        files = []
-                        for item in f_list:
-                            file_t = item.split()[0] # file type to look at
-                            t_num = int(item.split()[-1])-1 # scan to look at
-                            if file_t in m_dict:
-                                task_ord = m_dict[file_t]['task_ord']
-                                scans = m_dict[file_t]['scans']
-                                idx = [i for i, x in enumerate(task_ord) if x == t_num]
-                                for i in idx:
-                                    search = '_*'.join(scans[f"Scan {i+1}"])
-                                    files.append(glob.glob(f"{m_dict['WDIR']}/rawdata/{m_dict['f_sub']}/{file_t}/*{search}*.nii.gz"))
-                        data['IntendedFor'] = files
-                        break
+                    f_list = dic[key] #AP
+                    files = []
+                    for item in f_list:
+                        file_t = item.split()[0] # file type to look at
+                        t_num = int(item.split()[-1])-1 # scan to look at
+                        if file_t in info:
+                            print(f"running BIDSit for on {file_t} for {og_sub}")
+                            files.append(BIDSit(og_sub, info, file_t, t_num))
+                    data['IntendedFor'] = files
+                    print(data['IntendedFor'])
+                    break
     with open(json_f, 'w') as file:
         json.dump(data, file, indent=4)
-
+    if 'IntendedFor' in data.keys():
+        for item in files:
+            item = item.split('.')[0] + ".json"
+            with open(item, 'r') as this:
+                datum = json.load(this)
+                if data['PhaseEncodingDirection'] == "j-":
+                    dict_add = {'PhaseEncodingDirection': "j"}
+                if data['PhaseEncodingDirection'] == "j":
+                    dict_add = {'PhaseEncodingDirection': "j-"}
+                if data['PhaseEncodingDirection'] == "i-":
+                    dict_add = {'PhaseEncodingDirection': "i"}
+                if data['PhaseEncodingDirection'] == "i":
+                    dict_add = {'PhaseEncodingDirection': "i-"}
+            datum = {**datum, **dict_add}
+            with open(item, 'w') as this:
+                json.dump(datum, this, indent=4)
 ### --- MISC Functions --- ###
 # - make a directory - #
 def mkdir(path,extension=''):
     path = os.path.join(path, extension)
     if not os.path.exists(path):
         os.makedirs(path)
```

### Comparing `BIDSit-0.0.4/src/BIDSit/version.py` & `BIDSit-0.0.5/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
```

### Comparing `BIDSit-0.0.4/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.5/src/BIDSit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

