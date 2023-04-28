# Comparing `tmp/midsv-0.9.0.zip` & `tmp/midsv-0.9.5.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 17581 bytes, number of entries: 20
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-16 20:55 midsv-0.9.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-16 20:55 midsv-0.9.0/src/
--rw-r--r--  2.0 unx     1069 b- defN 23-Mar-16 20:55 midsv-0.9.0/LICENSE
--rw-r--r--  2.0 unx     6072 b- defN 23-Mar-16 20:55 midsv-0.9.0/README.md
--rw-r--r--  2.0 unx     6714 b- defN 23-Mar-16 20:55 midsv-0.9.0/PKG-INFO
--rw-r--r--  2.0 unx      893 b- defN 23-Mar-16 20:55 midsv-0.9.0/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-16 20:55 midsv-0.9.0/setup.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-16 20:55 midsv-0.9.0/src/midsv.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-16 20:55 midsv-0.9.0/src/midsv/
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      300 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     6714 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv.egg-info/top_level.txt
--rw-r--r--  2.0 unx      146 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/__init__.py
--rw-r--r--  2.0 unx     7318 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/format.py
--rw-r--r--  2.0 unx     1896 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/main.py
--rw-r--r--  2.0 unx      893 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/io.py
--rw-r--r--  2.0 unx     8916 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/convert.py
--rw-r--r--  2.0 unx     1559 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/validate.py
--rw-r--r--  2.0 unx     5933 b- defN 23-Mar-16 20:55 midsv-0.9.0/src/midsv/proofread.py
-20 files, 48468 bytes uncompressed, 14885 bytes compressed:  69.3%
+Zip file size: 17709 bytes, number of entries: 20
+drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 02:42 midsv-0.9.5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 02:42 midsv-0.9.5/src/
+-rw-r--r--  2.0 unx     1069 b- defN 23-Mar-22 02:41 midsv-0.9.5/LICENSE
+-rw-r--r--  2.0 unx     6072 b- defN 23-Mar-22 02:41 midsv-0.9.5/README.md
+-rw-r--r--  2.0 unx     6714 b- defN 23-Mar-22 02:42 midsv-0.9.5/PKG-INFO
+-rw-r--r--  2.0 unx      907 b- defN 23-Mar-22 02:41 midsv-0.9.5/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Mar-22 02:42 midsv-0.9.5/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 02:42 midsv-0.9.5/src/midsv.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 02:42 midsv-0.9.5/src/midsv/
+-rw-r--r--  2.0 unx        1 b- defN 23-Mar-22 02:42 midsv-0.9.5/src/midsv.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      300 b- defN 23-Mar-22 02:42 midsv-0.9.5/src/midsv.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     6714 b- defN 23-Mar-22 02:42 midsv-0.9.5/src/midsv.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        6 b- defN 23-Mar-22 02:42 midsv-0.9.5/src/midsv.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      146 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/__init__.py
+-rw-r--r--  2.0 unx     7414 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/format.py
+-rw-r--r--  2.0 unx     1982 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/main.py
+-rw-r--r--  2.0 unx      893 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/io.py
+-rw-r--r--  2.0 unx     8916 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/convert.py
+-rw-r--r--  2.0 unx     1559 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/validate.py
+-rw-r--r--  2.0 unx     6702 b- defN 23-Mar-22 02:41 midsv-0.9.5/src/midsv/proofread.py
+20 files, 49433 bytes uncompressed, 15013 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,61 +1,61 @@
-Filename: midsv-0.9.0/
+Filename: midsv-0.9.5/
 Comment: 
 
-Filename: midsv-0.9.0/src/
+Filename: midsv-0.9.5/src/
 Comment: 
 
-Filename: midsv-0.9.0/LICENSE
+Filename: midsv-0.9.5/LICENSE
 Comment: 
 
-Filename: midsv-0.9.0/README.md
+Filename: midsv-0.9.5/README.md
 Comment: 
 
-Filename: midsv-0.9.0/PKG-INFO
+Filename: midsv-0.9.5/PKG-INFO
 Comment: 
 
-Filename: midsv-0.9.0/setup.py
+Filename: midsv-0.9.5/setup.py
 Comment: 
 
