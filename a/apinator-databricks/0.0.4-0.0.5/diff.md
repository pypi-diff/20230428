# Comparing `tmp/apinator-databricks-0.0.4.tar.gz` & `tmp/apinator-databricks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-databricks-0.0.4.tar", last modified: Thu Apr 20 17:20:52 2023, max compression
+gzip compressed data, was "apinator-databricks-0.0.5.tar", last modified: Fri Apr 28 19:33:03 2023, max compression
```

## Comparing `apinator-databricks-0.0.4.tar` & `apinator-databricks-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      153 2023-04-20 17:20:45.370472 apinator-databricks-0.0.4/.bumpversion.cfg
--rw-r--r--   0        0        0      584 2023-04-19 20:33:39.872507 apinator-databricks-0.0.4/.github/workflows/dagger.yml
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-databricks-0.0.4/.gitignore
--rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-databricks-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-databricks-0.0.4/.ruff.toml
--rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-databricks-0.0.4/LICENSE
--rw-r--r--   0        0        0      655 2023-04-19 21:42:10.375582 apinator-databricks-0.0.4/README.md
--rw-r--r--   0        0        0       66 2023-04-20 17:20:45.369956 apinator-databricks-0.0.4/apinator_databricks/__init__.py
--rw-r--r--   0        0        0      871 2023-04-19 21:05:45.761926 apinator-databricks-0.0.4/apinator_databricks/_common/api.py
--rw-r--r--   0        0        0      254 2023-04-19 20:59:10.639252 apinator-databricks-0.0.4/apinator_databricks/_common/model.py
--rw-r--r--   0        0        0      198 2023-04-19 21:05:45.775892 apinator-databricks-0.0.4/apinator_databricks/common.py
--rw-r--r--   0        0        0      153 2023-04-19 21:05:45.767812 apinator-databricks-0.0.4/apinator_databricks/marketplace_provider/__init__.py
--rw-r--r--   0        0        0      651 2023-04-19 21:01:13.109298 apinator-databricks-0.0.4/apinator_databricks/marketplace_provider/api.py
--rw-r--r--   0        0        0     2178 2023-04-19 21:35:17.137497 apinator-databricks-0.0.4/apinator_databricks/marketplace_provider/model.py
--rw-r--r--   0        0        0      139 2023-04-19 21:04:33.333841 apinator-databricks-0.0.4/apinator_databricks/unity_catalog/__init__.py
--rw-r--r--   0        0        0     2479 2023-04-20 17:18:17.691440 apinator-databricks-0.0.4/apinator_databricks/unity_catalog/api.py
--rw-r--r--   0        0        0     3573 2023-04-20 17:00:47.987774 apinator-databricks-0.0.4/apinator_databricks/unity_catalog/model.py
--rw-r--r--   0        0        0      895 2023-04-19 20:28:33.161296 apinator-databricks-0.0.4/ci/main.py
--rw-r--r--   0        0        0      503 2023-04-19 20:48:53.408935 apinator-databricks-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      603 2023-04-20 17:20:45.369422 apinator-databricks-0.0.4/setup.cfg
--rw-r--r--   0        0        0        0 2023-04-18 01:05:39.006517 apinator-databricks-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1564 2023-04-19 21:40:03.159348 apinator-databricks-0.0.4/tests/test_marketplace_provider.py
--rw-r--r--   0        0        0     1452 2023-04-19 21:05:45.781659 apinator-databricks-0.0.4/tests/test_unity_catalog.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      145 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/.bumpversion.cfg
+-rw-r--r--   0        0        0      584 2023-04-20 17:19:38.874735 apinator-databricks-0.0.5/.github/workflows/dagger.yml
+-rw-r--r--   0        0        0      423 2023-04-28 19:32:29.902026 apinator-databricks-0.0.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     2162 2023-04-20 17:19:38.874735 apinator-databricks-0.0.5/.gitignore
+-rw-r--r--   0        0        0      696 2023-04-20 17:19:38.875754 apinator-databricks-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1044 2023-04-20 17:19:38.875754 apinator-databricks-0.0.5/.ruff.toml
+-rw-r--r--   0        0        0    11357 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/LICENSE
+-rw-r--r--   0        0        0      655 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/README.md
+-rw-r--r--   0        0        0       66 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/apinator_databricks/__init__.py
+-rw-r--r--   0        0        0      871 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/apinator_databricks/_common/api.py
+-rw-r--r--   0        0        0      301 2023-04-20 22:37:33.605665 apinator-databricks-0.0.5/apinator_databricks/_common/model.py
+-rw-r--r--   0        0        0      198 2023-04-20 17:19:38.876299 apinator-databricks-0.0.5/apinator_databricks/common.py
+-rw-r--r--   0        0        0      153 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/api.py
+-rw-r--r--   0        0        0     2252 2023-04-20 23:20:27.208660 apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/model.py
+-rw-r--r--   0        0        0      139 2023-04-20 17:19:38.877328 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/__init__.py
+-rw-r--r--   0        0        0     3391 2023-04-20 22:32:39.531667 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/api.py
+-rw-r--r--   0        0        0     4893 2023-04-20 22:50:59.150488 apinator-databricks-0.0.5/apinator_databricks/unity_catalog/model.py
+-rw-r--r--   0        0        0      895 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/ci/main.py
+-rw-r--r--   0        0        0      480 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      580 2023-04-28 19:31:54.469664 apinator-databricks-0.0.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-04-20 17:19:38.878327 apinator-databricks-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-20 17:19:38.879326 apinator-databricks-0.0.5/tests/test_marketplace_provider.py
+-rw-r--r--   0        0        0     1452 2023-04-20 17:19:38.879326 apinator-databricks-0.0.5/tests/test_unity_catalog.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 apinator-databricks-0.0.5/PKG-INFO
```

### Comparing `apinator-databricks-0.0.4/.github/workflows/dagger.yml` & `apinator-databricks-0.0.5/.github/workflows/dagger.yml`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/.gitignore` & `apinator-databricks-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/.ruff.toml` & `apinator-databricks-0.0.5/.ruff.toml`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# Enable Pyflakes `E` and `F` codes by default.
-#select = ["E", "F", "I", "UP", "RUF100"]
-select = ["E", "F", "I", "RUF100"]
-ignore = ["E501", "F722"]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-#fixable = ["A", "C", "D", "E", "F", "I", "UP"]
-fixable = ["A", "C", "D", "E", "F", "I"]
-unfixable = []
-
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-    "*/migrations/*",
-    "*/static/CACHE/*",
-    "docs",
-    "node_modules"
-]
-
-per-file-ignores = {}
-
-# Same as Black.
-line-length = 120
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-# Assume Python 3.7.
-target-version = "py37"
-
-[mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+# Enable Pyflakes `E` and `F` codes by default.
+#select = ["E", "F", "I", "UP", "RUF100"]
+select = ["E", "F", "I", "RUF100"]
+ignore = ["E501", "F722"]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+#fixable = ["A", "C", "D", "E", "F", "I", "UP"]
+fixable = ["A", "C", "D", "E", "F", "I"]
+unfixable = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "*/migrations/*",
+    "*/static/CACHE/*",
+    "docs",
+    "node_modules"
+]
+
+per-file-ignores = {}
+
+# Same as Black.
+line-length = 120
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.7.
+target-version = "py37"
+
+[mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
```

### Comparing `apinator-databricks-0.0.4/LICENSE` & `apinator-databricks-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `apinator-databricks-0.0.4/README.md` & `apinator-databricks-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/apinator_databricks/_common/api.py` & `apinator-databricks-0.0.5/apinator_databricks/_common/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/apinator_databricks/marketplace_provider/api.py` & `apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/api.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/apinator_databricks/marketplace_provider/model.py` & `apinator-databricks-0.0.5/apinator_databricks/marketplace_provider/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,24 +54,24 @@
         allow_population_by_field_name = True
 
 
 class EmbeddedNotebookFileParent(StrictBaseModel):
     parent_id: uuid.UUID
     file_parent_type: str
 
-
 class EmbeddedNotebookFileInfo(StrictBaseModel):
     id: uuid.UUID
-    display_name: Optional[str] = None
+    display_name: Optional[str]
     marketplace_file_type: str
     file_parent: EmbeddedNotebookFileParent
     mime_type: str
     download_link: str
     created_at: datetime
     updated_at: datetime
+    status: Optional[str] # Keeping this as str as enum values are not documented
 
 
 class ListingDetail(StrictBaseModel):
     description: str
     documentation_link: str = ""
     terms_of_service: str = ""
     contact_email: str = ""
```

### Comparing `apinator-databricks-0.0.4/apinator_databricks/unity_catalog/api.py` & `apinator-databricks-0.0.5/apinator_databricks/unity_catalog/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,7 +75,33 @@
                     "include_delta_metadata": "true",
                 },
             ),
             EndpointAction.retrieve(model.Table),
             EndpointAction.head(),
         ],
     )
