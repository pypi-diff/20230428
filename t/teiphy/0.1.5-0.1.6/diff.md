# Comparing `tmp/teiphy-0.1.5.tar.gz` & `tmp/teiphy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teiphy-0.1.5.tar", max compression
+gzip compressed data, was "teiphy-0.1.6.tar", max compression
```

## Comparing `teiphy-0.1.5.tar` & `teiphy-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-01-10 07:58:11.364932 teiphy-0.1.5/LICENSE
--rw-r--r--   0        0        0     5587 2023-01-10 07:58:11.364932 teiphy-0.1.5/README.rst
--rw-r--r--   0        0        0     1560 2023-01-10 07:58:11.368932 teiphy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      195 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/__init__.py
--rw-r--r--   0        0        0    75508 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/collation.py
--rw-r--r--   0        0        0      134 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/common.py
--rw-r--r--   0        0        0     1034 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/format.py
--rw-r--r--   0        0        0     5635 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/main.py
--rw-r--r--   0        0        0    13304 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/reading.py
--rw-r--r--   0        0        0     4680 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/variation_unit.py
--rw-r--r--   0        0        0     2860 2023-01-10 07:58:11.368932 teiphy-0.1.5/teiphy/witness.py
--rw-r--r--   0        0        0     6667 1970-01-01 00:00:00.000000 teiphy-0.1.5/setup.py
--rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 teiphy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-28 01:39:41.881352 teiphy-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5898 2023-04-28 01:39:41.881352 teiphy-0.1.6/README.rst
+-rw-r--r--   0        0        0     1578 2023-04-28 01:39:41.885352 teiphy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      195 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/__init__.py
+-rw-r--r--   0        0        0   112319 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/collation.py
+-rw-r--r--   0        0        0      134 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/common.py
+-rw-r--r--   0        0        0     1085 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/format.py
+-rw-r--r--   0        0        0     5929 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/main.py
+-rw-r--r--   0        0        0    12734 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/reading.py
+-rw-r--r--   0        0        0    18773 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/templates/beast_template.xml
+-rw-r--r--   0        0        0     7939 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/variation_unit.py
+-rw-r--r--   0        0        0     3034 2023-04-28 01:39:41.885352 teiphy-0.1.6/teiphy/witness.py
+-rw-r--r--   0        0        0     7354 1970-01-01 00:00:00.000000 teiphy-0.1.6/PKG-INFO
```

### Comparing `teiphy-0.1.5/LICENSE` & `teiphy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `teiphy-0.1.5/README.rst` & `teiphy-0.1.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. start-badges
 
 .. image:: https://raw.githubusercontent.com/jjmccollum/teiphy/main/docs/img/teiphy-logo.svg
 
 |license badge| |testing badge| |coverage badge| |docs badge| |black badge| |git3moji badge| 
-|iqtree badge| |raxml badge| |mrbayes badge| |stemma badge| |joss badge| |doi badge|
+|iqtree badge| |raxml badge| |mrbayes badge| |beast badge| |stemma badge| |joss badge| |doi badge|
 
 .. |license badge| image:: https://img.shields.io/badge/license-MIT-blue.svg?style=flat
     :target: https://choosealicense.com/licenses/mit/
 
 .. |testing badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml
 
@@ -28,14 +28,17 @@
 
 .. |raxml badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml/badge.svg
     :target: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml
 
 .. |mrbayes badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml/badge.svg
     :target: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml
 
+.. |beast badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/beast.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/beast.yml
+
 .. |stemma badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml/badge.svg
     :target: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml
 
 .. |joss badge| image:: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b/status.svg
     :target: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b
     
 .. |doi badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7455638.svg
@@ -47,15 +50,15 @@
 
 A Python package for converting TEI XML collations to NEXUS and other formats.
 
 Textual scholars have been using phylogenetics to analyze manuscript traditions since the early 1990s.
 Many standard phylogenetic software packages accept as input the `NEXUS file format <https://doi.org/10.1093/sysbio/46.4.590>`_.
 The ``teiphy`` program takes a collation of texts encoded using the `Text Encoding Initiative (TEI) guidelines <https://tei-c.org/release/doc/tei-p5-doc/en/html/TC.html>`_
 and converts it to a NEXUS format so that it can be used for phylogenetic analysis.
-It can also convert to other formats as well.
+It can also convert to other formats as well, including Hennig86 (for TNT), PHYLIP (for RAxML), FASTA, and the XML format used by BEAST 2.7.
 
 
 .. end-about
 
 
 .. start-quickstart
 
@@ -87,17 +90,17 @@
 
 To use the software, run the ``teiphy`` command line tool:
 
 .. code-block:: bash
 
     teiphy <input TEI XML> <output file>
 
-``teiphy`` can export to NEXUS, Hennig86 (TNT), PHYLIP (in the relaxed form used by RAxML), FASTA, CSV, TSV, Excel and STEMMA formats. 
+``teiphy`` can export to NEXUS, Hennig86 (TNT), PHYLIP (in the relaxed form used by RAxML), FASTA, BEAST 2.7 XML, CSV, TSV, Excel and STEMMA formats. 
 ``teiphy`` will try to infer the file format to export to from the extension of the output file. Accepted file extensions are:
-".nex", ".nexus", ".nxs", ".ph", ".phy", ".fa", ".fasta", ".tnt", ".csv", ".tsv", ".xlsx".
+".nex", ".nexus", ".nxs", ".ph", ".phy", ".fa", ".fasta", ".xml", ".tnt", ".csv", ".tsv", ".xlsx".
 
 To explicitly say which format you wish to export to, use the ``--format`` option. For example:
 
 .. code-block:: bash
 
     teiphy <input TEI XML> <output file> --format nexus