-Filename: midsv-0.9.0/setup.cfg
+Filename: midsv-0.9.5/setup.cfg
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv.egg-info/
+Filename: midsv-0.9.5/src/midsv.egg-info/
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/
+Filename: midsv-0.9.5/src/midsv/
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv.egg-info/dependency_links.txt
+Filename: midsv-0.9.5/src/midsv.egg-info/dependency_links.txt
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv.egg-info/SOURCES.txt
+Filename: midsv-0.9.5/src/midsv.egg-info/SOURCES.txt
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv.egg-info/PKG-INFO
+Filename: midsv-0.9.5/src/midsv.egg-info/PKG-INFO
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv.egg-info/top_level.txt
+Filename: midsv-0.9.5/src/midsv.egg-info/top_level.txt
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/__init__.py
+Filename: midsv-0.9.5/src/midsv/__init__.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/format.py
+Filename: midsv-0.9.5/src/midsv/format.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/main.py
+Filename: midsv-0.9.5/src/midsv/main.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/io.py
+Filename: midsv-0.9.5/src/midsv/io.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/convert.py
+Filename: midsv-0.9.5/src/midsv/convert.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/validate.py
+Filename: midsv-0.9.5/src/midsv/validate.py
 Comment: 
 
-Filename: midsv-0.9.0/src/midsv/proofread.py
+Filename: midsv-0.9.5/src/midsv/proofread.py
 Comment: 
 
 Zip file comment:
```

## Comparing `midsv-0.9.0/LICENSE` & `midsv-0.9.5/LICENSE`

 * *Files identical despite different names*

## Comparing `midsv-0.9.0/README.md` & `midsv-0.9.5/README.md`

 * *Files identical despite different names*

## Comparing `midsv-0.9.0/PKG-INFO` & `midsv-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midsv
-Version: 0.9.0
+Version: 0.9.5
 Summary: Python module to convert SAM to MIDSV format.
 Home-page: https://github.com/akikuno/midsv
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `midsv-0.9.0/setup.py` & `midsv-0.9.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="midsv",
-    version="0.9.0",
+    version="0.9.5",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="Python module to convert SAM to MIDSV format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/midsv",
-    packages=setuptools.find_packages(where="src",),
+    packages=setuptools.find_packages(
+        where="src",
+    ),
     package_dir={"": "src"},
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

## Comparing `midsv-0.9.0/src/midsv.egg-info/PKG-INFO` & `midsv-0.9.5/src/midsv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midsv
-Version: 0.9.0
+Version: 0.9.5
 Summary: Python module to convert SAM to MIDSV format.
 Home-page: https://github.com/akikuno/midsv
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `midsv-0.9.0/src/midsv/format.py` & `midsv-0.9.5/src/midsv/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,54 +98,52 @@
             right = int(right[:-1])
             alignment["SEQ"] = alignment["SEQ"][:-right]
             alignment["QUAL"] = alignment["QUAL"][:-right]
         sam_list.append(alignment)
     return sam_list
 
 
-def return_end_of_current_read(alignment:dict) -> int:
+def return_end_of_current_read(alignment: dict) -> int:
     start_of_current_read = alignment["POS"]
     cigar = alignment["CIGAR"]
     cigar_split = split_cigar(cigar)
     alignment_length = 0
     for cig in cigar_split:
         if "M" in cig or "D" in cig or "N" in cig:
             alignment_length += int(cig[:-1])
     return start_of_current_read + alignment_length - 1
 
 
 def realign_sequence(alignment: dict) -> dict:
-    """Discard insertion, and add deletion and spliced nucreotide to unify sequence length
-    """
+    """Discard insertion, and add deletion and spliced nucreotide to unify sequence length"""
     cigar = alignment["CIGAR"]
     cigar_split = split_cigar(cigar)
     sequence = alignment["SEQ"]
     sequence_ignored = ["N"] * alignment["POS"]
     start = 0
     for cig in cigar_split:
         if "M" in cig:
             end = start + int(cig[:-1])
-            sequence_ignored.append(sequence[start: end])
+            sequence_ignored.append(sequence[start:end])
             start = end
         elif "I" in cig:
             start += int(cig[:-1])
         elif any(x in cig for x in ["D", "N"]):
             sequence_ignored.append("N" * int(cig[:-1]))
     realignment = deepcopy(alignment)
     realignment["SEQ"] = "".join(sequence_ignored)
     return realignment
 
 
-
 def remove_resequence(samdict: list[list]) -> list[list]:
     """Remove non-microhomologic overlapped reads within the same QNAME.
     The overlapped sequences can be (1) realignments by microhomology or (2) resequence by sequencing error.
     The 'realignments' is not sequencing errors, and it preserves the same sequence.
     In contrast, the 'resequence' is a sequencing error with the following characteristics:
-    (1) The shorter reads are completely included in the longer reads
+    (1) The shorter reads that are completely included in the longer reads
     (2) Overlapped but not the same DNA sequence
     The resequenced fragments will be discarded and the longest alignment will be retain.
     Example reads are in `tests/data/overlap/real_overlap.sam` and `tests/data/overlap/real_overlap2.sam`
 
     Args:
         sam (list[list]): disctionalized SAM
 
@@ -157,40 +155,43 @@
     sam_nonoverlapped = []
     for _, alignments in sam_groupby:
         alignments = list(alignments)
         if len(alignments) == 1:
             sam_nonoverlapped += alignments
             continue
         alignments = [realign_sequence(alignment) for alignment in alignments]
-        alignments = sorted(alignments, key=lambda x: [x["POS"], -len(x["SEQ"])])
+        alignments = sorted(alignments, key=lambda x: [x["POS"]])
         is_overraped = False
         end_of_previous_read = -1
         previous_read = alignments[0]["SEQ"]
         for i, alignment in enumerate(alignments):
             if i == 0:
                 start_of_previous_read = alignment["POS"] - 1
                 end_of_previous_read = return_end_of_current_read(alignment)
                 continue
             start_of_current_read = alignment["POS"] - 1
             end_of_current_read = return_end_of_current_read(alignment)
-            # (1) The shorter reads are completely included in the longer reads
+            # (1) The shorter reads that are completely included in the longer reads
             if start_of_previous_read <= start_of_current_read and end_of_previous_read >= end_of_current_read:
                 is_overraped = True
                 break
             else:
                 start_overlap = max(start_of_previous_read, start_of_current_read)
                 end_overlap = min(end_of_previous_read, end_of_current_read)
-                for prev, curr in zip(previous_read[start_overlap: end_overlap], alignment["SEQ"][start_overlap: end_overlap]):
+                for prev, curr in zip(
+                    previous_read[start_overlap:end_overlap], alignment["SEQ"][start_overlap:end_overlap]
+                ):
                     if prev == "N" or curr == "N":
                         continue
                     # (2) Overlapped but not the same DNA sequence
                     if prev != curr:
                         is_overraped = True
                         break
             start_of_previous_read = start_of_current_read
             end_of_previous_read = return_end_of_current_read(alignment)
         if is_overraped:
             # The longest alignment will be retain
-            sam_nonoverlapped.append(alignments[0])
+            alignment = sorted(alignments, key=lambda x: -len(x["SEQ"]))[0]
+            sam_nonoverlapped.append(alignment)
         else:
             sam_nonoverlapped += alignments
     return sam_nonoverlapped
```