+
+    recipients = EndpointGroup(
+        "/recipients",
+        actions=[
+            EndpointAction.list(model.RecipientList),
+            EndpointAction.retrieve(model.Recipient),
+            EndpointAction.create(model.Recipient),
+            EndpointAction.update(model.Recipient),
+            EndpointAction.partial_update(model.Recipient),
+            EndpointAction.destroy(),
+            EndpointAction(
+                action_name="rotate_token",
+                method="POST",
+                url="/{id}/rotate-token",
+                response_model=model.Recipient,
+                arg_names=["id"],
+            ),
+            EndpointAction(
+                action_name="get_share_permissions",
+                method="GET",
+                url="/{id}/share-permissions",
+                response_model=model.RecipientPermissionList,
+                arg_names=["id"],
+            ),
+        ],
+    )
```

### Comparing `apinator-databricks-0.0.4/apinator_databricks/unity_catalog/model.py` & `apinator-databricks-0.0.5/apinator_databricks/unity_catalog/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import uuid
 from datetime import datetime
 from typing import Optional, List
 
 from apinator.common import StrictBaseModel
 from pydantic import Json, BaseModel
 
-from .._common.model import DatabricksBase
+from .._common.model import DatabricksBase, SecurableDatabricksBase
 
 
-class Catalog(DatabricksBase):
+class Catalog(SecurableDatabricksBase):
     name: str
     owner: str
     comment: str
     metastore_id: uuid.UUID
     catalogue_type: Optional[str]
     isolation_mode: str
     full_name: str
 
 
 class CatalogList(StrictBaseModel):
     catalogs: List[Catalog] = []
 
 