```

### Comparing `teiphy-0.1.5/pyproject.toml` & `teiphy-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teiphy"
-version = "0.1.5"
+version = "0.1.6"
 description = "Converts TEI XML collations to NEXUS and other formats"
 authors = ["Joey McCollum and Robert Turnbull"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/jjmccollum/teiphy"
 repository = "https://github.com/jjmccollum/teiphy"
 documentation = "https://jjmccollum.github.io/teiphy/"
@@ -26,14 +26,15 @@
 lxml = "^4.9.1"
 numpy = "^1.23.2"
 pandas = "^1.4.4"
 openpyxl = "^3.0.10"
 typer = "^0.6.1"
 rich = "^12.5.1"
 python-slugify = "^6.1.2"
+Jinja2 = "^3.1.2"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^5.1.1"
 pytest = "^7.2.0"
 coverage = "^6.4.4"
 nbsphinx = "^0.8.9"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `teiphy-0.1.5/teiphy/collation.py` & `teiphy-0.1.6/teiphy/collation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 #!/usr/bin/env python3
 
+from enum import Enum
 from typing import List, Union
 from pathlib import Path
+from datetime import datetime  # for calculating the current year (for dating and tree height purposes)
 import time  # to time calculations for users
 import string  # for easy retrieval of character ranges
 from lxml import etree as et  # for reading TEI XML inputs
 import numpy as np  # for collation matrix outputs
 import pandas as pd  # for writing to DataFrames, CSV, Excel, etc.
 from slugify import slugify  # for converting Unicode text from readings to ASCII for NEXUS
+from jinja2 import Environment, PackageLoader, select_autoescape  # for filling output XML templates
 
 from .common import xml_ns, tei_ns
 from .format import Format
 from .witness import Witness
 from .variation_unit import VariationUnit
 
 
 class ParsingException(Exception):
     pass
 
 
+class WitnessDateException(Exception):
+    pass
+
+
+class IntrinsicRelationsException(Exception):
+    pass
+
+
+class ClockModel(str, Enum):
+    strict = "strict"
+    uncorrelated = "uncorrelated"
+    local = "local"
+
+
 class Collation:
     """Base class for storing TEI XML collation data internally.
 
     This corresponds to the entire XML tree, rooted at the TEI element of the collation.
 
     Attributes:
         manuscript_suffixes: A list of suffixes used to distinguish manuscript subwitnesses like first hands, correctors, main texts, alternate texts, and multiple attestations from their base witnesses.
@@ -31,24 +48,26 @@
         fill_corrector_lacunae: A boolean flag indicating whether or not to fill "lacunae" in witnesses with type "corrector".
         witnesses: A list of Witness instances contained in this Collation.
         witness_index_by_id: A dictionary mapping base witness ID strings to their int indices in the witnesses list.
         variation_units: A list of VariationUnit instances contained in this Collation.
         readings_by_witness: A dictionary mapping base witness ID strings to lists of reading support coefficients for all units (with at least two substantive readings).
         substantive_variation_unit_ids: A list of ID strings for variation units with two or more substantive readings.
         substantive_variation_unit_reading_tuples: A list of (variation unit ID, reading ID) tuples for substantive readings.
+        origin_date_range: A list containing lower and upper bounds on the origin date of the collated work.
         verbose: A boolean flag indicating whether or not to print timing and debugging details for the user.
     """
 
     def __init__(
         self,
         xml: et.ElementTree,
         manuscript_suffixes: List[str] = [],
         trivial_reading_types: List[str] = [],
         missing_reading_types: List[str] = [],
         fill_corrector_lacunae: bool = False,
+        origin_date_range: List[int] = [],
         verbose: bool = False,
     ):
         """Constructs a new Collation instance with the given settings.
 
         Args:
             xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
             manuscript_suffixes: An optional list of suffixes used to distinguish manuscript subwitnesses like first hands, correctors, main texts, alternate texts, and multiple attestations from their base witnesses.
@@ -65,26 +84,70 @@
         self.witnesses = []
         self.witness_index_by_id = {}
         self.variation_units = []
         self.readings_by_witness = {}
         self.variation_unit_ids = []
         self.substantive_variation_unit_reading_tuples = []
         self.substantive_readings_by_variation_unit_id = {}
+        self.intrinsic_categories = []
+        self.intrinsic_odds_by_id = {}
+        self.transcriptional_categories = []
+        self.transcriptional_rates_by_id = {}
+        self.origin_date_range = []
         # Now parse the XML tree to populate these data structures:
         if self.verbose:
             print("Initializing collation...")
         t0 = time.time()
+        self.parse_origin_date_range(xml)
         self.parse_list_wit(xml)
         self.validate_wits(xml)
+        self.update_origin_date_range_from_witness_date_ranges()
+        if self.origin_date_range[0] is not None:
+            self.update_witness_date_ranges_from_origin_date_range()
+        self.parse_intrinsic_odds(xml)
+        self.parse_transcriptional_rates(xml)
         self.parse_apps(xml)
+        self.validate_intrinsic_relations()
         self.parse_readings_by_witness()
         t1 = time.time()
         if self.verbose:
             print("Total time to initialize collation: %0.4fs." % (t1 - t0))
 
+    def parse_origin_date_range(self, xml: et.ElementTree):
+        """Given an XML tree for a collation, populates this Collation's list of origin date bounds.
+        If no bounds are specified, then the current year is set to the default upper bound.
+
+        Args:
+            xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
+        """
+        if self.verbose:
+            print("Parsing origin date range...")
+        t0 = time.time()
+        self.origin_date_range = [None, datetime.now().year]
+        for date in xml.xpath(
+            "//tei:sourceDesc//tei:bibl//tei:date|//tei:sourceDesc//tei:biblStruct//tei:date|//tei:sourceDesc//tei:biblFull//tei:date",
+            namespaces={"tei": tei_ns},
+        ):
+            # Try the @when attribute first; if it is set, then it accounts for both ends of the date range:
+            if date.get("when") is not None:
+                self.origin_date_range[0] = int(date.get("when").split("-")[0])
+                self.origin_date_range[1] = self.origin_date_range[0]
+            # Failing that, if it has @from and @to attributes (indicating the period over which the work was completed),
+            # then the completion date of the work accounts for both ends of the date range:
+            elif date.get("to") is not None:
+                self.origin_date_range[0] = int(date.get("to").split("-")[0])
+                self.origin_date_range[1] = self.origin_date_range[0]
+            # Failing that, set lower and upper bounds on the origin date using the the @notBefore and @notAfter attributes:
+            elif date.get("notBefore") is not None or date.get("notAfter") is not None:
+                if date.get("notBefore") is not None:
+                    self.origin_date_range[0] = int(date.get("notBefore").split("-")[0])
+                if date.get("notAfter") is not None:
+                    self.origin_date_range[1] = int(date.get("notAfter").split("-")[0])
+        return
+
     def get_base_wit(self, wit: str):
         """Given a witness siglum, strips of the specified manuscript suffixes until the siglum matches one in the witness list or until no more suffixes can be stripped.
 
         Args:
             wit: A string representing a witness siglum, potentially including suffixes to be stripped.
         """
         base_wit = wit
@@ -150,14 +213,16 @@
             print("Finished processing %d witnesses in %0.4fs." % (len(self.witnesses), t1 - t0))
         return
 
     def validate_wits(self, xml: et.ElementTree):
         """Given an XML tree for a collation, checks if any witness sigla listed in a rdg, rdgGrp, or witDetail element,
         once stripped of ignored suffixes, is not found in the witness list.
         A warning will be issued for each distinct siglum like this.
+        This method also checks if the upper bound of any witness's date is earlier than the lower bound on the collated work's date of origin
+        and throws an exception if so.
 
         Args:
             xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
         """
         if self.verbose:
             print("Validating witness list against collation...")
         t0 = time.time()
@@ -177,19 +242,187 @@
                         extra_sigla.append(base_siglum)
         if len(extra_sigla) > 0:
             extra_sigla.sort()
             msg = ""
             msg += "WARNING: The following sigla occur in the collation that do not have corresponding witness entries in the listWit:\n"
             msg += ", ".join(extra_sigla)
             print(msg)
+        # If the lower bound on the date of origin is defined, then check each witness against it:
+        if self.origin_date_range[0] is not None:
+            bad_date_witness_sigla = []
+            bad_date_upper_bounds_by_witness = {}
+            for i, wit in enumerate(self.witnesses):
+                if wit.date_range[1] is not None and wit.date_range[1] < self.origin_date_range[0]:
+                    bad_date_witness_sigla.append(wit.id)
+                    bad_date_upper_bounds_by_witness[wit.id] = wit.date_range[1]
+            if len(bad_date_witness_sigla) > 0:
+                msg = ""
+                msg += "The following witnesses have their latest possible dates before the earliest date of origin %d specified for the collated work:\n"
+                msg += ", ".join(
+                    [
+                        (siglum + "(" + str(bad_date_upper_bounds_by_witness[siglum]) + ")")
+                        for siglum in bad_date_witness_sigla
+                    ]
+                )
+                raise WitnessDateException(msg)
         t1 = time.time()
         if self.verbose:
             print("Finished witness validation in %0.4fs." % (t1 - t0))
         return
 
+    def update_origin_date_range_from_witness_date_ranges(self):
+        """Conditionally updates the upper bound on the date of origin of the work represented by this Collation
+        based on the upper bounds on the witnesses' dates.
+        Since all witness dates have a default upper bound on the current year, they are assumed to be defined.
+        """
+        if self.verbose:
+            print("Updating upper bound on origin date using witness dates...")
+        t0 = time.time()
+        # Set the origin date to the earliest witness date upper bound:
+        min_witness_date_upper_bound = min([wit.date_range[1] for wit in self.witnesses])
+        self.origin_date_range[1] = min(self.origin_date_range[1], min_witness_date_upper_bound)
+        t1 = time.time()
+        if self.verbose:
+            print("Finished updating upper bound on origin date in %0.4fs." % (t1 - t0))
+        return
+
+    def update_witness_date_ranges_from_origin_date_range(self):
+        """Attempts to update the lower bounds on the witnesses' dates of origin of the work represented by this Collation
+        using the lower bound on the date of origin of the work represented by this Collation.
+        This method is only invoked if the collated work has a lower bound on its date of origin specified.
+        """
+        if self.verbose:
+            print("Updating lower bounds on witness dates using origin date...")
+        t0 = time.time()
+        # Set the origin date to the earliest witness date upper bound:
+        for i, wit in enumerate(self.witnesses):
+            wit.date_range[0] = (
+                max(wit.date_range[0], self.origin_date_range[0])
+                if wit.date_range[0] is not None
+                else self.origin_date_range[0]
+            )
+        t1 = time.time()
+        if self.verbose:
+            print("Finished updating lower bounds on witness dates in %0.4fs." % (t1 - t0))
+        return
+
+    def parse_intrinsic_odds(self, xml: et.ElementTree):
+        """Given an XML tree for a collation, populates this Collation's list of intrinsic probability categories
+        (e.g., "absolutely more likely," "highly more likely," "more likely," "slightly more likely," "equally likely")
+        and its dictionary mapping these categories to numerical odds.
+        If a category does not contain a certainty element specifying its number, then it will be assumed to be a parameter to be estimated.
+
+        Args:
+            xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
+        """
+        if self.verbose:
+            print("Parsing intrinsic odds categories...")
+        t0 = time.time()
+        self.intrinsic_categories = []
+        self.intrinsic_odds_by_id = {}
+        for interp in xml.xpath("//tei:interpGrp[@type=\"intrinsic\"]/tei:interp", namespaces={"tei": tei_ns}):
+            # These must be indexed by the xml:id attribute, so skip any that do not have one:
+            if interp.get("{%s}id" % xml_ns) is None:
+                continue
+            odds_category = interp.get("{%s}id" % xml_ns)
+            # If this element contains a certainty subelement with a fixed odds value for this category, then set it:
+            odds = None
+            for certainty in interp.xpath("./tei:certainty", namespaces={"tei": tei_ns}):
+                if certainty.get("degree") is not None:
+                    odds = float(certainty.get("degree"))
+                    break
+            self.intrinsic_categories.append(odds_category)
+            self.intrinsic_odds_by_id[odds_category] = odds
+        t1 = time.time()
+        if self.verbose:
+            print(
+                "Finished processing %d intrinsic odds categories in %0.4fs."
+                % (len(self.intrinsic_categories), t1 - t0)
+            )
+        return
+
+    def parse_transcriptional_rates(self, xml: et.ElementTree):
+        """Given an XML tree for a collation, populates this Collation's dictionary mapping transcriptional change categories
+        (e.g., "aural confusion," "visual error," "clarification") to numerical rates.
+        If a category does not contain a certainty element specifying its number, then it will be assumed to be a parameter to be estimated.
+
+        Args:
+            xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
+        """
+        if self.verbose:
+            print("Parsing transcriptional change categories...")
+        t0 = time.time()
+        self.transcriptional_categories = []
+        self.transcriptional_rates_by_id = {}
+        for interp in xml.xpath("//tei:interpGrp[@type=\"transcriptional\"]/tei:interp", namespaces={"tei": tei_ns}):
+            # These must be indexed by the xml:id attribute, so skip any that do not have one:
+            if interp.get("{%s}id" % xml_ns) is None:
+                continue
+            transcriptional_category = interp.get("{%s}id" % xml_ns)
+            # If this element contains a certainty subelement with a fixed rate for this category, then set it:
+            rate = None
+            for certainty in interp.xpath("./tei:certainty", namespaces={"tei": tei_ns}):
+                if certainty.get("degree") is not None:
+                    rate = float(certainty.get("degree"))
+                    break
+            self.transcriptional_categories.append(transcriptional_category)
+            self.transcriptional_rates_by_id[transcriptional_category] = rate
+        t1 = time.time()
+        if self.verbose:
+            print(
+                "Finished processing %d transcriptional change categories in %0.4fs."
+                % (len(self.transcriptional_rates_by_id), t1 - t0)
+            )
+        return
+
+    def validate_intrinsic_relations(self):
+        """Checks if any VariationUnit's intrinsic_relations map is not a forest.
+        If any is not, then an IntrinsicRelationsException is thrown describing the VariationUnit at fault.
+        """
+        if self.verbose:
+            print("Validating intrinsic relation graphs for variation units...")
+        t0 = time.time()
+        for vu in self.variation_units:
+            # Skip any variation units with an empty intrinsic_relations map:
+            if len(vu.intrinsic_relations) == 0:
+                continue
+            # For all others, start by identifying all reading IDs that are not related to by some other reading ID:
+            in_degree_by_reading = {}
+            for edge in vu.intrinsic_relations:
+                s = edge[0]
+                t = edge[1]
+                if s not in in_degree_by_reading:
+                    in_degree_by_reading[s] = 0
+                if t not in in_degree_by_reading:
+                    in_degree_by_reading[t] = 0
+                in_degree_by_reading[t] += 1
+            # If any reading has more than one relation pointing to it, then the intrinsic relations graph is not a forest:
+            excessive_in_degree_readings = [
+                rdg_id for rdg_id in in_degree_by_reading if in_degree_by_reading[rdg_id] > 1
+            ]
+            if len(excessive_in_degree_readings) > 0:
+                msg = ""
+                msg += (
+                    "In variation unit %s, the following readings have more than one intrinsic relation pointing to them: %s.\n"
+                    % (vu.id, ", ".join(excessive_in_degree_readings))
+                )
+                msg += "Please ensure that at least one reading has no relations pointing to it and that every reading has no more than one relation pointing to it."
+                raise IntrinsicRelationsException(msg)
+            # If every reading has another reading pointing to it, then the intrinsic relations graph contains a cycle and is not a forest:
+            starting_nodes = [rdg_id for rdg_id in in_degree_by_reading if in_degree_by_reading[rdg_id] == 0]
+            if len(starting_nodes) == 0:
+                msg = ""
+                msg += "In variation unit %s, the intrinsic relations contain a cycle.\n" % vu.id
+                msg += "Please ensure that at least one reading has no relations pointing to it and that every reading has no more than one relation pointing to it."
+                raise IntrinsicRelationsException(msg)
+        t1 = time.time()
+        if self.verbose:
+            print("Finished intrinsic relations validation in %0.4fs." % (t1 - t0))
+        return
+
     def parse_apps(self, xml: et.ElementTree):
         """Given an XML tree for a collation, populates its list of variation units from its app elements.
 
         Args:
             xml: An lxml.etree.ElementTree representing an XML tree rooted at a TEI element.
         """
         if self.verbose:
@@ -239,29 +472,37 @@
         # Initialize the output dictionary with empty sets for all base witnesses:
         for wit in self.witnesses:
             readings_by_witness_for_unit[wit.id] = [0] * len(self.substantive_readings_by_variation_unit_id[vu.id])
         # In a second pass, assign each base witness a set containing the readings it supports in this unit:
         for rdg in vu.readings:
             # Initialize the dictionary indicating support for this reading (or its disambiguations):
             rdg_support = [0] * len(self.substantive_readings_by_variation_unit_id[vu.id])
-            # If this is a missing reading (e.g., a lacuna or an overlap), then we can skip this reading, as its corresponding set will be empty:
+            # If this is a missing reading (e.g., a lacuna or an overlap), then we can skip it, as its corresponding set will be empty:
             if rdg.type in self.missing_reading_types:
                 continue
-            # If this reading is trivial, then it will contain an entry for the index of its parent substantive reading:
+            # Otherwise, if this reading is trivial, then it will contain an entry for the index of its parent substantive reading:
             elif rdg.type in self.trivial_reading_types:
-                rdg_support[reading_id_to_index[rdg.id]] += 1
-            # If this reading has one or more target readings, then add an entry for each of those readings according to their certainty in this reading:
-            elif len(rdg.certainties) > 0:
+                rdg_support[reading_id_to_index[rdg.id]] = 1
+            # Otherwise, if this reading has one or more nonzero certainty degrees,
+            # then set the entries for these readings to their degrees:
+            elif sum(rdg.certainties.values()) > 0:
                 for t in rdg.certainties:
-                    # For overlaps, the target may be to a reading not included in this unit, so skip it if its ID is unrecognized:
+                    # Skip any reading whose ID is unrecognized in this unit:
+                    if t in reading_id_to_index:
+                        rdg_support[reading_id_to_index[t]] = rdg.certainties[t]
+            # Otherwise, if this reading has one or more targets (i.e., if it is an ambiguous reading),
+            # then set the entries for each of its targets to 1:
+            elif len(rdg.targets) > 0:
+                for t in rdg.targets:
+                    # Skip any reading whose ID is unrecognized in this unit:
                     if t in reading_id_to_index:
-                        rdg_support[reading_id_to_index[t]] += rdg.certainties[t]
-            # Otherwise, this reading is itself substantive; add an entry for the index of this reading:
+                        rdg_support[reading_id_to_index[t]] = 1
+            # Otherwise, this reading is itself substantive; set the entry for the index of this reading to 1:
             else:
-                rdg_support[reading_id_to_index[rdg.id]] += 1
+                rdg_support[reading_id_to_index[rdg.id]] = 1
             # Proceed for each witness siglum in the support for this reading:
             for wit in rdg.wits:
                 # Is this siglum a base siglum?
                 base_wit = self.get_base_wit(wit)
                 if base_wit not in self.witness_index_by_id:
                     # If it is not, then it is probably just because we've encountered a corrector or some other secondary witness not included in the witness list;
                     # report this if we're in verbose mode and move on:
@@ -271,25 +512,17 @@
                             % (wit, base_wit, vu.id, rdg.id)
                         )
                     continue
                 # If we've found a base siglum, then add this reading's contribution to the base witness's reading set for this unit;
                 # normally the existing set will be empty, but if we reduce two suffixed sigla to the same base witness,
                 # then that witness may attest to multiple readings in the same unit:
                 readings_by_witness_for_unit[base_wit] = [
-                    (readings_by_witness_for_unit[base_wit][i] + rdg_support[i]) for i in range(len(rdg_support))
+                    (min(readings_by_witness_for_unit[base_wit][i] + rdg_support[i], 1))
+                    for i in range(len(rdg_support))
                 ]
-        # In a third pass, normalize the reading weights for all non-lacunose readings:
-        for wit in readings_by_witness_for_unit:
-            rdg_support = readings_by_witness_for_unit[wit]
-            norm = sum(rdg_support)
-            # Skip lacunae, as we can't normalize the vector of reading weights:
-            if norm == 0:
-                continue
-            for i in range(len(rdg_support)):
-                rdg_support[i] = rdg_support[i] / norm
         return readings_by_witness_for_unit
 
     def parse_readings_by_witness(self):
         """Populates the internal dictionary mapping witness IDs to a list of their reading support sets for all variation units, and then fills the empty reading support sets for witnesses of type "corrector" with the entries of the previous witness."""
         if self.verbose:
             print("Populating internal dictionary of witness readings...")
         t0 = time.time()
@@ -355,14 +588,15 @@
         file_addr: Union[Path, str],
         drop_constant: bool = False,
         char_state_labels: bool = True,
         frequency: bool = False,
         ambiguous_as_missing: bool = False,
         calibrate_dates: bool = False,
         mrbayes: bool = False,
+        clock_model: ClockModel = ClockModel.strict,
     ):
         """Writes this Collation to a NEXUS file with the given address.
 
         Args:
             file_addr: A string representing the path to an output NEXUS file; the file type should be .nex, .nexus, or .nxs.
             drop_constant (bool, optional): An optional flag indicating whether to ignore variation units with one substantive reading.
             char_state_labels: An optional flag indicating whether or not to include the CharStateLabels block.
@@ -370,17 +604,20 @@
                 instead of the StatesFormat=StatesPresent setting
                 (and thus represent all states with frequency vectors rather than symbols).
                 Note that this setting is necessary to make use of certainty degrees assigned to multiple ambiguous states in the collation.
             ambiguous_as_missing: An optional flag indicating whether to treat all ambiguous states as missing data.
                 If this flag is set, then only base symbols will be generated for the NEXUS file.
                 It is only applied if the frequency option is False.
             calibrate_dates: An optional flag indicating whether to add an Assumptions block that specifies date distributions for witnesses.
-                This option is intended for inputs to BEAST2.
+                This option is intended for inputs to BEAST 2.
             mrbayes: An optional flag indicating whether to add a MrBayes block that specifies model settings and age calibrations for witnesses.
                 This option is intended for inputs to MrBayes.
+            clock_model: A ClockModel option indicating which type of clock model to use.
+                This option is intended for inputs to MrBayes and BEAST 2.
+                MrBayes does not presently support a local clock model, so it will default to a strict clock model if a local clock model is specified.
         """
         # Populate a list of sites that will correspond to columns of the sequence alignment:
         substantive_variation_unit_ids = self.variation_unit_ids
         if drop_constant:
             substantive_variation_unit_ids = [
                 vu_id
                 for vu_id in self.variation_unit_ids
@@ -486,94 +723,93 @@
                             sequence += "{%s}" % "".join([str(rdg_ind) for rdg_ind in rdg_inds])
                 f.write("%s" % (sequence))
             f.write(";\n")
             # End the data block:
             f.write("End;")
             # If calibrate_dates is set, then add the assumptions block:
             if calibrate_dates:
-                # Attempt to get the minimum and maximum dates for witnesses; if we can't do this, then don't write an assumptions block:
-                min_date = None
-                max_date = None
-                try:
-                    min_date = min([wit.date_range[0] for wit in self.witnesses if wit.date_range[0] is not None])
-                    max_date = max([wit.date_range[1] for wit in self.witnesses if wit.date_range[1] is not None])
-                except Exception as e:
-                    print("WARNING: no witnesses have date ranges; no Assumptions block will be written!")
-                    return
                 f.write("\n\n")
                 f.write("Begin ASSUMPTIONS;\n")
                 # Set the scale to years:
                 f.write("\tOPTIONS SCALE = years;\n\n")
-                # Then calibrate the date distributions for each witness that has date information specified:
+                # Then calibrate the witness ages:
                 calibrate_strings = []
                 for i, wit in enumerate(self.witnesses):
                     taxlabel = taxlabels[i]
-                    # If either end of this witness's date range is empty, then use the min and max dates over all witnesses as defaults:
                     date_range = wit.date_range
-                    if date_range[0] is None and date_range[1] is None:
-                        date_range = tuple([min_date, max_date])
-                    elif date_range[0] is None:
-                        date_range = tuple([min_date, date_range[1]])
-                    elif date_range[1] is None:
-                        date_range = tuple([date_range[0], max_date])
-                    # If both ends of the date range are the same, then use a fixed distribution:
-                    if date_range[0] == date_range[1]:
-                        calibrate_string = "\tCALIBRATE %s = fixed(%d)" % (taxlabel, date_range[0])
-                    # If they are different, then use a uniform distribution:
+                    if date_range[0] is not None:
+                        # If there is a lower bound on the witness's date, then use either a fixed or uniform distribution,
+                        # depending on whether the upper and lower bounds match:
+                        min_age = datetime.now().year - date_range[1]
+                        max_age = datetime.now().year - date_range[0]
+                        if min_age == max_age:
+                            calibrate_string = "\tCALIBRATE %s = fixed(%d)" % (taxlabel, min_age)
+                            calibrate_strings.append(calibrate_string)
+                        else:
+                            calibrate_string = "\tCALIBRATE %s = uniform(%d,%d)" % (taxlabel, min_age, max_age)
+                            calibrate_strings.append(calibrate_string)
                     else:
-                        calibrate_string = "\tCALIBRATE %s = uniform(%d,%d)" % (taxlabel, date_range[0], date_range[1])
-                    calibrate_strings.append(calibrate_string)
+                        # If there is no lower bound on the witness's date, then use an offset log-normal distribution:
+                        min_age = datetime.now().year - date_range[1]
+                        calibrate_string = "\tCALIBRATE %s = offsetlognormal(%d,0.0,1.0)" % (taxlabel, min_age)
+                        calibrate_strings.append(calibrate_string)
                 # Then print the calibrate strings, separated by commas and line breaks and terminated by a semicolon:
                 f.write("%s;\n\n" % ",\n".join(calibrate_strings))
                 # End the assumptions block:
                 f.write("End;")
             # If mrbayes is set, then add the mrbayes block:
             if mrbayes:
                 f.write("\n\n")
                 f.write("Begin MRBAYES;\n")
                 # Turn on the autoclose feature by default:
                 f.write("\tset autoclose=yes;\n")
-                # Attempt to get the minimum and maximum dates for witnesses; if we can't do this, then don't write any age calibration settings:
-                min_date = None
-                max_date = None
-                try:
-                    min_date = min([wit.date_range[0] for wit in self.witnesses if wit.date_range[0] is not None])
-                    max_date = max([wit.date_range[1] for wit in self.witnesses if wit.date_range[1] is not None])
-                except Exception as e:
-                    print(
-                        "WARNING: no witnesses have date ranges; no clock model will be assumed and no date calibrations will be used!"
-                    )
-                if min_date is not None and max_date is not None:
-                    f.write("\n")
-                    f.write("\tprset brlenspr = clock:uniform;\n")
-                    f.write("\tprset nodeagepr = calibrated;\n")
-                    # Then calibrate the date distributions for each witness that has date information specified:
-                    calibrate_strings = []
-                    for i, wit in enumerate(self.witnesses):
-                        taxlabel = taxlabels[i]
-                        # If either end of this witness's date range is empty, then use the min and max dates over all witnesses as defaults:
-                        date_range = wit.date_range
-                        if date_range[0] is None and date_range[1] is None:
-                            date_range = tuple([min_date, max_date])
-                        elif date_range[0] is None:
-                            date_range = tuple([min_date, date_range[1]])
-                        elif date_range[1] is None:
-                            date_range = tuple([date_range[0], max_date])
-                        # If both ends of the date range are the same, then use a fixed distribution:
-                        if date_range[0] == date_range[1]:
-                            f.write(
-                                "\tcalibrate %s = fixed(%d);\n" % (taxlabel, max_date - date_range[0])
-                            )  # get age by subtracting date from latest date:
-                        # If they are different, then use a uniform distribution:
+                # Set the branch lengths to be governed by a birth-death clock model, and set up the parameters for this model:
+                f.write("\n")
+                f.write("\tprset brlenspr = clock:birthdeath;\n")
+                f.write("\tprset speciationpr = uniform(0.0,10.0);\n")
+                f.write("\tprset extinctionpr = beta(2.0,4.0);\n")
+                f.write("\tprset sampleprob = 0.01;\n")
+                # Use the specified clock model:
+                f.write("\n")
+                if clock_model == clock_model.uncorrelated:
+                    f.write("\tprset clockvarpr=igr;\n")
+                    f.write("\tprset clockratepr=lognormal(0.0,1.0);\n")
+                    f.write("\tprset igrvarpr=exponential(1.0);\n")
+                else:
+                    f.write("\tprset clockvarpr=strict;\n")
+                    f.write("\tprset clockratepr=lognormal(0.0,1.0);\n")
+                # Set the priors on the tree age depending on the date range for the origin of the collated work:
+                f.write("\n")
+                if self.origin_date_range[0] is not None:
+                    min_tree_age = datetime.now().year - self.origin_date_range[1]
+                    max_tree_age = datetime.now().year - self.origin_date_range[0]
+                    f.write("\tprset treeagepr = uniform(%d,%d);\n" % (min_tree_age, max_tree_age))
+                else:
+                    min_tree_age = datetime.now().year - self.origin_date_range[1]
+                    f.write("\tprset treeagepr = offsetgamma(%d,1.0,1.0);\n" % (min_tree_age))
+                # Then calibrate the witness ages:
+                f.write("\n")
+                f.write("\tprset nodeagepr = calibrated;\n")
+                for i, wit in enumerate(self.witnesses):
+                    taxlabel = taxlabels[i]
+                    date_range = wit.date_range
+                    if date_range[0] is not None:
+                        # If there is a lower bound on the witness's date, then use either a fixed or uniform distribution,
+                        # depending on whether the upper and lower bounds match:
+                        min_age = datetime.now().year - date_range[1]
+                        max_age = datetime.now().year - date_range[0]
+                        if min_age == max_age:
+                            f.write("\tcalibrate %s = fixed(%d);\n" % (taxlabel, min_age))
                         else:
-                            f.write(
-                                "\tcalibrate %s = uniform(%d,%d);\n"
-                                % (taxlabel, max_date - date_range[1], max_date - date_range[0])
-                            )  # get age range by subtracting start and end dates from latest date:
-                    f.write("\n")
+                            f.write("\tcalibrate %s = uniform(%d,%d);\n" % (taxlabel, min_age, max_age))
+                    else:
+                        # If there is no lower bound on the witness's date, then use an offset gamma distribution:
+                        min_age = datetime.now().year - date_range[1]
+                        f.write("\tcalibrate %s = offsetgamma(%d,1.0,1.0);\n" % (taxlabel, min_age))
+                f.write("\n")
                 # Add default settings for MCMC estimation of posterior distribution:
                 f.write("\tmcmcp ngen=100000;\n")
                 # Write the command to run MrBayes:
                 f.write("\tmcmc;\n")
                 # End the assumptions block:
                 f.write("End;")
         return
@@ -826,14 +1062,431 @@
                         sequence += symbols[rdg_inds[0]]
                         continue
                     # For multiple readings, print the missing symbol:
                     sequence += missing_symbol
                 f.write("%s\n" % (sequence))
         return
 
+    def get_beast_symbols(self):
+        """Returns a list of one-character symbols needed to represent the states of all substantive readings in BEAST format.
+
+        The number of symbols equals the maximum number of substantive readings at any variation unit.
+
+        Returns:
+            A list of individual characters representing states in readings.
+        """
+        possible_symbols = (
+            list(string.digits) + list(string.ascii_lowercase)[:22]
+        )  # NOTE: for BEAST, any number of states should theoretically be permissible, but since code maps are required for some reason, we will limit the number of symbols to 32 for now
+        # The number of symbols needed is equal to the length of the longest substantive reading vector:
+        nsymbols = 0
+        # If there are no witnesses, then no symbols are needed at all:
+        if len(self.witnesses) == 0:
+            return []
+        wit_id = self.witnesses[0].id
+        for rdg_support in self.readings_by_witness[wit_id]:
+            nsymbols = max(nsymbols, len(rdg_support))
+        beast_symbols = possible_symbols[:nsymbols]
+        return beast_symbols
+
+    def get_beast_date_map(self, taxlabels):
+        """Returns a string representing witness-to-date mappings in BEAST format.
+
+        Since this format requires single dates as opposed to date ranges,
+        witnesses with closed date ranges will be mapped to the average of their lower and upper bounds,
+        and witnesses with open date ranges will not be mapped.
+
+        Args:
+            taxlabels: A list of slugified taxon labels.
+
+        Returns:
+            A string containing comma-separated date calibrations of the form witness_id=date.
+        """
+        calibrate_strings = []
+        for i, wit in enumerate(self.witnesses):
+            taxlabel = taxlabels[i]
+            date_range = wit.date_range
+            # If either end of this witness's date range is empty, then do not include it:
+            if date_range[0] is None or date_range[1] is None:
+                continue
+            # Otherwise, take the midpoint of its date range as its date:
+            date = int((date_range[0] + date_range[1]) / 2)
+            calibrate_string = "%s=%d" % (taxlabel, date)
+            calibrate_strings.append(calibrate_string)
+        # Then output the full date map string:
+        date_map = ",".join(calibrate_strings)
+        return date_map
+
+    def get_beast_origin_span(self):
+        """Returns a tuple containing the lower and upper bounds for the height of the origin of the Birth-Death Skyline model.
+        The upper bound on the height of the tree is the difference between the current date
+        and the lower bound on the date of the original work, if both are defined;
+        otherwise, it is left undefined.
+        The lower bound on the height of the tree is the difference between the latest lower bound on a witness's date
+        and the upper bound on the date of the original work, if both are defined;
+        otherwise, it is zero.
+
+        Returns:
+            A tuple containing lower and upper bounds on the origin height for the Birth-Death Skyline model.
+        """
+        origin_span = [datetime.now().year - self.origin_date_range[1], None]
+        # If the lower bound on the original work is defined, then update the upper bound on the height of the origin:
+        if self.origin_date_range[0] is not None:
+            origin_span[1] = datetime.now().year - self.origin_date_range[0]
+        return tuple(origin_span)
+
+    def validate_latest_tip(self):
+        """Checks if the witness with the latest possible date has a fixed date
+        (i.e, if the lower and upper bounds for its date are the same).
+        If this is not true, then a warning is issued.
+        """
+        latest_date = None
+        latest_wit = None
+        for i, wit in enumerate(self.witnesses):
+            wit_id = wit.id
+            date_range = wit.date_range
+            if date_range[1] is not None:
+                if latest_date is not None:
+                    if date_range[1] > latest_date:
+                        latest_date = date_range[1]
+                        latest_wit = wit
+                else:
+                    latest_date = date_range[1]
+                    latest_wit = wit
+        if latest_wit.date_range[0] is None or latest_wit.date_range[0] != latest_wit.date_range[1]:
+            print(
+                "WARNING: the latest witness, %s, has a variable date range; this may result in precisely dated witness being misaligned in the trees output by BEAST."
+                % latest_wit.id
+            )
+        return
+
+    def get_beast_code_map_for_unit(self, symbols, missing_symbol, vu_ind):
+        """Returns a string containing state/reading code mappings in BEAST format using the given single-state and missing state symbols for the character/variation unit at the given index.
+        If the variation unit at the given index is a singleton unit (i.e., if it has only one substantive reading), then a code for a dummy state will be included.
+
+        Args:
+            vu_ind: An integer index for the desired unit.
+
+        Returns:
+            A string containing comma-separated code mappings.
+        """
+        vu = self.variation_units[vu_ind]
+        vu_id = vu.id
+        code_map = {}
+        for k in range(len(self.substantive_readings_by_variation_unit_id[vu.id])):
+            code_map[symbols[k]] = str(k)
+        # If this site is a singleton site, then add a code mapping for the dummy state:
+        if len(self.substantive_readings_by_variation_unit_id[vu.id]) == 1:
+            code_map[symbols[1]] = str(1)
+        # Then add a mapping for the missing state, including a dummy state if this is a singleton site:
+        code_map[missing_symbol] = " ".join(
+            str(k) for k in range(len(self.substantive_readings_by_variation_unit_id[vu.id]))
+        )
+        # If this site is a singleton site, then add the dummy state to the missing state mapping:
+        if len(self.substantive_readings_by_variation_unit_id[vu.id]) == 1:
+            code_map[missing_symbol] = code_map[missing_symbol] + " " + str(1)
+        # Then combine all of the mappings into a single string:
+        code_map_string = ", ".join([code + "=" + code_map[code] for code in code_map])
+        return code_map_string
+
+    def get_beast_equilibrium_frequencies_for_unit(self, vu_ind):
+        """Returns a string containing state/reading equilibrium frequencies in BEAST format for the character/variation unit at the given index.
+        Since the equilibrium frequencies are not used with the substitution models, the equilibrium frequencies simply correspond to a uniform distribution over the states.
+        If the variation unit at the given index is a singleton unit (i.e., if it has only one substantive reading), then an equilibrium frequency of 0 will be added for a dummy state.
+
+        Args:
+            vu_ind: An integer index for the desired unit.
+
+        Returns:
+            A string containing space-separated equilibrium frequencies.
+        """
+        vu = self.variation_units[vu_ind]
+        vu_id = vu.id
+        # If this unit is a singleton, then return the string "0.5 0.5":
+        if len(self.substantive_readings_by_variation_unit_id[vu_id]) == 1:
+            return "0.5 0.5"
+        # Otherwise, set the equilibrium frequencies according to a uniform distribution:
+        equilibrium_frequencies = [1.0 / len(self.substantive_readings_by_variation_unit_id[vu_id])] * len(
+            self.substantive_readings_by_variation_unit_id[vu_id]
+        )
+        equilibrium_frequencies_string = " ".join([str(w) for w in equilibrium_frequencies])
+        return equilibrium_frequencies_string
+
+    def get_beast_root_frequencies_for_unit(self, vu_ind):
+        """Returns a string containing state/reading root frequencies in BEAST format for the character/variation unit at the given index.
+        The root frequencies are calculated from the intrinsic odds at this unit.
+        If the variation unit at the given index is a singleton unit (i.e., if it has only one substantive reading), then a root frequency of 0 will be added for a dummy state.
+        If no intrinsic odds are specified, then a uniform distribution over all states is assumed.
+
+        Args:
+            vu_ind: An integer index for the desired unit.
+
+        Returns:
+            A string containing space-separated root frequencies.
+        """
+        vu = self.variation_units[vu_ind]
+        vu_id = vu.id
+        intrinsic_relations = vu.intrinsic_relations
+        intrinsic_odds_by_id = self.intrinsic_odds_by_id
+        # If this unit is a singleton, then return the string "1 0":
+        if len(self.substantive_readings_by_variation_unit_id[vu_id]) == 1:
+            return "1 0"
+        # If this unit has no intrinsic odds, then assume a uniform distribution over all readings:
+        if len(intrinsic_relations) == 0:
+            root_frequencies = [1.0 / len(self.substantive_readings_by_variation_unit_id[vu_id])] * len(
+                self.substantive_readings_by_variation_unit_id[vu_id]
+            )
+            root_frequencies_string = " ".join([str(w) for w in root_frequencies])
+            return root_frequencies_string
+        # We will populate the root frequencies based on the intrinsic odds of the readings:
+        root_frequencies_by_id = {}
+        for rdg_id in self.substantive_readings_by_variation_unit_id[vu_id]:
+            root_frequencies_by_id[rdg_id] = 0
+        # First, construct an adjacency list for efficient edge iteration:
+        neighbors_by_source = {}
+        for edge in intrinsic_relations:
+            s = edge[0]
+            t = edge[1]
+            if s not in neighbors_by_source:
+                neighbors_by_source[s] = []
+            if t not in neighbors_by_source:
+                neighbors_by_source[t] = []
+            neighbors_by_source[s].append(t)
+        # Next, identify all readings that are not targeted by any intrinsic odds relation:
+        in_degree_by_reading = {}
+        for edge in intrinsic_relations:
+            s = edge[0]
+            t = edge[1]
+            if s not in in_degree_by_reading:
+                in_degree_by_reading[s] = 0
+            if t not in in_degree_by_reading:
+                in_degree_by_reading[t] = 0
+            in_degree_by_reading[t] += 1
+        starting_nodes = [t for t in in_degree_by_reading if in_degree_by_reading[t] == 0]
+        # Set the root frequencies for these readings to 1 (they will be normalized later):
+        for starting_node in starting_nodes:
+            root_frequencies_by_id[starting_node] = 1.0
+        # Next, set the frequencies for the remaining readings recursively using the adjacency list:
+        def update_root_frequencies(s):
+            for t in neighbors_by_source[s]:
+                intrinsic_category = intrinsic_relations[(s, t)]
+                odds = (
+                    intrinsic_odds_by_id[intrinsic_category]
+                    if intrinsic_odds_by_id[intrinsic_category] is not None
+                    else 1.0
+                )  # TODO: This needs to be handled using parameters once we have it implemented in BEAST
+                root_frequencies_by_id[t] = root_frequencies_by_id[s] / odds
+                update_root_frequencies(t)
+            return
+
+        for starting_node in starting_nodes:
+            update_root_frequencies(starting_node)
+        # Then produce a normalized vector of root frequencies that corresponds to a probability distribution:
+        root_frequencies = [
+            root_frequencies_by_id[rdg_id] for rdg_id in self.substantive_readings_by_variation_unit_id[vu_id]
+        ]
+        total_frequencies = sum(root_frequencies)
+        for k in range(len(root_frequencies)):
+            root_frequencies[k] = root_frequencies[k] / total_frequencies
+        root_frequencies_string = " ".join([str(w) for w in root_frequencies])
+        return root_frequencies_string
+
+    def to_beast(
+        self, file_addr: Union[Path, str], drop_constant: bool = False, clock_model: ClockModel = ClockModel.strict
+    ):
+        """Writes this Collation to a file in BEAST format with the given address.
+
+        Args:
+            file_addr: A string representing the path to an output file.
+            drop_constant (bool, optional): An optional flag indicating whether to ignore variation units with one substantive reading.
+            clock_model: A ClockModel option indicating which clock model to use.
+        """
+        # Populate a list of sites that will correspond to columns of the sequence alignment:
+        substantive_variation_unit_ids = self.variation_unit_ids
+        if drop_constant:
+            substantive_variation_unit_ids = [
+                vu_id
+                for vu_id in self.variation_unit_ids
+                if len(self.substantive_readings_by_variation_unit_id[vu_id]) > 1
+            ]
+        substantive_variation_unit_ids_set = set(substantive_variation_unit_ids)
+        substantive_variation_unit_reading_tuples_set = set(self.substantive_variation_unit_reading_tuples)
+        # First, calculate the values we will be using for the main template:
+        taxlabels = [slugify(wit.id, lowercase=False, separator='_') for wit in self.witnesses]
+        missing_symbol = '?'
+        symbols = self.get_beast_symbols()
+        date_map = self.get_beast_date_map(taxlabels)
+        origin_span = self.get_beast_origin_span()
+        self.validate_latest_tip()
+        # Then populate the necessary objects for the BEAST XML Jinja template:
+        witness_objects = []
+        variation_unit_objects = []
+        intrinsic_category_objects = []
+        transcriptional_category_objects = []
+        # Start with witnesses:
+        for i, wit in enumerate(self.witnesses):
+            witness_object = {}
+            # Copy the ID for this witness:
+            witness_object["id"] = wit.id
+            # Copy its date bounds:
+            witness_object["min_date"] = wit.date_range[0]
+            witness_object["max_date"] = wit.date_range[1]
+            # Populate its sequence from its entries in the witness's readings dictionary:
+            sequence = ""
+            for j, rdg_support in enumerate(self.readings_by_witness[wit.id]):
+                vu_id = self.variation_unit_ids[j]
+                # Skip any variation units deemed non-substantive:
+                if vu_id not in substantive_variation_unit_ids:
+                    continue
+                # If this witness has a certainty of 0 for all readings, then it is a gap; assign a likelihood of 1 to each reading:
+                if sum(rdg_support) == 0:
+                    for k, w in enumerate(rdg_support):
+                        sequence += "1"
+                        if k < len(rdg_support) - 1:
+                            sequence += ", "
+                        else:
+                            if len(rdg_support) > 1:
+                                sequence += "; "
+                            else:
+                                # If this site is a singleton site, then add a dummy state:
+                                sequence += ", 0; "
+                # Otherwise, read the probabilities as they are given:
+                else:
+                    for k, w in enumerate(rdg_support):
+                        sequence += str(w)
+                        if k < len(rdg_support) - 1:
+                            sequence += ", "
+                        else:
+                            if len(rdg_support) > 1:
+                                sequence += "; "
+                            else:
+                                # If this site is a singleton site, then add a dummy state:
+                                sequence += ", 0; "
+            # Strip the final semicolon and space from the sequence:
+            sequence = sequence.strip("; ")
+            # Then set the witness object's sequence attribute to this string:
+            witness_object["sequence"] = sequence
+            witness_objects.append(witness_object)
+        # Then proceed to variation units:
+        for j, vu in enumerate(self.variation_units):
+            if vu.id not in substantive_variation_unit_ids_set:
+                continue
+            variation_unit_object = {}
+            # Copy the ID of this variation unit:
+            variation_unit_object["id"] = vu.id
+            # Copy this variation unit's number of substantive readings,
+            # setting it to 2 if it is a singleton unit:
+            variation_unit_object["nstates"] = (
+                len(self.substantive_readings_by_variation_unit_id[vu.id])
+                if len(self.substantive_readings_by_variation_unit_id[vu.id]) > 1
+                else 2
+            )
+            # Then construct the code map for this unit:
+            variation_unit_object["code_map"] = self.get_beast_code_map_for_unit(symbols, missing_symbol, j)
+            # Then populate a comma-separated string of reading labels for this unit:
+            rdg_texts = []
+            vu_label = vu.id
+            for rdg in vu.readings:
+                key = tuple([vu.id, rdg.id])
+                if key not in substantive_variation_unit_reading_tuples_set:
+                    continue
+                rdg_text = slugify(rdg.text, lowercase=False, allow_unicode=True, separator='_')
+                # Replace any empty reading text with an omission marker:
+                if rdg_text == "":
+                    rdg_text = "om."
+                rdg_texts.append(rdg_text)
+            # If this site is a singleton site, then add a dummy reading for the dummy state:
+            if len(self.substantive_readings_by_variation_unit_id[vu.id]) == 1:
+                rdg_texts.append("DUMMY")
+            rdg_texts_string = ", ".join(rdg_texts)
+            variation_unit_object["rdg_texts"] = rdg_texts_string
+            # Then populate this unit's equilibrium frequency string and its root frequency string:
+            variation_unit_object["equilibrium_frequencies"] = self.get_beast_equilibrium_frequencies_for_unit(j)
+            variation_unit_object["root_frequencies"] = self.get_beast_root_frequencies_for_unit(j)
+            # Then populate its transition rate matrix off-diagonal entries:
+            rate_objects = []
+            if len(self.substantive_readings_by_variation_unit_id[vu.id]) == 1:
+                # If this is a singleton site, then use an arbitrary 2x2 rate matrix:
+                rate_objects.append({"transcriptional_categories": ["default"], "expression": None})
+                rate_objects.append({"transcriptional_categories": ["default"], "expression": None})
+            else:
+                # Otherwise, proceed for every pair of readings in this unit:
+                for k_1, rdg_id_1 in enumerate(self.substantive_readings_by_variation_unit_id[vu.id]):
+                    for k_2, rdg_id_2 in enumerate(self.substantive_readings_by_variation_unit_id[vu.id]):
+                        # Skip diagonal elements:
+                        if k_1 == k_2:
+                            continue
+                        # If the first reading has no transcriptional relation to the second in this unit, then use the default rate:
+                        if (rdg_id_1, rdg_id_2) not in vu.transcriptional_relations:
+                            rate_objects.append({"transcriptional_categories": ["default"], "expression": None})
+                            continue
+                        # Otherwise, if only one category of transcriptional relations holds between the first and second readings,
+                        # then use its rate:
+                        if len(vu.transcriptional_relations[(rdg_id_1, rdg_id_2)]) == 1:
+                            # If there is only one such category, then add its rate as a standalone var element:
+                            transcriptional_category = list(vu.transcriptional_relations[(rdg_id_1, rdg_id_2)])[0]
+                            rate_objects.append(
+                                {"transcriptional_categories": [transcriptional_category], "expression": None}
+                            )
+                            continue
+                        # If there is more than one, then add a var element that is a sum of the individual categories' rates:
+                        transcriptional_categories = list(vu.transcriptional_relations[(rdg_id_1, rdg_id_2)])
+                        args = []
+                        for transcriptional_category in transcriptional_categories:
+                            args.append("%s_rate" % transcriptional_category)
+                        args_string = " ".join(args)
+                        ops = ["+"] * (len(args) - 1)
+                        ops_string = " ".join(ops)
+                        expression_string = " ".join([args_string, ops_string])
+                        rate_objects.append(
+                            {"transcriptional_categories": transcriptional_categories, "expression": expression_string}
+                        )
+            variation_unit_object["rates"] = rate_objects
+            variation_unit_objects.append(variation_unit_object)
+        # Then proceed to intrinsic odds categories:
+        for intrinsic_category in self.intrinsic_categories:
+            intrinsic_category_object = {}
+            # Copy the ID of this intrinsic category:
+            intrinsic_category_object["id"] = intrinsic_category
+            # Then copy the odds factors associated with this intrinsic category,
+            # setting it to 1.0 if it is not specified and setting the estimate attribute accordingly:
+            odds = self.intrinsic_odds_by_id[intrinsic_category]
+            intrinsic_category_object["odds"] = odds if odds is not None else 1.0
+            intrinsic_category_object["estimate"] = "false" if odds is not None else "true"
+            intrinsic_category_objects.append(intrinsic_category_object)
+        # The proceed to transcriptional rate categories:
+        for transcriptional_category in self.transcriptional_categories:
+            transcriptional_category_object = {}
+            # Copy the ID of this transcriptional category:
+            transcriptional_category_object["id"] = transcriptional_category
+            # Then copy the rate of this transcriptional category,
+            # setting it to 2.0 if it is not specified and setting the estimate attribute accordingly:
+            rate = self.transcriptional_rates_by_id[transcriptional_category]
+            transcriptional_category_object["rate"] = rate if rate is not None else 2.0
+            transcriptional_category_object["estimate"] = "false" if rate is not None else "true"
+            transcriptional_category_objects.append(transcriptional_category_object)
+        # Now render the output XML file using the Jinja template:
+        root_dir = Path(__file__).parent.parent
+        env = Environment(loader=PackageLoader("teiphy", "templates"), autoescape=select_autoescape())
+        template = env.get_template("beast_template.xml")
+        rendered = template.render(
+            nsymbols=len(symbols),
+            date_map=date_map,
+            origin_span=origin_span,
+            clock_model=clock_model.value,
+            clock_rate_categories=2 * len(self.witnesses) - 1,
+            witnesses=witness_objects,
+            variation_units=variation_unit_objects,
+            intrinsic_categories=intrinsic_category_objects,
+            transcriptional_categories=transcriptional_category_objects,
+        )
+        with open(file_addr, "w", encoding="utf-8") as f:
+            f.write(rendered)
+        return
+
     def to_numpy(self, drop_constant: bool = False, split_missing: bool = True):
         """Returns this Collation in the form of a NumPy array, along with arrays of its row and column labels.
 
         Args:
             drop_constant (bool, optional): An optional flag indicating whether to ignore variation units with one substantive reading.
             split_missing: An optional flag indicating whether or not to treat missing characters/variation units as having a contribution of 1 split over all states/readings; if False, then missing data is ignored (i.e., all states are 0). Default value is True.
 
@@ -1203,22 +1856,18 @@
             print("WARNING: no witnesses have date ranges; no chron file will be written!")
             return
         with open(chron_file_addr, "w", encoding="utf-8") as f:
             for wit in self.witnesses:
                 wit_label = slugify(wit.id, lowercase=False, allow_unicode=True, separator='_')
                 f.write(wit_label)
                 f.write(" " * (max_id_length - len(wit.id) + 1))
-                # If either end of this witness's date range is empty, then use the min and max dates over all witnesses as defaults:
+                # If either the lower bound on this witness's date is empty, then use the min and max dates over all witnesses as defaults:
                 date_range = wit.date_range
-                if date_range[0] is None and date_range[1] is None:
-                    date_range = tuple([min_date, max_date])
-                elif date_range[0] is None:
+                if date_range[0] is None:
                     date_range = tuple([min_date, date_range[1]])
-                elif date_range[1] is None:
-                    date_range = tuple([date_range[0], max_date])
                 # Then write the date range minimum, average, and maximum to the chron file:
                 low_date = str(date_range[0])
                 f.write(" " * (max_date_length - len(low_date) + 2))
                 f.write(low_date)
                 avg_date = str(int(((date_range[0] + date_range[1]) / 2)))
                 f.write(" " * (max_date_length - len(str(avg_date)) + 2))
                 f.write(avg_date)
@@ -1236,14 +1885,15 @@
         long_table: bool = False,
         split_missing: bool = True,
         char_state_labels: bool = True,
         frequency: bool = False,
         ambiguous_as_missing: bool = False,
         calibrate_dates: bool = False,
         mrbayes: bool = False,
+        clock_model: ClockModel = ClockModel.strict,
     ):
         """Writes this Collation to the file with the given address.
 
         Args:
             file_addr (Union[Path, str]): The path to the output file.
             format (Format, optional): The desired output format.
                 If None then it is infered from the file suffix.
@@ -1269,18 +1919,21 @@
                 Note that this setting is necessary to make use of certainty degrees assigned to multiple ambiguous states in the collation.
                 Default value is False.
             ambiguous_as_missing (bool, optional): An optional flag indicating whether to treat all ambiguous states as missing data.
                 If this flag is set, then only base symbols will be generated for the NEXUS file.
                 It is only applied if the frequency option is False.
             calibrate_dates: An optional flag indicating whether to add an Assumptions block that specifies date distributions for witnesses
                 in NEXUS output.
-                This option is intended for inputs to BEAST2.
+                This option is intended for inputs to BEAST 2.
             mrbayes: An optional flag indicating whether to add a MrBayes block that specifies model settings and age calibrations for witnesses
                 in NEXUS output.
                 This option is intended for inputs to MrBayes.
+            clock_model: A ClockModel option indicating which type of clock model to use.
+                This option is intended for inputs to MrBayes and BEAST 2.
+                MrBayes does not presently support a local clock model, so it will default to a strict clock model if a local clock model is specified.
         """
         file_addr = Path(file_addr)
         format = format or Format.infer(
             file_addr.suffix
         )  # an exception will be raised here if the format or suffix is invalid
 
         if format == Format.NEXUS:
@@ -1288,25 +1941,29 @@
                 file_addr,
                 drop_constant=drop_constant,
                 char_state_labels=char_state_labels,
                 frequency=frequency,
                 ambiguous_as_missing=ambiguous_as_missing,
                 calibrate_dates=calibrate_dates,
                 mrbayes=mrbayes,
+                clock_model=clock_model,
             )
 
         if format == format.HENNIG86:
             return self.to_hennig86(file_addr, drop_constant=drop_constant)
 
         if format == format.PHYLIP:
             return self.to_phylip(file_addr, drop_constant=drop_constant)
 
         if format == format.FASTA:
             return self.to_fasta(file_addr, drop_constant=drop_constant)
 
+        if format == format.BEAST:
+            return self.to_beast(file_addr, drop_constant=drop_constant, clock_model=clock_model)
+
         if format == Format.CSV:
             return self.to_csv(
                 file_addr, drop_constant=drop_constant, long_table=long_table, split_missing=split_missing
             )
 
         if format == Format.TSV:
             return self.to_csv(
```

### Comparing `teiphy-0.1.5/teiphy/format.py` & `teiphy-0.1.6/teiphy/format.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 
 
 class Format(Enum):
     NEXUS = 'NEXUS'
     HENNIG86 = 'HENNIG86'
     PHYLIP = 'PHYLIP'
     FASTA = 'FASTA'
+    BEAST = 'BEAST'
     CSV = 'CSV'
     TSV = 'TSV'
     EXCEL = 'EXCEL'
     STEMMA = 'STEMMA'
 
     @classmethod
     def infer(cls, suffix: str):
         suffix_map = {
             ".nex": cls.NEXUS,
             ".nexus": cls.NEXUS,
             ".nxs": cls.NEXUS,
+            ".tnt": cls.HENNIG86,
             ".ph": cls.PHYLIP,
             ".phy": cls.PHYLIP,
             ".fa": cls.FASTA,
             ".fasta": cls.FASTA,
-            ".tnt": cls.HENNIG86,
+            ".xml": cls.BEAST,
             ".csv": cls.CSV,
             ".tsv": cls.TSV,
             ".xlsx": cls.EXCEL,
         }
 
         suffix_lower = suffix.lower()
         if suffix_lower in suffix_map:
```

### Comparing `teiphy-0.1.5/teiphy/main.py` & `teiphy-0.1.6/teiphy/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List  # for list-like inputs
 from importlib.metadata import version  # for checking package version
 from pathlib import Path  # for validating file address inputs
 from lxml import etree as et  # for parsing XML input
 import typer
 
 from .format import Format
-from .collation import Collation
+from .collation import Collation, ClockModel
 
 
 app = typer.Typer(rich_markup_mode="rich")
 
 
 def version_callback(value: bool):
     if value:
@@ -53,27 +53,31 @@
     ),
     ambiguous_as_missing: bool = typer.Option(
         False,
         help="Use the missing symbol instead of multistate symbols (and thus treat all ambiguities as missing data) in NEXUS output; this option is only applied if the --frequency option is not set.",
     ),
     calibrate_dates: bool = typer.Option(
         False,
-        help="Add an Assumptions block containing date distributions for witnesses to NEXUS output; this option is intended for inputs to BEAST2.",
+        help="Add an Assumptions block containing age distributions for witnesses to NEXUS output; this option is intended for NEXUS inputs to BEAST 2.",
     ),
     mrbayes: bool = typer.Option(
         False,
         help="Add a MrBayes block containing model settings and age calibrations for witnesses to NEXUS output; this option is intended for inputs to MrBayes.",
     ),