## Comparing `midsv-0.9.0/src/midsv/main.py` & `midsv-0.9.5/src/midsv/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,9 +44,10 @@
         if midsv and qscore:
             alignment["QSCORE"] = convert.qual_to_qscore_midsv(alignment["QUAL"], alignment["MIDSV"])
         elif cssplit and qscore:
             alignment["QSCORE"] = convert.qual_to_qscore_cssplit(alignment["QUAL"], alignment["CSSPLIT"])
 
     samdict_polished = proofread.join(samdict)
     samdict_polished = proofread.pad(samdict_polished, sqheaders)
+    samdict_polished = proofread.remove_different_length(samdict_polished, sqheaders)
     samdict_polished = proofread.select(samdict_polished)
     return samdict_polished
```

## Comparing `midsv-0.9.0/src/midsv/io.py` & `midsv-0.9.5/src/midsv/io.py`

 * *Files identical despite different names*

## Comparing `midsv-0.9.0/src/midsv/convert.py` & `midsv-0.9.5/src/midsv/convert.py`

 * *Files identical despite different names*

## Comparing `midsv-0.9.0/src/midsv/validate.py` & `midsv-0.9.5/src/midsv/validate.py`

 * *Files identical despite different names*

## Comparing `midsv-0.9.0/src/midsv/proofread.py` & `midsv-0.9.5/src/midsv/proofread.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,14 +114,37 @@
             alignment["CSSPLIT"] = leftpad_cssplit + alignment["CSSPLIT"] + rightpad_cssplit
         if "QSCORE" in alignment:
             alignment["QSCORE"] = leftpad_qscore + alignment["QSCORE"] + rightpad_qscore
         samdict_padding.append(alignment)
     return samdict_padding
 
 
+def remove_different_length(samdict: list[dict], sqheaders: dict) -> list[dict]:
+    """remove different sequence length of the reference
+
+    Args:
+        sam (list[dict]): dictionarized SAM
+        sqheaders (dict): dictionary as {SQ:LN}
+
+    Returns:
+        list[dict]: filtered SAM by different sequence length of the reference
+    """
+    samdict_filtered = []
+    for alignment in samdict:
+        reflength = sqheaders[alignment["RNAME"]]
+        if "MIDSV" in alignment:
+            if len(alignment["MIDSV"].split(",")) != reflength:
+                continue
+        if "CSSPLIT" in alignment:
+            if len(alignment["CSSPLIT"].split(",")) != reflength:
+                continue
+        samdict_filtered.append(alignment)
+    return samdict_filtered
+
+
 def select(samdict: list[dict]) -> list[dict]:
     """Select QNAME, RNAME, MIDSV, CSSPLIT and QSCORE
 
     Args:
         sam (list[dict]): dictionarized SAM
 
     Returns:
```

