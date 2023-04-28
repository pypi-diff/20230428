# Comparing `tmp/releases-2.0.1.tar.gz` & `tmp/releases-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpz7g_gb8v/dist/releases-2.0.1.tar", last modified: Fri Apr 28 18:53:50 2023, max compression
+gzip compressed data, was "/tmp/tmpyadrnne_/dist/releases-2.1.0.tar", last modified: Sat Feb 25 00:01:32 2023, max compression
```

## Comparing `releases-2.0.1.tar` & `releases-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 18:53:50.000000 releases-2.0.1/
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:56:00.000000 releases-2.0.1/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-04-28 18:53:50.000000 releases-2.0.1/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     2386 2023-02-16 19:51:03.000000 releases-2.0.1/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)      524 2022-08-27 19:49:59.000000 releases-2.0.1/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)       31 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      484 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-04-28 18:53:50.000000 releases-2.0.1/releases.egg-info/PKG-INFO
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 18:53:50.000000 releases-2.0.1/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     9786 2023-04-28 18:37:50.000000 releases-2.0.1/tests/presentation.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5621 2022-12-19 02:06:53.000000 releases-2.0.1/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    16319 2023-04-28 18:37:50.000000 releases-2.0.1/tests/organization.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3500 2022-12-18 03:30:08.000000 releases-2.0.1/tests/_util.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 18:53:50.000000 releases-2.0.1/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)      162 2022-06-17 18:56:00.000000 releases-2.0.1/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      605 2023-04-28 18:37:50.000000 releases-2.0.1/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11688 2023-04-28 18:53:47.000000 releases-2.0.1/docs/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    19093 2023-02-17 23:17:42.000000 releases-2.0.1/docs/concepts.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     7547 2023-04-28 18:37:50.000000 releases-2.0.1/docs/usage.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 18:53:50.000000 releases-2.0.1/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)     2314 2022-08-27 19:49:59.000000 releases-2.0.1/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      311 2023-04-28 18:36:21.000000 releases-2.0.1/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 18:53:50.000000 releases-2.0.1/releases/
--rw-r--r--   0 jforcier  (1000) users      (100)    28229 2023-04-28 18:37:50.000000 releases-2.0.1/releases/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9956 2023-04-28 18:53:24.000000 releases-2.0.1/releases/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 18:53:50.000000 releases-2.0.1/releases/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2556 2023-02-16 19:52:34.000000 releases-2.0.1/releases/line_manager.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7388 2023-02-16 19:52:34.000000 releases-2.0.1/releases/models.py
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2022-06-17 18:56:00.000000 releases-2.0.1/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)       31 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      502 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        9 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-02-25 00:01:32.000000 releases-2.1.0/releases.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2022-06-17 18:56:00.000000 releases-2.1.0/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)      327 2022-12-31 04:35:57.000000 releases-2.1.0/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-02-25 00:01:32.000000 releases-2.1.0/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)    11927 2023-02-24 22:24:17.000000 releases-2.1.0/docs/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    19093 2023-02-17 23:17:42.000000 releases-2.1.0/docs/concepts.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      162 2022-06-17 18:56:00.000000 releases-2.1.0/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     8141 2023-02-24 22:23:42.000000 releases-2.1.0/docs/usage.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      605 2022-12-18 03:30:08.000000 releases-2.1.0/docs/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/releases/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2556 2023-02-16 19:52:34.000000 releases-2.1.0/releases/line_manager.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9939 2022-09-30 22:33:57.000000 releases-2.1.0/releases/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-24 22:23:42.000000 releases-2.1.0/releases/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7388 2023-02-16 19:52:34.000000 releases-2.1.0/releases/models.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28550 2023-02-24 22:23:42.000000 releases-2.1.0/releases/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-02-25 00:01:32.000000 releases-2.1.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3500 2022-12-18 03:30:08.000000 releases-2.1.0/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10659 2023-02-24 22:23:42.000000 releases-2.1.0/tests/presentation.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      102 2023-02-24 22:23:42.000000 releases-2.1.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19083 2023-02-24 22:23:42.000000 releases-2.1.0/tests/organization.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5621 2022-12-19 02:06:53.000000 releases-2.1.0/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2386 2023-02-16 19:51:03.000000 releases-2.1.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      524 2022-08-27 19:49:59.000000 releases-2.1.0/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4227 2023-02-25 00:01:32.000000 releases-2.1.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:56:00.000000 releases-2.1.0/LICENSE
+-rw-r--r--   0 jforcier  (1000) users      (100)     2314 2022-08-27 19:49:59.000000 releases-2.1.0/README.rst
```

### Comparing `releases-2.0.1/LICENSE` & `releases-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/PKG-INFO` & `releases-2.1.0/releases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: releases
-Version: 2.0.1
+Version: 2.1.0
 Summary: A Sphinx extension for changelog manipulation
 Home-page: https://github.com/bitprophet/releases
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: UNKNOWN
 Project-URL: Docs, https://releases.readthedocs.io
 Project-URL: Source, https://github.com/bitprophet/releases
