# Comparing `tmp/git_add_co_author-0.2.0.tar.gz` & `tmp/git_add_co_author-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_add_co_author-0.2.0.tar", max compression
+gzip compressed data, was "git_add_co_author-0.3.0.tar", max compression
```

## Comparing `git_add_co_author-0.2.0.tar` & `git_add_co_author-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2061 2023-04-28 20:19:08.859277 git_add_co_author-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.2.0/git_add_co_author/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-28 20:09:55.084340 git_add_co_author-0.2.0/git_add_co_author/__main__.py
--rw-r--r--   0        0        0      360 2023-04-28 20:20:15.241787 git_add_co_author-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 git_add_co_author-0.2.0/setup.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 git_add_co_author-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2195 2023-04-28 21:01:52.928450 git_add_co_author-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.3.0/git_add_co_author/__init__.py
+-rw-r--r--   0        0        0     2171 2023-04-28 21:17:31.737873 git_add_co_author-0.3.0/git_add_co_author/__main__.py
+-rw-r--r--   0        0        0      360 2023-04-28 21:18:18.580120 git_add_co_author-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 git_add_co_author-0.3.0/setup.py
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 git_add_co_author-0.3.0/PKG-INFO
```

### Comparing `git_add_co_author-0.2.0/README.md` & `git_add_co_author-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Git Add Co-Author
 