-class Schema(DatabricksBase):
+class Schema(SecurableDatabricksBase):
     name: str
     catalog_name: str
     owner: str
     comment: str
     properties: Optional[dict]
     metastore_id: uuid.UUID
     full_name: str
@@ -45,15 +45,15 @@
     type_json: Json[dict]
     type_name: str
     type_precision: int
     type_scale: int
     type_text: str
 
 
-class Table(DatabricksBase):
+class Table(SecurableDatabricksBase):
     name: str
     catalog_name: str
     schema_name: str
     table_type: str
     data_source_format: Optional[str]
     columns: List[Column]
     storage_location: Optional[str]
@@ -79,15 +79,15 @@
     added_by: str
     shared_as: str
     cdf_enabled: bool
     history_data_sharing_status: str
     status: str
 
 
-class SharePartial(DatabricksBase):
+class SharePartial(SecurableDatabricksBase):
     name: str
     owner: str
     full_name: str
     comment: str = ""
 
 
 class Share(SharePartial):
@@ -143,10 +143,52 @@
 
 
 class SharePermissionChange(StrictBaseModel):
     add: List[Privilege]
     remove: List[Privilege]
     principal: str
 
-
 class SharePermissionChanges(StrictBaseModel):
     changes: List[SharePermissionChange]