```

### Comparing `releases-2.0.1/setup.py` & `releases-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/tasks.py` & `releases-2.1.0/tasks.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/releases.egg-info/PKG-INFO` & `releases-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: releases
-Version: 2.0.1
+Version: 2.1.0
 Summary: A Sphinx extension for changelog manipulation
 Home-page: https://github.com/bitprophet/releases
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: UNKNOWN
 Project-URL: Docs, https://releases.readthedocs.io
 Project-URL: Source, https://github.com/bitprophet/releases
```

### Comparing `releases-2.0.1/tests/presentation.py` & `releases-2.1.0/tests/presentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,23 +35,25 @@
 
     def _generate(self, *entries, **kwargs):
         raw = kwargs.pop("raw", False)
         nodes = construct_nodes(releases(*entries, **kwargs))
         # By default, yield the contents of the bullet list.
         return nodes if raw else nodes[0][1][0]
 
-    def _test_link(self, kwargs, type_, expected):
+    def _test_link(self, kwargs, type_, expected, entries=None):
         app = make_app(**kwargs)
+        # Lazy-evaluated entries: (callable, *args)
+        entries = entries or [
+            (release, "1.0.2"),
+            (b, 15),
+            (release, "1.0.0"),
+        ]
         nodes = construct_nodes(
             construct_releases(
-                [
-                    release("1.0.2", app=app),
-                    entry(b(15, app=app)),
-                    release("1.0.0"),
-                ],
+                [entry(x[0](*x[1:], app=app)) for x in entries],
                 app=app,
             )[0]
         )
         # Shorthand for "I'll do my own asserts"
         if expected is None:
             return nodes
         if type_ == "release":
@@ -218,49 +220,68 @@
         assert para[2].astext() == "#15"
         assert "Bug" in para[0].astext()
         # Second/inline link
         _expect_type(para[6], reference)
         assert para[6].astext() == "#5"
         assert "Support" in para[4].astext()
 
