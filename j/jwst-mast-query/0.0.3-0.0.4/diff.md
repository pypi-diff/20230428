# Comparing `tmp/jwst_mast_query-0.0.3.tar.gz` & `tmp/jwst_mast_query-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwst_mast_query-0.0.3.tar", last modified: Fri Apr 21 17:08:19 2023, max compression
+gzip compressed data, was "jwst_mast_query-0.0.4.tar", last modified: Fri Apr 28 16:04:01 2023, max compression
```

## Comparing `jwst_mast_query-0.0.3.tar` & `jwst_mast_query-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.301061 jwst_mast_query-0.0.3/
--rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.3/.gitignore
--rw-r--r--   0 hilbert   (3978) staff       (20)     1822 2023-04-21 16:52:11.000000 jwst_mast_query-0.0.3/CHANGES.rst
--rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/LICENSE.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-04-21 17:08:19.300738 jwst_mast_query-0.0.3/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)    39611 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.3/README.md
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.295932 jwst_mast_query-0.0.3/jwst_mast_query/
--rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.3/jwst_mast_query/__init__.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8183 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_download.py
--rw-r--r--   0 hilbert   (3978) staff       (20)     8205 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    91453 2023-04-21 16:44:21.000000 jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.3/jwst_mast_query/pdastro.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.299015 jwst_mast_query-0.0.3/jwst_mast_query/scripts/
--rw-r--r--   0 hilbert   (3978) staff       (20)     1765 2023-04-04 21:08:28.000000 jwst_mast_query-0.0.3/jwst_mast_query/scripts/jwst_download.py
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.3/jwst_mast_query/sortable.js
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.299762 jwst_mast_query-0.0.3/jwst_mast_query/utils/
--rw-r--r--   0 hilbert   (3978) staff       (20)     3885 2023-04-17 16:28:47.000000 jwst_mast_query-0.0.3/jwst_mast_query/utils/constants.py
-drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-21 17:08:19.298637 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/
--rw-r--r--   0 hilbert   (3978) staff       (20)      848 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/PKG-INFO
--rw-r--r--   0 hilbert   (3978) staff       (20)      534 2023-04-21 17:08:19.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/SOURCES.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/dependency_links.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)      184 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/requires.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-04-21 17:08:18.000000 jwst_mast_query-0.0.3/jwst_mast_query.egg-info/top_level.txt
--rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.3/pyproject.toml
--rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-04-21 17:08:19.301226 jwst_mast_query-0.0.3/setup.cfg
--rwxr-xr-x   0 hilbert   (3978) staff       (20)     2828 2023-03-23 16:57:21.000000 jwst_mast_query-0.0.3/setup.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.410217 jwst_mast_query-0.0.4/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     2366 2022-03-04 20:55:11.000000 jwst_mast_query-0.0.4/.gitignore
+-rw-r--r--   0 hilbert   (3978) staff       (20)     2194 2023-04-28 15:55:05.000000 jwst_mast_query-0.0.4/CHANGES.rst
+-rw-r--r--   0 hilbert   (3978) staff       (20)     4528 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1553 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/LICENSE.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-04-28 16:04:01.409863 jwst_mast_query-0.0.4/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)    39611 2023-04-14 18:08:15.000000 jwst_mast_query-0.0.4/README.md
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.406109 jwst_mast_query-0.0.4/jwst_mast_query/
+-rw-r--r--   0 hilbert   (3978) staff       (20)       89 2022-02-16 16:07:13.000000 jwst_mast_query-0.0.4/jwst_mast_query/__init__.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8344 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_download.py
+-rw-r--r--   0 hilbert   (3978) staff       (20)     8471 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    91265 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)    59698 2023-03-24 17:47:19.000000 jwst_mast_query-0.0.4/jwst_mast_query/pdastro.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.408810 jwst_mast_query-0.0.4/jwst_mast_query/scripts/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     1793 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/scripts/jwst_download.py
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     8605 2023-03-10 17:35:18.000000 jwst_mast_query-0.0.4/jwst_mast_query/sortable.js
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.409289 jwst_mast_query-0.0.4/jwst_mast_query/utils/
+-rw-r--r--   0 hilbert   (3978) staff       (20)     3917 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/jwst_mast_query/utils/constants.py
+drwxr-xr-x   0 hilbert   (3978) staff       (20)        0 2023-04-28 16:04:01.408375 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/
+-rw-r--r--   0 hilbert   (3978) staff       (20)      812 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/PKG-INFO
+-rw-r--r--   0 hilbert   (3978) staff       (20)      534 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/SOURCES.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)        1 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/dependency_links.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)      191 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/requires.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       16 2023-04-28 16:04:01.000000 jwst_mast_query-0.0.4/jwst_mast_query.egg-info/top_level.txt
+-rw-r--r--   0 hilbert   (3978) staff       (20)       98 2021-10-12 14:30:09.000000 jwst_mast_query-0.0.4/pyproject.toml
+-rw-r--r--   0 hilbert   (3978) staff       (20)       38 2023-04-28 16:04:01.410340 jwst_mast_query-0.0.4/setup.cfg
+-rwxr-xr-x   0 hilbert   (3978) staff       (20)     2846 2023-04-28 15:49:10.000000 jwst_mast_query-0.0.4/setup.py
```

### Comparing `jwst_mast_query-0.0.3/.gitignore` & `jwst_mast_query-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/CHANGES.rst` & `jwst_mast_query-0.0.4/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+0.0.4
+=====
+
+Config File
+-----------
+
+Fix a bug that was causing parameters with default values other than None or [] to be set back to the default value after adjusting parameter values based on the contents of the config file. (#51)
+
+Environment
+-----------
+
+Add pillow as a dependency in setup.py, so that it is downloaded upon installation of jwst_mast_query. (#49)
+
+
 0.0.3
 =====
 
 Config File
 -----------
 
 Fix a bug that was preventing the date_select values in the cfg file from being used. (#39)
```

### Comparing `jwst_mast_query-0.0.3/CODE_OF_CONDUCT.md` & `jwst_mast_query-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/LICENSE.txt` & `jwst_mast_query-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/PKG-INFO` & `jwst_mast_query-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: jwst_mast_query
-Version: 0.0.3
+Version: 0.0.4
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
-License: UNKNOWN
 Keywords: astronomy
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Query MAST for JWST observations, select certain types of these products, provide a summary of these observations and products, and optionally download the selected products
-
```

### Comparing `jwst_mast_query-0.0.3/README.md` & `jwst_mast_query-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/jwst_download.py` & `jwst_mast_query-0.0.4/jwst_mast_query/jwst_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import astroquery
 import os,sys,shutil,re
 #import yaml
 from astropy.utils.data import download_file
 
 from jwst_mast_query.jwst_query import query_mast
 from jwst_mast_query.pdastro import makepath4file,AnotB
+from jwst_mast_query.utils.constants import PARAM_DEFAULTS
 #from pdastro import makepath4file,AnotB
 
 
 # MAST API documentation:
 # https://mast.stsci.edu/api/v0/pyex.html
 
 # MAST CAOM Field Descriptions:
@@ -58,18 +59,20 @@
         # options for output directory file
         #if 'JWSTDOWNLOAD_OUTDIR' in os.environ and os.environ['JWSTDOWNLOAD_OUTDIR'] != '':
         #    outrootdir = os.environ['JWSTDOWNLOAD_OUTDIR']
         #else:
         #    outrootdir = '.'
         #print('Default output rootdir: %s' % outrootdir)
 
-        parser.add_argument('-n','--skipdownload', action='store_true', default=False, help='skip downloading the data.  (default=%(default)s)')
+        parser.add_argument('-n','--skipdownload', action='store_true', default=PARAM_DEFAULTS['skipdownload'],
+                            help='skip downloading the data.  (default=%(default)s)')
 #        parser.add_argument('-o','--outrootdir', default=outrootdir, help=('output root directory. (default=%(default)s)'))
 #        parser.add_argument('--outsubdir', default=None, help=('subdir added to the output root directory. If None, then propID is used (default=%(default)s)'))
-        parser.add_argument('--clobber', action='store_true', default=None, help='existing files are overwritten, otherwise they are skipped (default=%(default)s)')
+        parser.add_argument('--clobber', action='store_true', default=PARAM_DEFAULTS['clobber'],
+                            help='existing files are overwritten, otherwise they are skipped (default=%(default)s)')
 
         return(parser)
 
     def download_product(self, url, outfilename, clobber=False):
         """
         Download the product url and save it to outfilename.
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.cfg` & `jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,21 @@
 date_select:
 
 # save the tables (selected products, obsTable, summary with suffix selprod.txt, obs.txt, summary.txt, respectively) with the
 # specified string as basename. Tables will be saved in outrootdir.
 # If left empty, the tables will not be saved.
 savetables:
 
+# If clobber is True, all files will be downloaded. If false, only files that do not already exist in the
+# local directory will be downloaded.
+clobber: False
+
+# If True, the data will not be downloaded. Only the summary tables will be produced
+skipdownload: False
+
 # columns returned from MAST to the obsTable
 # The default set in the code is mastcolumns_obsTable=['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime']
 mastcolumns_obsTable: ['proposal_id','dataURL','obsid','obs_id','t_min','t_exptime','instrument_name']
 
 # output columns for the tables. Note that the columns for the individual filetypes
 # are automatically added to the obsTable.
 # The defaults set in the code are:
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/jwst_query.py` & `jwst_mast_query-0.0.4/jwst_mast_query/jwst_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,14 @@
                                                                                                                             'already exist (default=%(default)s)'))
         parser.add_argument('--webpage_thumbnails_width', default=PARAM_DEFAULTS['webpage_thumbnails_width'], help=('Width in pixels of the resized jpg images '
                                                                                                                     'to be inserted into the index.html summary '
                                                                                                                     'file. (default=%(default)s)'))
         parser.add_argument('--webpage_thumbnails_height', default=PARAM_DEFAULTS['webpage_thumbnails_height'], help=('Height in pixels of the resized jpg images '
                                                                                                                       'to be inserted into the index.html summary '
                                                                                                                       'file. (default=%(default)s)'))
-        parser.add_argument('--skipdownload', action='store_true', default=PARAM_DEFAULTS['skipdownload'], help='If set, no files will be downloaded. (default=%(default)s)')
-
         return(parser)
 
     def get_arguments(self, args, configfile=None):
         '''
 
         Parameters
         ----------
@@ -427,15 +425,15 @@
             print('\n### OPTIONAL COMMAND LINE PARAMETERS:')
         argsdict = vars(args)
         for arg in argsdict:
 
             # skip config file
             if arg=='configfile': continue
 
-            if argsdict[arg] is not None and argsdict[arg] != []:
+            if argsdict[arg] != PARAM_DEFAULTS[arg]:
                 if args.verbose>2:
                     print('optional args: setting %s to %s' % (arg,argsdict[arg]))
                 self.params[arg]=argsdict[arg]
             else:
                 if arg not in  self.params:
                     self.params[arg]=None
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/pdastro.py` & `jwst_mast_query-0.0.4/jwst_mast_query/pdastro.py`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/scripts/jwst_download.py` & `jwst_mast_query-0.0.4/jwst_mast_query/scripts/jwst_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     download.set_outrootdir()
     if download.verbose: print(f'Outdir: {download.outrootdir}')
 
     # Make the tables, but don't show them yet, since the output files need to be updated first
     if download.mk_all_tables(showtables=True):
         sys.exit(0)
 
-    if not args.skipdownload and len(download.ix_selected_products)>0:
+    if not download.params['skipdownload'] and len(download.ix_selected_products)>0:
         download.download_products()
         print('\n######################\n### Downloaded Selected Products:\n######################')
         download.productTable.write(indices=download.ix_selected_products,columns=download.params['outcolumns_productTable'])
     else:
         if len(download.ix_selected_products)<=0:
             print('############## Nothing selected!!!! exiting...')
             sys.exit(0)
 
     # Make the webpages
-    if args.makewebpages:
+    if download.params['makewebpages']:
         download.mk_webpages4propIDs()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/sortable.js` & `jwst_mast_query-0.0.4/jwst_mast_query/sortable.js`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query/utils/constants.py` & `jwst_mast_query-0.0.4/jwst_mast_query/utils/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,34 +26,35 @@
                   'outcolumns_productTable': ['proposal_id','obsnum','obsID','parent_obsid','obs_id','sca','visit','dataproduct_type','productFilename','filetype','calib_level','size','description'],
                   'outcolumns_obsTable': ['proposal_id','obsnum','obsid','obs_id','t_min','t_exptime','date_min','instrument_name'],
                   'sortcols_productTable': ['calib_level','filetype','obsID'],
                   'sortcols_obsTable': ['date_min','proposal_id','obsnum'],
                   'sortcols_summaryTable': ['date_start','proposal_id','obsnum'],
                   'configfile': cfgfilename,
                   'token': defaulttoken,
-                  'instrument': 'nircam',
+                  'instrument': None,
                   'obsmode': None,
                   'propID': None,
                   'obsnums': None,
                   'obsid_select': [],
                   'obsid_list': [],
                   'sca': None,
                   'verbose': 0,
-                  'filetypes': ['uncal'],
+                  'filetypes': ['fits'],
                   'guidestars': False,
-                  'lookbacktime': 1,
+                  'lookbacktime': 1.,
                   'calib_levels': None,
                   'Nobs_per_batch': 2,
                   'obsnum2outsubdir': None,
                   'propIDs_obsnum2outsubdir': [],
                   'date_select': [],
                   'savetables': None,
                   'makewebpages': False,
                   'outrootdir': None,
                   'outsubdir': None,
+                  'clobber': False,
                   'skip_propID2outsubdir': False,
                   'skip_check_if_outfile_exists': False,
                   'skip_check_filesize': False,
                   'jpg_separate_subdir': False,
                   'webpage_tablefigsize_width': None,
                   'webpage_tablefigsize_height': None,
                   'webpage_level12_jpgs': ['_uncal.jpg', '_dark.jpg', '_rate.jpg', '_rateints.jpg', '_trapsfilled.jpg', '_cal.jpg', '_crf.jpg'],
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query.egg-info/PKG-INFO` & `jwst_mast_query-0.0.4/jwst_mast_query.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: jwst-mast-query
-Version: 0.0.3
+Version: 0.0.4
 Summary: Query MAST for JWST products, and download them
 Home-page: https://github.com/spacetelescope/jwst_mast_query
 Author: STScI (Rest)
 Author-email: arest@stsci.edu
-License: UNKNOWN
 Keywords: astronomy
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Query MAST for JWST observations, select certain types of these products, provide a summary of these observations and products, and optionally download the selected products
-
```

### Comparing `jwst_mast_query-0.0.3/jwst_mast_query.egg-info/SOURCES.txt` & `jwst_mast_query-0.0.4/jwst_mast_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jwst_mast_query-0.0.3/setup.py` & `jwst_mast_query-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         'astropy',
         'ipython',
         'jinja2',
         'numpy',
         'pandas',
         'pyyaml',
         'scipy',
-        'argparse'
+        'argparse',
+        'pillow'
     ],
     scripts=['jwst_mast_query/scripts/jwst_download.py'],
     include_package_data=True,
     extras_require={
         'docs': DOCS_REQUIRE,
         'test': TESTS_REQUIRE,
     },
```

