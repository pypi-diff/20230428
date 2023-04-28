# Comparing `tmp/besecure_developer_toolkit-0.0.2.tar.gz` & `tmp/besecure_developer_toolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besecure_developer_toolkit-0.0.2.tar", max compression
+gzip compressed data, was "besecure_developer_toolkit-0.0.3.tar", max compression
```

## Comparing `besecure_developer_toolkit-0.0.2.tar` & `besecure_developer_toolkit-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1873 2023-04-14 10:59:12.451665 besecure_developer_toolkit-0.0.2/README.md
--rw-r--r--   0        0        0      340 2023-04-10 11:19:33.073271 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/__init__.py
--rw-r--r--   0        0        0      203 2023-04-09 16:02:25.204287 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/__main__.py
--rw-r--r--   0        0        0     3080 2023-04-14 10:56:49.945336 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/cli.py
--rw-r--r--   0        0        0        0 2023-04-05 04:05:29.896606 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/config.py
--rw-r--r--   0        0        0     7232 2023-04-14 11:23:16.895125 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateOsspMaster.py
--rw-r--r--   0        0        0     3769 2023-04-14 11:24:48.998259 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateVersionData.py
--rw-r--r--   0        0        0     4318 2023-04-10 03:20:43.016876 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/GenerateReport.py
--rw-r--r--   0        0        0      612 2023-04-14 11:28:26.704427 besecure_developer_toolkit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1243 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/README.md
+-rw-r--r--   0        0        0      340 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/__main__.py
+-rw-r--r--   0        0        0     5674 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/cli.py
+-rw-r--r--   0        0        0        0 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/config.py
+-rw-r--r--   0        0        0     8561 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/src/create_ossp_master.py
+-rw-r--r--   0        0        0     5204 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/src/create_version_data.py
+-rw-r--r--   0        0        0     5254 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/src/generate_report.py
+-rw-r--r--   0        0        0      612 2023-04-28 06:28:51.018960 besecure_developer_toolkit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.3/PKG-INFO
```

### Comparing `besecure_developer_toolkit-0.0.2/README.md` & `besecure_developer_toolkit-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,58 @@
+Metadata-Version: 2.1
+Name: besecure-developer-toolkit
+Version: 0.0.3
+Summary: cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
+Author: asa1997
+Author-email: arunsureshampadath@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
+
 # Be-Secure Developer Toolkit (bes-dev-kit)
 
 bes-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 
-# Installation
+# Pre-requisites
 
-`$ python3 -m pip install besecure-developer-toolkit`
+1. Python 3.10
+2. pip
+3. Github personal access token
 
-# Pre-requisites
+# Installation
 