-    def unreleased_buckets_omit_major_version_when_only_one_exists(self):
-        result = self._generate(b(1), raw=True)[0][0][0]
-        html = str(result)  # since repr() from test-fail hides actual text
-        assert "Next bugfix release" in html
-
-    def unreleased_buckets_display_major_version_when_multiple(self):
-        entries = (
-            b(3),  # should appear in unreleased bugs for 2.x
-            "2.0.0",
-            b(2),  # should appear in unreleased bugs for 1.x
-            "1.0.1",
-            b(1),
-        )
-        # Expectation: [2.x unreleased, 1.x unreleased, 1.0.1]
-        two_x, one_x, _ = self._generate(*entries, raw=True)
-        html = str(two_x[0][0])
-        assert "Next 2.x bugfix release" in html
-        html = str(one_x[0][0])
-        assert "Next 1.x bugfix release" in html
-
-    def unreleased_displays_version_when_only_some_lines_displayed(self):
-        # I.e. if there's unreleased 1.x stuff but no unreleased 2.x, still
-        # display the "1.x".
-        entries = (
-            # Note lack of any bugfixes post 2.0.0
-            "2.0.0",
-            b(2),
-            "1.0.1",
-            b(1),
-        )
-        # Expectation: [1.x unreleased, 1.0.1] - no 2.x.
-        result = self._generate(*entries, raw=True)
-        assert len(result) == 2
-        html = str(result[0][0][0])
-        assert "Next 1.x bugfix release" in html
+    class unreleased:
+        def buckets_omit_major_version_when_only_one_exists(self):
+            result = self._generate(b(1), raw=True)[0][0][0]
+            html = str(result)  # since repr() from test-fail hides actual text
+            assert "Next bugfix release" in html
+
+        def buckets_display_major_version_when_multiple(self):
+            entries = (
+                b(3),  # should appear in unreleased bugs for 2.x
+                "2.0.0",
+                b(2),  # should appear in unreleased bugs for 1.x
+                "1.0.1",
+                b(1),
+            )
+            # Expectation: [2.x unreleased, 1.x unreleased, 1.0.1]
+            two_x, one_x, _ = self._generate(*entries, raw=True)
+            html = str(two_x[0][0])
+            assert "Next 2.x bugfix release" in html
+            html = str(one_x[0][0])
+            assert "Next 1.x bugfix release" in html
+
+        def displays_version_when_only_some_lines_displayed(self):
+            # I.e. if there's unreleased 1.x stuff but no unreleased 2.x, still
+            # display the "1.x".
+            entries = (
+                # Note lack of any bugfixes post 2.0.0
+                "2.0.0",
+                b(2),
+                "1.0.1",
+                b(1),
+            )
+            # Expectation: [1.x unreleased, 1.0.1] - no 2.x.
+            result = self._generate(*entries, raw=True)
+            assert len(result) == 2
+            html = str(result[0][0][0])
+            assert "Next 1.x bugfix release" in html
+
+        def feature_section_links_go_to_development_branch(self):
+            self._test_link(
+                kwargs=dict(release_uri="releasey_%s"),
+                type_="release",
+                expected="releasey_master",
+                entries=[(f, 15), (release, "1.0.0")],
+            )
+
+        def feature_section_links_can_configure_branch_name(self):
+            self._test_link(
+                kwargs=dict(
+                    development_branch="main", release_uri="releasey_%s"
+                ),
+                type_="release",
+                expected="releasey_main",
+                entries=[(f, 15), (release, "1.0.0")],
+            )
 
     def unstable_prehistory_active_means_only_one_unreleased_release(self):
         app = make_app(unstable_prehistory=True)
         entries = (b(2), f(3), "0.1.0", b(1))
         result = self._generate(*entries, app=app, raw=True, skip_initial=True)
         html = str(result[0][0][0])
         assert "Next release" in html
```

### Comparing `releases-2.0.1/tests/util.py` & `releases-2.1.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/tests/organization.py` & `releases-2.1.0/tests/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -185,14 +185,78 @@
         assert f2 in rendered["1.1.0"]
         assert f1 not in rendered["1.1.0"]
         # unreleased feature list should still get/see feature 1
         assert f1 in rendered["unreleased_1.x_feature"]
         # now-released feature 2 should not be in unreleased_feature
         assert f2 not in rendered["unreleased_1.x_feature"]
 
+    class unsupported_families_not_included_in_unreleased:
+        _entries = (
+            f(7),  # should appear in unreleased features for 3.x
+            b(6),  # should appear in unreleased bugs for 3.x
+            "3.0.0",
+            f(5),  # should appear in unreleased features for 2.x
+            b(4),  # should appear in unreleased bugs for 2.x
+            "2.0.0",
+            f(3),  # should appear in unreleased features for 1.x
+            b(2),  # should appear in unreleased bugs for 1.x
+            "1.0.1",
+            b(1),  # prehistory
+        )
+
+        def no_actual_hiding_when_given_but_contains_all_families(self):
+            # Expectation: everything
+            families = [1, 2, 3]
+            for option in (None, families):  # Also test default None
+                changelog = release_list(*self._entries)
+                releases = changelog2dict(
+                    construct_releases(
+                        changelog, make_app(supported_versions=option)
+                    )[0]
+                )
+                for major in families:
+                    for type_ in ("bugfix", "feature"):
+                        assert f"unreleased_{major}.x_{type_}" in releases
+
+        def one_old_family_hidden(self):
+            changelog = release_list(*self._entries)
+            releases = changelog2dict(
+                construct_releases(
+                    changelog, make_app(supported_versions=[2, 3])
+                )[0]
+            )
+            for type_ in ("bugfix", "feature"):
+                assert f"unreleased_1.x_{type_}" not in releases
+                assert f"unreleased_2.x_{type_}" in releases
+                assert f"unreleased_3.x_{type_}" in releases
+
+        def multiple_old_families_hidden(self):
+            changelog = release_list(*self._entries)
+            releases = changelog2dict(
+                construct_releases(
+                    changelog, make_app(supported_versions=[3])
+                )[0]
+            )
+            for type_ in ("bugfix", "feature"):
+                assert f"unreleased_1.x_{type_}" not in releases
+                assert f"unreleased_2.x_{type_}" not in releases
+                assert f"unreleased_3.x_{type_}" in releases
+
+        def in_between_family_hidden_for_mysterious_reasons(self):
+            changelog = release_list(*self._entries)
+            releases = changelog2dict(
+                construct_releases(
+                    changelog, make_app(supported_versions=[1, 3])
+                )[0]
+            )
+            for type_ in ("bugfix", "feature"):
+                assert f"unreleased_1.x_{type_}" in releases
+                assert f"unreleased_2.x_{type_}" not in releases
+                assert f"unreleased_3.x_{type_}" in releases
+
     def explicit_bugfix_releases_get_removed_from_unreleased(self):
         b1 = b(1)
         b2 = b(2)
         changelog = release_list("1.0.1", b1, b2)
         # Ensure that 1.0.1 specifies bug 2
         changelog[0][0].append(Text("2"))
         rendered, _ = construct_releases(changelog, make_app())
