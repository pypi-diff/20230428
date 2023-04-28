# Comparing `tmp/git_add_co_author-0.4.0.tar.gz` & `tmp/git_add_co_author-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_add_co_author-0.4.0.tar", max compression
+gzip compressed data, was "git_add_co_author-0.4.1.tar", max compression
```

## Comparing `git_add_co_author-0.4.0.tar` & `git_add_co_author-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2218 2023-04-28 21:29:06.899258 git_add_co_author-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.4.0/git_add_co_author/__init__.py
--rw-r--r--   0        0        0     2171 2023-04-28 21:17:31.737873 git_add_co_author-0.4.0/git_add_co_author/__main__.py
--rw-r--r--   0        0        0      360 2023-04-28 21:29:15.581867 git_add_co_author-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 git_add_co_author-0.4.0/setup.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 git_add_co_author-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2218 2023-04-28 21:29:06.899258 git_add_co_author-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.4.1/git_add_co_author/__init__.py
+-rw-r--r--   0        0        0     2171 2023-04-28 21:17:31.737873 git_add_co_author-0.4.1/git_add_co_author/__main__.py
+-rw-r--r--   0        0        0      464 2023-04-28 21:36:03.030286 git_add_co_author-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 git_add_co_author-0.4.1/setup.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 git_add_co_author-0.4.1/PKG-INFO
```

### Comparing `git_add_co_author-0.4.0/README.md` & `git_add_co_author-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `git_add_co_author-0.4.0/git_add_co_author/__main__.py` & `git_add_co_author-0.4.1/git_add_co_author/__main__.py`

 * *Files identical despite different names*

### Comparing `git_add_co_author-0.4.0/setup.py` & `git_add_co_author-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0', 'requests>=2.29.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'git-add-co-author',
-    'version': '0.4.0',
-    'description': '',
+    'version': '0.4.1',
+    'description': 'Git Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits.',
     'long_description': '# Git Add Co-Author\n\n## Demo\n![git-add-co-author](https://user-images.githubusercontent.com/29942790/235257344-93578bf7-104a-46b7-9785-ef6620a019b5.gif)\n\n\n\n## Overview\n\nGit Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits, ensuring proper credit is given to all contributors involved in the development process. This can be particularly useful for open-source projects, where multiple contributors are working together, or for pair programming sessions where two developers contribute to the same commit.\n\n## Installation\n\n1. Install the package using pip:\n\n```bash\npip install git-add-co-author\n```\n\n2. Obtain a personal access token from GitHub. You can generate one by following the instructions in the [GitHub documentation](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).\n\n3. Configure the script with your GitHub token:\n\n```bash\npython -m git_add_co_author --token <your_token>\n```\n\n## Usage\n\nTo add a co-author to your commit, simply run the script with the co-author\'s GitHub username:\n\n```bash\npython -m git_add_co_author --username <co_author_username>\n```\n\nFor example:\n\n```bash\npython -m git_add_co_author sansyrox\n```\n\nIf you do not want to authorize a token, you can add the co-author\'s name and email address directly:\n\n```bash\npython -m git_add_co_author --name "John Doe" --email "john.doe@example.com"\n```\n\n### Optional Configuration\n\nI alias this command as `alias gac="python -m git_add_co_author --username"` in my `.zshrc` file, so I can simply run `gac <co_author_username>` to add a co-author to my commit.\n\n## Rationale\n\nThe motivation behind creating this script is to provide an easy way to give credit to contributors in various situations:\n\n- In open-source projects, when a pull request (PR) is closed without merging but the idea or code is later implemented.\n- During pair programming sessions, where two or more developers work together on a single commit.\n\nExisting solutions were either too complicated or didn\'t work as expected, so Git Add Co-Author was developed as a simple, easy-to-use alternative.\n\n## License\n\nThis project is licensed under the MIT License.\n',
     'author': 'Sanskar Jethi',
     'author_email': 'sansyrox@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `git_add_co_author-0.4.0/PKG-INFO` & `git_add_co_author-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: git-add-co-author
-Version: 0.4.0
-Summary: 
+Version: 0.4.1
+Summary: Git Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits.
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Git Add Co-Author
```