+
+class RecipientPrivilegeAssignments(StrictBaseModel):
+    principal: Optional[str]
+    privileges: List[Privilege]
+
+class RecipientPermissionOut(StrictBaseModel):
+    privilege_assignments: List[RecipientPrivilegeAssignments] = []
+    share_name: str
+
+class RecipientPermissionList(StrictBaseModel):
+    permissions_out: List[RecipientPermissionOut]
+
+class RecipientAuthenticationType(str, enum.Enum):
+    TOKEN = "TOKEN"
+    DATABRICKS = "DATABRICKS"
+
+class RecipientIPAccessList(StrictBaseModel):
+    allowed_ip_addresses: List[str] = []
+
+class RecipientToken(DatabricksBase):
+    expiration_time: int
+    id: str
+    activation_url: Optional[str]
+
+class Recipient(SecurableDatabricksBase):
+    name: str
+    full_name: str
+    activated: Optional[bool]
+    authentication_type: RecipientAuthenticationType
+    data_recipient_global_metastore_id: Optional[str]
+    ip_access_list: Optional[RecipientIPAccessList]
+    cloud: Optional[str]
+    comment: Optional[str]
+    sharing_code: Optional[str]
+    properties_kvpairs: dict = {}
+    region: Optional[str]
+    tokens: Optional[List[RecipientToken]]
+    owner: str
+    activation_url: Optional[str]
+    metastore_id: Optional[str]
+
+class RecipientList(StrictBaseModel):
+    recipients: List[Recipient] = []
```

### Comparing `apinator-databricks-0.0.4/ci/main.py` & `apinator-databricks-0.0.5/ci/main.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/setup.cfg` & `apinator-databricks-0.0.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 302e 340d 0a6e 616d  ion = 0.0.4..nam
-00000020: 6520 3d20 6170 696e 6174 6f72 2d64 6174  e = apinator-dat
-00000030: 6162 7269 636b 730d 0a64 6573 6372 6970  abricks..descrip
-00000040: 7469 6f6e 203d 2041 5049 6e61 746f 7220  tion = APInator 
-00000050: 6269 6e64 696e 6720 746f 2044 6174 6162  binding to Datab
-00000060: 7269 636b 7320 4150 490d 0a61 7574 686f  ricks API..autho
-00000070: 7220 3d20 5265 6172 6320 4461 7461 0d0a  r = Rearc Data..
-00000080: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
-00000090: 6174 6140 7265 6172 632e 696f 0d0a 0d0a  ata@rearc.io....
-000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000b0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000c0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000d0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000000e0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-000000f0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-00000100: 2f67 6974 6875 622e 636f 6d2f 7265 6172  /github.com/rear
-00000110: 632d 6461 7461 2f61 7069 6e61 746f 722d  c-data/apinator-
-00000120: 6461 7461 6272 6963 6b73 0d0a 0d0a 7072  databricks....pr
-00000130: 6f6a 6563 745f 7572 6c73 203d 0d0a 2020  oject_urls =..  
-00000140: 2020 4275 6720 5472 6163 6b65 7220 3d20    Bug Tracker = 
-00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000160: 6f6d 2f72 6561 7263 2d64 6174 612f 6170  om/rearc-data/ap
-00000170: 696e 6174 6f72 2d64 6174 6162 7269 636b  inator-databrick
-00000180: 732f 6973 7375 6573 0d0a 636c 6173 7369  s/issues..classi
-00000190: 6669 6572 7320 3d0d 0a20 2020 2050 726f  fiers =..    Pro
-000001a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001c0: 0d0a 2020 2020 4c69 6365 6e73 6520 3a3a  ..    License ::
-000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001e0: 204d 4954 204c 6963 656e 7365 0d0a 2020   MIT License..  
-000001f0: 2020 4f70 6572 6174 696e 6720 5379 7374    Operating Syst
-00000200: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000210: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000220: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
-00000230: 6e64 3a0d 0a0d 0a5b 6f70 7469 6f6e 732e  nd:....[options.
-00000240: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000250: 7768 6572 6520 3d20 2e0d 0a              where = ...
+00000000: 5b6d 6574 6164 6174 615d 0a76 6572 7369  [metadata].versi
+00000010: 6f6e 203d 2030 2e30 2e35 0a6e 616d 6520  on = 0.0.5.name 
+00000020: 3d20 6170 696e 6174 6f72 2d64 6174 6162  = apinator-datab
+00000030: 7269 636b 730a 6465 7363 7269 7074 696f  ricks.descriptio
+00000040: 6e20 3d20 4150 496e 6174 6f72 2062 696e  n = APInator bin
+00000050: 6469 6e67 2074 6f20 4461 7461 6272 6963  ding to Databric
+00000060: 6b73 2041 5049 0a61 7574 686f 7220 3d20  ks API.author = 
+00000070: 5265 6172 6320 4461 7461 0a61 7574 686f  Rearc Data.autho
+00000080: 725f 656d 6169 6c20 3d20 6461 7461 4072  r_email = data@r
+00000090: 6561 7263 2e69 6f0a 0a6c 6f6e 675f 6465  earc.io..long_de
+000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000b0: 3a20 5245 4144 4d45 2e6d 640a 6c6f 6e67  : README.md.long
+000000c0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000d0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+000000e0: 2f6d 6172 6b64 6f77 6e0a 7572 6c20 3d20  /markdown.url = 
+000000f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000100: 6f6d 2f72 6561 7263 2d64 6174 612f 6170  om/rearc-data/ap
+00000110: 696e 6174 6f72 2d64 6174 6162 7269 636b  inator-databrick
+00000120: 730a 0a70 726f 6a65 6374 5f75 726c 7320  s..project_urls 
+00000130: 3d0a 2020 2020 4275 6720 5472 6163 6b65  =.    Bug Tracke
+00000140: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+00000150: 7562 2e63 6f6d 2f72 6561 7263 2d64 6174  ub.com/rearc-dat
+00000160: 612f 6170 696e 6174 6f72 2d64 6174 6162  a/apinator-datab
+00000170: 7269 636b 732f 6973 7375 6573 0a63 6c61  ricks/issues.cla
+00000180: 7373 6966 6965 7273 203d 0a20 2020 2050  ssifiers =.    P
+00000190: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001b0: 2033 0a20 2020 204c 6963 656e 7365 203a   3.    License :
+000001c0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001d0: 3a20 4d49 5420 4c69 6365 6e73 650a 2020  : MIT License.  
+000001e0: 2020 4f70 6572 6174 696e 6720 5379 7374    Operating Syst
+000001f0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000200: 6465 6e74 0a0a 5b6f 7074 696f 6e73 5d0a  dent..[options].
+00000210: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000220: 0a0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000230: 6765 732e 6669 6e64 5d0a 7768 6572 6520  ges.find].where 
+00000240: 3d20 2e0a                                = ..
```

### Comparing `apinator-databricks-0.0.4/tests/test_marketplace_provider.py` & `apinator-databricks-0.0.5/tests/test_marketplace_provider.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/tests/test_unity_catalog.py` & `apinator-databricks-0.0.5/tests/test_unity_catalog.py`

 * *Files identical despite different names*

### Comparing `apinator-databricks-0.0.4/PKG-INFO` & `apinator-databricks-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apinator-databricks
-Version: 0.0.4
+Version: 0.0.5
 Summary: APInator bindings for Databricks API
 Author-email: Rearc Data <data@rearc.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: apinator~=0.0.2
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
```

