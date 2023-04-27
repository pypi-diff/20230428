# Comparing `tmp/pathmatcher-1.7.5.tar.gz` & `tmp/pathmatcher-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pathmatcher-1.7.5.tar", last modified: Wed May 20 22:27:04 2020, max compression
+gzip compressed data, was "pathmatcher-1.8.0b2.tar", last modified: Thu Apr 27 22:06:41 2023, max compression
```

## Comparing `pathmatcher-1.7.5.tar` & `pathmatcher-1.8.0b2.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxrwx   0        0        0        0 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/
--rw-rw-rw-   0        0        0     1093 2020-05-17 05:21:27.000000 pathmatcher-1.7.5/LICENSE
--rw-rw-rw-   0        0        0       69 2020-05-20 21:18:04.000000 pathmatcher-1.7.5/MANIFEST.in
--rw-rw-rw-   0        0        0    32846 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0    28259 2020-05-20 22:25:27.000000 pathmatcher-1.7.5/README.md
-drwxrwxrwx   0        0        0        0 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/pathmatcher/
--rw-rw-rw-   0        0        0      168 2020-05-17 06:52:24.000000 pathmatcher-1.7.5/pathmatcher/__init__.py
--rw-rw-rw-   0        0        0       21 2020-05-20 21:29:58.000000 pathmatcher-1.7.5/pathmatcher/_version.py
-drwxrwxrwx   0        0        0        0 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/
--rw-rw-rw-   0        0        0      331 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/__init__.py
--rw-rw-rw-   0        0        0    61177 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/awmstools.py
--rw-rw-rw-   0        0        0     5267 2020-05-17 07:42:29.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/matlabcom.py
--rw-rw-rw-   0        0        0    18096 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/matlabpipe.py
--rw-rw-rw-   0        0        0     1069 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/mlabraw.py
--rw-rw-rw-   0        0        0    33031 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/mlabwrap/mlabwrap.py
-drwxrwxrwx   0        0        0        0 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/pathmatcher/pathlib2/
--rw-rw-rw-   0        0        0    54694 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/pathlib2/__init__.py
--rw-rw-rw-   0        0        0    43942 2020-05-17 05:57:11.000000 pathmatcher-1.7.5/pathmatcher/pathmatcher.py
--rw-rw-rw-   0        0        0    59094 2020-05-20 21:29:31.000000 pathmatcher-1.7.5/pathmatcher/reorientation_registration_helper.py
--rw-rw-rw-   0        0        0     3183 2020-05-17 05:10:45.000000 pathmatcher-1.7.5/pathmatcher/tee.py
-drwxrwxrwx   0        0        0        0 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/pathmatcher.egg-info/
--rw-rw-rw-   0        0        0    32846 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2020-05-20 22:27:03.000000 pathmatcher-1.7.5/pathmatcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-05-20 22:27:04.000000 pathmatcher-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0     3100 2020-05-17 07:45:40.000000 pathmatcher-1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/
+-rw-rw-rw-   0        0        0     1093 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0    29868 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/
+-rw-rw-rw-   0        0        0      168 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/_version.py
+-rw-rw-rw-   0        0        0     1955 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/expandhelper.m
+-rw-rw-rw-   0        0        0     8063 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/functionalcoreg.m
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/
+-rw-rw-rw-   0        0        0     2123 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/README.rst
+-rw-rw-rw-   0        0        0      331 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/__init__.py
+-rw-rw-rw-   0        0        0    61177 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py
+-rw-rw-rw-   0        0        0     5267 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py
+-rw-rw-rw-   0        0        0    18096 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py
+-rw-rw-rw-   0        0        0     1069 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py
+-rw-rw-rw-   0        0        0    33031 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/pathlib2/
+-rw-rw-rw-   0        0        0    54694 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py
+-rw-rw-rw-   0        0        0    43942 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py
+-rw-rw-rw-   0        0        0     3066 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/realignhelper.m
+-rw-rw-rw-   0        0        0      928 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/regex_files.m
+-rw-rw-rw-   0        0        0    62358 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py
+-rw-rw-rw-   0        0        0      227 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorienthelper.m
+-rw-rw-rw-   0        0        0     3297 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/tee.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher.egg-info/
+-rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9954 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pathmatcher-1.7.5/LICENSE` & `pathmatcher-1.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/PKG-INFO` & `pathmatcher-1.8.0b2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,416 +1,466 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.7.5
-Summary: Regular Expression Path Matcher
-Home-page: https://github.com/lrq3000/pathmatcher
-Author: Stephen Karl Larroque
-Author-email: lrq3000@gmail.com
-License: MIT
-Description: # Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
-        
-        [![PyPI-Status](https://img.shields.io/pypi/v/pathmatcher.svg)](https://pypi.org/project/pathmatcher)
-        [![PyPI-Versions](https://img.shields.io/pypi/pyversions/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
-        [![PyPI-Downloads](https://img.shields.io/pypi/dm/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
-        
-        Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
-        
-        If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
-        
-        If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
-        
-        This module works for any file management purpose, but it is particularly optimized via the reorientation_registration_helper.py submodule to work for neuroimaging, such as reorganizing very fast any dataset into a BIDS compliant format.
-        
-        This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. For an exemple, see the script `reorient_pipeline` at the root of this repository.
-        
-        As a Python module, it can not only match inputpaths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
-        
-        Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
-        
-        If you are not experienced with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp.
-        
-        ## Install
-        
-        Simply use pypi:
-        
-        ```
-        pip install --upgrade pathmatcher
-        ```
-        
-        Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
-        
-        ## Quickstart
-        
-        Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename.
-        
-        You can match them like this:
-        
-        ```
-        pathmatcher -i "root" -ri "(\dir)/(.*)" --test
-        ```
-        
-        The arguments are as follows:
-        * `-i` is the input root directory from where the recursive file search will start.
-        * `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes).
-        * `--test` will test whether at least one file can be matched. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
-        
-        Here is the output we get:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: root
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: None
-        - Output regex: None
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) --test
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
-        
-        Match: folderA/file1.txt
-        
-        0files [00:00, ?files/s]
-        End of simulation. 1 files matched.
-        ```
-        
-        Since we have matched one file, this shows the regexp works, we're good to go.
-        
-        Note: In the case it didn't work (no file matched), and there are lots of files, you can prematurely stop the file search by pressing CTRL+C.
-        
-        Next, type this:
-        
-        ```
-        pathmatcher -i "root" -ri "(\dir)/(.*)" -o "out" -ro "\1_\2" --copy
-        ```
-        
-        This reuses the previous command's input arguments (except `--test`) and adds the 3 following arguments:
-        * `--copy` will copy the matched files to an output folder, potentially with a modified filename if specified in `-ro`. Alternative commands are: `--move`, `--move_fast`, `--delete`, `--symlink`.
-        * `-o` is the output directory.
-        * `-ro` is the output paths regular expression. This allows to dynamically change the output filenames by reusing regexp groups from the matched input paths. Here, we reuse the subdirectory name captured in `\1` and reuse it to prepend before the original input path `\2`.
-        
-        Before applying any file modification operation, pathmatcher will provide a complete simulation report of what it plans to do, including whether there will be overwriting conflicts (eg, 2 different files will get the same filename).
-        
-        Here is the simulation report for our command above:
-        
-        ```
-        == REGEX PATH MATCHER SIMULATION REPORT ==
-        Total number of files matched: 6
-        Parameters:
-        - Input root: b'root'
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: b'out'
-        - Output regex: \1_\2
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
-        
-        List of matched files:
-        * folderA/file1.txt --> folderA_file1.txt  
-        * folderA/file2.txt --> folderA_file2.txt  
-        * folderA/file3.txt --> folderA_file3.txt  
-        * folderB/file4.txt --> folderB_file4.txt  
-        * folderB/file5.txt --> folderB_file5.txt  
-        * folderB/file6.txt --> folderB_file6.txt  
-        ```
-        
-        By default, the simulation report is saved as `pathmatcher_report.txt` in the current terminal folder (as shown by `pwd`) and is opened in the default text editor. This behavior can be modified using `--noreport``, which will print the simulation report directly in the terminal.
-        
-        Now, we manually review the simulation report, and we can see that everything is going as planned.
-        
-        Let's go back to the terminal:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: root
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: out
-        - Output regex: \1_\2
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
-        
-        12files [00:00, ?files/s]
-        End of simulation. 6 files matched.
-        Preparing simulation report, please wait a few seconds...
-        Opening simulation report with your default editor, a new window should open.
-        
-        
-        No conflict detected. You are good to go!
-        Do you want to apply the result of the path reorganization simulation on 6 files? [Y/N]:
-        ```
-        
-        The terminal confirms that there are no conflicts (which would have appeared in the simulation report too), and asks us whether we want to proceed.
-        
-        If we type `Y` and tap Enter, the files will be copied and renamed according to the simulation report above. If we type `N` or simply CTRL+C, the application stops.
-        
-        This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order).
-        
-        There is also the very powerful `--tree` option, also available as an argument in the Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command.
-        
-        Pro tip: if you can't get a file reorganization task done in a single command, try to break down your task into several smaller steps, such as for example first renaming, then moving, then renaming again, then moving again, then deleting the unnecessary files, etc. Usually, a seemingly impossible file reorganization task is easily done with a few smaller `pathmatcher` calls.
-        
-        ## Usage
-        
-        ```
-        usage: pathmatcher [-h] -i /some/path -ri "sub[^/]+/\d+" [-o /new/path] [-ro "newsub/\1"] [-c] [-s] [-m]
-                                   [--move_fast] [-d] [-t] [--dir] [-y] [-f] [--show_fullpath] [-ra 1:10-255]
-                                   [-re "newsub/\1"] [--report pathmatcher_report.txt] [--noreport] [--tree]
-                                   [-l /some/folder/filename.log] [-v] [--silent]
-        
-        Regex PathMatcher v1.7.4
-        Description: Match paths using regular expression, and then generate a report. Can also substitute using regex to generate output paths. A copy mode is also provided to allow the copy of files from input to output paths.
-        This app is essentially a path matcher using regexp, and it then rewrites the path using regexp, so that you can reuse elements from input path to build the output path.
-        This is very useful to reorganize folders for experiments, where scripts/softwares expect a specific directories layout in order to work.
-        
-        Advices
-        -------
-        - Filepath comparison: Paths are compared against filepaths, not just folders (but of course you can match folders with regex, but remember when designing your regexp that it will compared against files paths, not directories).
-        - Relative filepath: Paths are relative to the rootpath (except if --show-fullpath) and that they are always unix style, even on Windows (for consistency on all platforms and to easily reuse regexp).
-        - Partial matching: partial matching regex is accepted, so you don't need to model the full filepath, only the part you need (eg, 'myfile' will match '/myfolder/sub/myfile-034.mat').
-        - Unix filepaths: on all platforms, including Windows, paths will be in unix format (except if you set --show_fullpath). It makes things simpler for you to make crossplatform regex patterns.
-        - Use [^/]+ to match any file/folder in the filepath: because paths are always unix-like, you can use [^/]+ to match any part of the filepath. Eg, "([^/]+)/([^/]+)/data/mprage/.+\.(img|hdr|txt)" will match "UWS/John_Doe/data/mprage/12345_t1_mprage_98782.hdr".
-        - Split your big task in several smaller, simpler subtasks: instead of trying to do a regex that match T1, T2, DTI, everything at the same time, try to focus on only one modality at a time and execute them using multiple regex queries: eg, move first structural images, then functional images, then dti, etc. instead of all at once.
-        - Python module: this library can be used as a Python module to include in your scripts (just call `main(return_report=True)`).
-        
-        Note: use --gui (without any other argument) to launch the experimental gui (needs Gooey library).
-        
-        In addition to the switches provided below, using this program as a Python module also provides 2 additional options:
-         - return_report = True to return as a variable the files matched and the report instead of saving in a file.
-         - regroup = True will return the matched files (if return_report=True) in a tree structure of nested list/dicts depending on if the groups are named or not. Groups can also avoid being matched by using non-matching groups in regex.
-        
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -i /some/path, --input /some/path
-                                Path to the input folder
-          -ri "sub[^/]+/(\d+)", --regex_input "sub[^/]+/(\d+)"
-                                Regex to match input paths. Must be defined relatively from --input folder. Do not forget to enclose it in double quotes (and not single)! To match any directory, use [^/\]*? or the alias \dir, or \dirnodot if you want to match folders in combination with --dir switch.
-          -o /new/path, --output /new/path
-                                Path to the output folder (where file will get copied over if --copy)
-          -ro "newsub/\1", --regex_output "newsub/\1"
-                                Regex to substitute input paths to convert to output paths. Must be defined relatively from --output folder. If not provided but --output is specified, will keep the same directory layout as input (useful to extract specific files without changing layout). Do not forget to enclose it in double quotes!
-          -c, --copy            Copy the matched input paths to the regex-substituted output paths.
-          -s, --symlink         Copy with a symbolic/soft link the matched input paths to the regex-substituted output paths (works only on Linux).
-          -m, --move            Move the matched input paths to the regex-substituted output paths.
-          --move_fast           Move the matched input paths to the regex-substituted output paths, without checking first that the copy was done correctly.
-          -d, --delete          Delete the matched files.
-          -t, --test            Regex test mode: Stop after the first matched file and show the result of substitution. Useful to quickly check if the regex patterns are ok.
-          --dir                 Match directories too? (else only files are matched)
-          -y, --yes             Automatically accept the simulation and apply changes (good for batch processing and command chaining).
-          -f, --force           Force overwriting the target path already exists. Note that by default, if a file already exist, without this option, it won't get overwritten and no message will be displayed.
-          --show_fullpath       Show full paths instead of relative paths in the simulation.
-          -ra 1:10-255, --range 1:10-255
-                                Range mode: match only the files with filenames containing numbers in the specified range. The format is: (regex-match-group-id):(range-start)-(range-end). regex-match-group-id is the id of the regular expression that will contain the numbers that must be compared to the range. range-end is inclusive.
-          -re "newsub/\1", --regex_exists "newsub/\1"
-                                Regex of output path to check if the matched regex here is matched prior writing output files.
-          --report pathmatcher_report.txt
-                                Where to store the simulation report (default: pwd = current working dir).
-          --noreport            Do not create a report file, print the report in the console.
-          --tree                Regroup in a tree structure the matched files according to named and unnamed regex groups, and save the result as a json file (pathmatcher_tree.json).
-          -l /some/folder/filename.log, --log /some/folder/filename.log
-                                Path to the log file. (Output will be piped to both the stdout and the log file)
-          -v, --verbose         Verbose mode (show more output).
-          --silent              No console output (but if --log specified, the log will still be saved in the specified file).
-        
-        ```
-        
-        ## Libraries
-        
-        ### Required
-        
-        * core Python libraries...
-        * argparse
-        * pathlib2 (provided with the script)
-        * Tee (provided with the script)
-        
-        ### Optional
-        
-        * **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
-        * scandir (for faster file walking and simulation report)
-        * Gooey (for gui)
-        
-        ## Tutorial
-        
-        Here is a short introduction in the usage of `pathmatcher.py`.
-        
-        The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
-        
-        Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
-        
-        To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
-        
-        Now, in the commandline, execute the two following commands:
-        
-        ```python
-        python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
-        
-        python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
-        ```
-        
-        Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
-        
-        Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
-        
-        After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
-        
-        This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
-        
-        ```python
-        python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
-        
-        python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
-        ```
-        
-        Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
-        
-        ```python
-        python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
-        ```
-        
-        This will generate the whole list of T1 and show them in a report.
-        
-        Of course, you can also use absolute paths for `--input` and `--output`.
-        
-        And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
-        
-        ```python
-        python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
-        ```
-        
-        Result:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: C:\GigaData\BIDS\ABIDE
-        - Input regex: Caltech_([0-9]+)/.+/mprage.nii.gz
-        - Output root: C:\GigaData\BIDS\ABIDE-BIDS
-        - Output regex: sub-\1/anat/sub-\1_T1w.nii.gz
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends
-        on files count - filesize has no influence). Press CTRL+C to abort
-        
-        Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
-        
-        
-        End of simulation. 1 files matched.
-        ```
-        
-        Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
-        
-        ```python
-        from pathmatcher import main as pm
-        
-        # Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
-        # You can use the commandline arguments, but the script will be called without bash but directly inside Python
-        my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
-        
-        print(my_results)
-        ```
-        
-        A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
-        
-        ### Similar projects
-        
-        A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
-        
-        ## Auxiliary tool: Reorientation and registration helper
-        
-        ### Description
-        
-        A companion to help you reorient and coregister manually your structural and functional MRI in SPM, without having to click to select files.
-        
-        This helper script will scan all images in the specified input path, and will accompagny you step-by-step to do the reorientation and coregistration correctly.
-        
-        This script requires SPM12 (and MATLAB), and runs only on Windows (because of the matlab wrapper limitations).
-        
-        This script follows the following steps:
-        
-        1. Automatic reorientation of structural MRI using [spm_auto_reorient.m](https://github.com/lrq3000/spm_auto_reorient) (please install this script along with SPM12 beforehand).
-        2. Check reorient and adjust manually.
-        3. Side-by-side check of multiple subjects' structural MRI.
-        4. Detection of functional images (just walk through all folders to build a list of functional images and pair them to their respective structural images given the input regexp).
-        5. Automatic co-registration of functional images onto structural.
-        6. Manual co-registration of functional images with structural.
-        7. Extraction of framewise displacement motion metrics from functional images.
-        
-        This script will not only guide you through these steps, in the correct order, but it will also automatically load the files for you (no chance of doing a mistake or missing a subject), while showing you a progress bar (showing how many subjects are remaining and with a time estimate to finish).
-        
-        There is a CLI user interface: you can skip steps you already done or don't want to do, skip patients, or reload another image (for step 4, to check other functional images).
-        
-        Note that the last step, extraction of framewise displacement motion metrics from functional images, can be done without requiring matlab nor a matlab wrapper (and hence should work on any platform), by using the `--motiononly` and `--regex_motion` switches (this will directly look for the `rp_*.txt` files that you previously generated with `spm_realign`).
-        
-        ### Usage
-        
-        ```
-        usage: reorientation_registration_helper [-h] -i /some/path [-ra "reg_expr+/anat\.(img|nii)"]
-                                                         [-rf "reg_expr+/func\.(img|nii)"] [-rp "reg_expr+/rp_.+\.txt"] [-m]
-                                                         [-v]
-        
-        Reorientation and registration helper v1.7.4
-        Description: Guide and automate the file selection process that is required in SPM between each reorientation/registration.
-        
-        No more useless clicks, just do the reorientation/registration in batch, you don't need to worry about selecting the corresponding files, this helper will do it for you.
-        
-        If you have tqdm installed, a nice progress bar will tell you how many subjects are remaining to be processed and how much time will it take at your current pace.
-        
-        Note: you need to `pip install mlab` before using this script.
-        Note2: you need to have set both spm and spm_auto_reorient in your path in MATLAB before using this script.
-        Note3: you need the pathmatcher.py library (see lrq3000 github).
-        
-        
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -i /some/path, --input /some/path
-                                Path to the input folder (the root directory where you placed the files, the default supported tree structure being: "Condition/subject_id/data/(sess_id)?/(mprage|rest)/*.(img|nii)". You can also use --regex_anat and --regex_func to define your own directory layout.
-          -ra "(reg_expr)+/anat\.(img|nii)", --regex_anat "(reg_expr)+/anat\.(img|nii)"
-                                Regular expression to match anatomical images (default: Liege CRC scheme). Use regex groups to match with functional regex (if you want to do step 4 - manual coreg). Note: should target nii or img, not hdr.
-          -rf "(reg_expr)+/func\.(img|nii)", --regex_func "(reg_expr)+/func\.(img|nii)"
-                                Regular expression to match functional images (default: Liege CRC scheme). Regex groups will be matched with the anatomical regex, so you should provide the same groups for both regex. Note: should target nii or img, not hdr (using non-capturing group, eg: ".*\.(?:img|nii)". If a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule).
-          -rp "(reg_expr)+/rp_.+\.txt", --regex_motion "(reg_expr)+/rp_.+\.txt"
-                                Regular expression to match motion parameter files rp_*.txt as generated by spm_realign. If this argument is provided, motion parameters will be fetched from these files directly instead of recalculating from functional images. The regex needs to contain at least one group in parentheses to define a key for the output excel file.
-          -m, --motiononly      If true, and if --regex_motion is specified, then only this step will be done, using the already generated rpfiles.
-          -v, --verbose         Verbose mode (show more output).
-        
-        ```
-        
-        ### Libraries
-        
-        #### Required
-        
-        * argparse
-        * pathmatcher
-        * mlabwrap aka matlap_wrapper ([Python2](https://github.com/mrkrd/matlab_wrapper) version, [Python3](https://github.com/deeuu/matlab_wrapper/tree/python3) version as provided with this module)
-        * pypiwin32 (for mlabwrap)
-        * pip install --ignore-installed pywin32
-            * then execute `python Scripts\pywin32_postinstall.py -install` in an admin command prompt, see [this explanation](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api#comment103561767_58613735).
-        
-        #### Optional
-        
-        * scandir, to scan files faster
-        * tqdm, to show the progress bar
-        * numpy >= 1.18.1, for the optional last step to generate motion metrics from functional images
-        
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Utilities
+Version: 1.8.0b2
+Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
+Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
+Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
+Project-URL: Source, https://github.com/lrq3000/pathmatcher
+Project-URL: Tracker, https://github.com/lrq3000/pathmatcher/issues
+Project-URL: Download, https://github.com/lrq3000/pathmatcher/releases
+Keywords: file,folders,manipulation,copy,move,delete,batch,regex,regexp,regular expression,regular expressions,file trees,file tree,files tree,files trees,neuroimaging,mri,fmri,nifti,nii,reorientation,spm
+Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Intended Audience :: System Administrators
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: testmeta
+License-File: LICENSE
+
+# Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
+
+[![PyPI-Status](https://img.shields.io/pypi/v/pathmatcher.svg)](https://pypi.org/project/pathmatcher)
+[![PyPI-Versions](https://img.shields.io/pypi/pyversions/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
+[![PyPI-Downloads](https://img.shields.io/pypi/dm/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
+
+Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
+
+If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
+
+If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
+
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
+
+This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
+
+Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
+
+If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
+
+## Install
+
+For Python 3.7+:
+
+```
+pip install --upgrade pathmatcher
+```
+
+Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
+
+For the latest development release, use:
+
+```
+pip install --upgrade pathmatcher --pre
+```
+
+For the cutting-edge code (likely unstable, do not use in production!), use:
+
+```
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+```
+
+For Python 2.7 to 3.6, the last compatible version is v1.7.6:
+
+```
+pip install --upgrade pathmatcher==1.7.6
+```
+
+This will install two commands in your environment: `pathmatcher` and `reorientation_registration_helper`.
+
+## Quickstart
+
+This section is a hands-on introduction illustrating the steps of a typical session of pathmatching, from how to quickly draft a regular expression (regexp) that matches your files to how to apply it to fulfil your target file structure.
+
+Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename. Here is a schema of this files structure:
+
+```
+root
+|--- folderA
+        |--- file1.txt
+        |--- file2.txt
+        |--- file3.txt
+|--- folderB
+        |--- file4.txt
+        |--- file5.txt
+        |--- file6.txt
+```
+
+You can match them like this:
+
+```
+pathmatcher -i "root" -ri "(\dir)/(.*)" --test
+```
+
+The arguments are as follows:
+* `-i` is the input root directory from where the recursive file search will start.
+* `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes). Here, `(\dir)` will match `folderA` and `folderB`. If we had an unlimited number of depth in subfolders and we wanted to recurse, we could use `(\dir/)+` which means that we match: `\dir` a directory, `/` a path separator to next level (so we can chain multiple depths), `+` at least one subfolder level and as many as there are if there are multiple levels.
+* `--test` will test whether at least one file can be matched, and then stops. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
+
+Here is the output we get:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: root
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: None
+- Output regex: None
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) --test
+
+
+Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
+
+Match: folderA/file1.txt
+
+0files [00:00, ?files/s]
+End of simulation. 1 files matched.
+```
+
+Since we have matched one file, this shows the regexp works, we're good to go.
+
+Note: In the case it didn't work (no file matched), and there are lots of files, you can prematurely stop the file search by pressing CTRL+C.
+
+Next, type this:
+
+```
+pathmatcher -i "root" -ri "(\dir)/(.*)" -o "out" -ro "\1_\2" --copy
+```
+
+This reuses the previous command's input arguments (except `--test`) and adds the 3 following arguments:
+* `--copy` will copy the matched files to an output folder, potentially with a modified filename if specified in `-ro`. Alternative commands are: `--move`, `--move_fast`, `--delete`, `--symlink`.
+* `-o` is the output directory.
+* `-ro` is the output paths regular expression. This allows to dynamically change the output filenames by reusing regexp groups from the matched input paths. Here, we reuse the subdirectory name captured in `\1` and reuse it to prepend before the original input path `\2`.
+
+Before applying any file modification operation, pathmatcher will provide a complete simulation report of what it plans to do, including whether there will be overwriting conflicts (eg, 2 different files will get the same filename).
+
+Here is the simulation report for our command above:
+
+```
+== REGEX PATH MATCHER SIMULATION REPORT ==
+Total number of files matched: 6
+Parameters:
+- Input root: b'root'
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: b'out'
+- Output regex: \1_\2
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
+
+List of matched files:
+* folderA/file1.txt --> folderA_file1.txt  
+* folderA/file2.txt --> folderA_file2.txt  
+* folderA/file3.txt --> folderA_file3.txt  
+* folderB/file4.txt --> folderB_file4.txt  
+* folderB/file5.txt --> folderB_file5.txt  
+* folderB/file6.txt --> folderB_file6.txt  
+```
+
+By default, the simulation report is saved as `pathmatcher_report.txt` in the current terminal folder (as shown by `pwd`) and is opened in the default text editor. This behavior can be modified using `--noreport``, which will print the simulation report directly in the terminal.
+
+Now, we manually review the simulation report, and we can see that everything is going as planned.
+
+Let's go back to the terminal:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: root
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: out
+- Output regex: \1_\2
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
+
+
+Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
+
+12files [00:00, ?files/s]
+End of simulation. 6 files matched.
+Preparing simulation report, please wait a few seconds...
+Opening simulation report with your default editor, a new window should open.
+
+
+No conflict detected. You are good to go!
+Do you want to apply the result of the path reorganization simulation on 6 files? [Y/N]:
+```
+
+The terminal confirms that there are no conflicts (which would have appeared in the simulation report too), and asks us whether we want to proceed.
+
+If we type `Y` and tap Enter, the files will be copied and renamed according to the simulation report above. If we type `N` or simply CTRL+C, the application stops.
+
+This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order, so the walking order is always deterministic).
+
+There is also the very powerful `--tree` option, also available as an argument when used as a Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command and then post-process with your own script.
+
+Pro tip: if you can't get a file reorganization task done in a single command, try to break down your task into several smaller steps, such as for example first renaming, then moving, then renaming again, then moving again, then deleting the unnecessary files, etc. Usually, a seemingly impossible file reorganization task is easily done with a few smaller `pathmatcher` calls.
+
+## Usage
+
+```
+usage: pathmatcher [-h] -i /some/path -ri "sub[^/]+/\d+" [-o /new/path] [-ro "newsub/\1"] [-c] [-s] [-m]
+                           [--move_fast] [-d] [-t] [--dir] [-y] [-f] [--show_fullpath] [-ra 1:10-255]
+                           [-re "newsub/\1"] [--report pathmatcher_report.txt] [--noreport] [--tree]
+                           [-l /some/folder/filename.log] [-v] [--silent]
+
+Regex PathMatcher v1.7.4
+Description: Match paths using regular expression, and then generate a report. Can also substitute using regex to generate output paths. A copy mode is also provided to allow the copy of files from input to output paths.
+This app is essentially a path matcher using regexp, and it then rewrites the path using regexp, so that you can reuse elements from input path to build the output path.
+This is very useful to reorganize folders for experiments, where scripts/softwares expect a specific directories layout in order to work.
+
+Advices
+-------
+- Filepath comparison: Paths are compared against filepaths, not just folders (but of course you can match folders with regex, but remember when designing your regexp that it will compared against files paths, not directories).
+- Relative filepath: Paths are relative to the rootpath (except if --show-fullpath) and that they are always unix style, even on Windows (for consistency on all platforms and to easily reuse regexp).
+- Partial matching: partial matching regex is accepted, so you don't need to model the full filepath, only the part you need (eg, 'myfile' will match '/myfolder/sub/myfile-034.mat').
+- Unix filepaths: on all platforms, including Windows, paths will be in unix format (except if you set --show_fullpath). It makes things simpler for you to make crossplatform regex patterns.
+- Use [^/]+ to match any file/folder in the filepath: because paths are always unix-like, you can use [^/]+ to match any part of the filepath. Eg, "([^/]+)/([^/]+)/data/mprage/.+\.(img|hdr|txt)" will match "UWS/John_Doe/data/mprage/12345_t1_mprage_98782.hdr".
+- Split your big task in several smaller, simpler subtasks: instead of trying to do a regex that match T1, T2, DTI, everything at the same time, try to focus on only one modality at a time and execute them using multiple regex queries: eg, move first structural images, then functional images, then dti, etc. instead of all at once.
+- Python module: this library can be used as a Python module to include in your scripts (just call `main(return_report=True)`).
+
+Note: use --gui (without any other argument) to launch the experimental gui (needs Gooey library).
+
+In addition to the switches provided below, using this program as a Python module also provides 2 additional options:
+ - return_report = True to return as a variable the files matched and the report instead of saving in a file.
+ - regroup = True will return the matched files (if return_report=True) in a tree structure of nested list/dicts depending on if the groups are named or not. Groups can also avoid being matched by using non-matching groups in regex.
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i /some/path, --input /some/path
+                        Path to the input folder
+  -ri "sub[^/]+/(\d+)", --regex_input "sub[^/]+/(\d+)"
+                        Regex to match input paths. Must be defined relatively from --input folder. Do not forget to enclose it in double quotes (and not single)! To match any directory, use [^/\]*? or the alias \dir, or \dirnodot if you want to match folders in combination with --dir switch.
+  -o /new/path, --output /new/path
+                        Path to the output folder (where file will get copied over if --copy)
+  -ro "newsub/\1", --regex_output "newsub/\1"
+                        Regex to substitute input paths to convert to output paths. Must be defined relatively from --output folder. If not provided but --output is specified, will keep the same directory layout as input (useful to extract specific files without changing layout). Do not forget to enclose it in double quotes!
+  -c, --copy            Copy the matched input paths to the regex-substituted output paths.
+  -s, --symlink         Copy with a symbolic/soft link the matched input paths to the regex-substituted output paths (works only on Linux).
+  -m, --move            Move the matched input paths to the regex-substituted output paths.
+  --move_fast           Move the matched input paths to the regex-substituted output paths, without checking first that the copy was done correctly.
+  -d, --delete          Delete the matched files.
+  -t, --test            Regex test mode: Stop after the first matched file and show the result of substitution. Useful to quickly check if the regex patterns are ok.
+  --dir                 Match directories too? (else only files are matched)
+  -y, --yes             Automatically accept the simulation and apply changes (good for batch processing and command chaining).
+  -f, --force           Force overwriting the target path already exists. Note that by default, if a file already exist, without this option, it won't get overwritten and no message will be displayed.
+  --show_fullpath       Show full paths instead of relative paths in the simulation.
+  -ra 1:10-255, --range 1:10-255
+                        Range mode: match only the files with filenames containing numbers in the specified range. The format is: (regex-match-group-id):(range-start)-(range-end). regex-match-group-id is the id of the regular expression that will contain the numbers that must be compared to the range. range-end is inclusive.
+  -re "newsub/\1", --regex_exists "newsub/\1"
+                        Regex of output path to check if the matched regex here is matched prior writing output files.
+  --report pathmatcher_report.txt
+                        Where to store the simulation report (default: pwd = current working dir).
+  --noreport            Do not create a report file, print the report in the console.
+  --tree                Regroup in a tree structure the matched files according to named and unnamed regex groups, and save the result as a json file (pathmatcher_tree.json).
+  -l /some/folder/filename.log, --log /some/folder/filename.log
+                        Path to the log file. (Output will be piped to both the stdout and the log file)
+  -v, --verbose         Verbose mode (show more output).
+  --silent              No console output (but if --log specified, the log will still be saved in the specified file).
+
+```
+
+## Libraries
+
+### Required
+
+* core Python libraries...
+* argparse
+* pathlib2 (provided with the script)
+* Tee (provided with the script)
+
+### Optional
+
+* **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
+* scandir (for faster file walking and simulation report)
+* Gooey (for gui)
+
+## Tutorial
+
+Here is a short introduction in the usage of `pathmatcher.py`.
+
+The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
+
+Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
+
+To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
+
+Now, in the commandline, execute the two following commands:
+
+```python
+python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+
+python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+```
+
+Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
+
+Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
+
+After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
+
+This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
+
+```python
+python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+
+python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
+```
+
+Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
+
+```python
+python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
+```
+
+This will generate the whole list of T1 and show them in a report.
+
+Of course, you can also use absolute paths for `--input` and `--output`.
+
+And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
+
+```python
+python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+```
+
+Result:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: C:\GigaData\BIDS\ABIDE
+- Input regex: Caltech_([0-9]+)/.+/mprage.nii.gz
+- Output root: C:\GigaData\BIDS\ABIDE-BIDS
+- Output regex: sub-\1/anat/sub-\1_T1w.nii.gz
+
+
+Computing paths matching and simulation report, please wait (total time depends
+on files count - filesize has no influence). Press CTRL+C to abort
+
+Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
+
+
+End of simulation. 1 files matched.
+```
+
+Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
+
+```python
+from pathmatcher import main as pm
+
+# Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
+# You can use the commandline arguments, but the script will be called without bash but directly inside Python
+my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
+
+print(my_results)
+```
+
+A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
+
+### Similar projects
+
+A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
+
+## Auxiliary tool: Reorientation and registration helper
+
+### Description
+
+A companion to help you reorient and coregister manually your structural and functional MRI in SPM, without having to click to select files.
+
+This helper script will scan all images in the specified input path, and will accompagny you step-by-step to do the reorientation and coregistration correctly.
+
+This script requires SPM12 (and MATLAB), and runs only on Windows (because of the matlab wrapper limitations).
+
+This script follows the following steps:
+
+1. Automatic reorientation of structural MRI using [spm_auto_reorient.m](https://github.com/lrq3000/spm_auto_reorient) (please install this script along with SPM12 beforehand).
+2. Check reorient and adjust manually.
+3. Side-by-side check of multiple subjects' structural MRI.
+4. Detection of functional images (just walk through all folders to build a list of functional images and pair them to their respective structural images given the input regexp).
+5. Automatic co-registration of functional images onto structural.
+6. Manual co-registration of functional images with structural.
+7. Extraction of framewise displacement motion metrics from functional images.
+
+This script will not only guide you through these steps, in the correct order, but it will also automatically load the files for you (no chance of doing a mistake or missing a subject), while showing you a progress bar (showing how many subjects are remaining and with a time estimate to finish).
+
+There is a CLI user interface: you can skip steps you already done or don't want to do, skip patients, or reload another image (for step 4, to check other functional images).
+
+Note that the last step, extraction of framewise displacement motion metrics from functional images, can be done without requiring matlab nor a matlab wrapper (and hence should work on any platform), by using the `--motiononly` and `--regex_motion` switches (this will directly look for the `rp_*.txt` files that you previously generated with `spm_realign`).
+
+### Usage
+
+```
+usage: reorientation_registration_helper [-h] -i /some/path [-ra "reg_expr+/anat\.(img|nii)"]
+                                                 [-rf "reg_expr+/func\.(img|nii)"] [-rp "reg_expr+/rp_.+\.txt"] [-m]
+                                                 [-v]
+
+Reorientation and registration helper v1.7.4
+Description: Guide and automate the file selection process that is required in SPM between each reorientation/registration.
+
+No more useless clicks, just do the reorientation/registration in batch, you don't need to worry about selecting the corresponding files, this helper will do it for you.
+
+If you have tqdm installed, a nice progress bar will tell you how many subjects are remaining to be processed and how much time will it take at your current pace.
+
+Note: you need to `pip install mlab` before using this script.
+Note2: you need to have set both spm and spm_auto_reorient in your path in MATLAB before using this script.
+Note3: you need the pathmatcher.py library (see lrq3000 github).
+
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i /some/path, --input /some/path
+                        Path to the input folder (the root directory where you placed the files, the default supported tree structure being: "Condition/subject_id/data/(sess_id)?/(mprage|rest)/*.(img|nii)". You can also use --regex_anat and --regex_func to define your own directory layout.
+  -ra "(reg_expr)+/anat\.(img|nii)", --regex_anat "(reg_expr)+/anat\.(img|nii)"
+                        Regular expression to match anatomical images (default: Liege CRC scheme). Use regex groups to match with functional regex (if you want to do step 4 - manual coreg). Note: should target nii or img, not hdr.
+  -rf "(reg_expr)+/func\.(img|nii)", --regex_func "(reg_expr)+/func\.(img|nii)"
+                        Regular expression to match functional images (default: Liege CRC scheme). Regex groups will be matched with the anatomical regex, so you should provide the same groups for both regex. Note: should target nii or img, not hdr (using non-capturing group, eg: ".*\.(?:img|nii)". If a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule).
+  -rp "(reg_expr)+/rp_.+\.txt", --regex_motion "(reg_expr)+/rp_.+\.txt"
+                        Regular expression to match motion parameter files rp_*.txt as generated by spm_realign. If this argument is provided, motion parameters will be fetched from these files directly instead of recalculating from functional images. The regex needs to contain at least one group in parentheses to define a key for the output excel file.
+  -m, --motiononly      If true, and if --regex_motion is specified, then only this step will be done, using the already generated rpfiles.
+  -v, --verbose         Verbose mode (show more output).
+
+```
+
+### Libraries
+
+#### Required
+
+* argparse
+* pathmatcher
+* mlabwrap aka matlap_wrapper ([Python2](https://github.com/mrkrd/matlab_wrapper) version, [Python3](https://github.com/deeuu/matlab_wrapper/tree/python3) version as provided with this module)
+* pypiwin32 (for mlabwrap)
+* pip install --ignore-installed pywin32
+    * then execute `python Scripts\pywin32_postinstall.py -install` in an admin command prompt, see [this explanation](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api#comment103561767_58613735).
+
+#### Optional
+
+* scandir, to scan files faster
+* tqdm, to show the progress bar
+* numpy >= 1.18.1, for the optional last step to generate motion metrics from functional images
```

### Comparing `pathmatcher-1.7.5/README.md` & `pathmatcher-1.8.0b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,48 +6,80 @@
 
 Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
 
 If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
 
 If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
 
-This module works for any file management purpose, but it is particularly optimized via the reorientation_registration_helper.py submodule to work for neuroimaging, such as reorganizing very fast any dataset into a BIDS compliant format.
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
 
-This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. For an exemple, see the script `reorient_pipeline` at the root of this repository.
-
-As a Python module, it can not only match inputpaths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
+This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
 
 Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
 
-If you are not experienced with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp.
+If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
-Simply use pypi:
+For Python 3.7+:
 
 ```
 pip install --upgrade pathmatcher
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
+For the latest development release, use:
+
+```
+pip install --upgrade pathmatcher --pre
+```
+
+For the cutting-edge code (likely unstable, do not use in production!), use:
+
+```
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+```
+
+For Python 2.7 to 3.6, the last compatible version is v1.7.6:
+
+```
+pip install --upgrade pathmatcher==1.7.6
+```
+
+This will install two commands in your environment: `pathmatcher` and `reorientation_registration_helper`.
+
 ## Quickstart
 
-Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename.
+This section is a hands-on introduction illustrating the steps of a typical session of pathmatching, from how to quickly draft a regular expression (regexp) that matches your files to how to apply it to fulfil your target file structure.
+
+Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename. Here is a schema of this files structure:
+
+```
+root
+|--- folderA
+        |--- file1.txt
+        |--- file2.txt
+        |--- file3.txt
+|--- folderB
+        |--- file4.txt
+        |--- file5.txt
+        |--- file6.txt
+```
 
 You can match them like this:
 
 ```
 pathmatcher -i "root" -ri "(\dir)/(.*)" --test
 ```
 
 The arguments are as follows:
 * `-i` is the input root directory from where the recursive file search will start.
-* `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes).
-* `--test` will test whether at least one file can be matched. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
+* `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes). Here, `(\dir)` will match `folderA` and `folderB`. If we had an unlimited number of depth in subfolders and we wanted to recurse, we could use `(\dir/)+` which means that we match: `\dir` a directory, `/` a path separator to next level (so we can chain multiple depths), `+` at least one subfolder level and as many as there are if there are multiple levels.
+* `--test` will test whether at least one file can be matched, and then stops. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
 
 Here is the output we get:
 
 ```
 == Regex Path Matcher started ==
 
 Parameters:
@@ -133,17 +165,17 @@
 Do you want to apply the result of the path reorganization simulation on 6 files? [Y/N]:
 ```
 
 The terminal confirms that there are no conflicts (which would have appeared in the simulation report too), and asks us whether we want to proceed.
 
 If we type `Y` and tap Enter, the files will be copied and renamed according to the simulation report above. If we type `N` or simply CTRL+C, the application stops.
 
-This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order).
+This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order, so the walking order is always deterministic).
 
-There is also the very powerful `--tree` option, also available as an argument in the Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command.
+There is also the very powerful `--tree` option, also available as an argument when used as a Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command and then post-process with your own script.
 
 Pro tip: if you can't get a file reorganization task done in a single command, try to break down your task into several smaller steps, such as for example first renaming, then moving, then renaming again, then moving again, then deleting the unnecessary files, etc. Usually, a seemingly impossible file reorganization task is easily done with a few smaller `pathmatcher` calls.
 
 ## Usage
 
 ```
 usage: pathmatcher [-h] -i /some/path -ri "sub[^/]+/\d+" [-o /new/path] [-ro "newsub/\1"] [-c] [-s] [-m]
```

### Comparing `pathmatcher-1.7.5/pathmatcher/mlabwrap/awmstools.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/mlabwrap/matlabcom.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/mlabwrap/matlabpipe.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/mlabwrap/mlabraw.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/mlabwrap/mlabwrap.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/pathlib2/__init__.py` & `pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/pathmatcher.py` & `pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.7.5/pathmatcher/reorientation_registration_helper.py` & `pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -319,19 +319,19 @@
         widget_file = {}
         widget_text = {}
     # Required arguments
     main_parser.add_argument('-i', '--input', metavar='/some/path', type=str, required=True,
                         help='Path to the input folder (the root directory where you placed the files, the default supported tree structure being: "Condition/subject_id/data/(sess_id)?/(mprage|rest)/*.(img|nii)". You can also use --regex_anat and --regex_func to define your own directory layout.', **widget_dir)
 
     # Optional general arguments
-    main_parser.add_argument('-ra', '--regex_anat', metavar='"(reg_expr)+/anat\.(img|nii)"', type=str, required=False, default=None,
+    main_parser.add_argument('-ra', '--regex_anat', metavar='"(\dir)/(\dir)/data/(\dir/)?mprage/[^\\/]+\.(?:img|nii)"', type=str, required=False, default=None,
                         help='Regular expression to match anatomical images (default: Liege CRC scheme). Use regex groups to match with functional regex (if you want to do step 4 - manual coreg). Note: should target nii or img, not hdr.', **widget_text)
-    main_parser.add_argument('-rf', '--regex_func', metavar='"(reg_expr)+/func\.(img|nii)"', type=str, required=False, default=None,
-                        help='Regular expression to match functional images (default: Liege CRC scheme). Regex groups will be matched with the anatomical regex, so you should provide the same groups for both regex. Note: should target nii or img, not hdr (using non-capturing group, eg: ".*\.(?:img|nii)". If a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule).', **widget_text)
-    main_parser.add_argument('-rp', '--regex_motion', metavar='"(reg_expr)+/rp_.+\.txt"', type=str, required=False, default=None,
+    main_parser.add_argument('-rf', '--regex_func', metavar='"(\dir)/(\dir)/data/(?P<func>\dir/)?rest/[^\\/]+\.(?:img|nii)"', type=str, required=False, default=None,
+                        help='Regular expression to match functional images (default: Liege CRC scheme). Regex groups (parts inside parentheses) will be matched with the anatomical regex, so you should provide the same number of groups and at the same folder levels for both regex. The group can include an OR operator using a | (pipe) to match multiple functional conditions, eg, (?P<func>navigation|tennis), then both will be considered as separate session but both being matched to the same structural image. The groups should match for example the groups, subjects and sessions folders, and also the functional conditions if there are multiple ones. For functional conditions, please name the group with (?P<func>) so that the script will know these represent functional sessions, this allows to match multiple sessions with one shared structural image for example, eg, navigation task and tennis task. Indeed, if a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule - so if in that case you should have 1 less group in the -ra regex compared to -rf, hence do not group the mprage/struct folder in the -ra regex!). You are unlimited in the number of groups, but there can be only one "func" named group (intended for multiple functional conditions). This regex must obviously exclude the structural images that are matched with -ra. If you need a more flexible grouping scheme, use pathmatcher.py with the --tree argument. Use the --verbose flag to get more information on what is exactly matched at STEP 4. Note: should target nii or img, not hdr, using non-capturing group, eg: ".*\.(?:img|nii)".', **widget_text)
+    main_parser.add_argument('-rp', '--regex_motion', metavar='"(\dir)/(\dir)/data/(?P<motion>\dir/)?rest/rp_[^\\/]+\.txt"', type=str, required=False, default=None,
                         help='Regular expression to match motion parameter files rp_*.txt as generated by spm_realign. If this argument is provided, motion parameters will be fetched from these files directly instead of recalculating from functional images. The regex needs to contain at least one group in parentheses to define a key for the output excel file.', **widget_text)
     main_parser.add_argument('-m', '--motiononly', action='store_true', required=False, default=False,
                         help='If true, and if --regex_motion is specified, then only this step will be done, using the already generated rpfiles.')
     main_parser.add_argument('-v', '--verbose', action='store_true', required=False, default=False,
                         help='Verbose mode (show more output).')
 
 
@@ -501,27 +501,28 @@
         # == DETECT FUNCTIONAL IMAGES
         print("\n=> STEP4: DETECTION OF FUNCTIONAL IMAGES")
         print("Functional images will now be detected and associated with their relative structural images.\nPlease press ENTER and wait (can be a bit long)...")
         print("Note: nothing will be modified here.")
         input()
         # -- Walk files and detect functional images (we already got structural)
         os.chdir(rootfolderpath)  # reset to rootfolder to generate the simulation report there
-        func_list, conflict_flags = pathmatcher.pathmatcher(r' -i "{inputpath}" -ri "{regex_func}" --silent '.format(**template_vars), True)
+        func_list, conflict_flags = pathmatcher.pathmatcher(r' -i "{inputpath}" -ri "{regex_func}" --silent '.format(**template_vars), True)  # TODO: this can likely be replaced now by the --tree option, and the whole loop below too, potentially being much more concise
         func_list = [file[0] for file in func_list]  # extract only the input match, there's no output anyway
         print("Found %i functional images." % len(func_list))
 
         # -- Precomputing to pair together anatomical images and functional images of the same patient for the same condition
         # Technically, we construct a lookup table where the key is the concatenation of all regex groups
         # For this we use two regex that we apply on file paths: one for anatomical images and one for functional images.
         # The regex groups are then used as the key to assign this file in the lookup table, and then assigned to a subdict 'anat' or 'func' depending on the regex used.
         # This is both flexible because user can provide custom regex and precise because the key is normally unique
         # (this is more flexible than previous approach to walk both anat and func files at once because it would necessitate a 3rd regex)
         im_table = OrderedDict()  # Init lookup table. Always use an OrderedDict so that we walk the subjects id by the same order every time we launch the program (allows to skip already processed subjects)
         RE_anat = re.compile(regex_anat)
         RE_func = re.compile(regex_func)
+        all_func_conditions = set()  # just a set to report to user all conditions that were found, but this is not important for the code to work
         for img_list in [anat_list, func_list]:
             if img_list == anat_list:
                 im_type = 'anat'
             else:
                 im_type = 'func'
 
             for file in img_list:
@@ -530,25 +531,27 @@
                 if im_type == 'anat':
                     m = RE_anat.search(file)
                 else:  # im_type == 'func':
                     m = RE_func.search(file)
                 if m is None:
                     print('Error: no regex match found for type %s file: %s' % (im_type, file))
                 # Use these metadata to build our images lookup table, with every images grouped and organized according to these parameters
-                # TODO: maybe use a 3rd party lib to do this more elegantly? To group strings according to values in the string that match together?
+                # TODO: maybe use a 3rd party lib to do this more elegantly? To group strings according to values in the string that match together? Update years later: pathmatcher now includes a --tree option, this whole loop may be rewritten more elegantly using it.
                 mdict = m.groupdict()
                 if im_type == 'anat' or im_type not in mdict:
                     im_key = '_'.join(filter(None, m.groups()))  # Note: you can use non-capturing groups like (?:non-captured) to avoid capturing things you don't want but you still want to group (eg, for an OR)
                 else:
                     # A named group for func is present
                     mgroups = list(m.groups())
                     # Remove the value matched by 'func' from the non-dict groups
                     mgroups.remove(mdict[im_type])
-                    # Use the non-dict groups as the key
+                    # Use the non-dict groups as the key, this is a workaround to support multiple levels/groups without having to handle nasty multilevels dict nesting, but it reduces functionalities (such as counting and tree walking)
                     im_key = '_'.join(filter(None, mgroups))
+                    # add to list of all functional conditions, just a bookkeeping set to report to user, but useless for code to work
+                    all_func_conditions.add(mdict['func'])  # it's not an .update() because we are processing one match by one, so we will have only one specific condition appear here
                 # Create entry if does not exist
                 if im_key not in im_table:
                     # Creade node
                     im_table[im_key] = {}
                 if im_type not in im_table[im_key]:
                     if im_type == 'func' and im_type in mdict:
                         # Create node
@@ -564,18 +567,26 @@
                 # But files that are not meant to be grouped can be grouped in the end, so you need to make sure your regex is correct (can use pathmatcher or --verbose to check).
                 if im_type == 'anat' or im_type not in mdict:
                     im_table[im_key][im_type].append(os.path.join(rootfolderpath, file))
                 else:
                     # Named group for func is present, we create a subfolder for each value (so that multiple func folders can be stored)
                     im_table[im_key][im_type][mdict[im_type]].append(os.path.join(rootfolderpath, file))
 
-        # Precompute total number of subjects user will have to process (to show progress bar)
+        # Precompute total number of functional images groups the user will have to process (to show progress bar) - so it's not the total functional images count, but the number of groups of functional images, since the user will only have to coregister the first image and apply on all the others
         total_func_images = len(im_table)
+        print("Found %i groups of functional images to process." % total_func_images)
+        if 'func' in mdict:
+            print("And found %i functional conditions." % len(all_func_conditions))
+        if verbose:
+            print("Matched groups: %s" % list(im_table.keys()))
+            if 'func' in mdict:
+                print("Matched functional conditions: %s" % list(all_func_conditions))
 
-        # Expand 4D nifti images (get the volume numbers for them, so that we do not simply consider them as a single image)
+        # Expand 4D nifti images (get the volume numbers for them, so that we do not simply consider them as a single image) - note that this does NOT modify the nifti files, we expand in memory only
+        print("Expanding in-memory the 4D nifti images (no file is modified, this is necessary to access individual volumes and for the coregistration to work OK on save in SPM). All nifti files will be walked and check if 4D nifti, then expanded if true. Expanding means that we simply get the list of all volumes/frames inside a single 4D nifti file.")
         # for each key (can be each subject)
         for im_key in tqdm(im_table.keys(), total=total_func_images, leave=True, unit='subjects', desc='4DEXPAND'):
             # check if there is both anatomical and structural images available, if one is missing we simply skip
             if 'func' not in im_table[im_key]:
                 continue
             # prepare the functional images list (there might be multiple folders)
             if isinstance(im_table[im_key]['func'], dict):
@@ -649,16 +660,16 @@
                     # Support for 4D nifti: select the first volume of the functional image that will be used as the source for coregistration
                     # Also we do not use the expanded functional images list, since there is only one header for all volumes in a 4D nifti, we need to apply the coregistration translation on only the first volume, this will be propagated to all others
                     im_func += ',1'
                     # Send to MATLAB checkreg!
                     #mlab.workspace.functionalcoreg(im_anat, im_func, im_func_others, nout=0)  # matlab_wrapper
                     #mlab.run_func('functionalcoreg.m', im_anat, im_func, im_func_others)  # python-matlab-bridge
                     # Alternative for other libraries
-                    matlab.cd(os.path.dirname(im_func))  # Change MATLAB current directory to the functional images dir (no real reason)
-                    matlab.functionalcoreg(im_anat, im_func, im_func_others)
+                    mlab.cd(os.path.dirname(im_func))  # Change MATLAB current directory to the functional images dir (no real reason)
+                    mlab.functionalcoreg(im_anat, im_func, im_func_others)
 
         # == MANUAL COREGISTRATION
         print("\n=> STEP6: MANUAL COREGISTRATION OF FUNCTIONAL IMAGES")
         print("The first functional image for each session will now be displayed (bottom) along the corresponding anatomical image (top). Please reorient the functional image to match the anatomical image, and select all functional images to apply the reorientation.")
         print("This step is very important, because the automatic coregistration algorithms are not optimal (they cannot be, the problem is non-linear), and thus they can fall in local optimums. A good manual coregistration ensures the automatic coregistration will be on-the-spot!")
         print("NOTE: you need to right-click on the bottom image, then click on Reorient Images > Current image. Red contours of the bottom functional image will be overlaid on the top anatomical image, and a side menu will open to allow you to reorient the bottom image and apply on other functional images.")
         print("NOTE2: you can also enhance the contrasts by right-clicking on functional image and select Zoom > This image non zero, by setting the number of contours to 2 instead of 3, and by right-clicking on the anatomical image and select Image > Intensity Mapping > local > Equalised squared-histogram (you can also do the same intensity mapping change on the functional image, the contours will adapt according to the greater contrast).")
@@ -679,15 +690,15 @@
                 else:
                     # only one folder, we simply put it in a list so that we don't break the loop
                     funclists = {'0': im_table[im_key]['func_expanded']}
                 # For each functional image subfolder
                 for i, k in enumerate(funclists.keys()):
                     funclist = funclists[k]
                     # Wait for user to be ready
-                    uchoice = ask_next(msg='Open next registration for subject %s session %s (%i/%i)? Enter to [c]ontinue, Skip to [n]ext session, [S]kip to next subject, [A]bort: ' % (im_key, str(k), i+1, len(funclists)))  # ask user if we load the next file?
+                    uchoice = ask_next(msg='Open next registration for subject %s condition %s (%i/%i)? Enter to [c]ontinue, Skip to [n]ext condition, [S]kip to next subject, [A]bort: ' % (im_key, str(k), i+1, len(funclists)))  # ask user if we load the next file?
                     if uchoice is None: break
                     if uchoice == False: continue
                     select_t2_nb = 0  # for user to specify a specific T2 image, by default the first image (because in general we coregister the first volume on structural)
                     while 1:
                         # Pick a T1 and T2 images for this subject
                         if select_t2_nb is not None:
                             # Pick a specific image specified by user
```

### Comparing `pathmatcher-1.7.5/pathmatcher/tee.py` & `pathmatcher-1.8.0b2/pathmatcher/tee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-#
-
 from __future__ import unicode_literals
 from builtins import object
 import sys
 
 if sys.version_info < (3,):
     def b(x):
         return x
@@ -29,20 +26,26 @@
         if name is not None and mode is not None:
             self.filename = name
             self.filemode = mode
             self.file = open(name, mode)
 
     def close(self):
         """ Restore stdout and close file when Tee is closed """
-        self.flush() # commit all latest changes before exiting
+        try:
+            self.flush() # commit all latest changes before exiting
+        except:
+            pass  # sometimes it's already closed, just skip
         if not self.nostdout and hasattr(self, 'stdout'):
             sys.stdout = self.stdout
             self.stdout = None
         if self.file: self.file.close()
 
+    def __del__(self):
+        self.close()
+
     def write(self, data, end="\n", flush=True):
         """ Output data to stdout and/or file """
         if not self.silent:
             if not self.nostdout:
                 self.stdout.write(data)
                 self.stdout.write(end)
             if self.file is not None:
```

### Comparing `pathmatcher-1.7.5/pathmatcher.egg-info/PKG-INFO` & `pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,416 +1,466 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.7.5
-Summary: Regular Expression Path Matcher
-Home-page: https://github.com/lrq3000/pathmatcher
-Author: Stephen Karl Larroque
-Author-email: lrq3000@gmail.com
-License: MIT
-Description: # Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
-        
-        [![PyPI-Status](https://img.shields.io/pypi/v/pathmatcher.svg)](https://pypi.org/project/pathmatcher)
-        [![PyPI-Versions](https://img.shields.io/pypi/pyversions/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
-        [![PyPI-Downloads](https://img.shields.io/pypi/dm/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
-        
-        Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
-        
-        If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
-        
-        If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
-        
-        This module works for any file management purpose, but it is particularly optimized via the reorientation_registration_helper.py submodule to work for neuroimaging, such as reorganizing very fast any dataset into a BIDS compliant format.
-        
-        This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. For an exemple, see the script `reorient_pipeline` at the root of this repository.
-        
-        As a Python module, it can not only match inputpaths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
-        
-        Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
-        
-        If you are not experienced with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp.
-        
-        ## Install
-        
-        Simply use pypi:
-        
-        ```
-        pip install --upgrade pathmatcher
-        ```
-        
-        Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
-        
-        ## Quickstart
-        
-        Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename.
-        
-        You can match them like this:
-        
-        ```
-        pathmatcher -i "root" -ri "(\dir)/(.*)" --test
-        ```
-        
-        The arguments are as follows:
-        * `-i` is the input root directory from where the recursive file search will start.
-        * `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes).
-        * `--test` will test whether at least one file can be matched. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
-        
-        Here is the output we get:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: root
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: None
-        - Output regex: None
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) --test
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
-        
-        Match: folderA/file1.txt
-        
-        0files [00:00, ?files/s]
-        End of simulation. 1 files matched.
-        ```
-        
-        Since we have matched one file, this shows the regexp works, we're good to go.
-        
-        Note: In the case it didn't work (no file matched), and there are lots of files, you can prematurely stop the file search by pressing CTRL+C.
-        
-        Next, type this:
-        
-        ```
-        pathmatcher -i "root" -ri "(\dir)/(.*)" -o "out" -ro "\1_\2" --copy
-        ```
-        
-        This reuses the previous command's input arguments (except `--test`) and adds the 3 following arguments:
-        * `--copy` will copy the matched files to an output folder, potentially with a modified filename if specified in `-ro`. Alternative commands are: `--move`, `--move_fast`, `--delete`, `--symlink`.
-        * `-o` is the output directory.
-        * `-ro` is the output paths regular expression. This allows to dynamically change the output filenames by reusing regexp groups from the matched input paths. Here, we reuse the subdirectory name captured in `\1` and reuse it to prepend before the original input path `\2`.
-        
-        Before applying any file modification operation, pathmatcher will provide a complete simulation report of what it plans to do, including whether there will be overwriting conflicts (eg, 2 different files will get the same filename).
-        
-        Here is the simulation report for our command above:
-        
-        ```
-        == REGEX PATH MATCHER SIMULATION REPORT ==
-        Total number of files matched: 6
-        Parameters:
-        - Input root: b'root'
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: b'out'
-        - Output regex: \1_\2
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
-        
-        List of matched files:
-        * folderA/file1.txt --> folderA_file1.txt  
-        * folderA/file2.txt --> folderA_file2.txt  
-        * folderA/file3.txt --> folderA_file3.txt  
-        * folderB/file4.txt --> folderB_file4.txt  
-        * folderB/file5.txt --> folderB_file5.txt  
-        * folderB/file6.txt --> folderB_file6.txt  
-        ```
-        
-        By default, the simulation report is saved as `pathmatcher_report.txt` in the current terminal folder (as shown by `pwd`) and is opened in the default text editor. This behavior can be modified using `--noreport``, which will print the simulation report directly in the terminal.
-        
-        Now, we manually review the simulation report, and we can see that everything is going as planned.
-        
-        Let's go back to the terminal:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: root
-        - Input regex: ([^\\/]*?)/(.*)
-        - Output root: out
-        - Output regex: \1_\2
-        - Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
-        
-        12files [00:00, ?files/s]
-        End of simulation. 6 files matched.
-        Preparing simulation report, please wait a few seconds...
-        Opening simulation report with your default editor, a new window should open.
-        
-        
-        No conflict detected. You are good to go!
-        Do you want to apply the result of the path reorganization simulation on 6 files? [Y/N]:
-        ```
-        
-        The terminal confirms that there are no conflicts (which would have appeared in the simulation report too), and asks us whether we want to proceed.
-        
-        If we type `Y` and tap Enter, the files will be copied and renamed according to the simulation report above. If we type `N` or simply CTRL+C, the application stops.
-        
-        This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order).
-        
-        There is also the very powerful `--tree` option, also available as an argument in the Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command.
-        
-        Pro tip: if you can't get a file reorganization task done in a single command, try to break down your task into several smaller steps, such as for example first renaming, then moving, then renaming again, then moving again, then deleting the unnecessary files, etc. Usually, a seemingly impossible file reorganization task is easily done with a few smaller `pathmatcher` calls.
-        
-        ## Usage
-        
-        ```
-        usage: pathmatcher [-h] -i /some/path -ri "sub[^/]+/\d+" [-o /new/path] [-ro "newsub/\1"] [-c] [-s] [-m]
-                                   [--move_fast] [-d] [-t] [--dir] [-y] [-f] [--show_fullpath] [-ra 1:10-255]
-                                   [-re "newsub/\1"] [--report pathmatcher_report.txt] [--noreport] [--tree]
-                                   [-l /some/folder/filename.log] [-v] [--silent]
-        
-        Regex PathMatcher v1.7.4
-        Description: Match paths using regular expression, and then generate a report. Can also substitute using regex to generate output paths. A copy mode is also provided to allow the copy of files from input to output paths.
-        This app is essentially a path matcher using regexp, and it then rewrites the path using regexp, so that you can reuse elements from input path to build the output path.
-        This is very useful to reorganize folders for experiments, where scripts/softwares expect a specific directories layout in order to work.
-        
-        Advices
-        -------
-        - Filepath comparison: Paths are compared against filepaths, not just folders (but of course you can match folders with regex, but remember when designing your regexp that it will compared against files paths, not directories).
-        - Relative filepath: Paths are relative to the rootpath (except if --show-fullpath) and that they are always unix style, even on Windows (for consistency on all platforms and to easily reuse regexp).
-        - Partial matching: partial matching regex is accepted, so you don't need to model the full filepath, only the part you need (eg, 'myfile' will match '/myfolder/sub/myfile-034.mat').
-        - Unix filepaths: on all platforms, including Windows, paths will be in unix format (except if you set --show_fullpath). It makes things simpler for you to make crossplatform regex patterns.
-        - Use [^/]+ to match any file/folder in the filepath: because paths are always unix-like, you can use [^/]+ to match any part of the filepath. Eg, "([^/]+)/([^/]+)/data/mprage/.+\.(img|hdr|txt)" will match "UWS/John_Doe/data/mprage/12345_t1_mprage_98782.hdr".
-        - Split your big task in several smaller, simpler subtasks: instead of trying to do a regex that match T1, T2, DTI, everything at the same time, try to focus on only one modality at a time and execute them using multiple regex queries: eg, move first structural images, then functional images, then dti, etc. instead of all at once.
-        - Python module: this library can be used as a Python module to include in your scripts (just call `main(return_report=True)`).
-        
-        Note: use --gui (without any other argument) to launch the experimental gui (needs Gooey library).
-        
-        In addition to the switches provided below, using this program as a Python module also provides 2 additional options:
-         - return_report = True to return as a variable the files matched and the report instead of saving in a file.
-         - regroup = True will return the matched files (if return_report=True) in a tree structure of nested list/dicts depending on if the groups are named or not. Groups can also avoid being matched by using non-matching groups in regex.
-        
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -i /some/path, --input /some/path
-                                Path to the input folder
-          -ri "sub[^/]+/(\d+)", --regex_input "sub[^/]+/(\d+)"
-                                Regex to match input paths. Must be defined relatively from --input folder. Do not forget to enclose it in double quotes (and not single)! To match any directory, use [^/\]*? or the alias \dir, or \dirnodot if you want to match folders in combination with --dir switch.
-          -o /new/path, --output /new/path
-                                Path to the output folder (where file will get copied over if --copy)
-          -ro "newsub/\1", --regex_output "newsub/\1"
-                                Regex to substitute input paths to convert to output paths. Must be defined relatively from --output folder. If not provided but --output is specified, will keep the same directory layout as input (useful to extract specific files without changing layout). Do not forget to enclose it in double quotes!
-          -c, --copy            Copy the matched input paths to the regex-substituted output paths.
-          -s, --symlink         Copy with a symbolic/soft link the matched input paths to the regex-substituted output paths (works only on Linux).
-          -m, --move            Move the matched input paths to the regex-substituted output paths.
-          --move_fast           Move the matched input paths to the regex-substituted output paths, without checking first that the copy was done correctly.
-          -d, --delete          Delete the matched files.
-          -t, --test            Regex test mode: Stop after the first matched file and show the result of substitution. Useful to quickly check if the regex patterns are ok.
-          --dir                 Match directories too? (else only files are matched)
-          -y, --yes             Automatically accept the simulation and apply changes (good for batch processing and command chaining).
-          -f, --force           Force overwriting the target path already exists. Note that by default, if a file already exist, without this option, it won't get overwritten and no message will be displayed.
-          --show_fullpath       Show full paths instead of relative paths in the simulation.
-          -ra 1:10-255, --range 1:10-255
-                                Range mode: match only the files with filenames containing numbers in the specified range. The format is: (regex-match-group-id):(range-start)-(range-end). regex-match-group-id is the id of the regular expression that will contain the numbers that must be compared to the range. range-end is inclusive.
-          -re "newsub/\1", --regex_exists "newsub/\1"
-                                Regex of output path to check if the matched regex here is matched prior writing output files.
-          --report pathmatcher_report.txt
-                                Where to store the simulation report (default: pwd = current working dir).
-          --noreport            Do not create a report file, print the report in the console.
-          --tree                Regroup in a tree structure the matched files according to named and unnamed regex groups, and save the result as a json file (pathmatcher_tree.json).
-          -l /some/folder/filename.log, --log /some/folder/filename.log
-                                Path to the log file. (Output will be piped to both the stdout and the log file)
-          -v, --verbose         Verbose mode (show more output).
-          --silent              No console output (but if --log specified, the log will still be saved in the specified file).
-        
-        ```
-        
-        ## Libraries
-        
-        ### Required
-        
-        * core Python libraries...
-        * argparse
-        * pathlib2 (provided with the script)
-        * Tee (provided with the script)
-        
-        ### Optional
-        
-        * **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
-        * scandir (for faster file walking and simulation report)
-        * Gooey (for gui)
-        
-        ## Tutorial
-        
-        Here is a short introduction in the usage of `pathmatcher.py`.
-        
-        The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
-        
-        Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
-        
-        To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
-        
-        Now, in the commandline, execute the two following commands:
-        
-        ```python
-        python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
-        
-        python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
-        ```
-        
-        Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
-        
-        Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
-        
-        After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
-        
-        This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
-        
-        ```python
-        python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
-        
-        python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
-        ```
-        
-        Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
-        
-        ```python
-        python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
-        ```
-        
-        This will generate the whole list of T1 and show them in a report.
-        
-        Of course, you can also use absolute paths for `--input` and `--output`.
-        
-        And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
-        
-        ```python
-        python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
-        ```
-        
-        Result:
-        
-        ```
-        == Regex Path Matcher started ==
-        
-        Parameters:
-        - Input root: C:\GigaData\BIDS\ABIDE
-        - Input regex: Caltech_([0-9]+)/.+/mprage.nii.gz
-        - Output root: C:\GigaData\BIDS\ABIDE-BIDS
-        - Output regex: sub-\1/anat/sub-\1_T1w.nii.gz
-        
-        
-        Computing paths matching and simulation report, please wait (total time depends
-        on files count - filesize has no influence). Press CTRL+C to abort
-        
-        Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
-        
-        
-        End of simulation. 1 files matched.
-        ```
-        
-        Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
-        
-        ```python
-        from pathmatcher import main as pm
-        
-        # Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
-        # You can use the commandline arguments, but the script will be called without bash but directly inside Python
-        my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
-        
-        print(my_results)
-        ```
-        
-        A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
-        
-        ### Similar projects
-        
-        A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
-        
-        ## Auxiliary tool: Reorientation and registration helper
-        
-        ### Description
-        
-        A companion to help you reorient and coregister manually your structural and functional MRI in SPM, without having to click to select files.
-        
-        This helper script will scan all images in the specified input path, and will accompagny you step-by-step to do the reorientation and coregistration correctly.
-        
-        This script requires SPM12 (and MATLAB), and runs only on Windows (because of the matlab wrapper limitations).
-        
-        This script follows the following steps:
-        
-        1. Automatic reorientation of structural MRI using [spm_auto_reorient.m](https://github.com/lrq3000/spm_auto_reorient) (please install this script along with SPM12 beforehand).
-        2. Check reorient and adjust manually.
-        3. Side-by-side check of multiple subjects' structural MRI.
-        4. Detection of functional images (just walk through all folders to build a list of functional images and pair them to their respective structural images given the input regexp).
-        5. Automatic co-registration of functional images onto structural.
-        6. Manual co-registration of functional images with structural.
-        7. Extraction of framewise displacement motion metrics from functional images.
-        
-        This script will not only guide you through these steps, in the correct order, but it will also automatically load the files for you (no chance of doing a mistake or missing a subject), while showing you a progress bar (showing how many subjects are remaining and with a time estimate to finish).
-        
-        There is a CLI user interface: you can skip steps you already done or don't want to do, skip patients, or reload another image (for step 4, to check other functional images).
-        
-        Note that the last step, extraction of framewise displacement motion metrics from functional images, can be done without requiring matlab nor a matlab wrapper (and hence should work on any platform), by using the `--motiononly` and `--regex_motion` switches (this will directly look for the `rp_*.txt` files that you previously generated with `spm_realign`).
-        
-        ### Usage
-        
-        ```
-        usage: reorientation_registration_helper [-h] -i /some/path [-ra "reg_expr+/anat\.(img|nii)"]
-                                                         [-rf "reg_expr+/func\.(img|nii)"] [-rp "reg_expr+/rp_.+\.txt"] [-m]
-                                                         [-v]
-        
-        Reorientation and registration helper v1.7.4
-        Description: Guide and automate the file selection process that is required in SPM between each reorientation/registration.
-        
-        No more useless clicks, just do the reorientation/registration in batch, you don't need to worry about selecting the corresponding files, this helper will do it for you.
-        
-        If you have tqdm installed, a nice progress bar will tell you how many subjects are remaining to be processed and how much time will it take at your current pace.
-        
-        Note: you need to `pip install mlab` before using this script.
-        Note2: you need to have set both spm and spm_auto_reorient in your path in MATLAB before using this script.
-        Note3: you need the pathmatcher.py library (see lrq3000 github).
-        
-        
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -i /some/path, --input /some/path
-                                Path to the input folder (the root directory where you placed the files, the default supported tree structure being: "Condition/subject_id/data/(sess_id)?/(mprage|rest)/*.(img|nii)". You can also use --regex_anat and --regex_func to define your own directory layout.
-          -ra "(reg_expr)+/anat\.(img|nii)", --regex_anat "(reg_expr)+/anat\.(img|nii)"
-                                Regular expression to match anatomical images (default: Liege CRC scheme). Use regex groups to match with functional regex (if you want to do step 4 - manual coreg). Note: should target nii or img, not hdr.
-          -rf "(reg_expr)+/func\.(img|nii)", --regex_func "(reg_expr)+/func\.(img|nii)"
-                                Regular expression to match functional images (default: Liege CRC scheme). Regex groups will be matched with the anatomical regex, so you should provide the same groups for both regex. Note: should target nii or img, not hdr (using non-capturing group, eg: ".*\.(?:img|nii)". If a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule).
-          -rp "(reg_expr)+/rp_.+\.txt", --regex_motion "(reg_expr)+/rp_.+\.txt"
-                                Regular expression to match motion parameter files rp_*.txt as generated by spm_realign. If this argument is provided, motion parameters will be fetched from these files directly instead of recalculating from functional images. The regex needs to contain at least one group in parentheses to define a key for the output excel file.
-          -m, --motiononly      If true, and if --regex_motion is specified, then only this step will be done, using the already generated rpfiles.
-          -v, --verbose         Verbose mode (show more output).
-        
-        ```
-        
-        ### Libraries
-        
-        #### Required
-        
-        * argparse
-        * pathmatcher
-        * mlabwrap aka matlap_wrapper ([Python2](https://github.com/mrkrd/matlab_wrapper) version, [Python3](https://github.com/deeuu/matlab_wrapper/tree/python3) version as provided with this module)
-        * pypiwin32 (for mlabwrap)
-        * pip install --ignore-installed pywin32
-            * then execute `python Scripts\pywin32_postinstall.py -install` in an admin command prompt, see [this explanation](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api#comment103561767_58613735).
-        
-        #### Optional
-        
-        * scandir, to scan files faster
-        * tqdm, to show the progress bar
-        * numpy >= 1.18.1, for the optional last step to generate motion metrics from functional images
-        
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Utilities
+Version: 1.8.0b2
+Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
+Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
+Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
+Project-URL: Source, https://github.com/lrq3000/pathmatcher
+Project-URL: Tracker, https://github.com/lrq3000/pathmatcher/issues
+Project-URL: Download, https://github.com/lrq3000/pathmatcher/releases
+Keywords: file,folders,manipulation,copy,move,delete,batch,regex,regexp,regular expression,regular expressions,file trees,file tree,files tree,files trees,neuroimaging,mri,fmri,nifti,nii,reorientation,spm
+Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Intended Audience :: System Administrators
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: testmeta
+License-File: LICENSE
+
+# Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
+
+[![PyPI-Status](https://img.shields.io/pypi/v/pathmatcher.svg)](https://pypi.org/project/pathmatcher)
+[![PyPI-Versions](https://img.shields.io/pypi/pyversions/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
+[![PyPI-Downloads](https://img.shields.io/pypi/dm/pathmatcher.svg?logo=python&logoColor=white)](https://pypi.org/project/pathmatcher)
+
+Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
+
+If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
+
+If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
+
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
+
+This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
+
+Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
+
+If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
+
+## Install
+
+For Python 3.7+:
+
+```
+pip install --upgrade pathmatcher
+```
+
+Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
+
+For the latest development release, use:
+
+```
+pip install --upgrade pathmatcher --pre
+```
+
+For the cutting-edge code (likely unstable, do not use in production!), use:
+
+```
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+```
+
+For Python 2.7 to 3.6, the last compatible version is v1.7.6:
+
+```
+pip install --upgrade pathmatcher==1.7.6
+```
+
+This will install two commands in your environment: `pathmatcher` and `reorientation_registration_helper`.
+
+## Quickstart
+
+This section is a hands-on introduction illustrating the steps of a typical session of pathmatching, from how to quickly draft a regular expression (regexp) that matches your files to how to apply it to fulfil your target file structure.
+
+Let's say you have a directory named "root", with subdirectories, and inside each subdirectory you have some files. Now, you want to reorganize so that all files are in one single folder, but you want to keep the original subfolder name but prepend it in the filename. Here is a schema of this files structure:
+
+```
+root
+|--- folderA
+        |--- file1.txt
+        |--- file2.txt
+        |--- file3.txt
+|--- folderB
+        |--- file4.txt
+        |--- file5.txt
+        |--- file6.txt
+```
+
+You can match them like this:
+
+```
+pathmatcher -i "root" -ri "(\dir)/(.*)" --test
+```
+
+The arguments are as follows:
+* `-i` is the input root directory from where the recursive file search will start.
+* `-ri` is the input paths regular expression, to match the files you want. The matching is partial by default, so you can just type part of the filepath you want to match, not the whole (if you want the regex to match the whole path, use a regex starting with `^` and ending with `$` such as `"^my/whole/path.ext$"`). `(.*)` will match anything, and `\dir` is a special argument that will match any directory (or file) until the next subdirectory level, which kind of allows a virtual walk through a tree. All paths are specified with `/`, never with `\`, whatever the platform (including on Windows OSes). Here, `(\dir)` will match `folderA` and `folderB`. If we had an unlimited number of depth in subfolders and we wanted to recurse, we could use `(\dir/)+` which means that we match: `\dir` a directory, `/` a path separator to next level (so we can chain multiple depths), `+` at least one subfolder level and as many as there are if there are multiple levels.
+* `--test` will test whether at least one file can be matched, and then stops. This is great to quickly test whether a regular expression is adequately matching the thing you want, without having to walk through all files.
+
+Here is the output we get:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: root
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: None
+- Output regex: None
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) --test
+
+
+Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
+
+Match: folderA/file1.txt
+
+0files [00:00, ?files/s]
+End of simulation. 1 files matched.
+```
+
+Since we have matched one file, this shows the regexp works, we're good to go.
+
+Note: In the case it didn't work (no file matched), and there are lots of files, you can prematurely stop the file search by pressing CTRL+C.
+
+Next, type this:
+
+```
+pathmatcher -i "root" -ri "(\dir)/(.*)" -o "out" -ro "\1_\2" --copy
+```
+
+This reuses the previous command's input arguments (except `--test`) and adds the 3 following arguments:
+* `--copy` will copy the matched files to an output folder, potentially with a modified filename if specified in `-ro`. Alternative commands are: `--move`, `--move_fast`, `--delete`, `--symlink`.
+* `-o` is the output directory.
+* `-ro` is the output paths regular expression. This allows to dynamically change the output filenames by reusing regexp groups from the matched input paths. Here, we reuse the subdirectory name captured in `\1` and reuse it to prepend before the original input path `\2`.
+
+Before applying any file modification operation, pathmatcher will provide a complete simulation report of what it plans to do, including whether there will be overwriting conflicts (eg, 2 different files will get the same filename).
+
+Here is the simulation report for our command above:
+
+```
+== REGEX PATH MATCHER SIMULATION REPORT ==
+Total number of files matched: 6
+Parameters:
+- Input root: b'root'
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: b'out'
+- Output regex: \1_\2
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
+
+List of matched files:
+* folderA/file1.txt --> folderA_file1.txt  
+* folderA/file2.txt --> folderA_file2.txt  
+* folderA/file3.txt --> folderA_file3.txt  
+* folderB/file4.txt --> folderB_file4.txt  
+* folderB/file5.txt --> folderB_file5.txt  
+* folderB/file6.txt --> folderB_file6.txt  
+```
+
+By default, the simulation report is saved as `pathmatcher_report.txt` in the current terminal folder (as shown by `pwd`) and is opened in the default text editor. This behavior can be modified using `--noreport``, which will print the simulation report directly in the terminal.
+
+Now, we manually review the simulation report, and we can see that everything is going as planned.
+
+Let's go back to the terminal:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: root
+- Input regex: ([^\\/]*?)/(.*)
+- Output root: out
+- Output regex: \1_\2
+- Full arguments: X:\Path\To\pathmatcher -i root -ri (\dir)/(.*) -o out -ro \1_\2 --copy
+
+
+Computing paths matching and simulation report, please wait (total time depends on files count - filesize has no influence). Press CTRL+C to abort
+
+12files [00:00, ?files/s]
+End of simulation. 6 files matched.
+Preparing simulation report, please wait a few seconds...
+Opening simulation report with your default editor, a new window should open.
+
+
+No conflict detected. You are good to go!
+Do you want to apply the result of the path reorganization simulation on 6 files? [Y/N]:
+```
+
+The terminal confirms that there are no conflicts (which would have appeared in the simulation report too), and asks us whether we want to proceed.
+
+If we type `Y` and tap Enter, the files will be copied and renamed according to the simulation report above. If we type `N` or simply CTRL+C, the application stops.
+
+This concludes this quickstart. There is a lot more that you can do with this tool, such as matching a precise number range (let's say you have images numbered 1 to 100 and you want to delete the first 3, you can use `-ra 4:1-3 --delete` where `4` is the position of the input regexp matching group that matches the number in your input paths). By default, only paths leading to a file are considered as a leaf and hence walked, with directories being considered as nodes (this is to avoid processing multiple times the same directory leading to various paths - with files we are sure it's a leaf, there is a unique path in the tree leading to it in theory), but you can specify `--dir` to consider any directory as a leaf (in which case the walk order is as follows: first the files, then the deepest subdirectories, then progressively upwards to the root, and in alphabetical order, so the walking order is always deterministic).
+
+There is also the very powerful `--tree` option, also available as an argument when used as a Python module, which allows to group together in a tree-like structure the matched input files, which is a very powerful way to match multi-modal data and cluster them together in usually a single command and then post-process with your own script.
+
+Pro tip: if you can't get a file reorganization task done in a single command, try to break down your task into several smaller steps, such as for example first renaming, then moving, then renaming again, then moving again, then deleting the unnecessary files, etc. Usually, a seemingly impossible file reorganization task is easily done with a few smaller `pathmatcher` calls.
+
+## Usage
+
+```
+usage: pathmatcher [-h] -i /some/path -ri "sub[^/]+/\d+" [-o /new/path] [-ro "newsub/\1"] [-c] [-s] [-m]
+                           [--move_fast] [-d] [-t] [--dir] [-y] [-f] [--show_fullpath] [-ra 1:10-255]
+                           [-re "newsub/\1"] [--report pathmatcher_report.txt] [--noreport] [--tree]
+                           [-l /some/folder/filename.log] [-v] [--silent]
+
+Regex PathMatcher v1.7.4
+Description: Match paths using regular expression, and then generate a report. Can also substitute using regex to generate output paths. A copy mode is also provided to allow the copy of files from input to output paths.
+This app is essentially a path matcher using regexp, and it then rewrites the path using regexp, so that you can reuse elements from input path to build the output path.
+This is very useful to reorganize folders for experiments, where scripts/softwares expect a specific directories layout in order to work.
+
+Advices
+-------
+- Filepath comparison: Paths are compared against filepaths, not just folders (but of course you can match folders with regex, but remember when designing your regexp that it will compared against files paths, not directories).
+- Relative filepath: Paths are relative to the rootpath (except if --show-fullpath) and that they are always unix style, even on Windows (for consistency on all platforms and to easily reuse regexp).
+- Partial matching: partial matching regex is accepted, so you don't need to model the full filepath, only the part you need (eg, 'myfile' will match '/myfolder/sub/myfile-034.mat').
+- Unix filepaths: on all platforms, including Windows, paths will be in unix format (except if you set --show_fullpath). It makes things simpler for you to make crossplatform regex patterns.
+- Use [^/]+ to match any file/folder in the filepath: because paths are always unix-like, you can use [^/]+ to match any part of the filepath. Eg, "([^/]+)/([^/]+)/data/mprage/.+\.(img|hdr|txt)" will match "UWS/John_Doe/data/mprage/12345_t1_mprage_98782.hdr".
+- Split your big task in several smaller, simpler subtasks: instead of trying to do a regex that match T1, T2, DTI, everything at the same time, try to focus on only one modality at a time and execute them using multiple regex queries: eg, move first structural images, then functional images, then dti, etc. instead of all at once.
+- Python module: this library can be used as a Python module to include in your scripts (just call `main(return_report=True)`).
+
+Note: use --gui (without any other argument) to launch the experimental gui (needs Gooey library).
+
+In addition to the switches provided below, using this program as a Python module also provides 2 additional options:
+ - return_report = True to return as a variable the files matched and the report instead of saving in a file.
+ - regroup = True will return the matched files (if return_report=True) in a tree structure of nested list/dicts depending on if the groups are named or not. Groups can also avoid being matched by using non-matching groups in regex.
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i /some/path, --input /some/path
+                        Path to the input folder
+  -ri "sub[^/]+/(\d+)", --regex_input "sub[^/]+/(\d+)"
+                        Regex to match input paths. Must be defined relatively from --input folder. Do not forget to enclose it in double quotes (and not single)! To match any directory, use [^/\]*? or the alias \dir, or \dirnodot if you want to match folders in combination with --dir switch.
+  -o /new/path, --output /new/path
+                        Path to the output folder (where file will get copied over if --copy)
+  -ro "newsub/\1", --regex_output "newsub/\1"
+                        Regex to substitute input paths to convert to output paths. Must be defined relatively from --output folder. If not provided but --output is specified, will keep the same directory layout as input (useful to extract specific files without changing layout). Do not forget to enclose it in double quotes!
+  -c, --copy            Copy the matched input paths to the regex-substituted output paths.
+  -s, --symlink         Copy with a symbolic/soft link the matched input paths to the regex-substituted output paths (works only on Linux).
+  -m, --move            Move the matched input paths to the regex-substituted output paths.
+  --move_fast           Move the matched input paths to the regex-substituted output paths, without checking first that the copy was done correctly.
+  -d, --delete          Delete the matched files.
+  -t, --test            Regex test mode: Stop after the first matched file and show the result of substitution. Useful to quickly check if the regex patterns are ok.
+  --dir                 Match directories too? (else only files are matched)
+  -y, --yes             Automatically accept the simulation and apply changes (good for batch processing and command chaining).
+  -f, --force           Force overwriting the target path already exists. Note that by default, if a file already exist, without this option, it won't get overwritten and no message will be displayed.
+  --show_fullpath       Show full paths instead of relative paths in the simulation.
+  -ra 1:10-255, --range 1:10-255
+                        Range mode: match only the files with filenames containing numbers in the specified range. The format is: (regex-match-group-id):(range-start)-(range-end). regex-match-group-id is the id of the regular expression that will contain the numbers that must be compared to the range. range-end is inclusive.
+  -re "newsub/\1", --regex_exists "newsub/\1"
+                        Regex of output path to check if the matched regex here is matched prior writing output files.
+  --report pathmatcher_report.txt
+                        Where to store the simulation report (default: pwd = current working dir).
+  --noreport            Do not create a report file, print the report in the console.
+  --tree                Regroup in a tree structure the matched files according to named and unnamed regex groups, and save the result as a json file (pathmatcher_tree.json).
+  -l /some/folder/filename.log, --log /some/folder/filename.log
+                        Path to the log file. (Output will be piped to both the stdout and the log file)
+  -v, --verbose         Verbose mode (show more output).
+  --silent              No console output (but if --log specified, the log will still be saved in the specified file).
+
+```
+
+## Libraries
+
+### Required
+
+* core Python libraries...
+* argparse
+* pathlib2 (provided with the script)
+* Tee (provided with the script)
+
+### Optional
+
+* **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
+* scandir (for faster file walking and simulation report)
+* Gooey (for gui)
+
+## Tutorial
+
+Here is a short introduction in the usage of `pathmatcher.py`.
+
+The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
+
+Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
+
+To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
+
+Now, in the commandline, execute the two following commands:
+
+```python
+python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+
+python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+```
+
+Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
+
+Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
+
+After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
+
+This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
+
+```python
+python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+
+python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
+```
+
+Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
+
+```python
+python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
+```
+
+This will generate the whole list of T1 and show them in a report.
+
+Of course, you can also use absolute paths for `--input` and `--output`.
+
+And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
+
+```python
+python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+```
+
+Result:
+
+```
+== Regex Path Matcher started ==
+
+Parameters:
+- Input root: C:\GigaData\BIDS\ABIDE
+- Input regex: Caltech_([0-9]+)/.+/mprage.nii.gz
+- Output root: C:\GigaData\BIDS\ABIDE-BIDS
+- Output regex: sub-\1/anat/sub-\1_T1w.nii.gz
+
+
+Computing paths matching and simulation report, please wait (total time depends
+on files count - filesize has no influence). Press CTRL+C to abort
+
+Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
+
+
+End of simulation. 1 files matched.
+```
+
+Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
+
+```python
+from pathmatcher import main as pm
+
+# Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
+# You can use the commandline arguments, but the script will be called without bash but directly inside Python
+my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
+
+print(my_results)
+```
+
+A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
+
+### Similar projects
+
+A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
+
+## Auxiliary tool: Reorientation and registration helper
+
+### Description
+
+A companion to help you reorient and coregister manually your structural and functional MRI in SPM, without having to click to select files.
+
+This helper script will scan all images in the specified input path, and will accompagny you step-by-step to do the reorientation and coregistration correctly.
+
+This script requires SPM12 (and MATLAB), and runs only on Windows (because of the matlab wrapper limitations).
+
+This script follows the following steps:
+
+1. Automatic reorientation of structural MRI using [spm_auto_reorient.m](https://github.com/lrq3000/spm_auto_reorient) (please install this script along with SPM12 beforehand).
+2. Check reorient and adjust manually.
+3. Side-by-side check of multiple subjects' structural MRI.
+4. Detection of functional images (just walk through all folders to build a list of functional images and pair them to their respective structural images given the input regexp).
+5. Automatic co-registration of functional images onto structural.
+6. Manual co-registration of functional images with structural.
+7. Extraction of framewise displacement motion metrics from functional images.
+
+This script will not only guide you through these steps, in the correct order, but it will also automatically load the files for you (no chance of doing a mistake or missing a subject), while showing you a progress bar (showing how many subjects are remaining and with a time estimate to finish).
+
+There is a CLI user interface: you can skip steps you already done or don't want to do, skip patients, or reload another image (for step 4, to check other functional images).
+
+Note that the last step, extraction of framewise displacement motion metrics from functional images, can be done without requiring matlab nor a matlab wrapper (and hence should work on any platform), by using the `--motiononly` and `--regex_motion` switches (this will directly look for the `rp_*.txt` files that you previously generated with `spm_realign`).
+
+### Usage
+
+```
+usage: reorientation_registration_helper [-h] -i /some/path [-ra "reg_expr+/anat\.(img|nii)"]
+                                                 [-rf "reg_expr+/func\.(img|nii)"] [-rp "reg_expr+/rp_.+\.txt"] [-m]
+                                                 [-v]
+
+Reorientation and registration helper v1.7.4
+Description: Guide and automate the file selection process that is required in SPM between each reorientation/registration.
+
+No more useless clicks, just do the reorientation/registration in batch, you don't need to worry about selecting the corresponding files, this helper will do it for you.
+
+If you have tqdm installed, a nice progress bar will tell you how many subjects are remaining to be processed and how much time will it take at your current pace.
+
+Note: you need to `pip install mlab` before using this script.
+Note2: you need to have set both spm and spm_auto_reorient in your path in MATLAB before using this script.
+Note3: you need the pathmatcher.py library (see lrq3000 github).
+
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i /some/path, --input /some/path
+                        Path to the input folder (the root directory where you placed the files, the default supported tree structure being: "Condition/subject_id/data/(sess_id)?/(mprage|rest)/*.(img|nii)". You can also use --regex_anat and --regex_func to define your own directory layout.
+  -ra "(reg_expr)+/anat\.(img|nii)", --regex_anat "(reg_expr)+/anat\.(img|nii)"
+                        Regular expression to match anatomical images (default: Liege CRC scheme). Use regex groups to match with functional regex (if you want to do step 4 - manual coreg). Note: should target nii or img, not hdr.
+  -rf "(reg_expr)+/func\.(img|nii)", --regex_func "(reg_expr)+/func\.(img|nii)"
+                        Regular expression to match functional images (default: Liege CRC scheme). Regex groups will be matched with the anatomical regex, so you should provide the same groups for both regex. Note: should target nii or img, not hdr (using non-capturing group, eg: ".*\.(?:img|nii)". If a named group (?P<func>...) is specified, this will allow to separately coregister any file matching this group, which will be removed from the list of regex groups (thus this group is additional, it does not count in the "same number of groups" rule).
+  -rp "(reg_expr)+/rp_.+\.txt", --regex_motion "(reg_expr)+/rp_.+\.txt"
+                        Regular expression to match motion parameter files rp_*.txt as generated by spm_realign. If this argument is provided, motion parameters will be fetched from these files directly instead of recalculating from functional images. The regex needs to contain at least one group in parentheses to define a key for the output excel file.
+  -m, --motiononly      If true, and if --regex_motion is specified, then only this step will be done, using the already generated rpfiles.
+  -v, --verbose         Verbose mode (show more output).
+
+```
+
+### Libraries
+
+#### Required
+
+* argparse
+* pathmatcher
+* mlabwrap aka matlap_wrapper ([Python2](https://github.com/mrkrd/matlab_wrapper) version, [Python3](https://github.com/deeuu/matlab_wrapper/tree/python3) version as provided with this module)
+* pypiwin32 (for mlabwrap)
+* pip install --ignore-installed pywin32
+    * then execute `python Scripts\pywin32_postinstall.py -install` in an admin command prompt, see [this explanation](https://stackoverflow.com/questions/58612306/how-to-fix-importerror-dll-load-failed-while-importing-win32api#comment103561767_58613735).
+
+#### Optional
+
+* scandir, to scan files faster
+* tqdm, to show the progress bar
+* numpy >= 1.18.1, for the optional last step to generate motion metrics from functional images
```