+    clock: ClockModel = typer.Option(
+        ClockModel.strict,
+        help="The clock model to use; this option is intended for inputs to MrBayes and BEAST 2. MrBayes does not presently support a local clock model, so it will default to a strict clock model if a local clock model is specified.",
+    ),
     long_table: bool = typer.Option(
         False,
-        help="Generate a long table with columns for taxa, characters, reading indices, and reading values instead of a matrix. Not applicable for NEXUS, HENNIG86, PHYLIP, FASTA, or STEMMA format. Note that if this option is set, ambiguous readings will be treated as missing data, and the --split-missing option will be ignored.",
+        help="Generate a long table with columns for taxa, characters, reading indices, and reading values instead of a matrix. Not applicable for non-tabular formats. Note that if this option is set, ambiguous readings will be treated as missing data, and the --split-missing option will be ignored.",
     ),
     split_missing: bool = typer.Option(
         False,
-        help="Treat missing characters/variation units as having a contribution of 1 split over all states/readings; if False, then missing data is ignored (i.e., all states are 0). Not applicable for NEXUS, HENNIG86, PHYLIP, FASTA, or STEMMA format.",
+        help="Treat missing characters/variation units as having a contribution of 1 split over all states/readings; if False, then missing data is ignored (i.e., all states are 0). Not applicable for non-tabular formats.",
     ),
     verbose: bool = typer.Option(False, help="Enable verbose logging (mostly for debugging purposes)."),
     version: bool = typer.Option(
         False,
         callback=version_callback,
         is_eager=True,
         help="Print the current version.",
@@ -117,10 +121,11 @@
         format=format,
         drop_constant=drop_constant,
         char_state_labels=labels,
         frequency=frequency,
         ambiguous_as_missing=ambiguous_as_missing,
         calibrate_dates=calibrate_dates,
         mrbayes=mrbayes,
+        clock_model=clock,
         long_table=long_table,
         split_missing=split_missing,
     )