+## Demo
+![git-add-co-author](https://user-images.githubusercontent.com/29942790/235253455-12d5d664-7ff8-43ad-b1fe-63db986120aa.gif)
+
+
 ## Overview
 
 Git Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits, ensuring proper credit is given to all contributors involved in the development process. This can be particularly useful for open-source projects, where multiple contributors are working together, or for pair programming sessions where two developers contribute to the same commit.
 
 ## Installation
 
 1. Install the package using pip:
```

### Comparing `git_add_co_author-0.2.0/git_add_co_author/__main__.py` & `git_add_co_author-0.3.0/git_add_co_author/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import requests
 import subprocess
 import click
-import shelve
 
 DB_PATH = "/tmp/add-co-author"
 
 
-def add_co_author(username, name="", email="", token=""):
-    if token:
-        subprocess.call(["git", "config", "--global", "github.token", token])
-    else:
-        token = (
-            subprocess.check_output(["git", "config", "--global", "github.token"])
-            .decode("utf-8")
-            .strip()
-        )
-    if not token:
-        raise ValueError(
-            "GitHub token not found. Please provide a token with --token or configure one with `git config --global github.token <token>`"
-        )
-
+def add_co_author(username="", name="", email="", token=""):
     if not name and not email:
+        if not token:
+            raise ValueError(
+                "GitHub token not found. Please provide a token with --token or configure one with `git config --global github.token <token>`"
+            )
+
+        if not username:
+            raise ValueError(
+                "GitHub username not found. Please provide a username as the first argument."
+            )
+
         headers = {"Authorization": f"Bearer {token}"}
         response = requests.get(
             f"https://api.github.com/users/{username}", headers=headers
         )
         if response.status_code != 200:
             raise ValueError(
                 f"Error fetching GitHub profile for {username}: {response.status_code} {response.reason}"
@@ -39,29 +35,32 @@
     author = f"{name} <{email}>" if name and email else f"{name or email}"
     subprocess.call(
         ["git", "commit", "--amend", "--trailer=" + f"Co-Authored-By: { author }"]
     )
 
 
 def save_token(token):
-    with shelve.open(DB_PATH) as db:
-        db["token"] = token
+    subprocess.call(["git", "config", "--global", "github.add-co-author-token", token])
 
 
 def get_token():
-    with shelve.open(DB_PATH) as db:
-        return db.get("token", "")
+    token = (
+        subprocess.check_output(["git", "config", "--global", "github.token"])
+        .decode("utf-8")
+        .strip()
+    )
+    return token
 
 
 @click.command()
-@click.argument("username")
+@click.option("--username", "-u", help="The GitHub username.")
 @click.option("--name", "-n", help="The name of the co-author.")
 @click.option("--email", "-e", help="The email address of the co-author.")
 @click.option("--token", "-t", help="Your GitHub personal access token.")
-def main(username, name="", email="", token=""):
+def main(username="", name="", email="", token=""):
     if token:
         save_token(token)
     else:
         token = get_token()
         add_co_author(username, name, email, token)
```

### Comparing `git_add_co_author-0.2.0/setup.py` & `git_add_co_author-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0', 'requests>=2.29.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'git-add-co-author',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
-    'long_description': '# Git Add Co-Author\n\n## Overview\n\nGit Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits, ensuring proper credit is given to all contributors involved in the development process. This can be particularly useful for open-source projects, where multiple contributors are working together, or for pair programming sessions where two developers contribute to the same commit.\n\n## Installation\n\n1. Install the package using pip:\n\n```bash\npip install git-add-co-author\n```\n\n2. Obtain a personal access token from GitHub. You can generate one by following the instructions in the [GitHub documentation](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).\n\n3. Configure the script with your GitHub token:\n\n```bash\npython -m git_add_co_author --token <your_token>\n```\n\n## Usage\n\nTo add a co-author to your commit, simply run the script with the co-author\'s GitHub username:\n\n```bash\npython -m git_add_co_author <co_author_username>\n```\n\nFor example:\n\n```bash\npython -m git_add_co_author sansyrox\n```\n\nIf you do not want to authorize a token, you can add the co-author\'s name and email address directly:\n\n```bash\npython -m git_add_co_author --name "John Doe" --email "john.doe@example.com"\n```\n\n### Optional Configuration\n\nI alias this command as `alias gac="python -m git_add_co_author"` in my `.zshrc` file, so I can simply run `gac <co_author_username>` to add a co-author to my commit.\n\n## Rationale\n\nThe motivation behind creating this script is to provide an easy way to give credit to contributors in various situations:\n\n- In open-source projects, when a pull request (PR) is closed without merging but the idea or code is later implemented.\n- During pair programming sessions, where two or more developers work together on a single commit.\n\nExisting solutions were either too complicated or didn\'t work as expected, so Git Add Co-Author was developed as a simple, easy-to-use alternative.\n\n## License\n\nThis project is licensed under the MIT License.\n',
+    'long_description': '# Git Add Co-Author\n\n## Demo\n![git-add-co-author](https://user-images.githubusercontent.com/29942790/235253455-12d5d664-7ff8-43ad-b1fe-63db986120aa.gif)\n\n\n## Overview\n\nGit Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits, ensuring proper credit is given to all contributors involved in the development process. This can be particularly useful for open-source projects, where multiple contributors are working together, or for pair programming sessions where two developers contribute to the same commit.\n\n## Installation\n\n1. Install the package using pip:\n\n```bash\npip install git-add-co-author\n```\n\n2. Obtain a personal access token from GitHub. You can generate one by following the instructions in the [GitHub documentation](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).\n\n3. Configure the script with your GitHub token:\n\n```bash\npython -m git_add_co_author --token <your_token>\n```\n\n## Usage\n\nTo add a co-author to your commit, simply run the script with the co-author\'s GitHub username:\n\n```bash\npython -m git_add_co_author <co_author_username>\n```\n\nFor example:\n\n```bash\npython -m git_add_co_author sansyrox\n```\n\nIf you do not want to authorize a token, you can add the co-author\'s name and email address directly:\n\n```bash\npython -m git_add_co_author --name "John Doe" --email "john.doe@example.com"\n```\n\n### Optional Configuration\n\nI alias this command as `alias gac="python -m git_add_co_author"` in my `.zshrc` file, so I can simply run `gac <co_author_username>` to add a co-author to my commit.\n\n## Rationale\n\nThe motivation behind creating this script is to provide an easy way to give credit to contributors in various situations:\n\n- In open-source projects, when a pull request (PR) is closed without merging but the idea or code is later implemented.\n- During pair programming sessions, where two or more developers work together on a single commit.\n\nExisting solutions were either too complicated or didn\'t work as expected, so Git Add Co-Author was developed as a simple, easy-to-use alternative.\n\n## License\n\nThis project is licensed under the MIT License.\n',
     'author': 'Sanskar Jethi',
     'author_email': 'sansyrox@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `git_add_co_author-0.2.0/PKG-INFO` & `git_add_co_author-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: git-add-co-author
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Git Add Co-Author
 
+## Demo
+![git-add-co-author](https://user-images.githubusercontent.com/29942790/235253455-12d5d664-7ff8-43ad-b1fe-63db986120aa.gif)
+
+
 ## Overview
 
 Git Add Co-Author is a simple Python script that allows you to easily add co-authors to your Git commits, ensuring proper credit is given to all contributors involved in the development process. This can be particularly useful for open-source projects, where multiple contributors are working together, or for pair programming sessions where two developers contribute to the same commit.
 
 ## Installation
 
 1. Install the package using pip:
```

