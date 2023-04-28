# Comparing `tmp/copy-to-1.0.9.tar.gz` & `tmp/copy-to-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-to-1.0.9.tar", last modified: Wed Feb 22 02:29:04 2023, max compression
+gzip compressed data, was "copy-to-1.1.0.tar", last modified: Fri Apr 28 00:43:51 2023, max compression
```

## Comparing `copy-to-1.0.9.tar` & `copy-to-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-02-22 02:29:04.476020 copy-to-1.0.9/
--rw-r--r--   0 burp      (1000) burp      (1001)     1071 2023-02-17 18:19:55.000000 copy-to-1.0.9/LICENSE
--rw-r--r--   0 burp      (1000) burp      (1001)     1959 2023-02-22 02:29:04.476020 copy-to-1.0.9/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)     1369 2023-02-22 00:20:00.000000 copy-to-1.0.9/README.md
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-02-22 02:29:04.476020 copy-to-1.0.9/copy_to.egg-info/
--rw-r--r--   0 burp      (1000) burp      (1001)     1959 2023-02-22 02:29:04.000000 copy-to-1.0.9/copy_to.egg-info/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)      201 2023-02-22 02:29:04.000000 copy-to-1.0.9/copy_to.egg-info/SOURCES.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        1 2023-02-22 02:29:04.000000 copy-to-1.0.9/copy_to.egg-info/dependency_links.txt
--rw-r--r--   0 burp      (1000) burp      (1001)       41 2023-02-22 02:29:04.000000 copy-to-1.0.9/copy_to.egg-info/entry_points.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        8 2023-02-22 02:29:04.000000 copy-to-1.0.9/copy_to.egg-info/top_level.txt
--rwxr--r--   0 burp      (1000) burp      (1001)    20030 2023-02-22 02:25:04.000000 copy-to-1.0.9/copy_to.py
--rw-r--r--   0 burp      (1000) burp      (1001)      718 2023-02-22 02:28:33.000000 copy-to-1.0.9/pyproject.toml
--rw-r--r--   0 burp      (1000) burp      (1001)       38 2023-02-22 02:29:04.476020 copy-to-1.0.9/setup.cfg
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:43:51.757149 copy-to-1.1.0/
+-rw-r--r--   0 burp      (1000) burp      (1001)     1071 2023-04-25 14:58:58.000000 copy-to-1.1.0/LICENSE
+-rw-r--r--   0 burp      (1000) burp      (1001)     2193 2023-04-28 00:43:51.757149 copy-to-1.1.0/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)     1603 2023-04-28 00:43:04.000000 copy-to-1.1.0/README.md
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:43:51.757149 copy-to-1.1.0/copy_to.egg-info/
+-rw-r--r--   0 burp      (1000) burp      (1001)     2193 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)      201 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/SOURCES.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        1 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/dependency_links.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)       41 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/entry_points.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        8 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/top_level.txt
+-rwxr-xr-x   0 burp      (1000) burp      (1001)    22523 2023-04-28 00:33:19.000000 copy-to-1.1.0/copy_to.py
+-rw-r--r--   0 burp      (1000) burp      (1001)      718 2023-04-28 00:43:39.000000 copy-to-1.1.0/pyproject.toml
+-rw-r--r--   0 burp      (1000) burp      (1001)       38 2023-04-28 00:43:51.757149 copy-to-1.1.0/setup.cfg
```

### Comparing `copy-to-1.0.9/LICENSE` & `copy-to-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-to-1.0.9/copy_to.py` & `copy-to-1.1.0/copy_to.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,223 @@
-#!/usr/bin/env python
+#i!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 
-def main():
-    import os
-    import shutil
-    import json
-    import sys
-    import errno
-    import argparse
-    import argcomplete
-    from pathlib import Path 
-    import IPython
+import os
+import shutil
+import json
+import sys
+import errno
+import argparse
+import argcomplete
+from pathlib import Path 
+import subprocess
+
+
+os.popen("eval $(register-python-argcomplete copy-to)").read()
+file=os.path.expanduser("~/.config/copy_to/confs.json")
+complete=os.path.expanduser("~/.config/copy_to/")
+folder=os.path.expanduser("~/.config/copy_to/")
+
+if not os.path.exists(folder):
+    os.makedirs(folder)
+
+if not os.path.exists(file):
+    with open(file, "w") as outfile:
+        json.dump({}, outfile)
+
+with open(file, 'r') as infile:
+    envs = json.load(infile)
+
+with open(file, 'w') as outfile: 
+    if not 'group' in envs:
+        envs['group'] = [] 
+    json.dump(envs, outfile)
+
+def is_valid_dir(parser, arg):
+    if os.path.isdir(arg):
+        return os.path.abspath(arg)
+    elif os.path.isfile(arg):
+        print('%s is a file. A folder is required' % arg)
+        raise SystemExit              
+    else:
+        print("The directory %s does not exist!" % arg)
+        raise SystemExit
+
+def is_valid_file_or_dir(parser, arg):
+    arg=os.path.abspath(arg)
+    if os.path.isdir(arg):
+        return arg
+    elif os.path.isfile(arg):
+        return arg              
+    elif os.path.exists(os.path.join(os.getcwd(), arg)):
+        return os.path.join(os.getcwd(), arg)
+    else:
+        print("The file/directory %s does not exist!" % arg)
+        raise SystemExit
 
