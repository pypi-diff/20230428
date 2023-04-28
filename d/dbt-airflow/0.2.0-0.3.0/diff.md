# Comparing `tmp/dbt_airflow-0.2.0.tar.gz` & `tmp/dbt_airflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_airflow-0.2.0.tar", max compression
+gzip compressed data, was "dbt_airflow-0.3.0.tar", max compression
```

## Comparing `dbt_airflow-0.2.0.tar` & `dbt_airflow-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     5598 2023-02-24 18:33:47.711174 dbt_airflow-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-02-24 18:33:47.711174 dbt_airflow-0.2.0/dbt_airflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 18:33:47.711174 dbt_airflow-0.2.0/dbt_airflow/core/__init__.py
--rw-r--r--   0        0        0     1689 2023-02-24 18:33:47.711174 dbt_airflow-0.2.0/dbt_airflow/core/operators.py
--rw-r--r--   0        0        0     3448 2023-02-24 18:33:47.711174 dbt_airflow-0.2.0/dbt_airflow/core/task.py
--rw-r--r--   0        0        0     7728 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/core/task_builder.py
--rw-r--r--   0        0        0     2560 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/core/task_group.py
--rw-r--r--   0        0        0     1739 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/core/task_list.py
--rw-r--r--   0        0        0        0 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/domain/__init__.py
--rw-r--r--   0        0        0      702 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/parser/__init__.py
--rw-r--r--   0        0        0     1948 2023-02-24 18:33:47.715174 dbt_airflow-0.2.0/dbt_airflow/parser/dbt.py
--rw-r--r--   0        0        0     1113 2023-02-24 18:33:47.719174 dbt_airflow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6643 1970-01-01 00:00:00.000000 dbt_airflow-0.2.0/setup.py
--rw-r--r--   0        0        0     6426 1970-01-01 00:00:00.000000 dbt_airflow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8321 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/__init__.py
+-rw-r--r--   0        0        0     2827 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/operators.py
+-rw-r--r--   0        0        0     3839 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/task.py
+-rw-r--r--   0        0        0     7996 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/task_builder.py
+-rw-r--r--   0        0        0     2560 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/task_group.py
+-rw-r--r--   0        0        0     1739 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/core/task_list.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/domain/__init__.py
+-rw-r--r--   0        0        0      702 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/parser/__init__.py
+-rw-r--r--   0        0        0     1948 2023-04-28 13:43:47.668603 dbt_airflow-0.3.0/dbt_airflow/parser/dbt.py
+-rw-r--r--   0        0        0     1169 2023-04-28 13:43:47.672603 dbt_airflow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9149 1970-01-01 00:00:00.000000 dbt_airflow-0.3.0/PKG-INFO
```

### Comparing `dbt_airflow-0.2.0/dbt_airflow/core/task.py` & `dbt_airflow-0.3.0/dbt_airflow/core/task.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
     def __eq__(self, other):
         return self.task_id == other.task_id
 
 
 @dataclass(eq=False)
 class ExtraTask(AirflowTask):
+    """
+    This is a dataclass representing an extra task that is supposed to be inserted in a specific
+    place within the populated dbt project, based on the task names specified in
+    `upstream_task_ids` and/or `downstream_task_ids`.
+    """
     operator: BaseOperator
     operator_args: Dict[Any, Any] = field(default_factory=dict)
     upstream_task_ids: Set[str] = field(default_factory=set)
     downstream_task_ids: Set[str] = field(default_factory=set)
     task_group: Optional[str] = None
 
 
@@ -71,14 +76,18 @@
             resource_type=DbtResourceType.test,
             upstream_task_ids={parent_manifest_node_name},
             task_group=parent_node.task_group,
             package_name=parent_node.package_name,
         )
 
     def get_dbt_operator(self) -> Callable:
+        """
+        Returns a callable that corresponds to the dbt Airflow Operator based on the instance's
+        resource type.
+        """
         if self.resource_type == DbtResourceType.model:
             return DbtRunOperator
         if self.resource_type == DbtResourceType.test:
             return DbtTestOperator
         if self.resource_type == DbtResourceType.seed:
             return DbtSeedOperator
         return DbtSnapshotOperator
```

### Comparing `dbt_airflow-0.2.0/dbt_airflow/core/task_builder.py` & `dbt_airflow-0.3.0/dbt_airflow/core/task_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from dbt_airflow.core.task import DbtAirflowTask, ExtraTask
 from dbt_airflow.core.task_list import TaskList
 from dbt_airflow.parser.dbt import DbtResourceType, Manifest, Node
 
 
 class DbtAirflowTaskBuilder:
     """
-    TODO
+    This class implements functionality that is used to populate the dbt project as an Airflow DAG,
+    based on the user input. It also handles dbt model and test dependencies as well as any extra
+    tasks specified by user.
     """
 
     def __init__(
         self,
         manifest_path: str,
         extra_tasks: Optional[List[ExtraTask]] = None,
     ) -> None:
