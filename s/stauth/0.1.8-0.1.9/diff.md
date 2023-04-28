# Comparing `tmp/stauth-0.1.8.tar.gz` & `tmp/stauth-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stauth-0.1.8.tar", max compression
+gzip compressed data, was "stauth-0.1.9.tar", max compression
```

## Comparing `stauth-0.1.8.tar` & `stauth-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10255 2022-12-16 07:22:10.290264 stauth-0.1.8/LICENSE
--rw-r--r--   0        0        0      217 2023-01-26 17:00:15.120074 stauth-0.1.8/README.md
--rw-r--r--   0        0        0     1037 2023-03-30 11:37:34.718596 stauth-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       40 2022-12-19 12:14:28.904401 stauth-0.1.8/stauth/__init__.py
--rw-r--r--   0        0        0     8457 2023-03-30 11:34:27.584956 stauth-0.1.8/stauth/authenticate.py
--rw-r--r--   0        0        0     1897 2023-01-19 13:11:42.186232 stauth-0.1.8/stauth/util.py
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 stauth-0.1.8/setup.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 stauth-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10255 2022-12-16 07:22:10.290264 stauth-0.1.9/LICENSE
+-rw-r--r--   0        0        0      217 2023-01-26 17:00:15.120074 stauth-0.1.9/README.md
+-rw-r--r--   0        0        0     1037 2023-04-28 13:24:47.881227 stauth-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       40 2022-12-19 12:14:28.904401 stauth-0.1.9/stauth/__init__.py
+-rw-r--r--   0        0        0     8662 2023-04-28 12:19:12.357258 stauth-0.1.9/stauth/authenticate.py
+-rw-r--r--   0        0        0     1897 2023-01-19 13:11:42.186232 stauth-0.1.9/stauth/util.py
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 stauth-0.1.9/setup.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 stauth-0.1.9/PKG-INFO
```

### Comparing `stauth-0.1.8/LICENSE` & `stauth-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stauth-0.1.8/pyproject.toml` & `stauth-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 description = "Basic Streamlit authenticator"
 exclude = ["graphics/*", ".git", ".gitignore", ".venv/", ".mypy_cache/", "__pycache__", ".eggs/"]
 license = "Apache License 2.0"
 name = "stauth"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 bcrypt = "^4.0.1"
 extra-streamlit-components = "^0.1.56"
 pyjwt = "^2.6.0"
 python = ">=3.8.1,<3.9.7 || >3.9.7,<4.0"
 streamlit = "^1.16.0"
```

### Comparing `stauth-0.1.8/stauth/authenticate.py` & `stauth-0.1.9/stauth/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,17 +189,21 @@
                     for checkbox_label in checkbox_labels:
                         checkboxes.append(login_form.checkbox(checkbox_label))
                 if markdown_texts is not None:
                     for markdown_text in markdown_texts:
                         login_form.markdown(markdown_text)
 
                 # Check entered username and password; if it exists - authorize
-                if login_form.form_submit_button("Login") and all(checkboxes):
-                    st.session_state["username"] = username
-                    self._check_pw_auth(username, password)
+                if login_form.form_submit_button("Login"):
+                    if all(checkboxes):
+                        st.session_state["username"] = username
+                        self._check_pw_auth(username, password)
+                    else:
+                        st.warning("Please accept the terms and conditions")
+                        st.session_state["authentication_status"] = False
 
         username = st.session_state["username"]
         expiration = (
             self._users_as_dict[username]["expiration"]
             if st.session_state["authentication_status"]
             else None
         )
```

### Comparing `stauth-0.1.8/stauth/util.py` & `stauth-0.1.9/stauth/util.py`

 * *Files identical despite different names*

### Comparing `stauth-0.1.8/setup.py` & `stauth-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'extra-streamlit-components>=0.1.56,<0.2.0',
  'mypy==1.1.1',
  'pyjwt>=2.6.0,<3.0.0',
  'streamlit>=1.16.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'stauth',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Basic Streamlit authenticator',
     'long_description': '# stauth\n\nStreamlit authentication components\n  \n## Installation\n\n```python\npip install stauth\n```\n\n## Example\n\nClone the repo and launch the example Streamlit page:\n```console\npoetry run streamlit run example.py\n```\n',
     'author': 'Mysterious Ben',
     'author_email': 'datascience@tuta.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stauth-0.1.8/PKG-INFO` & `stauth-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stauth
-Version: 0.1.8
+Version: 0.1.9
 Summary: Basic Streamlit authenticator
 License: Apache-2.0
 Author: Mysterious Ben
 Author-email: datascience@tuta.io
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

