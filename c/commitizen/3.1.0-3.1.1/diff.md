# Comparing `tmp/commitizen-3.1.0.tar.gz` & `tmp/commitizen-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.1.0.tar", max compression
+gzip compressed data, was "commitizen-3.1.1.tar", max compression
```

## Comparing `commitizen-3.1.0.tar` & `commitizen-3.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-04-25 17:05:02.037353 commitizen-3.1.0/LICENSE
--rw-r--r--   0        0        0      593 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__version__.py
--rw-r--r--   0        0        0     8613 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/bump.py
--rw-r--r--   0        0        0    11909 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16605 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13932 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     6845 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3059 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12935 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1384 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     3016 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3125 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3310 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/version_types.py
--rw-r--r--   0        0        0     5800 2023-04-25 17:05:02.041354 commitizen-3.1.0/docs/README.md
--rw-r--r--   0        0        0     3959 2023-04-25 17:05:02.053353 commitizen-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-28 07:42:11.206104 commitizen-3.1.1/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     8613 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/bump.py
+-rw-r--r--   0        0        0    11956 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16605 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13932 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7266 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3059 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12935 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1384 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     3016 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3125 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3310 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/version_types.py
+-rw-r--r--   0        0        0     5800 2023-04-28 07:42:11.210104 commitizen-3.1.1/docs/README.md
+-rw-r--r--   0        0        0     3959 2023-04-28 07:42:11.222104 commitizen-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.1.1/PKG-INFO
```

### Comparing `commitizen-3.1.0/LICENSE` & `commitizen-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/__init__.py` & `commitizen-3.1.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/bump.py` & `commitizen-3.1.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/changelog.py` & `commitizen-3.1.1/commitizen/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,18 +86,20 @@
     change_type_map: Optional[Dict[str, str]] = None,
     changelog_message_builder_hook: Optional[Callable] = None,
     merge_prerelease: bool = False,
 ) -> Iterable[Dict]:
     pat = re.compile(changelog_pattern)
     map_pat = re.compile(commit_parser, re.MULTILINE)
     body_map_pat = re.compile(commit_parser, re.MULTILINE | re.DOTALL)
+    current_tag: Optional[GitTag] = None
 
     # Check if the latest commit is not tagged
-    latest_commit = commits[0]
-    current_tag: Optional[GitTag] = get_commit_tag(latest_commit, tags)
+    if commits:
+        latest_commit = commits[0]
+        current_tag = get_commit_tag(latest_commit, tags)
 
     current_tag_name: str = unreleased_version or "Unreleased"
     current_tag_date: str = ""
     if unreleased_version is not None:
         current_tag_date = date.today().isoformat()
     if current_tag is not None and current_tag.name:
         current_tag_name = current_tag.name
```

### Comparing `commitizen-3.1.0/commitizen/changelog_parser.py` & `commitizen-3.1.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cli.py` & `commitizen-3.1.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cmd.py` & `commitizen-3.1.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/commands/bump.py` & `commitizen-3.1.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/commands/changelog.py` & `commitizen-3.1.1/commitizen/commands/changelog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os.path
 from difflib import SequenceMatcher
 from operator import itemgetter
 from typing import Callable, Dict, List, Optional
 
+from packaging.version import parse
+
 from commitizen import bump, changelog, defaults, factory, git, out, version_types
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     DryRunExit,
     NoCommitsFoundError,
     NoPatternMapError,
     NoRevisionError,
@@ -32,14 +34,21 @@
         self.file_name = args.get("file_name") or self.config.settings.get(
             "changelog_file"
         )
         self.incremental = args["incremental"] or self.config.settings.get(
             "changelog_incremental"
         )
         self.dry_run = args["dry_run"]
+
+        self.current_version = (
+            args.get("current_version") or self.config.settings.get("version") or ""
+        )
+        self.current_version_instance = (
+            parse(self.current_version) if self.current_version else None
+        )
         self.unreleased_version = args["unreleased_version"]
         self.change_type_map = (
             self.config.settings.get("change_type_map") or self.cz.change_type_map
         )
         self.change_type_order = (
             self.config.settings.get("change_type_order")
             or self.cz.change_type_order
@@ -151,15 +160,18 @@
                 tags,
                 version=self.rev_range,
                 tag_format=self.tag_format,
                 version_type_cls=self.version_type,
             )
 
         commits = git.get_commits(start=start_rev, end=end_rev, args="--topo-order")
-        if not commits:
+        if not commits and (
+            self.current_version_instance is None
+            or not self.current_version_instance.is_prerelease
+        ):
             raise NoCommitsFoundError("No commits found")
 
         tree = changelog.generate_tree_from_commits(
             commits,
             tags,
             commit_parser,
             changelog_pattern,
```

### Comparing `commitizen-3.1.0/commitizen/commands/check.py` & `commitizen-3.1.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/commands/commit.py` & `commitizen-3.1.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/commands/init.py` & `commitizen-3.1.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/commands/version.py` & `commitizen-3.1.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/config/__init__.py` & `commitizen-3.1.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/config/base_config.py` & `commitizen-3.1.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/config/json_config.py` & `commitizen-3.1.1/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/config/toml_config.py` & `commitizen-3.1.1/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/config/yaml_config.py` & `commitizen-3.1.1/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/__init__.py` & `commitizen-3.1.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/base.py` & `commitizen-3.1.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/customize/customize.py` & `commitizen-3.1.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/jira/jira.py` & `commitizen-3.1.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.1.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/defaults.py` & `commitizen-3.1.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/exceptions.py` & `commitizen-3.1.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/factory.py` & `commitizen-3.1.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/git.py` & `commitizen-3.1.1/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/hooks.py` & `commitizen-3.1.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/out.py` & `commitizen-3.1.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/providers.py` & `commitizen-3.1.1/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/commitizen/version_types.py` & `commitizen-3.1.1/commitizen/version_types.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/docs/README.md` & `commitizen-3.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.0/pyproject.toml` & `commitizen-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.1.0"
+version = "3.1.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.1.0"
+version = "3.1.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -39,15 +39,15 @@
 decli = "^0.5.2"
 colorama = "^0.4.1"
 termcolor = ">= 1.1, < 3"
 packaging = ">=19"
 tomlkit = ">=0.5.3,<1.0.0"
 jinja2 = ">=2.10.3"
 pyyaml = ">=3.08"
-argcomplete = ">=1.12.1,<2.2"
+argcomplete = ">=1.12.1,<3.1"
 typing-extensions = { version = "^4.0.1", python = "<3.8" }
 charset-normalizer = ">=2.1.0,<4"
 # Use the Python 3.11 compatible API: https://github.com/python/importlib_metadata#compatibility
 importlib_metadata = { version = ">=4.13,<5"}
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.34"
```

### Comparing `commitizen-3.1.0/PKG-INFO` & `commitizen-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: argcomplete (>=1.12.1,<2.2)
+Requires-Dist: argcomplete (>=1.12.1,<3.1)
 Requires-Dist: charset-normalizer (>=2.1.0,<4)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
 Requires-Dist: decli (>=0.5.2,<0.6.0)
 Requires-Dist: importlib_metadata (>=4.13,<5)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: packaging (>=19)
 Requires-Dist: pyyaml (>=3.08)
```