```

### Comparing `teiphy-0.1.5/teiphy/reading.py` & `teiphy-0.1.6/teiphy/reading.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,14 @@
             # Populate its certainties map and text recursively using its children:
             self.certainties = {}
             for t in self.targets:
                 self.certainties[t] = 0
             self.text = xml.text if xml.text is not None else ""
             for child in xml:
                 self.parse(child, verbose)
-            # Normalize its certainties map:
-            norm = sum(self.certainties.values())
-            if norm == 0:
-                # If the norm is zero, then presumably no certainty elements were included under this element;
-                # just set the value for each target to 1 and normalize as usual:
-                for t in self.targets:
-                    self.certainties[t] = 1
-                    norm += 1
-            if norm > 0:
-                for t in self.certainties:
-                    self.certainties[t] = self.certainties[t] / norm
             # Strip any surrounding whitespace left over from spaces added between word elements:
             self.text = self.text.strip()
             # Populate its ID, using its xml:id if it has one; otherwise, use its n attribute if it has one; otherwise, use its text:
             self.id = ""
             if xml.get("{%s}id" % xml_ns) is not None:
                 self.id = xml.get("{%s}id" % xml_ns)
             elif xml.get("n") is not None:
@@ -246,14 +235,14 @@
             for child in xml:
                 self.parse(child, verbose)
                 self.text = self.text.strip() + "/"  # add a slash between each possibility
             self.text = self.text.strip("/")  # remove the last one we added
             self.text += "]"
             self.text += xml.tail if xml.tail is not None else ""
             return
