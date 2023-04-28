# Comparing `tmp/pdb4all-0.4.9.tar.gz` & `tmp/pdb4all-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb4all-0.4.9.tar", last modified: Mon Jun 21 12:47:07 2021, max compression
+gzip compressed data, was "pdb4all-0.5.1.tar", last modified: Thu Apr 27 16:30:40 2023, max compression
```

## Comparing `pdb4all-0.4.9.tar` & `pdb4all-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 12:47:07.420415 pdb4all-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-06-21 12:46:58.000000 pdb4all-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-06-21 12:47:07.420415 pdb4all-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-06-21 12:46:58.000000 pdb4all-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 12:47:07.416415 pdb4all-0.4.9/pdb4all/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2021-06-21 12:46:58.000000 pdb4all-0.4.9/pdb4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-06-21 12:46:58.000000 pdb4all-0.4.9/pdb4all/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9791 2021-06-21 12:46:58.000000 pdb4all-0.4.9/pdb4all/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    40290 2021-06-21 12:46:58.000000 pdb4all-0.4.9/pdb4all/pdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    13693 2021-06-21 12:46:58.000000 pdb4all-0.4.9/pdb4all/rosetta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 12:47:07.420415 pdb4all-0.4.9/pdb4all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-06-21 12:47:07.000000 pdb4all-0.4.9/pdb4all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-06-21 12:47:07.000000 pdb4all-0.4.9/pdb4all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-21 12:47:07.000000 pdb4all-0.4.9/pdb4all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-06-21 12:47:07.000000 pdb4all-0.4.9/pdb4all.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-21 12:47:07.000000 pdb4all-0.4.9/pdb4all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-21 12:47:07.420415 pdb4all-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2021-06-21 12:46:58.000000 pdb4all-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:30:40.039011 pdb4all-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 16:30:23.000000 pdb4all-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 16:30:40.039011 pdb4all-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-27 16:30:23.000000 pdb4all-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:30:40.035011 pdb4all-0.5.1/pdb4all/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54732 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/rosetta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-27 16:30:23.000000 pdb4all-0.5.1/pdb4all/traj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:30:40.039011 pdb4all-0.5.1/pdb4all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 16:30:39.000000 pdb4all-0.5.1/pdb4all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 16:30:40.000000 pdb4all-0.5.1/pdb4all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:30:39.000000 pdb4all-0.5.1/pdb4all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 16:30:39.000000 pdb4all-0.5.1/pdb4all.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 16:30:39.000000 pdb4all-0.5.1/pdb4all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:30:40.039011 pdb4all-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-27 16:30:23.000000 pdb4all-0.5.1/setup.py
```

### Comparing `pdb4all-0.4.9/LICENSE` & `pdb4all-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb4all-0.4.9/PKG-INFO` & `pdb4all-0.5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: pdb4all
-Version: 0.4.9
+Version: 0.5.1
 Summary: Convert between common protein pdb formats and names 
 Home-page: https://github.com/boneta/pdb4all
 Author: Sergio Boneta
 Author-email: boneta@unizar.es
 License: GPLv3
