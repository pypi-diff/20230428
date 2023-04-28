# Comparing `tmp/varvamp-0.7.tar.gz` & `tmp/varvamp-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.7.tar", last modified: Tue Apr 18 14:46:09 2023, max compression
+gzip compressed data, was "varvamp-0.8.tar", last modified: Tue Apr 25 07:38:33 2023, max compression
```

## Comparing `varvamp-0.7.tar` & `varvamp-0.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-18 14:46:09.310270 varvamp-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 14:45:49.000000 varvamp-0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:46:09.310270 varvamp-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-18 14:45:49.000000 varvamp-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/conserved.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-25 07:38:33.757910 varvamp-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-25 07:38:17.000000 varvamp-0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:38:33.757910 varvamp-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 07:38:17.000000 varvamp-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.753910 varvamp-0.8/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-25 07:38:17.000000 varvamp-0.8/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:38:33.757910 varvamp-0.8/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 07:38:33.000000 varvamp-0.8/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.7/PKG-INFO` & `varvamp-0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.7
+Version: 0.8
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -15,29 +15,35 @@
 # varVAMP
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
-<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg /> 
+<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
+<img src="./docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
+<img src="./docs/sanger.png" alt="sanger" />
+
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
+<img src="./docs/tiled.png" alt="tiled" />
+
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
+<img src="./docs/qpcr.png" alt="qpcr" />
+
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
```

### Comparing `varvamp-0.7/README.md` & `varvamp-0.8/varvamp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,49 @@
+Metadata-Version: 2.1
+Name: varvamp
+Version: 0.8
+Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
+Home-page: https://github.com/jonas-fuchs/varVAMP
+Author: Dr. Jonas Fuchs
+Author-email: jonas.fuchs@uniklinik-freiburg.de
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 **var**iable **V**irus**AMP**licons (varVAMP) is a tool to design primers for highly diverse viruses. The input is an alignment of your viral (full-genome) sequences.
 
 # varVAMP
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
-<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg /> 
+<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
+<img src="./docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
+<img src="./docs/sanger.png" alt="sanger" />
+
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
+<img src="./docs/tiled.png" alt="tiled" />
+
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
+<img src="./docs/qpcr.png" alt="qpcr" />
+
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
```

### Comparing `varvamp-0.7/setup.py` & `varvamp-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp/command.py` & `varvamp-0.8/varvamp/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import time
 import argparse
 
 # varVAMP
 from varvamp.scripts import alignment
 from varvamp.scripts import config
 from varvamp.scripts import consensus
-from varvamp.scripts import conserved
+from varvamp.scripts import regions
 from varvamp.scripts import logging
+from varvamp.scripts import param_estimation
 from varvamp.scripts import primers
 from varvamp.scripts import qpcr
 from varvamp.scripts import reporting
 from varvamp.scripts import scheme
 from varvamp import __version__
 from . import _program
 