```

### Comparing `releases-2.0.1/tests/_util.py` & `releases-2.1.0/tests/_util.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/docs/conf.py` & `releases-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/docs/changelog.rst` & `releases-2.1.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 =========
 Changelog
 =========
 
-- :release:`2.0.1 <2023-04-28>`
-- :bug:`-` Fix up an internal utility which monkeypatches a Sphinx/docutils
-  internal, so that it accepts arbitrary args/kwargs instead of exploding on
-  newer Sphinxes.
+- :release:`2.1.0 <2023-02-24>`
+- :feature:`-` Add a new configuration setting,
+  ``releases_supported_versions``, allowing you to limit how many "Next 1.x
+  feature release" (or bugfix, etc) sections appear at the top of your
+  changelog.
+- :feature:`-` Allow controlling the name of your development branch for source
+  code links (eg "Next 1.x feature release" section headers) via the new
+  ``releases_development_branch`` config option.
 - :release:`2.0.0 <2022-12-31>`
 - :bug:`- major` Changelog transformation sometimes failed to occur when
   running under a 'single HTML file' Sphinx builder (eg ``singlehtml``), which
   resulted in 'unknown node' errors. This has been fixed.
 - :support:`-` Administrivia overhaul: enhanced README, packaging metadata
   cleaned up/expanded, CI moved to Circle-CI, renamed dev branch to ``main``,
   and more besides.
```

### Comparing `releases-2.0.1/docs/concepts.rst` & `releases-2.1.0/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/docs/usage.rst` & `releases-2.1.0/docs/usage.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 =====
 Usage
 =====
 
 To use Releases, mimic the format seen in `its own changelog
-<https://raw.github.com/bitprophet/releases/master/docs/changelog.rst>`_ or in
+<https://raw.github.com/bitprophet/releases/main/docs/changelog.rst>`_ or in
 `Fabric's changelog
-<https://raw.github.com/fabric/fabric/master/sites/www/changelog.rst>`_.
+<https://raw.github.com/fabric/fabric/main/sites/www/changelog.rst>`_.
 Specifically:
 
 * Install ``releases`` and update your Sphinx ``conf.py`` to include it in the
   ``extensions`` list setting: ``extensions = ['releases']``.
 
     * Also set the ``releases_release_uri`` and ``releases_issue_uri`` top
       level options - they determine the targets of the issue & release links
@@ -37,14 +37,23 @@
       you may want to set ``releases_unstable_prehistory = True``.
 
         * This is also useful if you've just imported a non-Releases changelog,
           where your issues are all basic list-items and you don't want to go
           through and add bug/feature/support/etc roles.
         * See :ref:`the appropriate conceptual docs <unstable-prehistory>` for
           details on this behavior.