-        # If it is a ref element, then set its text (stripped of "#" characters) in diagonal brackets:
+        # If it is a ref element, then set its text (stripped of "#" characters) in parentheses:
         if raw_tag == "ref":
-            self.text += "<"
+            self.text += "("
             self.text += xml.get("target").strip("#") if xml.get("target") is not None else ""
-            self.text += ">"
+            self.text += ")"
             self.text += xml.tail if xml.tail is not None else ""
             return
```

### Comparing `teiphy-0.1.5/teiphy/witness.py` & `teiphy-0.1.6/teiphy/witness.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 
+from datetime import datetime  # for calculating the current year (for dating purposes)
 from lxml import etree as et
 
 from .common import xml_ns, tei_ns
 
 
 class Witness:
     """Base class for storing TEI XML witness data internally.
 
     This corresponds to a witness element in the collation.
 
     Attributes:
         id: The ID string of this Witness. It should be unique.
         type: A string representing the type of witness. Examples include "corrector", "version", and "father".
-        date_range: A tuple containing a low and high date for this Witness.
+        date_range: A list containing a low and high date for this Witness.
     """
 
     def __init__(self, xml: et.Element, verbose: bool = False):
         """Constructs a new Witness instance from the TEI XML input.
 
         Args:
             xml: A witness element.
@@ -30,31 +31,30 @@
         elif xml.get("n") is not None:
             self.id = xml.get("n")
         else:
             self.id = xml.text
         # If it has a type, then save that; otherwise, default to "manuscript":
         self.type = xml.get("type") if xml.get("type") is not None else "manuscript"
         # If it has an origDate descendant, then use the dates in its attributes:
-        self.date_range = tuple([None, None])
+        self.date_range = [None, datetime.now().year]
         for orig_date in xml.xpath(".//tei:origDate", namespaces={"tei": tei_ns}):
-            date_range = [None, None]
+            date_range = [None, datetime.now().year]
             # Try the @when attribute first; if it is set, then it accounts for both ends of the date range:
             if orig_date.get("when") is not None:
-                date_range[0] = int(orig_date.get("when"))
+                date_range[0] = int(orig_date.get("when").split("-")[0])
                 date_range[1] = date_range[0]
-            # Failing that, try the @from and @to attributes:
-            elif orig_date.get("from") is not None or orig_date.get("to") is not None:
-                if orig_date.get("from") is not None or orig_date.get("to") is not None:
-                    date_range[0] = int(orig_date.get("from"))
-                if orig_date.get("to") is not None:
-                    date_range[1] = int(orig_date.get("to"))
-            # Failing that, try the @notBefore and @notAfter attributes:
+            # Failing that, if it has @from and @to attributes (indicating the period over which the manuscript was completed),
+            # then the completion date of the work accounts for both ends of the date range:
+            elif orig_date.get("to") is not None:
+                date_range[0] = int(orig_date.get("to").split("-")[0])
+                date_range[1] = date_range[0]
+            # Failing that, set lower and upper bounds on the witness's date using the the @notBefore and @notAfter attributes:
             elif orig_date.get("notBefore") is not None or orig_date.get("notAfter") is not None:
                 if orig_date.get("notBefore") is not None:
-                    date_range[0] = int(orig_date.get("notBefore"))
+                    date_range[0] = int(orig_date.get("notBefore").split("-")[0])
                 if orig_date.get("notAfter") is not None:
-                    date_range[1] = int(orig_date.get("notAfter"))
-            self.date_range = tuple(date_range)
+                    date_range[1] = int(orig_date.get("notAfter").split("-")[0])
+            self.date_range = date_range
             break
 
         if verbose:
             print("New Witness (id: %s, type: %s, date_range: %s)" % (self.id, self.type, str(self.date_range)))
```

### Comparing `teiphy-0.1.5/setup.py` & `teiphy-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,181 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: teiphy
+Version: 0.1.6
+Summary: Converts TEI XML collations to NEXUS and other formats
+Home-page: https://github.com/jjmccollum/teiphy
+License: MIT
+Keywords: Python,phylogenetics,text encoding,TEI,NEXUS
+Author: Joey McCollum and Robert Turnbull
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: numpy (>=1.23.2,<2.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pandas (>=1.4.4,<2.0.0)
+Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: typer (>=0.6.1,<0.7.0)
+Project-URL: Documentation, https://jjmccollum.github.io/teiphy/
+Project-URL: Repository, https://github.com/jjmccollum/teiphy
+Description-Content-Type: text/x-rst
 
-packages = \
-['teiphy']
+.. start-badges
 
-package_data = \
-{'': ['*']}
+.. image:: https://raw.githubusercontent.com/jjmccollum/teiphy/main/docs/img/teiphy-logo.svg
 
-install_requires = \
-['lxml>=4.9.1,<5.0.0',
- 'numpy>=1.23.2,<2.0.0',
- 'openpyxl>=3.0.10,<4.0.0',
- 'pandas>=1.4.4,<2.0.0',
- 'python-slugify>=6.1.2,<7.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'typer>=0.6.1,<0.7.0']
-
-entry_points = \
-{'console_scripts': ['teiphy = teiphy.main:app']}
-
-setup_kwargs = {
-    'name': 'teiphy',
-    'version': '0.1.5',
-    'description': 'Converts TEI XML collations to NEXUS and other formats',
-    'long_description': '.. start-badges\n\n.. image:: https://raw.githubusercontent.com/jjmccollum/teiphy/main/docs/img/teiphy-logo.svg\n\n|license badge| |testing badge| |coverage badge| |docs badge| |black badge| |git3moji badge| \n|iqtree badge| |raxml badge| |mrbayes badge| |stemma badge| |joss badge| |doi badge|\n\n.. |license badge| image:: https://img.shields.io/badge/license-MIT-blue.svg?style=flat\n    :target: https://choosealicense.com/licenses/mit/\n\n.. |testing badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml/badge.svg\n    :target: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml\n\n.. |docs badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/docs.yml/badge.svg\n    :target: https://jjmccollum.github.io/teiphy\n    \n.. |black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    \n.. |coverage badge| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jjmccollum/62997df516f95bbda6eaefa02b9570aa/raw/coverage-badge.json\n    :target: https://jjmccollum.github.io/teiphy/coverage/\n\n.. |git3moji badge| image:: https://img.shields.io/badge/git3moji-%E2%9A%A1%EF%B8%8F%F0%9F%90%9B%F0%9F%93%BA%F0%9F%91%AE%F0%9F%94%A4-fffad8.svg\n    :target: https://robinpokorny.github.io/git3moji/\n\n.. |iqtree badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/iqtree.yml/badge.svg\n    :target: https://github.com/jjmccollum/teiphy/actions/workflows/iqtree.yml\n\n.. |raxml badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml/badge.svg\n    :target: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml\n\n.. |mrbayes badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml/badge.svg\n    :target: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml\n\n.. |stemma badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml/badge.svg\n    :target: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml\n\n.. |joss badge| image:: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b/status.svg\n    :target: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b\n    \n.. |doi badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7455638.svg\n   :target: https://doi.org/10.5281/zenodo.7455638\n\n.. end-badges\n\n.. start-about\n\nA Python package for converting TEI XML collations to NEXUS and other formats.\n\nTextual scholars have been using phylogenetics to analyze manuscript traditions since the early 1990s.\nMany standard phylogenetic software packages accept as input the `NEXUS file format <https://doi.org/10.1093/sysbio/46.4.590>`_.\nThe ``teiphy`` program takes a collation of texts encoded using the `Text Encoding Initiative (TEI) guidelines <https://tei-c.org/release/doc/tei-p5-doc/en/html/TC.html>`_\nand converts it to a NEXUS format so that it can be used for phylogenetic analysis.\nIt can also convert to other formats as well.\n\n\n.. end-about\n\n\n.. start-quickstart\n\nInstallation\n============\n\nThe software can be installed using ``pip``:\n\n.. code-block:: bash\n\n    pip install teiphy\n\nAlternatively, you can install the package by cloning this repository and installing it with poetry:\n\n.. code-block:: bash\n\n    git clone https://github.com/jjmccollum/teiphy.git\n    cd teiphy\n    poetry install\n\nOnce the package is installed, you can run all unit tests via the command\n\n.. code-block:: bash\n\n    poetry run pytest\n\nUsage\n============\n\nTo use the software, run the ``teiphy`` command line tool:\n\n.. code-block:: bash\n\n    teiphy <input TEI XML> <output file>\n\n``teiphy`` can export to NEXUS, Hennig86 (TNT), PHYLIP (in the relaxed form used by RAxML), FASTA, CSV, TSV, Excel and STEMMA formats. \n``teiphy`` will try to infer the file format to export to from the extension of the output file. Accepted file extensions are:\n".nex", ".nexus", ".nxs", ".ph", ".phy", ".fa", ".fasta", ".tnt", ".csv", ".tsv", ".xlsx".\n\nTo explicitly say which format you wish to export to, use the ``--format`` option. For example:\n\n.. code-block:: bash\n\n    teiphy <input TEI XML> <output file> --format nexus\n\nFor more information about the other options, see the help with:\n\n.. code-block:: bash\n\n    teiphy --help\n\nOr see the documentation with explanations about `advanced usage <https://jjmccollum.github.io/teiphy/advanced.html>`_.\n\nThe software can also be used in Python directly. \nSee `API Reference <https://jjmccollum.github.io/teiphy/reference.html>`_ in the documentation for more information.\n\n.. end-quickstart\n\nCredits\n============\n\n.. start-credits\n\n``teiphy`` was designed by Joey McCollum (Australian Catholic University) and Robert Turnbull (University of Melbourne).\nWe received additional help from Stephen C. Carlson (Australian Catholic University).\n\nIf you use this software, please cite the paper: Joey McCollum and Robert Turnbull, "``teiphy``: A Python Package for Converting TEI XML Collations to NEXUS and Other Formats," *JOSS* 7.80 (2022): 4879, DOI: 10.21105/joss.04879.\n\n.. code-block:: bibtex\n\n    @article{McCollum2022, \n        author = {Joey McCollum and Robert Turnbull}, \n        title = {{teiphy: A Python Package for Converting TEI XML Collations to NEXUS and Other Formats}}, \n        journal = {Journal of Open Source Software},\n        year = {2022}, \n        volume = {7}, \n        number = {80}, \n        pages = {4879},\n        publisher = {The Open Journal}, \n        doi = {10.21105/joss.04879}, \n        url = {https://doi.org/10.21105/joss.04879}\n    }\n\n\n.. end-credits\n',
-    'author': 'Joey McCollum and Robert Turnbull',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jjmccollum/teiphy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+|license badge| |testing badge| |coverage badge| |docs badge| |black badge| |git3moji badge| 
+|iqtree badge| |raxml badge| |mrbayes badge| |beast badge| |stemma badge| |joss badge| |doi badge|
 
+.. |license badge| image:: https://img.shields.io/badge/license-MIT-blue.svg?style=flat
+    :target: https://choosealicense.com/licenses/mit/
+
+.. |testing badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/testing.yml
+
+.. |docs badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/docs.yml/badge.svg
+    :target: https://jjmccollum.github.io/teiphy
+    
+.. |black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    
+.. |coverage badge| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jjmccollum/62997df516f95bbda6eaefa02b9570aa/raw/coverage-badge.json
+    :target: https://jjmccollum.github.io/teiphy/coverage/
+
+.. |git3moji badge| image:: https://img.shields.io/badge/git3moji-%E2%9A%A1%EF%B8%8F%F0%9F%90%9B%F0%9F%93%BA%F0%9F%91%AE%F0%9F%94%A4-fffad8.svg
+    :target: https://robinpokorny.github.io/git3moji/
+
+.. |iqtree badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/iqtree.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/iqtree.yml
+
+.. |raxml badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/raxml.yml
+
+.. |mrbayes badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/mrbayes.yml
+
+.. |beast badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/beast.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/beast.yml
+
+.. |stemma badge| image:: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml/badge.svg
+    :target: https://github.com/jjmccollum/teiphy/actions/workflows/stemma.yml
+
+.. |joss badge| image:: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b/status.svg
+    :target: https://joss.theoj.org/papers/e0a813f4cdf56e9f6ae5d555ce6ed93b
+    
+.. |doi badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7455638.svg
+   :target: https://doi.org/10.5281/zenodo.7455638
+
+.. end-badges
+
+.. start-about
+
+A Python package for converting TEI XML collations to NEXUS and other formats.
+
+Textual scholars have been using phylogenetics to analyze manuscript traditions since the early 1990s.
+Many standard phylogenetic software packages accept as input the `NEXUS file format <https://doi.org/10.1093/sysbio/46.4.590>`_.
+The ``teiphy`` program takes a collation of texts encoded using the `Text Encoding Initiative (TEI) guidelines <https://tei-c.org/release/doc/tei-p5-doc/en/html/TC.html>`_
+and converts it to a NEXUS format so that it can be used for phylogenetic analysis.
+It can also convert to other formats as well, including Hennig86 (for TNT), PHYLIP (for RAxML), FASTA, and the XML format used by BEAST 2.7.
+
+
+.. end-about
+
+
+.. start-quickstart
+
+Installation
+============
+
+The software can be installed using ``pip``:
+
+.. code-block:: bash
+
+    pip install teiphy
+
+Alternatively, you can install the package by cloning this repository and installing it with poetry:
+
+.. code-block:: bash
+
+    git clone https://github.com/jjmccollum/teiphy.git
+    cd teiphy
+    poetry install
+
+Once the package is installed, you can run all unit tests via the command
+
+.. code-block:: bash
+
+    poetry run pytest
+
+Usage
+============
+
+To use the software, run the ``teiphy`` command line tool:
+
+.. code-block:: bash
+
+    teiphy <input TEI XML> <output file>
+
+``teiphy`` can export to NEXUS, Hennig86 (TNT), PHYLIP (in the relaxed form used by RAxML), FASTA, BEAST 2.7 XML, CSV, TSV, Excel and STEMMA formats. 
+``teiphy`` will try to infer the file format to export to from the extension of the output file. Accepted file extensions are:
+".nex", ".nexus", ".nxs", ".ph", ".phy", ".fa", ".fasta", ".xml", ".tnt", ".csv", ".tsv", ".xlsx".
+
+To explicitly say which format you wish to export to, use the ``--format`` option. For example:
+
+.. code-block:: bash
+
+    teiphy <input TEI XML> <output file> --format nexus
+
+For more information about the other options, see the help with:
+
+.. code-block:: bash
+
+    teiphy --help
+
+Or see the documentation with explanations about `advanced usage <https://jjmccollum.github.io/teiphy/advanced.html>`_.
+
+The software can also be used in Python directly. 
+See `API Reference <https://jjmccollum.github.io/teiphy/reference.html>`_ in the documentation for more information.
+
+.. end-quickstart
+
+Credits
+============
+
+.. start-credits
+
+``teiphy`` was designed by Joey McCollum (Australian Catholic University) and Robert Turnbull (University of Melbourne).
+We received additional help from Stephen C. Carlson (Australian Catholic University).
+
+If you use this software, please cite the paper: Joey McCollum and Robert Turnbull, "``teiphy``: A Python Package for Converting TEI XML Collations to NEXUS and Other Formats," *JOSS* 7.80 (2022): 4879, DOI: 10.21105/joss.04879.
+
+.. code-block:: bibtex
+
+    @article{McCollum2022, 
+        author = {Joey McCollum and Robert Turnbull}, 
+        title = {{teiphy: A Python Package for Converting TEI XML Collations to NEXUS and Other Formats}}, 
+        journal = {Journal of Open Source Software},
+        year = {2022}, 
+        volume = {7}, 
+        number = {80}, 
+        pages = {4879},
+        publisher = {The Open Journal}, 
+        doi = {10.21105/joss.04879}, 
+        url = {https://doi.org/10.21105/joss.04879}
+    }
+
+
+.. end-credits
 
-setup(**setup_kwargs)
```