@@ -27,15 +29,15 @@
         if extra_tasks is None:
             self.extra_tasks = []
         else:
             self.extra_tasks = extra_tasks
 
     def _add_extra_tasks(self) -> None:
         """
-
+        Adds extra tasks specified in DbtTaskGroup
         """
         if not self.extra_tasks:
             logging.info('No extra tasks were provided. Skipping..')
             return
 
         for task in self.extra_tasks:
             self.task_list.append(task)
```

### Comparing `dbt_airflow-0.2.0/dbt_airflow/core/task_group.py` & `dbt_airflow-0.3.0/dbt_airflow/core/task_group.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.2.0/dbt_airflow/core/task_list.py` & `dbt_airflow-0.3.0/dbt_airflow/core/task_list.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.2.0/dbt_airflow/exceptions.py` & `dbt_airflow-0.3.0/dbt_airflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.2.0/dbt_airflow/parser/dbt.py` & `dbt_airflow-0.3.0/dbt_airflow/parser/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.2.0/pyproject.toml` & `dbt_airflow-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-airflow"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python package that creates fine-grained Airflow tasks for dbt"
 repository = "https://github.com/gmyrianthous/dbt-airflow"
 authors = ["Giorgos Myrianthous <giorgos.myrianthous@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dbt_airflow" }]
 
@@ -13,18 +13,20 @@
 dbt-core = ">=1.2.0"
 apache-airflow = ">=2.0.0,<3"
 pydantic = "^1.10.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1,<8"
 commitizen = "^2.40.0"