-1. [Poetry](https://python-poetry.org/)
-2. Python 3.x
-3. pip
-4. Github personal access token
-
-# Setting env variables
-
-`Note: Should be done before testing/running`
-
-1. Creating a json file in your user home dir under the name `bes-dev-kit.json`.
-2. Copy the below contents and paste it inside the file.
-   
-        {
-        "GITHUB_ORG": "Be-Secure",
-        "OSSPOI_DIR": "<complete_path_to>/besecure-osspoi-datastore",
-        "ASSESSMENT_DIR": "<complete_path_to>/besecure-assessment-datastore",
-        "GITHUB_AUTH_TOKEN": "<token>"
-        }
-3. Update `OSSPOI_DIR` and `ASSESSMENT_DIR` with complete path to your `besecure-assessment-datastore` and `besecure-osspoi-datastore`  dirs.
-4. Add your github personal access token
+`$ python3 -m pip install besecure-developer-toolkit`
 
 
 # Setting up locally
 
 1. Install [poetry](https://python-poetry.org/). Use the [link](https://python-poetry.org/docs/) to install Poetry.
 2. Clone the repo.
 3. Move into the cloned directory.
-4. Create a new virtual env using Poetry - `$ poetry shell`
-5. Run the command to install the tool- `$ poetry install`
-6. Check installation - `$ bes-dev-kit --help`
+4. Run the command - `$ poetry add "typer[all]"`
+5. Create a new virtual env using Poetry - `$ poetry shell`
+6. Run the command to install the tool- `$ poetry install`
+7. Check installation - `$ bes-dev-kit --help`
 
 # Usage
 
 ### Generate Metadata
 
 Command helps to generate metadata such as OSSP-master file data and version details file.
 
 `$ bes-dev-kit generate metadata`
-
 For more options use `--help` at end.
 
 ### Generate Reports
 
 `$ bes-dev-kit generate report <report name>`
 
 `<report name> - scorecard, codeql, criticality_score`
 
 For more options use `--help` at end.
 
-`Note: All three reports can be generated at once by passing all report names - $ bes-dev-kit generate report scorecard criticality_score codeql`
+`Note: All three reports can be generated at once by passing all report names - $ bes-dev-kit generate report scorecard criticality_score codeql`
+
```

### Comparing `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateOsspMaster.py` & `besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/src/create_ossp_master.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,217 @@
-import sys, os, json, subprocess
-from urllib.request import urlopen
+"""
+    licence part todo
+"""
+import sys
+import os
+import json
+import urllib.request
+import requests
 from rich import print
 
+
 class OSSPMaster():
-    
-    def __init__(self, id: int, name: str) -> None:
-        self.id = id
+    """
+        Generate OSSPMaster report.
+    """
+
+    def __init__(self, issue_id: int, name: str) -> None:
+        self.issue_id = issue_id
         self.name = name
-    
-    def check_issue_exists(self,id) -> None:
+
+    @staticmethod
+    def check_issue_exists(issue_id: int):
+        """Function to check if the issue exists
+
+        Args:
+            issue_id (int): Issue issue_id
+
+        Returns:
+            bool: True if issue exists and False if otherwise
+        """
+        url = f"https://api.github.com/repos/Be-Secure/Be-Secure/issues/{issue_id}"
         try:
-            urlopen('https://github.com/Be-Secure/Be-Secure/issues/'+str(id))
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            print(exc_type, fname, exc_tb.tb_lineno)
-            print("Could not find issue with id : "+str(id))
-            sys.exit()
-    
-    def check_issue_related_to_project(self):
-            
-        json_data = json.loads(urlopen(f'https://api.github.com/repos/Be-Secure/Be-Secure/issues/{self.id}').read())
-        issue_title = json_data["title"]
-        project_name = str(str(issue_title).split(":")[1]).replace(" ","")
-        if project_name != self.name:
-            print(f"[bold red]Alert! [yellow]Mismatch issue_id-project : [green] Issue id {self.id} does not match the project {self.name}")
-            sys.exit()
-        else:
-            pass
+            response = requests.head(url, timeout=10)
+            return response.status_code < 400
+        except requests.exceptions.RequestException:
+            return False
 
-        
-    
-    def check_repo_exists(self,name) -> None:
+    def check_issue_related_to_project(self):
+        """
+            Check project name from issue
+        """
+        url = f'https://api.github.com/repos/Be-Secure/Be-Secure/issues/{self.issue_id}'
+        with urllib.request.urlopen(url) as raw_data:
+            json_data = json.loads(raw_data.read())
+            issue_title = json_data["title"]
+            project_name = str(str(issue_title).split(":")[1]).replace(" ", "")
+            if project_name != self.name:
+                print("[bold red]Alert![yellow] Mismatch issue_id-project:" +
+                        f"[green] Issue id {self.issue_id} " +
+                        f"does not match the project {self.name}")
+                sys.exit()
+
+    @staticmethod
+    def check_repo_exists(name: str):
+        """Checks if the repo exists
+
+        Args:
+            name (str): Project name
+        """
+        url = f"https://api.github.com/repos/Be-Secure/{name}"
         try:
-            urlopen('https://api.github.com/repos/Be-Secure/'+name)
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            print(exc_type, fname, exc_tb.tb_lineno)
-            print("Could not find "+ name +" under Be-Secure")
-            sys.exit()
-    
-    def write_tech_stack(self,bes_id):
-        raw_data = urlopen("https://api.github.com/repos/Be-Secure/Be-Secure/issues/"+str(bes_id))
-
-        data = json.loads(raw_data.read())
-
-        body_data = iter(data["body"].splitlines())
-        found = "false"
-        for i in body_data:
-            if i == "### Tech Stack":
-                found = "true"
-                continue
-            if len(i.strip()) == 0:
-                continue
-            if len(i.strip()) != 0 and found == "true":
-                s = str(i.split(" [")[1])
-                s = str(s.split("]")[0])
-                break    
-        return s
-    def write_project_repos_data(self,project_data):
+            response = requests.head(url, timeout=10)
+            return response.status_code < 400
+        except requests.exceptions.RequestException:
+            return False
+
+    def write_tech_stack(self, bes_id):
+        """
+            Check the tech Stack of the Project
+        """
+        url = f"https://api.github.com/repos/Be-Secure/Be-Secure/issues/{str(bes_id)}"
+        with urllib.request.urlopen(url) as raw_data:
+            data = json.loads(raw_data.read())
+            body_data = iter(data["body"].splitlines())
+            found = "false"
+            for i in body_data:
+                if i == "### Tech Stack":
+                    found = "true"
+                    continue
+                if len(i.strip()) == 0:
+                    continue
+                if len(i.strip()) != 0 and found == "true":
+                    stack = str(i.split(" [")[1])
+                    stack = str(stack.split("]", maxsplit=1)[0])
+                    break
+        return stack
+
+    def write_project_repos_data(self, project_data):
+        """
+            Create json report for repository related content
+            like: main_github_url, main_bes_url etc...
+        """
         project_repos = {
-        "main_github_url": "",
-        "main_bes_url": "",
-        "all_projects": [                                                                        
-            {
-                "id": 0,
-                "name": "",
-                "url": ""
-            }
-        ],
-        "all_bes_repos": [                                                                  
-            {
-                "id": 0,
-                "name": "",
-                "url": ""
-            }
-                    
-        ]
+            "main_github_url": "",
+            "main_bes_url": "",
+            "all_projects": [
+                {
+                    "id": 0,
+                    "name": "",
+                    "url": ""
+                }
+            ],
+            "all_bes_repos": [
+                {
+                    "id": 0,
+                    "name": "",
+                    "url": ""
+                }
+
+            ]
         }
-        project_repos.update({"main_github_url": project_data["parent"]["html_url"]}) 
+        project_repos.update(
+            {"main_github_url": project_data["parent"]["html_url"]})
         project_repos.update({"main_bes_url": project_data["html_url"]})
-        project_repos["all_projects"][0]["id"] = project_data["parent"]["id"]     
+        project_repos["all_projects"][0]["id"] = project_data["parent"]["id"]
         project_repos["all_projects"][0]["name"] = project_data["parent"]["full_name"]
         project_repos["all_projects"][0]["url"] = project_data["parent"]["html_url"]
         project_repos["all_bes_repos"][0]["id"] = project_data["id"]
         project_repos["all_bes_repos"][0]["name"] = project_data["full_name"]
-        project_repos["all_bes_repos"][0]["url"] = project_data["html_url"]         
+        project_repos["all_bes_repos"][0]["url"] = project_data["html_url"]
         return project_repos
 
     def write_tags(self, bes_id):
-        url = 'https://api.github.com/repos/Be-Secure/Be-Secure/issues/'+str(bes_id)+'/labels'
-        tags_json_data = urlopen(url)
-        tags_dict = json.loads(tags_json_data.read())
-        tags = []
-        for i in range(len(tags_dict)):
-            tags.append(tags_dict[i]["name"])
-        return tags
-    
-    def write_languages(self,name):
-        raw_data = urlopen("https://api.github.com/repos/Be-Secure/"+name+"/languages")
-        data = json.loads(raw_data.read())
+        """
+            get the tags from github labels
+        """
+        url = 'https://api.github.com/repos/Be-Secure/Be-Secure/issues/' + \
+            str(bes_id)+'/labels'
+        with urllib.request.urlopen(url) as tags_json_data:
+            tags_dict = json.loads(tags_json_data.read())
+            tags = []
+            # pylint: disable=unused-variable
+            for i, tag_name in enumerate(tags_dict):
+                tags.append(tag_name["name"])
+            return tags
+
+    def write_languages(self, name):
+        """
+            fetch the languages from github URL
+        """
+        url = f"https://api.github.com/repos/Be-Secure/{name}/languages"
+        with urllib.request.urlopen(url) as raw_data:
+            data = json.loads(raw_data.read())
         return data
-    
-    def write_to_ossp_master(self, f, ossp_master_json, data, overwrite: bool):
-            if overwrite:
-                for i in range(len(ossp_master_json["items"])):
-                    if ossp_master_json["items"][i]["id"] == self.id:
-                        ossp_master_json["items"][i] = data
-                        break
-            else:    
-                ossp_master_json["items"].append(data)
-            f.seek(0)
-            f.write(json.dumps(ossp_master_json, indent=4))
-            f.truncate()
-        
-    
-    
-    def GenerateOsspMaster(self, overwrite: bool):
-        self.check_issue_exists(self.id)
-        self.check_repo_exists(self.name)
+
+    def write_to_ossp_master(self, file_pointer, ossp_master_json, data, overwrite: bool):
+        """
+            Add or override the project details in ossp_master
+        """
+        if overwrite:
+            for i in range(len(ossp_master_json["items"])):
+                if ossp_master_json["items"][i]["id"] == self.issue_id:
+                    ossp_master_json["items"][i] = data
+                    break
+        else:
+            ossp_master_json["items"].append(data)
+        file_pointer.seek(0)
+        file_pointer.write(json.dumps(ossp_master_json, indent=4))
+        file_pointer.truncate()
+
+    def generate_ossp_master(self, overwrite: bool):
+        """
+            Generate ossp master json report
+        """
+        if self.check_issue_exists(self.issue_id) is False:
+            print("[bold red]Alert! [green]Issue " +
+                  f"[yellow]{self.issue_id} [green]does not exist")
+            sys.exit()
+        if self.check_repo_exists(self.name) is False:
+            print("[bold red]Alert! [green]Repo [yellow]" +
+                  f"{self.name} [green]does not exist")
+            sys.exit()
         self.check_issue_related_to_project()
         osspoi_dir = os.environ['OSSPOI_DIR']
-        namespace = os.environ['GITHUB_ORG']
-        token = os.environ['GITHUB_AUTH_TOKEN']
         write_flag = True
-        f = open(osspoi_dir+"/OSSP-Master.json", "r+")
-        ossp_master_json = json.load(f)
-        if not overwrite:                 
-            for i in range(len(ossp_master_json["items"])):
-                if ossp_master_json["items"][i]["id"] == self.id:
-                    print("[bold red]Alert! [green]Entry for "+str(self.id)+"-"+self.name+" already present under OSSP-Master.json")
-                    write_flag = False
-                    break
-                else:
-                    write_flag = True
-        if write_flag:
-            # proc = subprocess.Popen([f'curl -L -H "Accept: application/vnd.github+json" -H "Authorization: Bearer <YOUR-TOKEN>"-H "X-GitHub-Api-Version: 2022-11-28" https://api.github.com//{namespace}/{self.name}'], stdout=subprocess.PIPE, shell=True)
-            # (out, err) = proc.communicate()
-            url_data = urlopen('https://api.github.com/repos/Be-Secure/'+self.name)
-            project_data = json.loads(url_data.read())
-            ossp_data = json.loads('{}')
-            repo_keys = [ "id", "bes_tracking_id", "issue_url", "name", "full_name", "description", "bes_technology_stack", "watchers_count", "forks_count", "stargazers_count", "size", "open_issues", "created_at", "updated_at", "pushed_at", "git_url", "clone_url", "html_url", "homepage", "owner", "project_repos", "license", "language", "tags" ]
-            for i in repo_keys:
-                if i == "id" or i == "bes_tracking_id":
-                    ossp_data[i] = self.id
-                elif i == "issue_url":
-                    ossp_data[i] = 'https://github.com/Be-Secure/Be-Secure/issues/'+str(self.id)
-                elif i == "bes_technology_stack":
-                    ossp_data[i] = self.write_tech_stack(self.id)
-                elif i == "project_repos":
-                    ossp_data[i] = self.write_project_repos_data(project_data)
-                elif i == "tags":
-                    ossp_data[i] = self.write_tags(self.id)
-                elif i == "language":
-                    ossp_data[i] = self.write_languages(self.name)
-                else:
-                    ossp_data[i] = project_data[i]
-            self.write_to_ossp_master(f, ossp_master_json, ossp_data, overwrite)
-            f.close()        
-        
-        
-    
-    
-
+        with open(f"{osspoi_dir}/OSSP-Master.json", "r+", encoding="utf-8") as file_pointer:
+            ossp_master_json = json.load(file_pointer)
+            if not overwrite:
+                for i in range(len(ossp_master_json["items"])):
+                    if ossp_master_json["items"][i]["id"] == self.issue_id:
+                        print("[bold red]Alert! [green]Entry for "+str(self.issue_id) +
+                            "-"+self.name+" already present under OSSP-Master.json")
+                        write_flag = False
+                        break
+            if write_flag:
+                url = f"https://api.github.com/repos/Be-Secure/{self.name}"
+                with urllib.request.urlopen(url) as url_data:
+                    project_data = json.loads(url_data.read())
+                ossp_data = json.loads('{}')
+                repo_keys = [
+                    "id", "bes_tracking_id", "issue_url", "name",
+                    "full_name", "description", "bes_technology_stack",
+                    "watchers_count", "forks_count", "stargazers_count",
+                    "size", "open_issues", "created_at", "updated_at",
+                    "pushed_at", "git_url", "clone_url", "html_url",
+                    "homepage", "owner", "project_repos", "license",
+                    "language", "tags"
+                ]
+                for i in repo_keys:
+                    if i in ('id', 'bes_tracking_id'):
+                        ossp_data[i] = self.issue_id
+                    elif i == "issue_url":
+                        ossp_data[i] = 'https://github.com/Be-Secure/Be-Secure/issues/' + \
+                            str(self.issue_id)
+                    elif i == "bes_technology_stack":
+                        ossp_data[i] = self.write_tech_stack(self.issue_id)
+                    elif i == "project_repos":
+                        ossp_data[i] = self.write_project_repos_data(project_data)
+                    elif i == "tags":
+                        ossp_data[i] = self.write_tags(self.issue_id)
+                    elif i == "language":
+                        ossp_data[i] = self.write_languages(self.name)
+                    else:
+                        ossp_data[i] = project_data[i]
+                self.write_to_ossp_master(
+                    file_pointer, ossp_master_json, ossp_data, overwrite)
+            file_pointer.close()
```

### Comparing `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/GenerateReport.py` & `besecure_developer_toolkit-0.0.3/besecure_developer_toolkit/src/generate_report.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,134 @@
-import json, sys, os
+"""
+    licence part todo
+"""
+import json
+import sys
+import os
 from urllib.request import urlopen
 from rich import print
 
 
 class Report():
-    def __init__(self, id:int, name: str, version: str, report: str):
-        self.id = id
+    """
+        Create report for scorcard, codeQl, and criticality_score
+    """
+    def __init__(self, issue_id: int, name: str, version: str, report: str):
+        self.issue_id = issue_id
         self.name = name
         self.report = report
         self.version = version
-        
-    def fetch_report(self, url):
 
+    def fetch_report(self, url):
+        """
+            create json report for criticality_score, codeql, and scorecard
+        """
         if self.report == "criticality_score":
-            os.system('criticality_score --repo '+url+' --format json >> /tmp/'+self.report+'.json')
-            f_critical = open('/tmp/'+self.report+'.json', 'r')
+            os.system('criticality_score --repo '+url +
+                      ' --format json >> /tmp/'+self.report+'.json')
+            f_critical = open('/tmp/'+self.report+'.json', 'r', encoding="utf-8")
             data = json.load(f_critical)
             f_critical.close()
-       
         elif self.report == "codeql":
             token = os.environ['GITHUB_AUTH_TOKEN']
-            cmd = 'curl -s -L -H "Accept: application/vnd.github+json" -H "Authorization: Bearer '+token+'" -H "X-GitHub-Api-Version: 2022-11-28" '+url
+            cmd = 'curl -s -L -H "Accept: application/vnd.github+json" \
+                -H "Authorization: Bearer ' + \
+                token+'" -H "X-GitHub-Api-Version: 2022-11-28" '+url
             os.system(cmd+' >> /tmp/'+self.report+'.json')
-            codeql_f = open('/tmp/'+self.report+'.json', 'r')
+            codeql_f = open('/tmp/'+self.report+'.json', 'r', encoding="utf-8")
             data = json.load(codeql_f)
-            codeql_f.close()            
-       
-        else:          
+            codeql_f.close()
+        else:
             try:
                 raw_data = urlopen(url)
-            except Exception as e:
+            except Exception as err:
                 exc_type, exc_obj, exc_tb = sys.exc_info()
                 fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
                 print(exc_type, fname, exc_tb.tb_lineno)
-                sys.exit(str(e))
+                sys.exit(str(err))
             data = json.loads(raw_data.read())
-        
+
         return data
 
     def write_report(self, data):
-        
+        """
+            create report for criticality_score, codeql, and scorecard
+            in assesment data store
+        """
         assessment_dir = os.environ['ASSESSMENT_DIR']
-        
-        path = assessment_dir+'/'+self.name+'/'+self.version+'/'+self.report
-        
+        if self.report == "codeql":
+            path = assessment_dir+'/'+self.name+'/'+self.version+'/sast'
+        else:
+            path = assessment_dir+'/'+self.name+'/'+self.version+'/'+self.report
         try:
             os.makedirs(path, exist_ok=True)
-        except:
-            pass
-        f = open(path + '/' + self.name + '-' + self.version + '-' + self.report + '-report.json', "w")
-        
+        except FileExistsError as err:
+            print(f"error to create file Error: {err}")
+        f = open(path + '/' + self.name + '-' + self.version +
+                 '-' + self.report + '-report.json', "w", encoding="utf-8")
         f.write(json.dumps(data, indent=4))
-    
+
     def update_version_data(self):
-        
+        """
+            provide versiondetails for version and read from assessment data store
+        """
         osspoi_dir = os.environ['OSSPOI_DIR']
         assessment_dir = os.environ['ASSESSMENT_DIR']
-        report_file = open(assessment_dir+'/'+self.name+'/'+self.version+'/'+self.report+'/'+self.name + '-' + self.version + '-' + self.report + '-report.json', "r")
-        version_file = open(osspoi_dir+"/version_details/"+str(self.id) + "-" + self.name + "-" "Versiondetails.json", "r+")
-        
+        report_file = open(assessment_dir+'/'+self.name+'/'+self.version+'/'+self.report +
+                            '/'+self.name + '-' + self.version +
+                            '-' + self.report + '-report.json', "r", encoding="utf-8")
+        version_file = open(osspoi_dir+"/version_details/"+str(self.issue_id) +
+                            "-" + self.name + "-" "Versiondetails.json", "r+", encoding="utf-8")
+
         score_data = json.load(report_file)
         if self.report == "scorecard":
             score = score_data["score"]
         elif self.report == "criticality_score":
             score = score_data["criticality_score"]
-        
+
         version_data = json.load(version_file)
         for i in range(len(version_data)):
+            # Fixme
             if version_data[i]["version"] == self.version:
                 version_data[i][self.report] = score
-            else:
-                pass
         version_file.seek(0)
         version_file.write(json.dumps(version_data, indent=4))
         version_file.truncate()
         report_file.close()
         version_file.close()
-                
-            
-            
+
     def cleanup(self):
-        if self.report == "scorecard":
-            pass
-        else:
+        """
+            remove file from tmp
+        """
+        if self.report != "scorecard":
             os.remove('/tmp/'+self.report+'.json')
 
     def main(self):
-    
+        """
+            generate report for scorecard, criticality_score amd codeql
+        """
         if self.report == "scorecard":
             url = "https://api.securityscorecards.dev/projects/github.com/Be-Secure/"+self.name
-    
+
         elif self.report == "criticality_score":
             if "GITHUB_AUTH_TOKEN" not in os.environ:
-                print("[bold red] Alert! [green] Please use the below command to set your personal access token and try again.")
+                print(
+                    "[bold red] Alert! [green] Please use the below \
+                          command to set your personal access token and try again.")
                 print("[yellow]export GITHUB_AUTH_TOKEN=token")
                 sys.exit()
             url = 'github.com/Be-Secure/'+self.name
-                               
+
         elif self.report == "codeql":
             if "GITHUB_AUTH_TOKEN" not in os.environ:
-                print("[bold red] Alert! [green] Please use the below command to set your personal access token and try again.")
+                print(
+                    "[bold red] Alert! [green] Please use the \
+                        below command to set your personal access token and try again.")
                 print("[yellow]export GITHUB_AUTH_TOKEN=token")
                 sys.exit()
-            url = 'https://api.github.com/repos/Be-Secure/'+ self.name +'/code-scanning/alerts?tool_name=CodeQL'
-        
+            url = 'https://api.github.com/repos/Be-Secure/' + \
+                self.name + '/code-scanning/alerts?tool_name=CodeQL'
+
         data = self.fetch_report(url)
         self.write_report(data)
         self.cleanup()
-
```

### Comparing `besecure_developer_toolkit-0.0.2/pyproject.toml` & `besecure_developer_toolkit-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "besecure-developer-toolkit"
-version = "0.0.2"
+version = "0.0.3"
 description = "cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse)."
 authors = ["asa1997 <arunsureshampadath@gmail.com>"]
 readme = "README.md"
 packages = [{include = "besecure_developer_toolkit"}]
 
 [tool.poetry.scripts]
 bes-dev-kit = "besecure_developer_toolkit.__main__:cli.app"
```

