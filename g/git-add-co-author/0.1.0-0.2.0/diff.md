# Comparing `tmp/git_add_co_author-0.1.0.tar.gz` & `tmp/git_add_co_author-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_add_co_author-0.1.0.tar", max compression
+gzip compressed data, was "git_add_co_author-0.2.0.tar", max compression
```

## Comparing `git_add_co_author-0.1.0.tar` & `git_add_co_author-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      416 2023-04-27 22:19:29.709451 git_add_co_author-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.1.0/git_add_co_author/__init__.py
--rw-r--r--   0        0        0     1551 2023-04-27 22:16:32.112420 git_add_co_author-0.1.0/git_add_co_author/__main__.py
--rw-r--r--   0        0        0      360 2023-04-27 21:39:05.401888 git_add_co_author-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 git_add_co_author-0.1.0/setup.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 git_add_co_author-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2061 2023-04-28 20:19:08.859277 git_add_co_author-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 21:31:09.655115 git_add_co_author-0.2.0/git_add_co_author/__init__.py
+-rw-r--r--   0        0        0     2118 2023-04-28 20:09:55.084340 git_add_co_author-0.2.0/git_add_co_author/__main__.py
+-rw-r--r--   0        0        0      360 2023-04-28 20:20:15.241787 git_add_co_author-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 git_add_co_author-0.2.0/setup.py
+-rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 git_add_co_author-0.2.0/PKG-INFO
```

### Comparing `git_add_co_author-0.1.0/git_add_co_author/__main__.py` & `git_add_co_author-0.2.0/git_add_co_author/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,69 @@
 import requests
 import subprocess
 import click
+import shelve
 
+DB_PATH = "/tmp/add-co-author"
 
-@click.command()
-@click.argument('username')
-@click.option('--name', '-n', help='The name of the co-author.')
-@click.option('--email', '-e', help='The email address of the co-author.')
-@click.option('--token', '-t', help='Your GitHub personal access token.')
-def add_co_author(username, name='', email='', token=''):
+
+def add_co_author(username, name="", email="", token=""):
     if token:
-        subprocess.call(['git', 'config', '--global', 'github.token', token])
+        subprocess.call(["git", "config", "--global", "github.token", token])
     else:
-        token = subprocess.check_output(['git', 'config', '--global', 'github.token']).decode('utf-8').strip()
+        token = (
+            subprocess.check_output(["git", "config", "--global", "github.token"])
+            .decode("utf-8")
+            .strip()
+        )
     if not token:
-        raise ValueError('GitHub token not found. Please provide a token with --token or configure one with `git config --global github.token <token>`')
+        raise ValueError(
+            "GitHub token not found. Please provide a token with --token or configure one with `git config --global github.token <token>`"
+        )
 
     if not name and not email:
         headers = {"Authorization": f"Bearer {token}"}
-        response = requests.get(f'https://api.github.com/users/{username}', headers=headers)
+        response = requests.get(
+            f"https://api.github.com/users/{username}", headers=headers
+        )
         if response.status_code != 200:
-            raise ValueError(f'Error fetching GitHub profile for {username}: {response.status_code} {response.reason}')
+            raise ValueError(
+                f"Error fetching GitHub profile for {username}: {response.status_code} {response.reason}"
+            )
         data = response.json()
-        name = data.get('name', '')
-        email = data.get('email', '')
+        name = data.get("name", "")
+        email = data.get("email", "")
         if not name and not email:
-            raise ValueError(f'GitHub profile for {username} does not have a name or email address')
-    author = f'{name} <{email}>' if name and email else f'{name or email}'
-    subprocess.call(['git', 'commit', '--amend', '--trailer=' + f"Co-Authored-By: { author }"])
+            raise ValueError(
+                f"GitHub profile for {username} does not have a name or email address"
+            )
+    author = f"{name} <{email}>" if name and email else f"{name or email}"
+    subprocess.call(
+        ["git", "commit", "--amend", "--trailer=" + f"Co-Authored-By: { author }"]
+    )
+
+
+def save_token(token):
+    with shelve.open(DB_PATH) as db:
+        db["token"] = token
+
+
+def get_token():
+    with shelve.open(DB_PATH) as db:
+        return db.get("token", "")
+
+
+@click.command()
+@click.argument("username")
+@click.option("--name", "-n", help="The name of the co-author.")
+@click.option("--email", "-e", help="The email address of the co-author.")
+@click.option("--token", "-t", help="Your GitHub personal access token.")
+def main(username, name="", email="", token=""):
+    if token:
+        save_token(token)
+    else:
+        token = get_token()
+        add_co_author(username, name, email, token)
 
-if __name__ == '__main__':
-    add_co_author()
 
+if __name__ == "__main__":
+    main()
```