-Description: # pdb4all
-        *Convert between common protein pdb formats and names*
-        
-        ### Installation
-        Requires `python 3.7+`. No additional dependencies are needed. \
-        It should work on 2.7+ but no warranty is provided.
-        
-        *pdb4all* is frequently uploaded to [PyPI](https://pypi.org/project/pdb4all/). To install it, execute the following command:
-        ```
-          pip install pdb4all
-        ```
-        
-        ### Usage
-        ```
-          pdb4all <options> .pdb
-        ```
-        
-        #### Currently supported ForceFields name conventions
-          * Amber
-          * Charmm
-          * OPLS
-        
-        #### Currently supported formats (software)
-          * Fasta
-          * Maestro
-          * GROMACS
-          * fDynamo
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pdb4all
+
+![python](https://img.shields.io/badge/python-3.7+-red.svg)
+[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+*Convert between common protein pdb formats and names*
+
+### Installation
+Requires `python 3.7+`. No additional dependencies are needed.
+
+*pdb4all* is frequently uploaded to [PyPI](https://pypi.org/project/pdb4all/). To install it, execute the following command:
+```
+  pip install pdb4all
+```
+
+### Usage
+```
+  pdb4all <options> .pdb
+```
+
+#### Currently supported ForceFields name conventions
+  * Amber
+  * Charmm
+  * OPLS
+
+#### Currently supported formats (software)
+  * Fasta
+  * Maestro
+  * GROMACS
+  * fDynamo
```

### Comparing `pdb4all-0.4.9/README.md` & `pdb4all-0.5.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # pdb4all
+
+![python](https://img.shields.io/badge/python-3.7+-red.svg)
+[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
 *Convert between common protein pdb formats and names*
 
 ### Installation
-Requires `python 3.7+`. No additional dependencies are needed. \
-It should work on 2.7+ but no warranty is provided.
+Requires `python 3.7+`. No additional dependencies are needed.
 
 *pdb4all* is frequently uploaded to [PyPI](https://pypi.org/project/pdb4all/). To install it, execute the following command:
 ```
   pip install pdb4all
 ```
 
 ### Usage
```

### Comparing `pdb4all-0.4.9/pdb4all/__init__.py` & `pdb4all-0.5.1/pdb4all/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #######################################################################
 ##                                                                   ##
 ##                              pdb4all                              ##
 ##                                                                   ##
 #######################################################################
 #
 #
-# Copyright (C) 2021, Sergio Boneta
+# Copyright (C) 2022, Sergio Boneta
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -33,10 +33,11 @@
   =======
 
   Protein conversion between common pdb formats and name conventions
 
 
 """
 
-__version__ = '0.4.9'
+__version__ = '0.5.1'
 
 from pdb4all.pdb import *
+from pdb4all.traj import *
```

### Comparing `pdb4all-0.4.9/pdb4all/__main__.py` & `pdb4all-0.5.1/pdb4all/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import os
 import sys
 import argparse
 
 from pdb4all import __version__
-from pdb4all.pdb import PDB, standard_preparation
+from pdb4all.pdb import PDB
 
 
 ##  PARSER  ###########################################################
 ## OpenBabel inspired
 
 def __parserbuilder():
     # supported formats
@@ -38,25 +38,27 @@
                         action='version',
                         version='pdb4all  v{}\nby Sergio Boneta / GPL'.format(__version__))
     parser.add_argument('I',
                         metavar='.pdb',
                         type=str,
                         help='input pdb file')
     parser.add_argument('-i',
-                        required=True,
+                        required=False,
                         metavar='<format>',
                         type=str,
                         choices=input_formats,
-                        help='input pdb format (software)')
+                        default='maestro',
+                        help='input pdb format (def: maestro)')
     parser.add_argument('-o',
-                        required=True,
+                        required=False,
                         metavar='<format>',
                         type=str,
                         choices=output_formats,
-                        help='output pdb format (software)')
+                        default='gmx',
+                        help='output pdb format (def: gmx)')
     parser.add_argument('-O',
                         metavar='.pdb',
                         type=str,
                         help='output pdb file')
     parser.add_argument('-iff',
                         metavar='ff',
                         type=str,
@@ -65,14 +67,17 @@
                         help='input Force Field format (def: amber)')
     parser.add_argument('-off',
                         metavar='ff',
                         type=str,
                         choices=ff_formats,
                         default='amber',
                         help='output Force Field format (def: amber)')
+    parser.add_argument('--extract-ligands',
+                        action='store_true',
+                        help='extract ligands to independent .pdb files')
     parser.add_argument('--dynamize',
                         action='store_true',
                         help='extra fDynamo files (.crd, seq, lig_opls)')
     parser.add_argument('--center',
                         action='store_true',
                         help='move system to center (0,0,0)')
     parser.add_argument('--simple',
@@ -87,19 +92,19 @@
 def main():
     # parser
     parser = __parserbuilder()
     args = parser.parse_args()
 
     # names of files
     infile    = args.I
-    basein    = os.path.splitext(infile)[0]
     inpformat = args.i
     outformat = args.o
     inpff     = args.iff
     outff     = args.off
+    basein, extin = os.path.splitext(infile)
     if args.O is not None:
         outfile = args.O
         baseout = os.path.splitext(outfile)[0]
     else:
         if outformat == 'fasta':
             baseout = basein
             outfile = baseout + ".fasta"
@@ -108,46 +113,52 @@
             outfile = baseout + ".resid"
         else:
             baseout = basein + "_" + outformat
             outfile = baseout + ".pdb"
 
     # read crd or pdb
     my_pdb = PDB()
-    if infile.split('.')[-1] == 'crd':
-        my_pdb.read_crd(infile)
-    else:
-        my_pdb.read(infile, strict=args.simple)
+    my_pdb.read(infile, strict=args.simple)
 
     # main selection
     if outformat == 'fasta':
         my_pdb.write_fasta(outfile, gaps=False)
     elif outformat == 'intseq':
         my_pdb.write_intseq(outfile)
     else:
         if outformat == 'gmx':
             my_pdb.substitute('name', 'HXT', 'OXT')
-            standard_preparation(my_pdb, inpformat, outformat, outff)
+            my_pdb.standard_preparation(inpformat, outformat, outff)
             my_pdb.guess_protonres()
-            if args.center: my_pdb.center(guess_elements=False, center=[0., 0., 0.], monoisotopic=False)
-            my_pdb.write(outfile, title=True, remark4=True, renum_atoms=True, onlyProtein=True)
+            if args.center:
+                my_pdb.center(guess_elements=False, center=[0., 0., 0.], monoisotopic=False)
+            my_pdb.write(outfile, title=True, remark4=True, renum_atoms=True, onlyProtein=args.extract_ligands)
+            if args.extract_ligands:
+                for ligand in my_pdb.ligands:
+                    my_ligand = PDB()
+                    my_ligand.pdb = [my_pdb.pdb[n] for n in my_pdb.findall(resName=ligand)]
+                    my_ligand.clean_field('ATOM', 'HETATM')
+                    my_ligand.write('lig_' + ligand + '.pdb', remark4=False, renum_atoms=True)
 
         elif outformat == 'dynamo':
-            standard_preparation(my_pdb, inpformat, outformat, outff)
+            my_pdb.standard_preparation(inpformat, outformat, outff)
             my_pdb.cys2cyx()
             my_pdb.substitute('name', 'OC1', 'O')
             my_pdb.substitute('name', 'OC2', 'OXT')
             my_pdb.substitute('resName', 'NA', 'SOD')
             my_pdb.guess_his()
-            my_pdb.renum_res(continuous=False, protectProtein=False, guess_segments=True)
+            my_pdb.guess_segments(keepknown=True, useChains=True)
+            my_pdb.renum_res(continuous=False, protectProtein=False, guess_segments=False)
             my_pdb.renum_atoms()
-            if args.center: my_pdb.center(guess_elements=False, center=[0., 0., 0.], monoisotopic=False)
+            if args.center:
+                my_pdb.center(guess_elements=False, center=[0., 0., 0.], monoisotopic=False)
             if args.dynamize:
                 my_pdb.write_crd(baseout + '.crd')
                 my_pdb.write_seq(baseout + '.seq', variants=True, ssbonds=True)
-                for ligand in my_pdb.ligands: my_pdb.write_ligand(ligand)
+                my_pdb.write_ff_ligands()
             for n in ['occupancy', 'tempFactor', 'element', 'charge', 'chainID']: my_pdb.clean_field(n)
             my_pdb.write(outfile, title=True, remark4=True, renum_atoms=True, onlyProtein=False)
 
     sys.stderr.write("{:s} --> {:s} \n".format(infile, outfile))
 
 
 if __name__ == "__main__":
```

### Comparing `pdb4all-0.4.9/pdb4all/constants.py` & `pdb4all-0.5.1/pdb4all/constants.py`

 * *Files identical despite different names*

### Comparing `pdb4all-0.4.9/pdb4all/pdb.py` & `pdb4all-0.5.1/pdb4all/pdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,44 +3,69 @@
   Main PDB class
 =======================================================================
 
   Classes
   -------
     pdb
 
-  Functions
-  ---------
-    standard_preparation
-
 """
 
 import math as m
+import os
+import tempfile
 from copy import deepcopy
+from inspect import getfullargspec
+from urllib.request import urlopen
 
 from pdb4all.constants import *
 from pdb4all.rosetta import *
 
 
 # PDB Strict formatting
 # ATOM/HETATM  serial  name   altLoc  resName  chainID  resSeq  iCode  x       y     z      occupancy  tempFactor  segment  element  charge
 # 1-6          7-11    13-16  17      18-20    22       23-26   27     31-38  39-46  47-54  55-60      61-66       73-76    77-78    79-80
 
 # PDB Column formatting (simple)
 # ATOM/HETATM  #Atom  Atom  Res  [Chain]  #Res  X  Y  Z  Occup  TempFac  [Segment]
 
+# GRO Strict formatting
+# resSeq  resName  name   serial  x      y      z
+# 1-5     6-10     11-15  16-20   21-28  29-36  37-44
+
 
 ##  Main PDB class  ###################################################
 class PDB:
     '''
         Main PDB class
 
         Attributes
         ----------
         title : str
+        atom_empty : dict
+            dictoriary with empty atom properties
         pdb : list of dic
+            a list of atoms in order, each being a dictionary
+            of properties with defined types:
+                'ATOM'       : str
+                'serial'     : int
+                'name'       : str
+                'altLoc'     : str
+                'resName'    : str
+                'chainID'    : str
+                'resSeq'     : int
+                'iCode'      : str
+                'x'          : float
+                'y'          : float
+                'z'          : float
+                'occupancy'  : float
+                'tempFactor' : float
+                'segment'    : str
+                'element'    : str
+                'charge'     : str
+
 
         Properties
         ----------
         natoms : int
             number of atoms
         nres : int
             number of protein residues
@@ -61,22 +86,36 @@
         protein_weight : float
             molecular average protein weight (Da)
 
         Methods
         -------
         __init__(file)
             initalization and optional pdb read
-        read(file,strict)
+        read(file, format)
+            wrapper to read files based on extension/format
+        read_pdb(file,strict)
             read pdb from file
+        read_pqr(file)
+            read APBS' pqr files
+        read_gro(file)
+            read GROMACS' gro from file
         read_crd(file)
             read dynamo's crd from file
         read_xyz(file)
             read XYZ from file
-        write(file,title,remark4,renum_atoms,onlyProtein,notProtein)
+        fetch(id)
+            fetch PDB and dowload it from RCSB
+        write(file, format)
+            wrapper to write files based on extension/format
+        write_pdb(file,title,remark4,renum_atoms,onlyProtein,notProtein)
             write pdb to file
+        write_pqr(file, renum_atoms)
+            write APBS' pqr to file
+        write_gro(file, renum_atoms)
+            write GROMACS' gro to file
         write_fasta(file,gaps)
             write fasta to file
         write_xyz(file)
             write XYZ to file
         write_intseq(file)
             write sequence in fDynamo's interaction format to file
         write_crd(file)
@@ -85,37 +124,47 @@
             write fDynamo's seq to file
         write_ligand(ligand)
             write fDynamo's topology of ligand to file
         substitute(field,origin,destination,protectProtein,onlyProtein)
             change matching values of field
         clean_field(field,value)
             change all values of field to zero/empty/value
-        findall(**field_and_values)
-            find a list of atom index that match all fields
-        remove(field,value)
-            remove atoms that match field
+        findall(match_all,**fields_and_values)
+            find a list of atom index that match all/any fields
+        remove(match_all,**fields_and_values)
+            remove all atoms that match all/any fields
+        remove_ligands()
+            remove all ligands
+        remove_waters()
+            remove all waters
+        keep_only(match_all,**fields_and_values)
+            keep only atoms that match all/any fields
         all2ATOM()
             change all ATOM/HETATM to ATOM
         translate_residues(destination,origin)
             translate resName between standards
         translate_names(destination,origin)
             translate atom names between standards
         canonical_order(canon)
             reorder protein atoms inside residues
-        renum_atoms()
-            renumerate all atoms from 1
-        renum_res(continuous,protectProtein,guess_segments)
-            renumerate residues, each group from 1: protein/ligands/solvent/ions
+        order_by_atom(keepnames, protectProtein)
+            reorder atoms by element(reversed Periodic Table) in each residue and change their names in order
+        renum_atoms(start)
+            renumber all atoms from 'start' (def: 1)
+        renum_res(start,continuous,protectProtein,guess_segments)
+            renumber residues, each group from 'start' (def: 1): protein/ligands/solvent/ions
         guess_elements(keepknown)
             guess elements of all atoms
         guess_segments(keepknown,useChains)
             guess segments, one for each group: protein/ligands/solvent/ions
         weight(guess_elements,onlyProtein,monoisotopic)
             molecular weight (Da)
-        center(guess_elements,center,monoisotopic)
+        com(geometric,guess_elements,monoisotopic):
+            calculate center of mass
+        center(center,geometric,guess_elements,monoisotopic)
             move system's COM to center
         cys2cyx()
             change resName of CYS to CYX if corresponds
         guess_his()
             change HIS to corresponding HID/HIE/HIP
         guess_glh()
             change GLU to GLH if corresponds
@@ -123,14 +172,17 @@
             change ASP to ASH if corresponds
         guess_lyn()
             change LYS to LYN if corresponds
         guess_protonres()
             change resName based on protonation for HIS/GLU/ASP/LYS
             shortcut to call guess_his()/guess_glh()/guess_ash()/guess_lyn()
 
+        standard_preparation()
+            standard protein preparation
+
         Static Methods
         --------------
         pymol_sele_macro(atom_dict)
             build a PyMOL's selection macro notation for an atom
     '''
 
     atom_empty = {
@@ -141,34 +193,86 @@
         'resName'    : "",
         'chainID'    : "",
         'resSeq'     : 0,
         'iCode'      : "",
         'x'          : 0.0,
         'y'          : 0.0,
         'z'          : 0.0,
-        'occupancy'  : 0.0,
+        'occupancy'  : 1.0,
         'tempFactor' : 0.0,
         'segment'    : "",
         'element'    : "",
         'charge'     : ""
         }
 
-    def __init__( self, file=None ):
+    def __init__(self, file=None) -> None:
         '''Class initialization'''
         self.title = ''
         self.pdb = []
         if file is not None:
             self.read(file)
 
-    def __del__( self ):
-        del self.title
-        del self.pdb
+    def __repr__(self) -> str:
+        return '<PDB: {:d} atoms :: {:d} protein residues & {:d} ligands>' \
+            .format(self.natoms, self.nres, len(self.ligands))
+
+    def __bool__(self) -> bool:
+        return bool(self.pdb) or bool(self.title)
+
+    def __len__(self) -> int:
+        return self.natoms
+
+    def deepcopy(self) -> 'PDB':
+        return deepcopy(self)
+
+    ## read -----------------------------------------------------------
+    def read(self, file, format=None, **kargs) -> None:
+        '''
+            Wrapper to read files based on extension/format
+
+            If format is not specified, the extension of the file
+            is used. If the file does not exist but the name looks
+            like a PDB ID, it tries to be fetched.
+
+            Supported formats: pdb, pqr, gro, crd, xyz
+
+        '''
+        reader = {
+            'pdb' : self.read_pdb,
+            'pqr' : self.read_pqr,
+            'gro' : self.read_gro,
+            'crd' : self.read_crd,
+            'xyz' : self.read_xyz
+            }
+        # check if file exists or is a PDB ID
+        if not os.path.exists(file):
+            if len(file) == 4 and file.isalnum():
+                try:
+                    self.fetch(file)
+                    return
+                except:
+                    pass
+            raise FileNotFoundError(f'No such file or directory: {file}')
+        # assign format based on input argument/file extension/default
+        extension = os.path.splitext(file)[1][1:]
+        if format is not None:
+            if format.lower() in reader:
+                format = format.lower()
+            else:
+                raise ValueError('Unknown format to read: {}'.format(format))
+        elif extension.lower() in reader:
+            format = extension.lower()
+        else:
+            format = 'pdb'
+        # read file based on format & pass only arguments expected by function
+        kargs = {k:v for k,v in kargs.items() if k in getfullargspec(reader[format]).args[1:]}
+        reader[format](file, **kargs)
 
     ## read pdb from file ---------------------------------------------
-    def read( self, file, strict=True ):
+    def read_pdb(self, file, strict=True) -> None:
         '''Read PDB file'''
 
         # initialize object (in case of reuse)
         self.__init__()
 
         # open file
         with open( file, 'rt' ) as inp:
@@ -225,16 +329,56 @@
                             'element' : '', 'charge' : '' }
                 # check if segment column present
                 try: newline.update({ 'segment': str(line[10+c]) })
                 except: newline.update({ 'segment' : str('') })
 
             self.pdb.append(newline)
 
+    ## read pqr from file ---------------------------------------------
+    def read_pqr(self, file) -> None:
+        '''Read APBS' pqr files'''
+        self.read_pdb(file, strict=False)
+        for atom in self.pdb:
+            atom['charge'] = atom['occupancy']
+        for field in ['tempFactor', 'segment']:
+            self.clean_field(field)
+
+    ## read gro from file ---------------------------------------------
+    def read_gro(self, file) -> None:
+        '''Read GROMACS' gro from file'''
+
+        # initialize object (in case of reuse)
+        self.__init__()
+
+        # open file
+        with open(file, 'rt') as inp:
+            ingro = inp.readlines()
+            ingro = [line for line in ingro if line.strip()]
+
+        # title
+        self.title = str(ingro.pop(0)).strip()
+        # number of atoms
+        natoms = int(ingro.pop(0))
+
+        # create pdb list of dictionaries
+        for line in ingro[:natoms]:
+            newatom = deepcopy(self.atom_empty)
+            newatom.update({
+                'resSeq': int(line[0:5]),
+                'resName': str(line[5:10]).strip(),
+                'name': str(line[10:15]).strip(),
+                'serial': int(line[15:20]),
+                'x': float(line[20:28])*10.,
+                'y': float(line[28:36])*10.,
+                'z': float(line[36:44])*10.
+                })
+            self.pdb.append(newatom)
+
     ## read crd from file ---------------------------------------------
-    def read_crd( self, file ):
+    def read_crd(self, file) -> None:
         '''Read dynamo's crd from file'''
 
         # initialize object (in case of reuse)
         self.__init__()
 
         # open file
         with open( file, 'rt' ) as inp:
@@ -258,15 +402,15 @@
                 a['element'] = Ptable_inv_n[int(line[2])]
                 a['x']       = float(line[3])
                 a['y']       = float(line[4])
                 a['z']       = float(line[5])
                 self.pdb.append(deepcopy(a))
 
     ## read XYZ from file ---------------------------------------------
-    def read_xyz( self, file ):
+    def read_xyz(self, file) -> None:
         '''Read XYZ from file'''
 
         # initialize object (in case of reuse)
         self.__init__()
 
         # open file
         with open( file, 'rt' ) as inp:
@@ -281,44 +425,126 @@
         a = deepcopy(self.atom_empty)
         for n in range(natoms):
             line = inxyz[n].split()
             a['element'] = str(line.pop(0))
             a['x'], a['y'], a['z'] = map(float, line)
             self.pdb.append(deepcopy(a))
 
+    ## fetch PDB from internet ----------------------------------------
+    def fetch(self, id) -> None:
+        '''Fetch PDB and dowload it from RCSB'''
+        # fetch PDB
+        url = f"https://files.rcsb.org/view/{id}.pdb"
+        pdb_data = urlopen(url).read().decode('utf-8')
+        # write to temporary file and read as PDB
+        with tempfile.NamedTemporaryFile(mode='w', delete=False) as tmp:
+            tmp.write(pdb_data)
+            tmp.flush()
+            self.read_pdb(tmp.name)
+
+    ## write ----------------------------------------------------------
+    def write(self, file, format=None, **kargs) -> None:
+        '''
+            Wrapper to write files based on extension/format
+
+            Supported formats: pdb, pqr, gro, crd, seq, xyz, fasta
+        '''
+        writer = {
+            'pdb' : self.write_pdb,
+            'pqr' : self.write_pqr,
+            'gro' : self.write_gro,
+            'crd' : self.write_crd,
+            'seq' : self.write_seq,
+            'xyz' : self.write_xyz,
+            'fasta' : self.write_fasta
+            }
+        # assign format based on input argument/file extension/default
+        extension = os.path.splitext(file)[1][1:]
+        if format is not None:
+            if format.lower() in writer:
+                format = format.lower()
+            else:
+                raise ValueError('Unknown format to write: {}'.format(format))
+        elif extension.lower() in writer:
+            format = extension.lower()
+        else:
+            format = 'pdb'
+        # write file based on format & pass only arguments expected by function
+        kargs = {k:v for k,v in kargs.items() if k in getfullargspec(writer[format]).args[1:]}
+        writer[format](file, **kargs)
+
     ## write pdb to file ----------------------------------------------
-    def write( self, file, title=False, remark4=False, renum_atoms=True, onlyProtein=False, notProtein=False ):
+    def write_pdb(self, file, title=False, remark4=False, renum_atoms=True, onlyProtein=False, notProtein=False) -> None:
         '''Write PDB file'''
-        # renumerate atoms
         if renum_atoms: self.renum_atoms()
-        # open file
-        with open( file, 'wt' ) as outp:
+        with open(file, 'wt') as outp:
             if remark4: outp.write("REMARK   4      COMPLIES WITH FORMAT V. 3.3, 21-NOV-2012\n")
             if title: outp.write("TITLE     {:70s}\n".format(self.title))
-            for n in range(self.natoms):
-                line = self.pdb[n].copy()
+            for line in deepcopy(self.pdb):
                 # discart if not aminoacid and onlyProtein
                 if onlyProtein and line['resName'] not in aa: continue
                 # discart if aminoacid and notProtein
                 if notProtein and line['resName'] in aa: continue
                 # correct alignment of atom name
                 if len(line['name']) == 3: line['name'] = ' ' + line['name']
+                # correct very high numbers
+                if line['resSeq'] > 9999:
+                    line['resSeq'] -= 10000 * (line['resSeq'] // 10000)
+                if line['serial'] > 99999:
+                    line['serial'] -= 100000 * (line['serial'] // 100000)
                 # format pdb
-                # formatted_line = "{:<6s}{:>5d} {:^4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}      {:<4s}{:>2s}{:<2s}" \
-                # .format( line['ATOM'], line['serial'], line['name'], line['altLoc'], line['resName'], line['chainID'], line['resSeq'], line['iCode'], \
-                # line['x'], line['y'], line['z'], line['occupancy'], line['tempFactor'], line['segment'], line['element'], line['charge'] )
-                formatted_line = "{:<6s}{:>5d} {:^4s}{:1s}{:>3s} {:1s}{:>4.4}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}      {:<4s}{:>2s}{:<2s}" \
-                .format( line['ATOM'], line['serial'], line['name'], line['altLoc'], line['resName'], line['chainID'], str(line['resSeq']), line['iCode'], \
-                line['x'], line['y'], line['z'], line['occupancy'], line['tempFactor'], line['segment'], line['element'], line['charge'] )
+                formatted_line = "{:<6s}{:>5d} {:^4s}{:1s}{:>3s} {:1s}{:>4d}{:1s}   {:>8.3f}{:>8.3f}{:>8.3f}{:>6.2f}{:>6.2f}      {:<4s}{:>2s}{:<2s}" \
+                                 .format(line['ATOM'], line['serial'], \
+                                         line['name'], line['altLoc'], line['resName'], \
+                                         line['chainID'], line['resSeq'], line['iCode'], \
+                                         line['x'], line['y'], line['z'], line['occupancy'], line['tempFactor'], \
+                                         line['segment'], line['element'], line['charge'])
                 # write
                 outp.write( formatted_line + "\n" )
             outp.write("END\n")  # final 'END'
 
+    ## write pqr to file ----------------------------------------------
+    def write_pqr(self, file, renum_atoms=True) -> None:
+        '''Write PQR file'''
+        # https://apbs.readthedocs.io/en/latest/formats/pqr.html
+        # Field_name Atom_number Atom_name Residue_name Chain_ID Residue_number X Y Z Charge Radius
+        if renum_atoms: self.renum_atoms()
+        with open(file, 'wt') as outp:
+            for line in deepcopy(self.pdb):
+                # correct alignment of atom name
+                if len(line['name']) == 3: line['name'] = ' ' + line['name']
+                # format pqr (white-space separated)
+                formatted_line = "{:<6s} {:>4d} {:^4s} {:>3s} {:1s} {:>3d}     {:>7.3f} {:>7.3f} {:>7.3f} {:>5.2f} {:>5.2f}" \
+                                 .format(line['ATOM'], line['serial'], \
+                                         line['name'], line['resName'], \
+                                         line['chainID'], line['resSeq'], \
+                                         line['x'], line['y'], line['z'], \
+                                         line['charge'], 0.0 )
+                # write
+                outp.write( formatted_line + "\n" )
+            outp.write("END\n")
+
+    ## write gro to file ----------------------------------------------
+    def write_gro(self, file, renum_atoms=True) -> None:
+        '''Write GROMACS' gro file'''
+        if renum_atoms: self.renum_atoms()
+        with open( file, 'wt' ) as outp:
+            outp.write("{:s}\n  {:d}\n".format(self.title, self.natoms))
+            # write atoms
+            for n in range(self.natoms):
+                line = self.pdb[n].copy()
+                # format gro
+                formatted_line = "{:>5d}{:>5s}{:>5s}{:>5d}{:>8.3f}{:>8.3f}{:>8.3f}" \
+                    .format(line['resSeq'], line['resName'], line['name'], line['serial'], line['x']/10., line['y']/10., line['z']/10.)
+                # write
+                outp.write( formatted_line + "\n" )
+            outp.write("   0.00000   0.00000   0.00000\n")
+
     ## write fasta to file --------------------------------------------
-    def write_fasta( self, file, gaps=False ):
+    def write_fasta(self, file, gaps=False) -> None:
         '''Write fasta file'''
         if not gaps:
             seq = [ i[2] for i in self.sequence ]
         else:
             seq = []; n = 0
             for i in range(self.sequence[0][0], self.sequence[-1][0]+1):
                 if self.sequence[n][0] == i:
@@ -333,37 +559,37 @@
             # sequence
             nline = int(m.ceil(self.nres / 70))
             for n in range(nline):
                 formatted_line = "{:<s}".format(''.join(seq[0+n*70:70+n*70]))
                 outp.write( formatted_line + "\n" )
 
     ## write XYZ to file ----------------------------------------------
-    def write_xyz( self, file ):
+    def write_xyz(self, file) -> None:
         '''Write XYZ file'''
         self.guess_elements()
         with open( file, 'wt' ) as outp:
             outp.write(" {}\n".format(self.natoms))
             outp.write(" {}\n".format(self.title))
             for atom in self.pdb:
                 outp.write(" {:<6s}  {:>18.10f} {:>18.10f} {:>18.10f}\n"
                            .format(atom['element'], atom['x'], atom['y'], atom['z']))
 
     ## write interaction sequence to file -----------------------------
-    def write_intseq( self, file ):
+    def write_intseq(self, file) -> None:
         '''Write interaction sequence to file'''
         seq = self.sequence
         # open file
         with open( file, 'wt' ) as outp:
             # sequence format: X#
             for res in seq:
                 formatted_line = "{:<s}{:<d}".format(res[2],res[0])
                 outp.write( formatted_line + "\n" )
 
     ## write dynamo crd to file ---------------------------------------
-    def write_crd( self, file ):
+    def write_crd(self, file) -> None:
         '''Write dynamo crd file'''
         # open file
         with open(file, 'wt') as outp:
             # crd total properties
             outp.write("!===============================================================================\n")
             outp.write("{:<d} {:<d}  {:<d}\n".format(self.natoms, self.nres_tot, self.nseg))
             outp.write("!===============================================================================\n")
@@ -385,25 +611,29 @@
                     outp.write("{:>7d}\n".format(segments[subsys]))
                 # residue statement
                 resName = self.pdb[n]['resName']
                 resSeq = self.pdb[n]['resSeq']
                 outp.write("Residue {:>5d}  {:s}\n".format(resSeq, resName))
                 # atom statement (count number of atoms in residue and print all)
                 nres = n
-                while nres < natoms and self.pdb[nres]['resName'] == resName and self.pdb[nres]['resSeq'] == resSeq : nres += 1
+                while nres < natoms and \
+                      self.pdb[nres]['resName'] == resName and \
+                      self.pdb[nres]['resSeq'] == resSeq and \
+                      self.pdb[nres]['segment'] == subsys:
+                    nres += 1
                 outp.write("{:7d}\n".format(nres - n))
                 while n < nres:
                     outp.write("{:>7d} {:<4s} {:>10d} {:>18.10f}{:>18.10f}{:>18.10f}\n"
                         .format(self.pdb[n]['serial'], self.pdb[n]['name'],
                         Ptable[self.pdb[n]['element']]['N'], self.pdb[n]['x'],
                         self.pdb[n]['y'], self.pdb[n]['z']))
                     n += 1
 
     ## write dynamo seq to file ---------------------------------------
-    def write_seq( self, file, variants=True, ssbonds=True ):
+    def write_seq(self, file, variants=True, ssbonds=True) -> None:
         '''Write dynamo seq file'''
         # open file
         with open(file, 'wt') as outp:
             outp.write("Sequence\n{:>5d}\n".format(self.nseg))
             # initializations
             natoms = self.natoms
             segments = self.segments
@@ -414,40 +644,40 @@
             while n < natoms:
                 # subsystem statement
                 if self.pdb[n]['segment'] != subsys:
                     nline = 0
                     subsys = self.pdb[n]['segment']
                     outp.write("\nSubsystem  {:s}\n{:>5d}\n".format(subsys,segments[subsys]))
                 # residues
-                if self.pdb[n]['resName'] != self.pdb[n-1]['resName'] or self.pdb[n]['resSeq'] != self.pdb[n-1]['resSeq']:
+                if self.pdb[n]['resName'] != self.pdb[n-1]['resName'] or \
+                   self.pdb[n]['resSeq'] != self.pdb[n-1]['resSeq'] or \
+                   self.pdb[n]['segment'] != self.pdb[n-1]['segment']:
                     nline += 1
                     outp.write("{:s} ; ".format(self.pdb[n]['resName']))
                     if nline % 13 == 0:
                         nline = 0
                         outp.write("\n")
                 if n+1 < natoms and self.pdb[n+1]['segment'] != subsys:
-                    if variants and subsys == 'A':
+                    if variants and self.pdb[n]['resName'] in aa:
                         outp.write("\nVARIANT          N_TERMINAL  {:<s}  {:<d}".format(sequence[0][1],sequence[0][0]))
                         outp.write("\nVARIANT          C_TERMINAL  {:<s}  {:<d}".format(sequence[-1][1],sequence[-1][0]))
                         outp.write("\nEnd\n")
                     else:
                         outp.write("\nEnd\n")
                 n += 1
             outp.write("\nEnd\n")
             if ssbonds:
                 for ssbond in self.ssbonds:
                     outp.write("\nLink DISULPHIDE_BRIDGE A CYX {:>3d} A CYX {:>3d}".format(*ssbond))
             outp.write("\nEnd")
 
-    ## write dynamo ligand opls to file -------------------------------
-    def write_ligand( self, ligand ):
-        '''Write dynamo ligand topology file'''
-        file=ligand+".ff"
-        # get ligand lines index
-        lig_index = [i for i, n in enumerate(self.pdb) if n['resName']==ligand]
+    ## write dynamo topology of ligand to file ------------------------
+    def write_ff(self, file, lig_name='UNK', lig_index=None) -> None:
+        '''Write dynamo topology file'''
+        lig_index = lig_index if lig_index is not None else list(range(self.natoms))
         # bonds: calculate upper distance matrix, consider bond if below threshold
         bond_thr = 1.7  # bond threshold
         bonds = []
         for i in lig_index:
             for j in range(i+1, lig_index[-1]+1):
                 dist = m.sqrt( (self.pdb[i]['x']-self.pdb[j]['x'])**2 + (self.pdb[i]['y']-self.pdb[j]['y'])**2 + (self.pdb[i]['z']-self.pdb[j]['z'])**2 )
                 if dist < bond_thr and (self.pdb[i]['element'] or self.pdb[j]['element']) != 'H':
@@ -463,15 +693,15 @@
                 bonds_sorted = sorted(bonds_i)
                 bonds_sorted.insert(2,name)
                 impropers.append(bonds_sorted)
         # open file
         with open(file, 'wt') as outp:
             # header
             outp.write("!-------------------------------------------------------------------------------\n")
-            outp.write("Residue {:s}\n".format(ligand))
+            outp.write("Residue {:s}\n".format(lig_name))
             outp.write("!-------------------------------------------------------------------------------\n")
             outp.write("! # Atoms, bonds and impropers.\n")
             outp.write(" {}   {}   {}\n""".format(len(lig_index),len(bonds),len(impropers)))
             # atoms
             for n in lig_index:
                 if self.pdb[n]['element'] != '':
                     outp.write("{:<4s}  {:<2s}    0.0\n".format(self.pdb[n]['name'], self.pdb[n]['element']))
@@ -492,31 +722,39 @@
             for b in impropers:
                 nline += 1
                 outp.write("{:<4s} {:<4s} {:<4s} {:<4s} ; ".format(b[0],b[1],b[2],b[3]))
                 if nline % 3 == 0:
                     nline = 0
                     outp.write("\n")
 
+    ## write dynamo ff for all ligands --------------------------------
+    def write_ff_ligands(self) -> None:
+        '''Write dynamo topology files for all ligands'''
+        for lig_name, lig_resSeq, lig_segment in self.ligands_long:
+            lig_index = self.findall(resName=lig_name, resSeq=lig_resSeq, segment=lig_segment)
+            lig_file = f"{lig_name}_{lig_resSeq}_{lig_segment}.ff"
+            self.write_ff(lig_file, lig_name, lig_index)
+
     ## substitute field -----------------------------------------------
-    def substitute( self, field, origin, destination, protectProtein=False, onlyProtein=False ):
+    def substitute(self, field, origin, destination, protectProtein=False, onlyProtein=False) -> None:
         '''Change field values that match'''
         if protectProtein and onlyProtein:
             return
         elif protectProtein:
             for n in self.pdb:
                 if not n['resName'] in aa and n[field] == origin: n[field] = destination
         elif onlyProtein:
             for n in self.pdb:
                 if n['resName'] in aa and n[field] == origin: n[field] = destination
         else:
             for n in self.pdb:
                 if n[field] == origin: n[field] = destination
 
     ## empty/zero or value field --------------------------------------
-    def clean_field( self, field, value=None ):
+    def clean_field(self, field, value=None) -> None:
         '''Makes field zero/empty or value'''
 
         # check field
         if field not in self.atom_empty.keys():
             raise ValueError("Not valid field")
 
         # check input value or empty
@@ -530,126 +768,188 @@
             value = 0.0
 
         # substitute field value
         for n in self.pdb:
             n[field] = value
 
     ## return atoms that match fields ---------------------------------
-    def findall( self, **field_and_values ):
-        '''Find a list of atom index that match all fields'''
-        
-        # check fields
-        if field_and_values.keys() - self.atom_empty.keys():
+    def findall(self, match_all=True, **fields_and_values) -> list:
+        '''Find a list of atom index that match all/any fields'''
+        # check input fields
+        if fields_and_values.keys() - self.atom_empty.keys():
             raise ValueError("Not valid field provided")
-
+        # find any/all atoms that match
+        matcher = all if match_all else any
         return [n for n, atom in enumerate(self.pdb)
-                if all(atom[key]==value for key, value in field_and_values.items())]
+                if matcher(atom[key]==value for key, value in fields_and_values.items())]
 
-    ## remove atom based on field -------------------------------------
-    def remove( self, field, value ):
-        '''Remove atoms based on match on a field'''
-        matching_index = self.findall(**{field:value})
+    ## remove atoms that match fields ---------------------------------
+    def remove(self, match_all=True, **fields_and_values) -> None:
+        '''Remove all atoms that match all/any fields'''
+        matching_index = self.findall(match_all=match_all, **fields_and_values)
         for n in sorted(matching_index, reverse=True):
             del self.pdb[n]
 
+    ## remove ligands -------------------------------------------------
+    def remove_ligands(self) -> None:
+        '''Remove all ligands'''
+        for ligand in self.ligands:
+            self.remove(resName=ligand)
+
+    ## remove waters --------------------------------------------------
+    def remove_waters(self) -> None:
+        '''Remove all waters (try to)'''
+        water_resNames = ('HOH', 'WAT', 'SOL', 'TIP3', 'TIP4', 'TIP5', 'SPC')
+        for water in water_resNames:
+            self.remove(resName=water)
+
+    ## keep only atoms that match fields --------------------------------
+    def keep_only(self, match_all=True, **fields_and_values) -> None:
+        '''Keep only atoms that match all/any fields'''
+        matching_index = self.findall(match_all=match_all, **fields_and_values)
+        self.pdb = [atom for n, atom in enumerate(self.pdb) if n in matching_index]
+
     ## all to ATOM ----------------------------------------------------
-    def all2ATOM( self ):
+    def all2ATOM(self) -> None:
         '''Change all ATOM/HETATM to ATOM'''
         self.clean_field('ATOM', 'ATOM')
 
     ## transate resNames between ff -----------------------------------
-    def translate_residues( self, destination, origin=None ):
+    def translate_residues(self, destination, origin=None) -> None:
         '''Translate resNames between ff'''
         if origin is None:
             formats = rosetta_residues.keys()
         else:
             formats = [origin]
         for j in formats:
             if j == destination: continue
             for n in self.pdb:
                 resName = n['resName']
                 if resName in rosetta_residues[j]:
                     n['resName'] = rosetta_residues[destination][rosetta_residues[j].index(resName)]
 
     ## transate names between formats ---------------------------------
-    def translate_names( self, destination, origin ):
+    def translate_names(self, destination, origin, onlyProtein=True) -> None:
         '''Translate atom names between formats'''
         for n in self.pdb:
             resName = n['resName']
             name = n['name']
+            if onlyProtein and not resName in aa: continue
             if resName in rosetta_atoms[origin] and name in rosetta_atoms[origin][resName]:
                 n['name'] = rosetta_atoms[destination][resName][rosetta_atoms[origin][resName].index(name)]
 
     ## reorder protein atoms ------------------------------------------
-    def canonical_order( self, canon='dynamo' ):
+    def canonical_order(self, canon='dynamo') -> None:
         '''Reorder protein atoms'''
         nres = self.nres
         # find protein
         for linen in range(self.natoms):
             if self.pdb[linen]['resName'] in aa: break
         res = 1
         while res <= nres:
             # residue number and name
             resSeq = self.pdb[linen]['resSeq']
             resName = self.pdb[linen]['resName']
             # find last residue line
             linen_end = linen
-            while True and linen_end < self.natoms:
-                if self.pdb[linen_end]['resSeq'] == resSeq and self.pdb[linen_end]['resName'] == resName: linen_end += 1
-                else: break
+            while linen_end+1 < self.natoms:
+                if self.pdb[linen_end+1]['resSeq'] != resSeq or self.pdb[linen_end+1]['resName'] != resName:
+                    break
+                linen_end += 1
             # reorder atoms (modified bubble sort algorithm)
             for j in range(linen, linen_end-1):
                 swapped = False
                 for i in range(linen, linen_end-j+linen-1):
                     try:
                         if rosetta_atoms[canon][resName].index(self.pdb[i]['name']) > rosetta_atoms[canon][resName].index(self.pdb[i+1]['name']):
                             self.pdb[i], self.pdb[i+1] = self.pdb[i+1], self.pdb[i]
                             swapped = True
                     except ValueError:
                         self.pdb[i], self.pdb[i+1] = self.pdb[i+1], self.pdb[i]
                         swapped = True
                 if not swapped: break
             linen = linen_end +1
             res += 1
+        self.renum_atoms()
 
-    ## renumerate atoms -----------------------------------------------
-    def renum_atoms( self ):
-        '''Renumerate all atoms from 1'''
-        for n in range(self.natoms):
-            self.pdb[n]['serial'] = n + 1
+    ## reorder atoms by element ---------------------------------------
+    def order_by_atom(self, keepnames=False, protectProtein=True) -> None:
+        '''Reorder atoms by element (reversed Periodic Table) in each residue and change their names in order'''
+        if not all([n['element'] for n in self.pdb]):
+            self.guess_elements()
+        Ptable_elements_reverse = list(Ptable.keys())[::-1]
+        nres_tot = self.nres_tot
+        linen = 0
+        res = 1
+        while res <= nres_tot:
+            # residue number and name
+            resSeq = self.pdb[linen]['resSeq']
+            resName = self.pdb[linen]['resName']
+            # find last residue line
+            linen_end = linen
+            while linen_end+1 < self.natoms:
+                if self.pdb[linen_end+1]['resSeq'] != resSeq or self.pdb[linen_end+1]['resName'] != resName:
+                    break
+                linen_end += 1
+            # skip protein
+            if not (protectProtein and resName in aa):
+                # reorder atoms (modified bubble sort algorithm)
+                for j in range(linen, linen_end-1):
+                    swapped = False
+                    for i in range(linen, linen_end-j+linen-1):
+                        if Ptable_elements_reverse.index(self.pdb[i]['element']) > Ptable_elements_reverse.index(self.pdb[i+1]['element']):
+                            self.pdb[i], self.pdb[i+1] = self.pdb[i+1], self.pdb[i]
+                            swapped = True
+                    if not swapped: break
+                # rename atoms
+                if not keepnames:
+                    elements = []
+                    for i in range(linen, linen_end+1):
+                        element = f"{self.pdb[i]['element']}"
+                        elements.append(element)
+                        self.pdb[i]['name'] = f"{element}{elements.count(element)}"
+            linen = linen_end +1
+            res += 1
+        self.renum_atoms()
 
-    ## renumerate residues --------------------------------------------
-    def renum_res( self, continuous=False, protectProtein=False, guess_segments=False ):
-        '''Renumerate residues, each group from 1: Protein / Ligands / Solvent / Ions'''
+    ## renumber atoms -------------------------------------------------
+    def renum_atoms(self, start=1) -> None:
+        '''Renumber all atoms from 'start' (def: 1)'''
+        for id, n in enumerate(self.pdb):
+            n['serial'] = id + start
+
+    ## renumber residues ----------------------------------------------
+    def renum_res(self, start=1, continuous=False, protectProtein=False, guess_segments=False) -> None:
+        '''Renumber residues, each group from 'start' (def: 1): Protein / Ligands / Solvent / Ions'''
         if guess_segments: self.guess_segments()
-        resSeq = 0
+        resSeq = start - 1
         resSeq_prev = 0
         resName_prev = ''
         segment_prev = ''
         if continuous:  # all residues in global list, ignore protectProtein
             for n in self.pdb:
                 if n['resName'] != resName_prev or n['resSeq'] != resSeq_prev:
                     resName_prev = n['resName']
                     resSeq_prev = n['resSeq']
                     resSeq += 1
                 n['resSeq'] = resSeq
-        else:  # renumerate with a new list for each segment
+        else:  # renumber with a new list for each segment
             for n in self.pdb:
                 if protectProtein and n['resName'] in aa: continue
                 if n['segment'] != segment_prev:
                     segment_prev = n['segment']
-                    resSeq = 0
+                    resSeq = start - 1
                 if n['resName'] != resName_prev or n['resSeq'] != resSeq_prev:
                     resName_prev = n['resName']
                     resSeq_prev = n['resSeq']
                     resSeq += 1
                 n['resSeq'] = resSeq
 
     ## guess elements -------------------------------------------------
-    def guess_elements( self, keepknown=True ):
+    def guess_elements(self, keepknown=True) -> None:
         '''Guess elements for all atoms'''
         for n in self.pdb:
             if keepknown and n['element'] != '': continue
             name = ''.join([i for i in n['name'] if i.isalpha()])
             if n['resName'] in aa:  # protein
                 if name[0] in Ptable:
                     n['element'] = name[0]
@@ -657,15 +957,15 @@
                     n['element'] = name[1]
             elif n['resName'] in ions:  # ions
                 n['element'] = name[0] + name[1].lower()
             else:  # rest
                 n['element'] = name[0]
 
     ## guess segments -------------------------------------------------
-    def guess_segments( self, keepknown=True, useChains=False ):
+    def guess_segments(self, keepknown=True, useChains=True) -> None:
         '''Guess segments for each group: Protein / Ligands / Solvent / Ions'''
         ligands = self.ligands
         for n in self.pdb:
             if not keepknown: n['segment'] = ''
             if useChains and n['chainID'] != '':
                 n['segment'] = n['chainID']
                 continue
@@ -677,56 +977,64 @@
                 n['segment'] = solvent[resName]
             elif resName in ions:
                 n['segment'] = "ION"
             elif resName in ligands:
                 n['segment'] = segment_letters[ligands.index(resName) + 1]
 
     ## molecular weight -----------------------------------------------
-    def weight( self, guess_elements=True, onlyProtein=True, monoisotopic=False ):
+    def weight(self, guess_elements=True, onlyProtein=True, monoisotopic=False) -> float:
         '''Molecular weight (Da)'''
         if guess_elements: self.guess_elements()
         mass = 0.0
-        if monoisotopic: atomic_mass = 'm'
-        else: atomic_mass = 'm_std'
+        atomic_mass = 'm' if monoisotopic else 'm_std'
         for n in self.pdb:
             if not onlyProtein or n['resName'] in aa:
                 mass += Ptable[ n['element'] ][atomic_mass]
         return mass
 
-    ## move com to center ---------------------------------------------
-    def center( self, guess_elements=True, center=[0., 0., 0.], monoisotopic=False ):
-        '''Move system com to the center'''
-        if guess_elements: self.guess_elements()
-        if monoisotopic: atomic_mass = 'm'
-        else: atomic_mass = 'm_std'
-        m_total = self.weight(guess_elements=False, onlyProtein=False, monoisotopic=monoisotopic)
-        com = [0.0, 0.0, 0.0]
+    ## center of mass -------------------------------------------------
+    def com(self, geometric=False,  guess_elements=True, monoisotopic=False) -> list:
+        '''Calculate center of mass'''
+        atomic_mass = 'm' if monoisotopic else 'm_std'
+        # calculate total mass
+        if geometric:
+            m_total = float(self.natoms)
+        else:
+            if guess_elements: self.guess_elements()
+            m_total = self.weight(guess_elements=False, onlyProtein=False, monoisotopic=monoisotopic)
         # calculate com
+        com = [0.0, 0.0, 0.0]
         for n in self.pdb:
+            n_mass = 1.0 if geometric else Ptable[n['element']][atomic_mass]
             for i, j in zip( [0,1,2], ['x','y','z'] ):
-                com[i] += n[j] * Ptable[n['element']][atomic_mass]
+                com[i] += n[j] * n_mass
         com = [ i / m_total for i in com ]
-        # move com
+        return com
+
+    ## move COM to center ---------------------------------------------
+    def center(self, center=[0., 0., 0.], geometric=False, guess_elements=True, monoisotopic=False) -> None:
+        '''Move system's COM to the center'''
+        com = self.com(geometric=geometric, guess_elements=guess_elements, monoisotopic=monoisotopic)
         for n in self.pdb:
             for i, j in zip( [0,1,2], ['x','y','z'] ):
-                n[j] -= com[i] + center[i]
+                n[j] -= com[i] - center[i]
 
     ## change names CYS for CYX ---------------------------------------
-    def cys2cyx( self ):
+    def cys2cyx(self) -> None:
         '''Change resName of CYS for CYX if not HG'''
         # get resSeq for SG and HG atoms
         sg = { line['resSeq'] for n, line in enumerate(self.pdb) if line['name']=='SG' and line['resName'] in aa }
         hg = { line['resSeq'] for n, line in enumerate(self.pdb) if line['name']=='HG' and line['resName'] in aa }
         # change names
         for n in self.pdb:
             if n['resName'] == 'CYS' and n['resSeq'] in sg.difference(hg): n['resName'] = 'CYX'
             elif n['resName'] == 'CYX' and n['resSeq'] in sg.intersection(hg): n['resName'] = 'CYS'
 
     ## change HIS for HID/HIE/HIP -------------------------------------
-    def guess_his( self ):
+    def guess_his(self) -> None:
         '''Change HIS for corresponding HID/HIE/HIP'''
         # get resSeq for N HIS
         nhis = [ n for n, line in enumerate(self.pdb) if line['name']=='N' and line['resName']=='HIS' ]
         for linen in nhis:
             # residue number and name
             resSeq = self.pdb[linen]['resSeq']
             resName = self.pdb[linen]['resName']
@@ -745,15 +1053,15 @@
             else:
                 raise ValueError('Strange HIS found')
             # change resName
             for n in range(linen,linen_end):
                 self.pdb[n]['resName'] = histype
 
     ## change GLU for GLH ---------------------------------------------
-    def guess_glh( self ):
+    def guess_glh(self) -> None:
         '''Change GLU for corresponding GLH'''
         # get resSeq for N HIS
         nglu = [ n for n, line in enumerate(self.pdb) if line['name']=='N' and line['resName']=='GLU' ]
         for linen in nglu:
             # residue number and name
             resSeq = self.pdb[linen]['resSeq']
             resName = self.pdb[linen]['resName']
@@ -765,15 +1073,15 @@
             # determine GLH
             if 'HE2' in { line['name'] for line in self.pdb[linen:linen_end] }:
                 # change resName
                 for n in range(linen,linen_end):
                     self.pdb[n]['resName'] = 'GLH'
 
     ## change ASP for ASH ---------------------------------------------
-    def guess_ash( self ):
+    def guess_ash(self) -> None:
         '''Change ASP for corresponding ASH'''
         # get resSeq for N HIS
         nasp = [ n for n, line in enumerate(self.pdb) if line['name']=='N' and line['resName']=='ASP' ]
         for linen in nasp:
             # residue number and name
             resSeq = self.pdb[linen]['resSeq']
             resName = self.pdb[linen]['resName']
@@ -785,15 +1093,15 @@
             # determine ASH
             if 'HD2' in { line['name'] for line in self.pdb[linen:linen_end] }:
                 # change resName
                 for n in range(linen,linen_end):
                     self.pdb[n]['resName'] = 'ASH'
 
     ## change LYS for LYN ---------------------------------------------
-    def guess_lyn( self ):
+    def guess_lyn(self) -> None:
         '''Change LYS for corresponding LYN'''
         # get resSeq for N HIS
         nasp = [ n for n, line in enumerate(self.pdb) if line['name']=='N' and line['resName']=='LYS' ]
         for linen in nasp:
             # residue number and name
             resSeq = self.pdb[linen]['resSeq']
             resName = self.pdb[linen]['resName']
@@ -805,97 +1113,113 @@
             # determine ASH
             if 'HZ3' not in { line['name'] for line in self.pdb[linen:linen_end] }:
                 # change resName
                 for n in range(linen,linen_end):
                     self.pdb[n]['resName'] = 'LYN'
 
     ## guess protonation resName of key residues ----------------------
-    def guess_protonres( self ):
+    def guess_protonres(self) -> None:
         '''Change residues based on their protonation (HIS,GLU,ASP,LYS)'''
         self.guess_his()
         self.guess_glh()
         self.guess_ash()
         self.guess_lyn()
 
     ## number of atoms ------------------------------------------------
     @property
-    def natoms( self ):
+    def natoms(self) -> int:
         '''Number of atoms'''
         return len(self.pdb)
 
     ## number of protein residues -------------------------------------
     @property
-    def nres( self ):
+    def nres(self) -> int:
         '''Number of protein residues'''
         return len(self.sequence)
 
     ## number of total residues ---------------------------------------
     @property
-    def nres_tot( self ):
+    def nres_tot(self) -> int:
         '''Number of total residues'''
         nres_tot = 1
         for n in range(1, self.natoms):
-            if self.pdb[n]['resName'] != self.pdb[n-1]['resName'] or self.pdb[n]['resSeq'] != self.pdb[n-1]['resSeq']:
+            if self.pdb[n]['resName'] != self.pdb[n-1]['resName'] or \
+               self.pdb[n]['resSeq'] != self.pdb[n-1]['resSeq'] or \
+               self.pdb[n]['chainID'] != self.pdb[n-1]['chainID'] or \
+               self.pdb[n]['segment'] != self.pdb[n-1]['segment']:
                 nres_tot += 1
         return nres_tot
 
     ## number of segments ---------------------------------------------
     @property
-    def nseg( self ):
+    def nseg(self) -> int:
         '''Number of segments'''
         return len(self.segments.keys())
 
+    ## number of ligands ----------------------------------------------
+    @property
+    def nlig(self) -> int:
+        '''Number of ligands'''
+        return len(self.ligands)
+
     ## list of list of coordinates ------------------------------------
     @property
-    def xyz( self ):
+    def xyz(self) -> list:
         '''List of list of coordinates [[x,y,z]]'''
         return [[a['x'], a['y'], a['z']] for a in self.pdb]
 
     ## dictionary of segments -----------------------------------------
     @property
-    def segments( self ):
+    def segments(self) -> dict:
         '''Dictionary of segments: { seg : #res }'''
         seg = {}
         for n in range(self.natoms):
             if self.pdb[n]['segment'] == '': raise ValueError("Not all segments assigned")
             if self.pdb[n]['segment'] not in seg:
                 seg.update({ self.pdb[n]['segment'] : 1 })
             elif self.pdb[n]['resSeq'] != self.pdb[n-1]['resSeq'] or self.pdb[n]['resName'] != self.pdb[n-1]['resName']:
                 seg[self.pdb[n]['segment']] += 1
         return seg
 
     ## residue sequence -----------------------------------------------
     @property
-    def sequence( self ):
+    def sequence(self) -> list:
         '''List of protein residues: [[ #, XXX, X ]]'''
         letter_seq = []
         for n in self.pdb:
             if n['resName'] in aa:
              res = n['resSeq']; break
         for n in self.pdb:
             if n['resName'] in aa and n['resSeq'] >= res:
                 res = n['resSeq'] + 1
                 letter_seq.append([ n['resSeq'], n['resName'], aa_letters[n['resName']] ])
         return letter_seq
 
     ## ligands list ---------------------------------------------------
     @property
-    def ligands( self ):
+    def ligands(self) -> list:
         '''List of ligands: [ XXX ]'''
-        ligands = []
-        for n in self.pdb:
-            resName = n['resName']
-            if resName not in aa and resName not in solvent \
-               and resName not in ions and resName not in ligands:
-                ligands.append(n['resName'])
-        return ligands
+        return [i[0] for i in self.ligands_long]
+
+    ## ligands long information list ----------------------------------
+    @property
+    def ligands_long(self) -> list:
+        '''Dict of extended ligand information: [[ XXX, resSeq, segment]]'''
+        ligands_long = []
+        for atom in self.pdb:
+            if atom['resName'] in aa | solvent.keys() | ions.keys():
+                continue
+            ligand = (atom['resName'], atom['resSeq'], atom['segment'])
+            if ligand not in ligands_long:
+                ligands_long.append(ligand)
+        return ligands_long
 
     ## dishuphide bridges list ----------------------------------------
     @property
-    def ssbonds( self ):
+    def ssbonds(self) -> list:
         '''S-S bonds list: [[ #resSeq, #resSeq ]]'''
         ss_bond_thr = 3.0  # maximum distance to consider S-S bond (A)
         # get lines from SG atoms from CYX
         sg = [ line for n, line in enumerate(self.pdb) if line['name']=='SG' and line['resName']=='CYX' ]
         # calculate upper distance matrix, consider bond if below threshold
         ss_bonds = []
         for i in range(len(sg)):
@@ -904,31 +1228,34 @@
                 if dist < ss_bond_thr:
                     ss_bonds.append([sg[i]['resSeq'],sg[j]['resSeq']])
         if len(ss_bonds) != len(sg)/2: raise ValueError("Issues with SS bonds")
         return ss_bonds
 
     ## protein weight -------------------------------------------------
     @property
-    def protein_weight( self ):
+    def protein_weight(self) -> float:
         '''Molecular average protein weight (Da)'''
         return self.weight( guess_elements=True, onlyProtein=True, monoisotopic=False )
 
     ## build a PyMOL's selection macro notation for an atom -----------
     @staticmethod
-    def pymol_sele_macro( atom_dict ):
+    def pymol_sele_macro(atom_dict) -> str:
         '''Build a PyMOL's selection macro notation for an atom'''
         # https://pymolwiki.org/index.php/Selection_Macros
         # /object-name/segi-identifier/chain-identifier/resi-identifier/name-identifier
         fields = [str(atom_dict[k]) if atom_dict[k] else "" for k in ('segment', 'chainID', 'name')]
         residue = [str(atom_dict[k]) for k in ('resName', 'resSeq') if atom_dict[k]]
         fields.insert(2, "`".join(residue))
         return "//{}".format("/".join(fields))
 
-
-##  Standard protein preparation  #####################################
-def standard_preparation( molec, inpformat, outformat, ff='amber' ):
-    '''Standard protein preparation'''
-    molec.all2ATOM()
-    molec.translate_residues(ff, origin=None)
-    molec.translate_names(outformat, origin=inpformat)
-    molec.canonical_order(outformat)
-    molec.guess_elements(keepknown=False)
+    ## standard protein preparation -----------------------------------
+    def standard_preparation(self, inpformat, outformat, ff='amber') -> None:
+        '''
+            Standard protein preparation
+
+            all2ATOM, translate_residues, translate_names, canonical_order, guess_elements
+        '''
+        self.all2ATOM()
+        self.translate_residues(ff, origin=None)
+        self.translate_names(outformat, origin=inpformat)
+        self.canonical_order(outformat)
+        self.guess_elements(keepknown=False)
```

### Comparing `pdb4all-0.4.9/pdb4all/rosetta.py` & `pdb4all-0.5.1/pdb4all/rosetta.py`

 * *Files identical despite different names*

### Comparing `pdb4all-0.4.9/pdb4all.egg-info/PKG-INFO` & `pdb4all-0.5.1/pdb4all.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: pdb4all
-Version: 0.4.9
+Version: 0.5.1
 Summary: Convert between common protein pdb formats and names 
 Home-page: https://github.com/boneta/pdb4all
 Author: Sergio Boneta
 Author-email: boneta@unizar.es
 License: GPLv3
-Description: # pdb4all
-        *Convert between common protein pdb formats and names*
-        
-        ### Installation
-        Requires `python 3.7+`. No additional dependencies are needed. \
-        It should work on 2.7+ but no warranty is provided.
-        
-        *pdb4all* is frequently uploaded to [PyPI](https://pypi.org/project/pdb4all/). To install it, execute the following command:
-        ```
-          pip install pdb4all
-        ```
-        
-        ### Usage
-        ```
-          pdb4all <options> .pdb
-        ```
-        
-        #### Currently supported ForceFields name conventions
-          * Amber
-          * Charmm
-          * OPLS
-        
-        #### Currently supported formats (software)
-          * Fasta
-          * Maestro
-          * GROMACS
-          * fDynamo
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pdb4all
+
+![python](https://img.shields.io/badge/python-3.7+-red.svg)
+[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+*Convert between common protein pdb formats and names*
+
+### Installation
+Requires `python 3.7+`. No additional dependencies are needed.
+
+*pdb4all* is frequently uploaded to [PyPI](https://pypi.org/project/pdb4all/). To install it, execute the following command:
+```
+  pip install pdb4all
+```
+
+### Usage
+```
+  pdb4all <options> .pdb
+```
+
+#### Currently supported ForceFields name conventions
+  * Amber
+  * Charmm
+  * OPLS
+
+#### Currently supported formats (software)
+  * Fasta
+  * Maestro
+  * GROMACS
+  * fDynamo
```