@@ -53,25 +54,25 @@
         nargs=2,
         help="alignment file and dir to write results"
     )
     for par in (SANGER_parser, TILED_parser, QPCR_parser):
         par.add_argument(
             "-t",
             "--threshold",
-            metavar="0.89",
+            metavar="",
             type=float,
-            default=0.89,
-            help="threshold for conserved nucleotides"
+            default=None,
+            help="threshold for consensus nucleotides"
         )
         par.add_argument(
             "-a",
             "--n-ambig",
-            metavar="4",
+            metavar="",
             type=int,
-            default=4,
+            default=None,
             help="max number of ambiguous characters in a primer"
         )
     for par in (SANGER_parser, TILED_parser):
         par.add_argument(
             "-ol",
             "--opt-length",
             help="optimal length of the amplicons",
@@ -104,31 +105,31 @@
         help="report the top n best hits"
     )
     QPCR_parser.add_argument(
         "-pa",
         "--pn-ambig",
         metavar="1",
         type=int,
-        default=1,
+        default=None,
         help="max number of ambiguous characters in a probe"
     )
     QPCR_parser.add_argument(
         "-n",
         "--test-n",
         type=int,
         metavar="50",
         default=50,
         help="test the top n qPCR amplicons for secondary structures at the minimal primer temperature"
     )
     QPCR_parser.add_argument(
         "-d",
         "--deltaG",
         type=int,
-        metavar="-1",
-        default=-1,
+        metavar="-3",
+        default=-3,
         help="minimum free energy (kcal/mol/K) cutoff at the lowest primer melting temp"
     )
     parser.add_argument(
         "--verbose",
         action=argparse.BooleanOptionalAction,
         default=True,
         help="show varvamp console output"
@@ -146,75 +147,94 @@
         return parser.parse_args(sysargs)
 
 
 def shared_workflow(args, log_file):
     """
     part of the workflow that is shared by all modes
     """
+    # start varvamp
+    logging.varvamp_progress(log_file, mode=args.mode)
 
+    # read in alignment and preprocess
+    preprocessed_alignment = alignment.preprocess(args.input[0])
+
+    # estimate threshold or number of ambiguous bases if args were not supplied
+    if args.threshold is None or args.n_ambig is None:
+        args.threshold, args.n_ambig = param_estimation.get_parameters(preprocessed_alignment, args, log_file)
+    if args.mode == "qpcr" and args.n_ambig >= 1 and args.pn_ambig is None:
+        args.pn_ambig = args.n_ambig - 1
+        with open(log_file, "a") as f:
+            print(f"Automatic parameter selection set -pn {args.pn_ambig}.", file=f)
+
+    # check arguments
     logging.raise_arg_errors(args, log_file)
-    logging.varvamp_progress(log_file)
+
     # config check
     logging.confirm_config(args, log_file)
     logging.varvamp_progress(
         log_file,
         progress=0.1,
         job="Checking config.",
         progress_text="config file passed"
     )
-    # preprocess and clean alignment of gaps
+
+    # clean alignment of gaps
     alignment_cleaned, gaps_to_mask = alignment.process_alignment(
-        args.input[0],
+        preprocessed_alignment,
         args.threshold
     )
     logging.varvamp_progress(
         log_file,
         progress=0.2,
         job="Preprocessing alignment and cleaning gaps.",
         progress_text=f"{len(gaps_to_mask)} gaps with {alignment.calculate_total_masked_gaps(gaps_to_mask)} nucleotides"
     )
+
     # create consensus sequences
     majority_consensus, ambiguous_consensus = consensus.create_consensus(
         alignment_cleaned,
         args.threshold
     )
     logging.varvamp_progress(
         log_file,
         progress=0.3,
         job="Creating consensus sequences.",
         progress_text=f"length of the consensus is {len(majority_consensus)} nt"
     )
-    # generate conserved region list
-    conserved_regions = conserved.find_regions(
+
+    # generate primer region list
+    primer_regions = regions.find_regions(
         ambiguous_consensus,
         args.n_ambig
     )
-    if not conserved_regions:
+    if not primer_regions:
         logging.raise_error(
-            "nothing conserved. Lower the threshold!",
+            "no primer regions found. Lower the threshold!",
             log_file,
             exit=True
         )
     logging.varvamp_progress(
         log_file,
         progress=0.4,
-        job="Finding conserved primer regions.",
-        progress_text=f"{conserved.mean(conserved_regions, majority_consensus)} % conserved"
+        job="Finding primer regions.",
+        progress_text=f"{regions.mean(primer_regions, majority_consensus)} % of the consensus sequence will be evaluated for primers"
     )
-    # produce kmers for all conserved regions
-    kmers = conserved.produce_kmers(
-        conserved_regions,
+
+    # produce kmers for all primer regions
+    kmers = regions.produce_kmers(
+        primer_regions,
         majority_consensus
     )
     logging.varvamp_progress(
         log_file,
         progress=0.5,
         job="Digesting into kmers.",
         progress_text=f"{len(kmers)} kmers"
     )
+
     # find potential primers
     left_primer_candidates, right_primer_candidates = primers.find_primers(
         kmers,
         ambiguous_consensus,
         alignment_cleaned
     )
     for type, primer_candidates in [("+", left_primer_candidates), ("-", right_primer_candidates)]:
@@ -227,15 +247,15 @@
     logging.varvamp_progress(
         log_file,
         progress=0.6,
         job="Filtering for primers.",
         progress_text=f"{len(left_primer_candidates)} fw and {len(right_primer_candidates)} rw potential primers"
     )
 
-    return alignment_cleaned, majority_consensus, ambiguous_consensus, conserved_regions, left_primer_candidates, right_primer_candidates
+    return alignment_cleaned, majority_consensus, ambiguous_consensus, primer_regions, left_primer_candidates, right_primer_candidates
 
 
 def sanger_and_tiled_shared_workflow(args, left_primer_candidates, right_primer_candidates, log_file):
     """
     part of the workflow shared by the sanger and tiled mode
     """
 
@@ -243,14 +263,15 @@
     all_primers = primers.find_best_primers(left_primer_candidates, right_primer_candidates)
     logging.varvamp_progress(
         log_file,
         progress=0.7,
         job="Considering only high scoring primers.",
         progress_text=f"{len(all_primers['+'])} fw and {len(all_primers['-'])} rw primers"
     )
+
     # find all possible amplicons
     amplicons = scheme.find_amplicons(
         all_primers,
         args.opt_length,
         args.max_length
     )
     if not amplicons:
@@ -286,32 +307,38 @@
 
 
 def tiled_workflow(args, amplicons, left_primer_candidates, right_primer_candidates, all_primers, ambiguous_consensus, log_file):
     """
     part of the workflow specific for the tiled mode
     """
 
+    # create graph
     amplicon_graph = scheme.create_amplicon_graph(amplicons, args.overlap)
+
     # search for amplicon scheme
     coverage, amplicon_scheme = scheme.find_best_covering_scheme(
         amplicons,
         amplicon_graph,
         all_primers
     )
+
+    # check for dimers
     dimers_not_solved = scheme.check_and_solve_heterodimers(
         amplicon_scheme,
         left_primer_candidates,
         right_primer_candidates,
         all_primers)
     if dimers_not_solved:
         logging.raise_error(
             f"varVAMP found {len(dimers_not_solved)} primer dimers without replacements. Check the dimer file and perform the PCR for incomaptible amplicons in a sperate reaction.",
             log_file
         )
         reporting.write_dimers(dir, dimers_not_solved)
+
+    # evaluate coverage
     percent_coverage = round(coverage/len(ambiguous_consensus)*100, 2)
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Creating amplicon scheme.",
         progress_text=f"{percent_coverage} % total coverage with {len(amplicon_scheme[0]) + len(amplicon_scheme[1])} amplicons"
     )
@@ -328,27 +355,28 @@
 
 
 def qpcr_workflow(args, alignment_cleaned, ambiguous_consensus, majority_consensus, left_primer_candidates, right_primer_candidates, log_file):
     """
     part of the workflow specific for the tiled mode
     """
     # find regions for qPCR probes
-    probe_conserved_regions = conserved.find_regions(
+    probe_regions = regions.find_regions(
         ambiguous_consensus,
         args.pn_ambig
     )
-    if not probe_conserved_regions:
+    if not probe_regions:
         logging.raise_error(
-            "no conserved regions that fullfill probe criterias! lower threshold or increase number of ambiguous chars in probe\n",
+            "no regions that fullfill probe criterias! lower threshold or increase number of ambiguous chars in probe\n",
             log_file,
             exit=True
         )
+
     # digest probe regions
-    probe_kmers = conserved.produce_kmers(
-        probe_conserved_regions,
+    probe_kmers = regions.produce_kmers(
+        probe_regions,
         majority_consensus,
         config.QPROBE_SIZES
     )
     # find potential probes
     qpcr_probes = qpcr.get_qpcr_probes(probe_kmers, ambiguous_consensus, alignment_cleaned)
     if not qpcr_probes:
         logging.raise_error(
@@ -358,43 +386,46 @@
         )
     logging.varvamp_progress(
         log_file,
         progress=0.7,
         job="Finding qPCR probes.",
         progress_text=f"{len(qpcr_probes)} potential qPCR probes"
     )
+
     # find unique high scoring amplicons with internal probe
     qpcr_scheme_candidates = qpcr.find_qcr_schemes(qpcr_probes, left_primer_candidates, right_primer_candidates, majority_consensus)
     if not qpcr_scheme_candidates:
         logging.raise_error(
             "no qPCR scheme candidates found. lower threshold or increase number of ambiguous chars in primer and/or probe\n",
             log_file,
             exit=True
         )
     logging.varvamp_progress(
         log_file,
         progress=0.8,
         job="Finding unique amplicons with probe.",
         progress_text=f"{len(qpcr_scheme_candidates)} unique amplicons with internal probe"
     )
+
+    # test amplicons for deltaG
     final_schemes = qpcr.test_amplicon_deltaG(qpcr_scheme_candidates, majority_consensus, args.test_n, args.deltaG)
     if not final_schemes:
         logging.raise_error(
             "no qPCR amplicon passed the deltaG threshold\n",
             log_file,
             exit=True
         )
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Filtering amplicons for deltaG.",
         progress_text=f"{len(final_schemes)} non-overlapping qPCR schemes that passed deltaG cutoff"
     )
 
-    return probe_conserved_regions, final_schemes
+    return probe_regions, final_schemes
 
 
 def main(sysargs=sys.argv[1:]):
     """
     main varvamp workflow
     """
 
@@ -402,18 +433,18 @@
     args = get_args(sysargs)
     if not args.verbose:
         sys.stdout = open(os.devnull, 'w')
     start_time = time.process_time()
     results_dir, data_dir, log_file = logging.create_dir_structure(args.input[1])
 
     # mode unspecific part of the workflow
-    alignment_cleaned, majority_consensus, ambiguous_consensus, conserved_regions, left_primer_candidates, right_primer_candidates = shared_workflow(args, log_file)
+    alignment_cleaned, majority_consensus, ambiguous_consensus, primer_regions, left_primer_candidates, right_primer_candidates = shared_workflow(args, log_file)
 
     # write files that are shared in all modes
-    reporting.write_conserved_to_bed(conserved_regions, data_dir)
+    reporting.write_regions_to_bed(primer_regions, data_dir)
     reporting.write_alignment(data_dir, alignment_cleaned)
     reporting.write_fasta(data_dir, "majority_consensus", majority_consensus)
     reporting.write_fasta(results_dir, "ambiguous_consensus", ambiguous_consensus)
 
     # SANGER/TILED mode
     if args.mode == "tiled" or args.mode == "sanger":
         all_primers, amplicons = sanger_and_tiled_shared_workflow(
@@ -446,36 +477,38 @@
             amplicon_scheme,
             ambiguous_consensus,
             args.mode
         )
         reporting.varvamp_plot(
             results_dir,
             alignment_cleaned,
-            conserved_regions,
+            primer_regions,
             all_primers=all_primers,
             amplicon_scheme=amplicon_scheme,
         )
         reporting.per_base_mismatch_plot(results_dir, amplicon_scheme, args.threshold)
+
     # QPCR mode
     if args.mode == "qpcr":
-        probe_conserved_regions, final_schemes = qpcr_workflow(
+        probe_regions, final_schemes = qpcr_workflow(
             args,
             alignment_cleaned,
             ambiguous_consensus,
             majority_consensus,
             left_primer_candidates,
             right_primer_candidates,
             log_file
         )
-        reporting.write_conserved_to_bed(probe_conserved_regions, data_dir, "probe")
+        # write files
+        reporting.write_regions_to_bed(probe_regions, data_dir, "probe")
         reporting.write_qpcr_to_files(results_dir, final_schemes, ambiguous_consensus)
         reporting.varvamp_plot(
             results_dir,
             alignment_cleaned,
-            conserved_regions,
-            probe_conserved_regions=probe_conserved_regions,
+            primer_regions,
+            probe_regions=probe_regions,
             amplicon_scheme=final_schemes
         )
         reporting.per_base_mismatch_plot(results_dir, final_schemes, args.threshold, mode="QPCR")
 
     # varVAMP finished
     logging.varvamp_progress(log_file, progress=1, start_time=start_time)
```

### Comparing `varvamp-0.7/varvamp/scripts/alignment.py` & `varvamp-0.8/varvamp/scripts/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 
     for sequence in AlignIO.read(alignment_path, "fasta"):
         alignment_list.append([sequence.id, str(sequence.seq)])
 
     return alignment_list
 
 
-def preprocess(alignment):
+def preprocess(alignment_path):
     """
     force nucleotides to lower and
     back transcripe if its RNA
     """
+
     preprocessed_alignment = []
+    # read alignment
+    alignment = read_alignment(alignment_path)
 
     for sequence in alignment:
         seq = Seq(sequence[1])
         seq = seq.lower()
         if "u" in seq:
             seq = seq.back_transcribe()
         preprocessed_alignment.append([sequence[0], str(seq)])
@@ -196,34 +199,32 @@
             masked_seq = masked_seq + mask
 
         cleaned_alignment.append([sequence[0], masked_seq])
 
     return cleaned_alignment
 
 
-def process_alignment(alignment_path, threshold):
+def process_alignment(preprocessed_alignment, threshold):
     """
     proprocesses alignment and cleans gaps
     """
-    alignment = read_alignment(alignment_path)
-    gap_cutoff = len(alignment)*(1-threshold)
+    gap_cutoff = len(preprocessed_alignment)*(1-threshold)
 
-    alignment_preprocessed = preprocess(alignment)
-    all_gaps = find_gaps_in_alignment(alignment_preprocessed)
+    all_gaps = find_gaps_in_alignment(preprocessed_alignment)
     unique_gaps = find_unique_gaps(all_gaps)
 
     if unique_gaps:
         gap_dic = create_gap_dictionary(unique_gaps, all_gaps)
         gaps_to_mask = find_gaps_to_mask(gap_dic, gap_cutoff)
         alignment_cleaned = clean_gaps(
-            alignment_preprocessed, gaps_to_mask
+            preprocessed_alignment, gaps_to_mask
         )
     else:
         gaps_to_mask = []
-        alignment_cleaned = alignment_preprocessed
+        alignment_cleaned = preprocessed_alignment
 
     return alignment_cleaned, gaps_to_mask
 
 
 def calculate_total_masked_gaps(gaps_to_mask):
     """
     calculates the cummulative length of gaps
```

### Comparing `varvamp-0.7/varvamp/scripts/config.py` & `varvamp-0.8/varvamp/scripts/config.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp/scripts/consensus.py` & `varvamp-0.8/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp/scripts/conserved.py` & `varvamp-0.8/varvamp/scripts/regions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,94 @@
 """
-finding and digesting conserved regions.
+finding and digesting potential primer regions.
 """
 
 # varVAMP
 from varvamp.scripts import config
 
 
 def find_regions(consensus_amb, allowed_ambiguous):
     """
-    finds conserved regions as specified by a
+    finds primer regions as specified by a
     certain amount of ambiguous bases in a given
     sequence length
     """
-    # init the variables
+
     current_window = []
-    writable = False
-    in_ambiguous_region = True
+    primer_regions = []
     last_amb = 0
-    conserved_regions = []
 
-    # append enough Ns to ensure that last window is closed
-    seq = str(consensus_amb) + allowed_ambiguous*'N'
+    # append one N so the last window is closed
+    seq = str(consensus_amb) + "N"
 
     for idx, nuc in enumerate(seq):
-        if in_ambiguous_region and nuc in config.NUCS:
-            in_ambiguous_region = False
-            # just entered a new stretch of non-ambiguous bases
-            # may be time to open a new window
-            if not current_window:
-                # track window start and ambiguous chars so far
-                current_window = [idx, 0]
-                all_previous_ambiguous_pos = []
-            continue
-        if nuc not in config.NUCS:
-            if current_window:
-                in_ambiguous_region = True
-                amb_to_amb_len = idx - last_amb
-                all_previous_ambiguous_pos.append(idx)
-                # check if there were too many previous amb char in subwindow
-                # or if N is reached -> writeable
-                if current_window[1] == allowed_ambiguous or nuc == "N":
-                    writable = True
-                    # are the current and last ambig char sufficiently far?
-                    if amb_to_amb_len >= config.PRIMER_SIZES[0] and nuc != "N":
-                        current_window[1] = 0
-                        all_previous_ambiguous_pos = [idx]
-                        writable = False
-
+        # open a new window if none is there and we have a nucleotide
+        if nuc in config.NUCS and not current_window:
+            current_window = [idx, 0]
+            all_previous_ambiguous_pos = []
+        # if we have a non-nucleotide, check if its time to writ the window
+        elif nuc not in config.NUCS and current_window:
+            # are the current and last ambig char sufficiently far?
+            if idx - last_amb >= config.PRIMER_SIZES[0] and nuc != "N":
+                current_window[1] = 1
+                all_previous_ambiguous_pos = [idx]
+            else:
                 current_window[1] += 1
-
-                if writable:
-                    writable = False
-                    # check if the writable window has a sufficient length.
-                    window_length = idx-current_window[0]
-                    if window_length >= config.PRIMER_SIZES[0]:
-                        conserved_regions.append([current_window[0], idx])
-                    # reset the window start to the last ambig char
-                    if nuc != "N":
-                        current_window[0] = all_previous_ambiguous_pos[0]+1
-                        current_window[1] = current_window[1] - 1
-                        all_previous_ambiguous_pos.pop(0)
-                    # or open a new window
-                    else:
-                        current_window = []
-
+                all_previous_ambiguous_pos.append(idx)
+            # check if there were too many previous amb char in subwindow
+            # or if N is reached -> writeable
+            if current_window[1] > allowed_ambiguous or nuc == "N":
+                # check if the writable window has a sufficient length.
+                if idx-current_window[0] >= config.PRIMER_SIZES[0]:
+                    primer_regions.append([current_window[0], idx])
+                # open new window if N is reached
+                if nuc == "N":
+                    current_window = []
+                # or reset to a previous ambig char
+                else:
+                    current_window[0] = all_previous_ambiguous_pos[0]+1
+                    current_window[1] = current_window[1] - 1
+                    all_previous_ambiguous_pos.pop(0)
             last_amb = idx
 
-    return conserved_regions
+    return primer_regions
 
 
-def mean(conserved_regions, consensus):
+def mean(primer_regions, consensus):
     """
     calculate the percentage of regions
-    that are conserved
+    that cover the consensus sequence
     """
     covered_set = set()
-    for region in conserved_regions:
+    for region in primer_regions:
         pos_list = list(range(region[0], region[1]))
         [covered_set.add(x) for x in pos_list]
     return round(len(covered_set)/len(consensus)*100, 1)
 
 
 def digest_seq(seq, kmer_size):
     """
     digest the sequence into kmers
     """
     return[[seq[i:i+kmer_size], i, i+len(seq[i:i+kmer_size])] for i in range(len(seq)-kmer_size+1)]
 
 
-def produce_kmers(conserved_regions, consensus, sizes=config.PRIMER_SIZES):
+def produce_kmers(primer_regions, consensus, sizes=config.PRIMER_SIZES):
     """
-    produce kmers for all conserved regions
+    produce kmers for all primer regions
     """
     kmers = []
 
-    for region in conserved_regions:
+    for region in primer_regions:
         sliced_seq = consensus[region[0]:region[1]]
         for kmer_size in range(sizes[0], sizes[1]+1):
             kmers_temp = digest_seq(sliced_seq, kmer_size)
             # adjust the start and stop position of the kmers
             for kmer_temp in kmers_temp:
                 kmer_temp[1] = kmer_temp[1]+region[0]
                 kmer_temp[2] = kmer_temp[2]+region[0]
+                # check if kmer is already in list (overlapping regions)
                 if kmer_temp in kmers:
                     continue
                 kmers.append(kmer_temp)
 
     return kmers
```

### Comparing `varvamp-0.7/varvamp/scripts/logging.py` & `varvamp-0.8/varvamp/scripts/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     os.makedirs(data_dir)
 
     log_file = os.path.join(results_dir, "varvamp_log.txt")
 
     return results_dir, data_dir, log_file
 
 
-def varvamp_progress(log_file, start_time=None, progress=0, job="", progress_text=""):
+def varvamp_progress(log_file, mode=None, start_time=None, progress=0, job="", progress_text=""):
     """
     progress bar, main progress logging and folder creation
     """
     barLength = 40
     block = int(round(barLength*progress))
 
     if progress == 0:
         print(
             "\nStarting \033[31m\033[1mvarVAMP ◥(ºwº)◤\033[0m primer design\n",
             flush=True
         )
         with open(log_file, 'w') as f:
-            f.write('VARVAMP log \n\n')
+            print(f"VARVAMP log \n\nMODE = {mode}\n", file=f)
     else:
         if progress == 1:
             stop_time = str(round(time.process_time() - start_time, 2))
             progress_text = f"all done \n\n\rvarVAMP finished in {stop_time} sec!\n{datetime.datetime.now()}"
             job = "Finalizing output."
         print(
             "\rJob:\t\t " + job + "\nProgress: \t [{0}] {1}%".format("█"*block + "-"*(barLength-block), progress*100) + "\t" + progress_text,
@@ -374,20 +374,15 @@
             log_file
         )
 
     # write all settings to file
     var_dic = vars(config)
     with open(log_file, 'a') as f:
         print(
-            f"MODE = {args.mode}",
-            sep="\n",
-            file=f
-        )
-        print(
-            "\nsettings that can be adjusted via arguments\n",
+            "\nARG SETTINGS\n",
             f"THRESHOLD = {args.threshold}",
             f"PRIMER_ALLOWED_N_AMB = {args.n_ambig}",
             sep="\n",
             file=f
         )
         if args.mode in ("tiled", "sanger"):
             print(
@@ -413,17 +408,17 @@
                 f"PROBE_ALLOWED_N_AMB = {args.pn_ambig}",
                 f"TEST_DELTAG_N_AMPLICONS = {args.test_n}",
                 f"DELTAG_CUTOFF = {args.deltaG}",
                 sep="\n",
                 file=f
             )
         print(
-            "\nconfig settings\n",
+            "\nCONFIG SETTINGS\n",
             sep="\n",
             file=f
         )
         for var in all_vars[0]:
             print(f"{var} = {var_dic[var]}", file=f)
         if args.mode == "qpcr":
             for var in all_vars[1]:
                 print(f"{var} = {var_dic[var]}", file=f)
-        print("\nprogress", file=f)
+        print("\nPROGRESS", file=f)
```

### Comparing `varvamp-0.7/varvamp/scripts/primers.py` & `varvamp-0.8/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp/scripts/qpcr.py` & `varvamp-0.8/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp/scripts/reporting.py` & `varvamp-0.8/varvamp/scripts/reporting.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,27 @@
     name = "alignment_cleaned.fasta"
     out = os.path.join(dir, name)
     with open(out, "w") as o:
         for seq in alignment:
             print(f">{seq[0]}\n{seq[1]}", file=o)
 
 
-def write_conserved_to_bed(conserved_regions, dir, mode=None):
+def write_regions_to_bed(primer_regions, dir, mode=None):
     """
-    write conserved regions as bed file
+    write primer regions as bed file
     """
 
     if mode == "probe":
-        outfile = f"{dir}probe_conserved_regions.bed"
+        outfile = f"{dir}probe_regions.bed"
     else:
-        outfile = f"{dir}primer_conserved_regions.bed"
+        outfile = f"{dir}primer_regions.bed"
     counter = 0
 
     with open(outfile, 'w') as o:
-        for region in conserved_regions:
+        for region in primer_regions:
             print(
                 "ambiguous_consensus",
                 region[0],
                 region[1],
                 "region_"+str(counter),
                 sep="\t",
                 file=o
@@ -366,22 +366,22 @@
     ax[0].set_xlim(0, max(entropy_df["position"]))
     ax[0].set_ylabel("alignment entropy")
     ax[0].set_title("final amplicon design")
     ax[0].spines['top'].set_visible(False)
     ax[0].spines['right'].set_visible(False)
 
 
-def conserved_subplot(ax, conserved_regions, location=0.95, color="darkorange", description="possible primer regions"):
+def region_subplot(ax, primer_regions, location=0.95, color="darkorange", description="possible primer regions"):
     """
-    creates the conserved regions subplot
+    creates the primer regions subplot
     """
-    for region in conserved_regions:
+    for region in primer_regions:
         ax[1].hlines(location, region[0], region[1], linewidth=5, color=color)
     # legend
-    ax[1].hlines(location, conserved_regions[0][1], conserved_regions[0][1], label=description, linewidth=5, color=color)
+    ax[1].hlines(location, primer_regions[0][1], primer_regions[0][1], label=description, linewidth=5, color=color)
 
 
 def all_primer_subplot(ax, all_primers):
     """
     creates the all primer subplot
     """
     for direction in all_primers:
@@ -391,16 +391,16 @@
             primer_label = "all right primers"
         elif direction == "+":
             primer_position = 0.8
             primer_color = "dimgrey"
             primer_label = "all left primers"
         for primer in all_primers[direction]:
             ax[1].hlines(primer_position, all_primers[direction][primer][1], all_primers[direction][primer][2], linewidth=5, color=primer_color)
-    # legend
-    ax[1].hlines(primer_position, all_primers[direction][primer][1], all_primers[direction][primer][2], linewidth=5, color=primer_color, label=primer_label)
+        # legend
+        ax[1].hlines(primer_position, all_primers[direction][primer][1], all_primers[direction][primer][2], linewidth=5, color=primer_color, label=primer_label)
 
 
 def amplicon_subplot(ax, amplicon_scheme):
     """
     creates the amplicon subplot
     """
     counter = 0
@@ -451,33 +451,33 @@
         counter += 1
     # legends
     ax[1].hlines(0.8, left[1]+config.PRIMER_SIZES[1], right[2]-config.PRIMER_SIZES[1], linewidth=5, label="amplicons")
     ax[1].hlines(0.8, left[1], left[2], linewidth=5, color="red", label="primers")
     ax[1].hlines(0.75, probe[1], probe[2], linewidth=5, color="darkgrey", label="probe")
 
 
-def varvamp_plot(dir, alignment_cleaned, conserved_regions, all_primers=None, amplicon_scheme=None, probe_conserved_regions=None):
+def varvamp_plot(dir, alignment_cleaned, primer_regions, all_primers=None, amplicon_scheme=None, probe_regions=None):
     """
     creates overview plot for the amplicon design
     and per base coverage plots
     """
     # first plot: overview
     # create pdf name
     name = "amplicon_plot.pdf"
     out = os.path.join(dir, name)
     # ini figure
     fig, ax = plt.subplots(2, 1, figsize=[22, 6], squeeze=True, sharex=True, gridspec_kw={'height_ratios': [4, 1]})
     fig.subplots_adjust(hspace=0)
     # entropy plot
     entropy_subplot(ax, alignment_cleaned)
-    # conserved regions plot
-    conserved_subplot(ax, conserved_regions)
-    # conserved region plot for probes
-    if probe_conserved_regions is not None and amplicon_scheme is not None:
-        conserved_subplot(ax, probe_conserved_regions, 0.9, color="dimgrey", description="possible probe regions")
+    # primer regions plot
+    region_subplot(ax, primer_regions)
+    # probe region plot for probes
+    if probe_regions is not None and amplicon_scheme is not None:
+        region_subplot(ax, probe_regions, 0.9, color="dimgrey", description="possible probe regions")
         qpcr_subplot(ax, amplicon_scheme)
     # all primer plot
     elif all_primers is not None and amplicon_scheme is not None:
         all_primer_subplot(ax, all_primers)
         # amplicon, text and primer plot
         amplicon_subplot(ax, amplicon_scheme)
     # finalize
```

### Comparing `varvamp-0.7/varvamp/scripts/scheme.py` & `varvamp-0.8/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.7/varvamp.egg-info/PKG-INFO` & `varvamp-0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-Metadata-Version: 2.1
-Name: varvamp
-Version: 0.7
-Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
-Home-page: https://github.com/jonas-fuchs/varVAMP
-Author: Dr. Jonas Fuchs
-Author-email: jonas.fuchs@uniklinik-freiburg.de
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 **var**iable **V**irus**AMP**licons (varVAMP) is a tool to design primers for highly diverse viruses. The input is an alignment of your viral (full-genome) sequences.
 
 # varVAMP
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
-<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg /> 
+<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
+<img src="./docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
+<img src="./docs/sanger.png" alt="sanger" />
+
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
+<img src="./docs/tiled.png" alt="tiled" />
+
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
+<img src="./docs/qpcr.png" alt="qpcr" />
+
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
```

### Comparing `varvamp-0.7/varvamp.egg-info/SOURCES.txt` & `varvamp-0.8/varvamp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 varvamp.egg-info/not-zip-safe
 varvamp.egg-info/requires.txt
 varvamp.egg-info/top_level.txt
 varvamp/scripts/__init__.py
 varvamp/scripts/alignment.py
 varvamp/scripts/config.py
 varvamp/scripts/consensus.py
-varvamp/scripts/conserved.py
 varvamp/scripts/logging.py
+varvamp/scripts/param_estimation.py
 varvamp/scripts/primers.py
 varvamp/scripts/qpcr.py
+varvamp/scripts/regions.py
 varvamp/scripts/reporting.py
 varvamp/scripts/scheme.py
```