-    from os.path import dirname, abspath
+def copy_to(dest, src):
+    for element in src:
+        exist_dest=os.path.join(dest, os.path.basename(os.path.normpath(element)))
+        if os.path.isfile(element):
+            shutil.copy2(element, exist_dest)
+            print("Copied to " + str(exist_dest))
+
+        elif os.path.isdir(element):
+            shutil.copytree(element, exist_dest, dirs_exist_ok=True)
+            print("Copied to " + str(exist_dest) + " and all it's inner content")
+
+def copy_from(dest, src):
+    for element in src:
+        exist_dest=os.path.join(dest, os.path.basename(os.path.normpath(element)))
+        if os.path.isfile(exist_dest):
+            shutil.copy2(exist_dest, element)
+            print("Copied to " + str(element))
+
+        elif os.path.isdir(exist_dest):
+            shutil.copytree(exist_dest, element, dirs_exist_ok=True)
+            print("Copied to " + str(element) + " and all it's inner content")
+
+
+def listAll():
+    for name, value in envs.items():
+        if not name == 'group':
+            print(name.upper() + ":")
+            print("     Dest:   '" + str(value['dest']) + "'")
+            print("     Src :")
+            for idx, src in enumerate(value['src']):
+                print("          " + str(idx+1) + ") '" + str(src) + "'")
+
+
+def filterListDoubles(a):
+    # https://stackoverflow.com/questions/9835762/how-do-i-find-the-duplicates-in-a-list-and-create-another-list-with-them
+    seen = set()
+    ret = [x for x in a if x not in seen and not seen.add(x)]
+    return ret
+
+def PathCompleter(**kwargs):
+    return os.path
+
+def PathOnlyDirsCompleter(**kwargs):
+    return [ name for name in os.listdir(str(os.getcwd())) if os.path.isdir(os.path.join(os.getcwd()), name) ]
+
+def SourceComplete():    
+    return range(1,4)
+
+def exist_name(parser, x):
+    not_exists=True
+    if x in envs or x == 'group' or x in envs['group']:
+        print("The name %s already exists as conf name!" % x)
+        listAll()
+        raise SystemExit 
+    return x
+
+def get_names(special=False):
+    names=[]
+    with open(file, 'r') as outfile:
+        envs = json.load(outfile)
+        for key, name in envs.items():
+            if not key == "group":
+                names.append(key)
+            else:
+                for e in envs['group']:
+                    names.append(e)
+        if special:
+            names.append("all")
+        return names
+
+def get_reg_names():
+    with open(file, 'r') as outfile:
+        envs = json.load(outfile)
+        names=[]
+        for key, name in envs.items():
+            if not key == "group":
+                names.append(key)
+        return names
+
+def get_group_names():
+    with open(file, 'r') as outfile:
+        envs = json.load(outfile)
+        names=[]
+        for e in envs['group']:
+            names.append(e)
+        return names
+
+def get_main_parser():
+    choices = argcomplete.completers.ChoicesCompleter
+    parser = argparse.ArgumentParser(description="Setup configuration to copy files and directories to",formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    subparser = parser.add_subparsers(dest='command')
+    list1 = subparser.add_parser('list')
+    run = subparser.add_parser('run')
+    run_reverse = subparser.add_parser('run-reverse')
+    add = subparser.add_parser('add')
+    delete = subparser.add_parser('delete')
+    add_source = subparser.add_parser('add-source')
+    add_group = subparser.add_parser('add-group')
+    delete_group = subparser.add_parser('delete-group')
+    reset_destination = subparser.add_parser('reset-destination')
+    delete_source = subparser.add_parser('delete-source')
+    reset_source = subparser.add_parser('reset-source')
+    help1 = subparser.add_parser('help')
+    list1.add_argument("name" , nargs='?', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_names(True))
+    run.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_names(True))
+    run_reverse.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_names(True))
+    delete.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    delete.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_reg_names())
+    add.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    add.add_argument("name" , type=lambda x: exist_name(parser, x) ,help="Configuration name", metavar="Configuration Name, ")
+    add.add_argument("dest" , type=lambda x: is_valid_dir(parser, x), metavar="Destination directory")
+    add.add_argument("src" , nargs='*', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
+    add_group.add_argument("groupname" , type=lambda x: exist_name(parser, x) ,help="Group name holding multiple configuration names", metavar="Group Name")
+    add_group.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    add_group.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_reg_names())
+    delete_group.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    delete_group.add_argument("groupname" , type=str ,help="Group name holding multiple configuration names", metavar="Group Name", choices=get_group_names())
+    add_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
+    add_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    add_source.add_argument("src" , nargs='+', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
+    reset_destination.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    reset_destination.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
+    reset_destination.add_argument("dest" , type=lambda x: is_valid_dir(parser, x), metavar="Destination directory", help="Destination directory")
+    delete_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    delete_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
+    delete_source.add_argument("src_num" , nargs='*', type=int, metavar="Source files and directories or Index numbers", help="Source files and directories or Index numbers")
+    reset_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
+    reset_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
+    reset_source.add_argument("src" , nargs='*', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
+    argcomplete.autocomplete(parser)
+    return parser
+
+def main():
+    os.popen("eval $(register-python-argcomplete copy-to)").read()
+    """from os.path import dirname, abspath
     d = dirname(abspath(__file__))
 
-    sys.path.append(d)
+    sys.path.append(d)"""
     #file=os.path.expanduser("~/.copy_to_confs.json")
+    
     file=os.path.expanduser("~/.config/copy_to/confs.json")
     complete=os.path.expanduser("~/.config/copy_to/")
     folder=os.path.expanduser("~/.config/copy_to/")
 
     if not os.path.exists(folder):
-        os.makedirs(folder)
+        os.makedirs(folder)                         
 
     if not os.path.exists(file):
         with open(file, "w") as outfile:
             json.dump({}, outfile)
 
     with open(file, 'r') as outfile:
         envs = json.load(outfile)
 
     with open(file, 'w') as outfile: 
         if not 'group' in envs:
             envs['group'] = [] 
         json.dump(envs, outfile)
 
-
-    def is_valid_dir(parser, arg):
-        if os.path.isdir(arg):
-            return os.path.abspath(arg)
-        elif os.path.isfile(arg):
-            print('%s is a file. A folder is required' % arg)
-            raise SystemExit              
-        else:
-            print("The directory %s does not exist!" % arg)
-            raise SystemExit
-
-    def is_valid_file_or_dir(parser, arg):
-        arg=os.path.abspath(arg)
-        if os.path.isdir(arg):
-            return arg
-        elif os.path.isfile(arg):
-            return arg              
-        elif os.path.exists(os.path.join(os.getcwd(), arg)):
-            return os.path.join(os.getcwd(), arg)
-        else:
-            print("The file/directory %s does not exist!" % arg)
-            raise SystemExit
-
-    def copy_to(dest, src):
-
-        for element in src:
-            exist_dest=os.path.join(dest, os.path.basename(os.path.normpath(element)))
-            if os.path.isfile(element):
-                shutil.copy2(element, exist_dest)
-                print("Copied to " + str(exist_dest))
-
-            elif os.path.isdir(element):
-                shutil.copytree(element, exist_dest, dirs_exist_ok=True)
-                print("Copied to " + str(exist_dest) + " and all it's inner content")
-
-
-    def listAll():
-        for name, value in envs.items():
-            if not name == 'group':
-                print(name.upper() + ":")
-                print("     Dest:   '" + str(value['dest']) + "'")
-                print("     Src :")
-                for idx, src in enumerate(value['src']):
-                    print("          " + str(idx+1) + ") '" + str(src) + "'")
-
-
-    def filterListDoubles(a):
-        # https://stackoverflow.com/questions/9835762/how-do-i-find-the-duplicates-in-a-list-and-create-another-list-with-them
-        seen = set()
-        ret = [x for x in a if x not in seen and not seen.add(x)]
-        return ret
-
-    def PathCompleter(**kwargs):
-        return os.path
-
-    def PathOnlyDirsCompleter(**kwargs):
-        return [ name for name in os.listdir(str(os.getcwd())) if os.path.isdir(os.path.join(os.getcwd()), name) ]
-
-    def SourceComplete():
-        return range(1,4)
-
-    def exist_name(parser, x):
-        not_exists=True
-        if x in envs or x == 'group' or x in envs['group']:
-            print("The name %s already exists as conf name!" % x)
-            listAll()
-            raise SystemExit 
-        return x
-
-    def get_names(special=False):
-        names=[]
-        with open(file, 'r') as outfile:
-            envs = json.load(outfile)
-            for key, name in envs.items():
-                if not key == "group":
-                    names.append(key)
-                else:
-                    for e in envs['group']:
-                        names.append(e)
-            if special:
-                names.append("all")
-            return names
-
-    def get_reg_names():
-        with open(file, 'r') as outfile:
-            envs = json.load(outfile)
-            names=[]
-            for key, name in envs.items():
-                if not key == "group":
-                    names.append(key)
-            return names
-
-    def get_group_names():
-        with open(file, 'r') as outfile:
-            envs = json.load(outfile)
-            names=[]
-            for e in envs['group']:
-                names.append(e)
-            return names
-
-        choices = argcomplete.completers.ChoicesCompleter
-        parser = argparse.ArgumentParser(description="Setup configuration to copy files and directories to",formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-        subparser = parser.add_subparsers(dest='command')
-        list1 = subparser.add_parser('list')
-        run = subparser.add_parser('run')
-        add = subparser.add_parser('add')
-        delete = subparser.add_parser('delete')
-        add_source = subparser.add_parser('add-source')
-        add_group = subparser.add_parser('add-group')
-        delete_group = subparser.add_parser('delete-group')
-        reset_destination = subparser.add_parser('reset-destination')
-        delete_source = subparser.add_parser('delete-source')
-        reset_source = subparser.add_parser('reset-source')
-        help1 = subparser.add_parser('help')
-        list1.add_argument("name" , nargs='?', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_names(True))
-        run.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_names(True))
-        delete.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        delete.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_reg_names())
-        add.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        add.add_argument("name" , type=lambda x: exist_name(parser, x) ,help="Configuration name", metavar="Configuration Name, ")
-        add.add_argument("dest" , type=lambda x: is_valid_dir(parser, x), metavar="Destination directory")
-        add.add_argument("src" , nargs='*', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
-        add_group.add_argument("groupname" , type=lambda x: exist_name(parser, x) ,help="Group name holding multiple configuration names", metavar="Group Name")
-        add_group.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        add_group.add_argument("name" , nargs='+', type=str ,help="Configuration name", metavar="Configuration Name", choices=get_reg_names())
-        delete_group.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        delete_group.add_argument("groupname" , type=str ,help="Group name holding multiple configuration names", metavar="Group Name", choices=get_group_names())
-        add_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
-        add_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        add_source.add_argument("src" , nargs='+', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
-        reset_destination.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        reset_destination.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
-        reset_destination.add_argument("dest" , type=lambda x: is_valid_dir(parser, x), metavar="Destination directory", help="Destination directory")
-        delete_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        delete_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
-        delete_source.add_argument("src_num" , nargs='*', type=int, metavar="Source files and directories or Index numbers", help="Source files and directories or Index numbers")
-        reset_source.add_argument("-l", "--list", action='store_true', required=False, help="List configuration")
-        reset_source.add_argument("name" , type=str ,help="Configuration name for modifications", metavar="Configuration Name",  choices=get_reg_names())
-        reset_source.add_argument("src" , nargs='*', type=lambda x: is_valid_file_or_dir(parser, x), metavar="Source files and directories", help="Source files and directories")
-        argcomplete.autocomplete(parser)
-
-
+    parser = get_main_parser()
     args = parser.parse_args()
 
     name= args.name if "name" in args else ""
     dest= args.dest if "dest" in args else []
     src=args.src if "src" in args else []
     if type(name) is list:
         name = filterListDoubles(name)
@@ -229,20 +265,62 @@
                     raise SystemExit
             for i in var1:
                 i=str(i)
                 print('\n' + i.upper() + ':')
                 dest = envs[i]['dest']
                 src = envs[i]['src']
                 copy_to(dest, src)
+
+    if args.command == 'run-reverse':
+        if envs == {}:
+            print("Add an configuration with 'copy-to add dest src' first to copy all it's files to destination")
+            raise SystemExit
+        elif not 'name' in args:
+            print("Give up an configuration to copy objects between")
+            raise SystemExit
+        elif args.name == ['all']:
+            for i in envs:
+                if not i == 'group':
+                    print('\n' + i.upper() + ':')
+                    dest = envs[i]['dest']
+                    src = envs[i]['src']
+                    copy_from(dest, src)   
+        else:
+            var = []
+            grps = []
+            for key in name:
+                if key in envs['group']:
+                    var.append(envs['group'][key])
+                    grps.append(key)
+            var1=[]
+            for i in var:
+                for e in i:
+                    var1.append(e)
+            for key in name:
+                if not key in grps:
+                    var1.append(key)
+            var1 = filterListDoubles(var1)
+            for key in var1:
+                if not key in envs:
+                    print("Look again. " + key + " isn't in there.")
+                    listAll()
+                    raise SystemExit
+            for i in var1:
+                i=str(i)
+                print('\n' + i.upper() + ':')
+                dest = envs[i]['dest']
+                src = envs[i]['src']
+                copy_from(dest, src)
+                
     elif args.command == 'add':
         if not 'name' in args:
             print("Give up a configuration name to copy objects between")
             raise SystemExit
-        elif args.name == 'group':
-            print("Name 'group' is reserved to keep track of groupnames")
+        elif args.name == 'group' or args.name == 'all':
+            print("Name 'group' and 'all' are reserved in namespace")
             raise SystemExit
         elif name in envs:
             print("Look again. " + str(name) + " is/are already used as name.")
             listAll()
             raise SystemExit
         elif name in envs['group']:
             print("Look again. " + str(name) + " is/are already used as groupname.")
@@ -261,16 +339,16 @@
             args.name = name
             args.command = 'list'
 
     elif args.command == 'add-group':
         if not 'groupname' in args:
             print("Give up an configuration to copy objects between")
             raise SystemExit
-        elif args.groupname == 'group':
-            print("Name 'group' is reserved to keep track of groupnames")
+        elif args.groupname == 'group' or args.groupname == 'all' :
+            print("Name 'group' and 'all' are reserved in namespace")
             raise SystemExit
         elif args.groupname in envs:
             print("Can't have both the same groupname and regular name. Change " + str(args.groupname))
             raise SystemExit
         elif args.groupname in envs['group']:
             print("Change " + str(args.groupname) + ". It's already taken")
             raise SystemExit
@@ -431,22 +509,26 @@
                 json.dump(envs, outfile)
             print('Reset source of '+ str(name) + ' to', src)
 
     if args.command == None :
         parser.print_help()
     else: 
         if args.command == 'list' and "name" in args and args.name:
-            if args.name == ['all']:
+            if args.name == 'all':
                 listAll()
             else:
                 for key, value in envs.items():
                     if name == key:
                         print(key.upper() + ":")
                         print("     Dest:   '" + str(value['dest']) + "'")
                         print("     Src: ")
                         for idx, src in enumerate(value['src']):
                             print("          " + str(idx+1) + ") '" + str(src) + "'")
         elif not args.command == None and args.command == 'list' or list in args:
             listAll()
         else:
             pass
 
+if __name__ == "__main__":
+#!/usr/bin/env python
+# PYTHON_ARGCOMPLETE_OK
+    main()
```

### Comparing `copy-to-1.0.9/pyproject.toml` & `copy-to-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "argcomplete"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "copy-to"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Stan Nys", email="stan96@duck.com" },
 ]
 
 description = "A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration"
 readme = "README.md"
 requires-python = ">=3.7"
```