+mkdocs-material = "^8.2"
+mkdocstrings-python = "^0.8.2"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "0.3.0"
 version_files = [
     "pyproject.toml:^version"
 ]
 update_changelog_on_bump = true
 style = [
     ["qmark", "fg:#ff9d00 bold"],
     ["question", "bold"],
```

### Comparing `dbt_airflow-0.2.0/PKG-INFO` & `dbt_airflow-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-airflow
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python package that creates fine-grained Airflow tasks for dbt
 Home-page: https://github.com/gmyrianthous/dbt-airflow
 License: MIT
 Author: Giorgos Myrianthous
 Author-email: giorgos.myrianthous@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -16,41 +16,62 @@
 Requires-Dist: apache-airflow (>=2.0.0,<3)
 Requires-Dist: dbt-core (>=1.2.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/gmyrianthous/dbt-airflow
 Description-Content-Type: text/markdown
 
 # dbt-airflow
-A Python package that helps Data and Analytics engineers render dbt projects on Apache Airflow
-in a way that every single dbt resource (model, test, seed and snapshot) is represented by a single
-Airflow task. 
+A Python package that helps Data and Analytics engineers render dbt projects in Apache Airflow DAGs such that
+models, seeds, snapshots and tests are represented by individual Airflow Task.
+
+`dbt` is a command-line tool that enables data teams build, maintain and test data models in a scalable fashion. The 
+biggest challenge though is how to embed `dbt` in modern data workflows and infrastructure. dbt CLI is indeed a powerful
+tool, but if used as is, it will create silos in the way an organisation manages its data. Every contributor is able to 
+run `dbt` commands from their local machine (or even a host machine), but how do you know if a model run by another 
+contributor has failed, or succeeded? How can you enable shared visibility over data models, within the team? 
+
+One way to host dbt projects and orchestrate dbt tasks is via Apache Airflow. In its simplest form, an Airflow DAG
+that will build and test data models will consist of two tasks, one that executes `dbt run` command followed by an 
+Airflow task that executes `dbt test`. 
+
+<img style="display: block; margin: 0 auto" src="docs/blob/dbt_run_test_dag.png" alt="test">
+
+But what happens when model builds or tests fail? Should we re-run the whole dbt project (that could involve hundreds of 
+different models and/or tests) just to run a single model we've just fixed? This doesn't seem to be a good practice 
+since re-running the whole project  will be time-consuming and expensive. 
+
+A potential solution to this problem is to create individual Airflow tasks for every model, seed, snapshot and test
+within the dbt project. If we were about to do this work manually, we would have to put huge effort that would also be 
+prone to errors. Additionally, it would beat  the purpose of dbt, that among other features, it also automates model 
+dependency management.
+
+`dbt-airflow` is a package that builds a layer in-between Apache Airflow and dbt, and enables teams to automatically
+render their dbt projects in a granular level such that they have full control to individual dbt resource types. Every
+dbt model, seed, snapshot or test will have its own Airflow Task so that you can perform any action at a task-level. 
+
+Here's how the popular Jaffle Shop dbt project will be rendered on Apache Airflow via `dbt-airflow`:
+
+<img style="display: block; margin: 0 auto" src="docs/blob/dbt_jaffle_shop_dag.png" alt="test">
+
 
 ### Features
-- Render dbt project as a TaskGroup in Airflow Tasks
+- Render a `dbt` project as a `TaskGroup` consisting of Airflow Tasks that correspond to dbt models, seeds, snapshots
+and tests
 - Every `model`, `seed` and `snapshot` resource that has at least a single test, will also have a corresponding
-test task as a downstream.
-- Add extra tasks before or after the whole dbt project
-- Add extra tasks after specific dbt tasks
+test task as a downstream task
+- Add tasks before or after the whole dbt project
+- Introduce extra tasks within the dbt project tasks and specify any downstream or upstream dependencies
+- Create sub-`TaskGroup`s of dbt Airflow tasks based on your project's folder structure 
 
 ## How does it work
 The library essentially builds on top of the metadata generated by `dbt-core` and are stored in 
-the `target/manifest.json` file in your dbt project directory.  
-
-## Domain Requirements
-
-- Every dbt project, when compiled, will generate a metadata file under `<dbt-project-dir>/target/manifest.json`
-- The manifest file contains information about the interdependencies of the project's data models
-- `dbt-airflow` aims to extract these dependencies such that every dbt entity (snapshot, model, test and seed) has 
-  its own task in a Airflow DAG while entity dependencies are persisted
-- Snapshots are never an upstream dependency of any task
-- The creation of snpashots on seeds does not make sense, and thus not handled 
-  not even sure if this is even possible on dbt side)
-- Models may have tests
-- Snapshots may have tests
-- Seeds may have tests
+the `target/manifest.json` file in your dbt project directory. This means that you first need to compile (or run 
+any other dbt command that creates the `manifest` file) before creating your Airflow DAG. This means the `dbt-airflow` 
+package expects that you have already compiled your dbt project so that an up to date manifest file can then be used
+to render the individual tasks.
 
 ---
 
 # Installation
 
 The package is available on PyPI and can be installed through `pip`:
 ```bash
@@ -61,22 +82,17 @@
 different adapters, each dedicated to a different technology (such as Postgres or BigQuery). Therefore, before running
 `dbt-airflow` you also need to ensure that the required adapter(s) are installed in your environment. 
 
 For the full list of available adapters please refer to the official 
 [dbt documentation](https://docs.getdbt.com/docs/available-adapters). 
 
 ---
-
 # Usage
-`dbt-airflow` can be used either as a normal Python package, or through the 
-command line interface. 
 
-Given that there are possibly many different ways for deploying Airflow and automating different aspects
-of data workflows that involve Airflow, dbt and potentially other tools as well, we wanted to offer more
-flexibility by providing different approaches for using `dbt-airflow`.
+
 
 ### Building an Airflow DAG using `dbt-airflow`
 
 ```python3
 from datetime import datetime
 from pathlib import Path
 
@@ -149,41 +165,65 @@
     )
 
     t1 >> tg >> t2
 
 ```
 
 # Contributing
+This is an open-source project and everyone is welcome in contributing. Before 
+
 If you would like to contribute to `dbt-airflow` project, you will essentially need to follow the steps outlined below:
 1. Create a fork of the repository
 2. Set up the development environment on your local machine (see the detailed guide below)
 3. Write and test your contribution
 4. Create a Pull Request
 
+## Running the tests
+This project uses `poetry` tool for dependency management. You'll have to install `poetry` and install the dependencies
+specified in `pyproject.toml`. If you'd like to run the tests, make sure to do so within the poetry environment, as
+shown below. 
+
+```bash
+# Install poetry
+$ pip install poetry==1.3.0
+
+# Install dependencies in poetry venv
+$ poetry install 
+
+# Run tests
+$ poetry run tests -rP -vv
+
+# Run specific test(s)
+$ poetry run tests -k "test_name_or_prefix" -rP -vv
+```
+
+
 ##  Setting up your local development environment
 
 TO BE FINALISED
 ```bash
 docker-compose build
 
 docker-compose up
 
 # Access postgres db (changed to port 5433 given that we have an additional postgres instance for Airflow itsefl)
 docker ps  # get the container id of postgres-sakila
 docker exec -it <container-id> /bin/bash
 psql -U postgres -p 5433 
 ```
 
+## Releasing a new package version
+Every single merge into `main` branch will trigger a new patch, minor or major version upgrade based on the commit messages pushed
+from the Pull Request.
+The automated release mechanism is based on [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#summary).
+Every single commit must follow the structural elements described in Conventional Commits' specification. 
+The repository also contains pre-commit hooks that will ensure compliance to the specification. 
 ```bash
-# Install poetry
-pip install poetry
-
-# Install dependencies in poetry venv
-poetry install 
+# Install `pre-commit` package
+$ pip install pre-commit
 
-# Run tests
-poetry run tests -rP -vv
-
-# Run specific test(s)
-poetry run tests -k "test_name_or_prefix" -rP -vv
+# Install hooks from `.pre-commit-config.yaml`
+$ pre-commit install
+pre-commit installed at .git/hooks/pre-commit
 ```
 
+
```