+    * If your development branch which is linked to for unreleased changelog
+      items, does not match the current default (``master`` as of version 2.0,
+      to be changed to ``main`` in 3.0), you may override it via
+      ``releases_development_branch``.
+    * Projects with a long history of major release versions may want to
+      specify which of them get 'unreleased' entries at the top of the
+      changelog; set ``releases_supported_versions`` to a list of major version
+      numbers, eg ``releases_supported_versions = [2, 3]`` to drop any "Next
+      1.x (feature|bugfix)" buckets.
 
 * Create a Sphinx document named ``changelog.rst`` containing a bulleted list
   somewhere at its topmost level.
 
     * If you wish to use a different document name, use another config option
       (as per previous bullet point), ``releases_document_name``. E.g.
       ``releases_document_name = "CHANGES"`` would cause Releases to mutate a
```

### Comparing `releases-2.0.1/README.rst` & `releases-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/releases/__init__.py` & `releases-2.1.0/releases/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     try:
         return Spec(keyword)
     # I've only ever seen Spec fail with ValueError.
     except ValueError:
         return None
 
 
+# TODO 3.0: make this less dumb, do away with %s, just have callers do
+# f-strings or un-opinionated .format
 def interpolate(text, number):
     if "%s" in text:
         return text % number
     return text.format(number=number)
 
 
 def issues_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
@@ -177,18 +179,15 @@
 
 
 def generate_unreleased_entry(header, line, issues, manager, app):
     log = partial(_log, config=app.config)
     nodelist = [
         release_nodes(
             header,
-            # TODO: should link to master for newest family and...what
-            # exactly, for the others? Expectation isn't necessarily to
-            # have a branch per family? Or is there? Maybe there must be..
-            "master",
+            app.config.releases_development_branch,
             None,
             app.config,
         )
     ]
     log(f"Creating {line!r} faux-release with {issues!r}")
     return {
         "obj": Release(number=line, date=None, nodelist=nodelist),
@@ -201,14 +200,18 @@
     Generate new abstract 'releases' for unreleased issues.
 
     There's one for each combination of bug-vs-feature & major release line.
 
     When only one major release line exists, that dimension is ignored.
     """
     for family, lines in manager.items():
+        # Skip over any unsupported lines
+        supported = app.config.releases_supported_versions
+        if supported is not None and family not in supported:
+            continue
         for type_ in ("bugfix", "feature"):
             bucket = f"unreleased_{type_}"
             if bucket not in lines:  # Implies unstable prehistory + 0.x fam
                 continue
             issues = lines[bucket]
             fam_prefix = f"{family}.x " if len(manager) > 1 else ""
             header = f"Next {fam_prefix}{type_} release"
@@ -640,20 +643,25 @@
         # E.g. 'https://github.com/fabric/fabric/issues/'
         ("issue_uri", None),
         # Release-tag base URI setting: releases_release_uri
         # E.g. 'https://github.com/fabric/fabric/tree/'
         ("release_uri", None),
         # Convenience Github version of above
         ("github_path", None),
+        # Which branch to use for unreleased feature items
+        # TODO 3.0: s/master/main/
+        ("development_branch", "master"),
+        # Which versions to show unreleased buckets for
+        ("supported_versions", None),
         # Which document to use as the changelog
         ("document_name", ["changelog"]),
         # Debug output
         ("debug", False),
         # Whether to enable linear history during 0.x release timeline
-        # TODO: flip this to True by default in our 3.0 release
+        # TODO 3.0: flip this to True by default?
         ("unstable_prehistory", False),
     ):
         app.add_config_value(
             name=f"releases_{key}", default=default, rebuild="html"
         )
     if isinstance(app.config.releases_document_name, str):
         app.config.releases_document_name = [app.config.releases_document_name]
```

### Comparing `releases-2.0.1/releases/util.py` & `releases-2.1.0/releases/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         # - bring over all per-line buckets from manager (flattening)
         # Here, all that's left in the per-family bucket should be lines, not
         # unreleased_*
         ret.update(manager[family])
     return ret
 
 
-def _faux_write_doctree(self, docname, doctree, *args, **kwargs):
+def _faux_write_doctree(self, docname, doctree):
     self._read_doctree = doctree
 
 
 def get_doctree(path, **kwargs):
     """
     Obtain a mostly-rendered Sphinx doctree from the RST file at ``path``.
```

### Comparing `releases-2.0.1/releases/line_manager.py` & `releases-2.1.0/releases/line_manager.py`

 * *Files identical despite different names*

### Comparing `releases-2.0.1/releases/models.py` & `releases-2.1.0/releases/models.py`

 * *Files identical despite different names*

