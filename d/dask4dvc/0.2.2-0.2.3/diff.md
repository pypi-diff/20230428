# Comparing `tmp/dask4dvc-0.2.2.tar.gz` & `tmp/dask4dvc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.2.2.tar", max compression
+gzip compressed data, was "dask4dvc-0.2.3.tar", max compression
```

## Comparing `dask4dvc-0.2.2.tar` & `dask4dvc-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.2/LICENSE
--rw-r--r--   0        0        0     2252 2023-04-22 14:35:15.965210 dask4dvc-0.2.2/README.md
--rw-r--r--   0        0        0      656 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.2/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     4437 2023-04-22 14:47:14.907460 dask4dvc-0.2.2/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     3547 2023-04-22 14:47:14.907460 dask4dvc-0.2.2/dask4dvc/dvc_queue.py
--rw-r--r--   0        0        0     5655 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/dvc_repro.py
--rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.2/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      272 2023-04-22 10:39:57.388361 dask4dvc-0.2.2/dask4dvc/utils/config.py
--rw-r--r--   0        0        0     1184 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.2/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1274 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 dask4dvc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2099 2023-04-28 12:30:08.363546 dask4dvc-0.2.3/README.md
+-rw-r--r--   0        0        0      571 2023-04-28 10:58:50.814191 dask4dvc-0.2.3/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.3/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     4796 2023-04-28 12:30:08.363546 dask4dvc-0.2.3/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     6158 2023-04-28 12:30:08.363546 dask4dvc-0.2.3/dask4dvc/dvc_repro.py
+-rw-r--r--   0        0        0       24 2023-04-28 10:58:50.814191 dask4dvc-0.2.3/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0     1184 2023-04-27 22:12:22.405218 dask4dvc-0.2.3/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0     1274 2023-04-28 12:30:08.373546 dask4dvc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dask4dvc-0.2.3/PKG-INFO
```

### Comparing `dask4dvc-0.2.2/LICENSE` & `dask4dvc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.2/README.md` & `dask4dvc-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,53 @@
+Metadata-Version: 2.1
+Name: dask4dvc
+Version: 0.2.3
+Summary: Use dask to run the DVC graph
+License: Apache-2.0
+Keywords: data-science,HPC,dask,DVC
+Author: zincwarecode
+Author-email: zincwarecode@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bokeh (>=2.4.2,<3)
+Requires-Dist: dask (>=2022.7.1,<2023.0.0)
+Requires-Dist: dask-jobqueue (>=0.8.1,<0.9.0)
+Requires-Dist: distributed (>=2022.7.1,<2023.0.0)
+Requires-Dist: dvc (>=2.54.0,<3.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: repository, https://github.com/zincware/dask4dvc
+Description-Content-Type: text/markdown
+
 [![Coverage Status](https://coveralls.io/repos/github/zincware/dask4dvc/badge.svg?branch=main)](https://coveralls.io/github/zincware/dask4dvc?branch=main)
 ![PyTest](https://github.com/zincware/dask4dvc/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
-The `dask4dvc` package will try to run the DVC graph in parallel.
+The `dask4dvc repro` package will run the DVC graph in parallel where possible.
+Currently, `dask4dvc run` will not run stages per experiment sequentially.
 
-> :warning: This is an experimental package **not** affiliated in any way with iterative or DVC. ``dask4dvc`` will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc`.
+> :warning: This is an experimental package **not** affiliated in any way with iterative or DVC.
 
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
-- `dvc queue start --jobs 1` becomes `dask4dvc run`
+- `dvc queue start` becomes `dask4dvc run`
 
 You can follow the progress using `dask4dvc <cmd> --dashboard`.
 
-> `dask4dvc run --parallel` is available for `dvc queue start --jobs <max-workers>` but it currently leads to the failure of some experiments.
-
-> The `dask4dvc` error messages are currently really sparse. For better error messages please use the DVC commands.
 
 ### SLURM Cluster
 
 You can use `dask4dvc` easily with a slurm cluster.
 This requires a running dask scheduler:
 ```python
 from dask_jobqueue import SLURMCluster
@@ -41,15 +63,18 @@
 )
 cluster.adapt()
 ```
 
 with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
 
 You can also use config files with `dask4dvc repro --config myconfig.yaml`.
+All `dask.distributed` Clusters should be supported.
 
 ```yaml
 default:
   SGECluster:
     queue: regular
     cores: 10
     memory: 16 GB
 ```
+
+![dask4dvc repro](https://raw.githubusercontent.com/zincware/dask4dvc/main/misc/dask4dvc_1.gif "dask4dvc repro")
```

### Comparing `dask4dvc-0.2.2/dask4dvc/cli/main.py` & `dask4dvc-0.2.3/dask4dvc/cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,135 @@
 """All methods that come directly from 'dask4dvc' CLI interace."""
 
 import importlib.metadata
 import logging
+import subprocess
 import typing
 import webbrowser
 
 import dask.distributed
+import dvc.cli
 import dvc.repo
 import typer
 
-from dask4dvc import dvc_queue, dvc_repro, utils
+from dask4dvc import dvc_repro
+from dask4dvc.utils.dask import get_cluster_from_config, wait_for_futures
 
 app = typer.Typer()
 
 log = logging.getLogger(__name__)
 
 
 class Help:
     """Collect typer help strings that are used multiple times."""
 
     address: str = (
         "This can be the address of a DASK Scheduler server like '127.0.0.1:31415'. If"
         " 'None' Dask will launch a new Server."
     )
-    parallel: str = (
-        "Split the DVC Graph into individual Nodes and run them in parallel if possible."
-    )
     leave: str = "Ask before stopping the client"
     config: str = "path to config file, e.g. 'dask4dvc.yaml'"
-    retries: str = "Number of retries to acquire dvc lock."
     max_workers: str = (
         "Maximum number of workers to use. Using '1' will be the same as 'dvc repro' but"
         " slower."
     )
     dashboard: str = "Open Dask Dashboard in Browser"
 
 
 @app.command()
+def clean() -> None:
+    """Remove all dask4dvc experiments from the queue."""
+    dvc_repro.remove_experiments()
+
+
+@app.command()
 def repro(
-    targets: typing.List[str] = typer.Argument(None),
+    targets: typing.List[str] = typer.Argument(
+        None, help="Name of stages to reproduce. Leave emtpy to run the full graph."
+    ),
     address: str = typer.Option(None, help=Help.address),
     leave: bool = typer.Option(True, help=Help.leave),
     config: str = typer.Option(None, help=Help.config),
     max_workers: int = typer.Option(None, help=Help.max_workers),
-    retries: int = typer.Option(10, help=Help.retries),
-    force: bool = typer.Option(False, "--force/", "-f/", help="use `dvc repro --force`"),
     dashboard: bool = typer.Option(False, help=Help.dashboard),
+    option: typing.List[str] = typer.Option(
+        None, "-o", "--option", help="Additional dvc repro options"
+    ),
+    cleanup: bool = typer.Option(True, help="Remove temporary experiments when done"),
 ) -> None:
     """Replicate 'dvc repro' command using dask."""
-    utils.CONFIG.retries = retries
+    if len(option) != 0:
+        typer.echo("Additional dvc repro options are not implemented yet")
+        raise typer.Exit(1)
+
+    repo = dvc.repo.Repo()
+    stages = dvc_repro.queue_consecutive_stages(repo, targets, option)
 
     if config is not None:
         assert address is None, "Can not use address and config file"
-        address = utils.dask.get_cluster_from_config(config)
+        address = get_cluster_from_config(config)
 
     with dask.distributed.Client(address) as client:
         if dashboard:
             webbrowser.open(client.dashboard_link)
         if max_workers is not None:
             client.cluster.adapt(minimum=1, maximum=max_workers)
         log.info(client)
-        results = dvc_repro.parallel_submit(client, targets=targets, force=force)
 
-        utils.dask.wait_for_futures(client, results)
+        mapping, experiments = dvc_repro.parallel_submit(client, repo, stages)
+
+        wait_for_futures(client, mapping)
+        if all(x.status == "finished" for x in mapping.values()):
+            log.info("All stages finished successfully")
+            # dvc.cli.main(["exp", "apply", experiments[-1]])
+            dask.distributed.wait(
+                client.submit(subprocess.check_call, ["dvc", "repro", *targets])
+            )
+        if cleanup:
+            dvc_repro.remove_experiments(experiments)
+
         if not leave:
-            utils.main.wait()
+            _ = input("Press Enter to close the client")
 
 
 @app.command()
 def run(
-    targets: typing.List[str] = typer.Argument(None),
+    targets: typing.List[str] = typer.Argument(
+        None, help="Name of the DVC experiments to reproduce. Leave emtpy to run all."
+    ),
     address: str = typer.Option(None, help=Help.address),
-    config: str = typer.Option(None, help=Help.config),
-    dashboard: bool = typer.Option(False, help=Help.dashboard),
     leave: bool = typer.Option(True, help=Help.leave),
+    config: str = typer.Option(None, help=Help.config),
     max_workers: int = typer.Option(None, help=Help.max_workers),
-    parallel: bool = typer.Option(
-        False, help="Run experiments in parallel. Some experiments might fail!"
-    ),
+    dashboard: bool = typer.Option(False, help=Help.dashboard),
 ) -> None:
-    """Run DVC experiments in parallel using dask."""
-    # TODO do not wait for results and then submit next, but do all in parallel
+    """Replicate 'dvc queue start' using dask."""
     if len(targets) == 0:
-        with dvc.repo.Repo() as repo:
-            targets = [x.name for x in repo.experiments.celery_queue.iter_queued()]
+        targets = None
 
-    if len(targets) == 0:
-        typer.echo("No experiments to run.")
-        raise typer.Exit()
+    repo = dvc.repo.Repo()
 
     if config is not None:
         assert address is None, "Can not use address and config file"
-        address = utils.dask.get_cluster_from_config(config)
+        address = get_cluster_from_config(config)
 
-    typer.echo(f"Running {targets}.")
     with dask.distributed.Client(address) as client:
         if dashboard:
             webbrowser.open(client.dashboard_link)
         if max_workers is not None:
             client.cluster.adapt(minimum=1, maximum=max_workers)
-        results = {}
+        log.info(client)
+
+        mapping, _ = dvc_repro.experiment_submit(client, repo, targets)
+
+        wait_for_futures(client, mapping)
+        # dvc_repro.remove_experiments(experiments)
 
-        for target in targets:
-            results[target] = dvc_queue.run_single_experiment(target)
-            if not parallel:
-                utils.dask.wait_for_futures(client, results[target])
-        if parallel:
-            utils.dask.wait_for_futures(client, results)
         if not leave:
-            utils.main.wait()
+            _ = input("Press Enter to close the client")
 
 
 def version_callback(value: bool) -> None:
     """Get the installed dask4dvc version."""
     if value:
         typer.echo(f"dask4dvc {importlib.metadata.version('dask4dvc')}")
         raise typer.Exit()
```

### Comparing `dask4dvc-0.2.2/dask4dvc/dvc_repro.py` & `dask4dvc-0.2.3/dask4dvc/dvc_repro.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,190 +1,191 @@
-"""Some general 'dask4dvc' methods."""
-
-
-import contextlib
+"""Dask4DVC to DVC repo interface."""
+import dataclasses
+import functools
 import logging
-import os
-import random
 import subprocess
-import time
 import typing
+import uuid
 
 import dask.distributed
-import dvc.exceptions
-import dvc.lock
+import dvc.cli
 import dvc.repo
-import dvc.stage
-import dvc.utils.strictyaml
+from dvc.repo.experiments.executor.local import TempDirExecutor
+from dvc.repo.experiments.queue import tasks
+from dvc.repo.experiments.queue.base import BaseStashQueue, QueueEntry
 from dvc.repo.reproduce import _get_steps
-from dvc.stage.cache import RunCacheNotFoundError
-
-from dask4dvc import utils
+from dvc.stage import PipelineStage
 
 log = logging.getLogger(__name__)
 
 
-def _run_locked_cmd(
-    repo: dvc.repo.Repo, func: typing.Callable, *args: tuple, **kwargs: dict
-) -> typing.Any:
-    """Retry running a DVC command until the lock is released.
+def queue_consecutive_stages(
+    repo: dvc.repo.Repo,
+    targets: typing.List[str],
+    options: list = None,
+) -> typing.Dict[PipelineStage, str]:
+    """Create an experiment for each stage in the DAG.
 
     Parameters
     ----------
-    repo: dvc.repo.Repo
-        The DVC repository.
-    func: callable
-        The DVC command to run. e.g. 'repo.reproduce'
-    *args: list
-        The positional arguments for the command.
-    **kwargs: dict
-        The keyword arguments for the command.
+    repo : dvc.repo.Repo
+        The DVC repo to gather the stages from
+    targets : typing.List[str], optional
+        The stages to queue, by default it will use all stages in the DAG
+    options : list, optional
+        Additional options to pass to `dvc exp run`, by default None
 
 
     Returns
     -------
-    typing.Any: the return value of the command.
+    typing.Dict[PipelineStage, str]
+        A dictionary mapping each stage to its experiment name
     """
-    err = ValueError("Something went wrong")
-    for _ in range(utils.CONFIG.retries):
+    if len(targets) == 0:
+        stages = repo.index.graph.nodes
+    else:
+        stages = [repo.stage.get_target(x) for x in targets]
+
+    ordered_stages = _get_steps(
+        repo.index.graph, stages, downstream=False, single_item=False
+    )
+
+    experiment_names = {}
+
+    cmd = ["exp", "run", "--queue"]
+    if options is not None:
+        cmd.extend(options)
+    for stage in ordered_stages:
         try:
-            while repo.lock.is_locked:
-                time.sleep(random.random() * 5)  # between 0 and 5 seconds
-            return func(*args, **kwargs)
-        except (dvc.lock.LockError, dvc.utils.strictyaml.YAMLValidationError) as err:
-            log.debug(err)
-    raise err
+            name = f"{stage.name}-dask4dvc-{str(uuid.uuid4())[:8]}"
+            experiment_names[stage] = name
+            dvc.cli.main(cmd + ["--name", name, stage.name])
+        except AttributeError:
+            # has no attribute name
+            log.warning(f"Skipping stage {stage} because it is not a pipeline stage")
 
+    return experiment_names
 
-def _load_run_cache(repo: dvc.repo.Repo, stage: dvc.stage.Stage) -> None:
-    """Load the run cache for the given stage.
-
-    Raises
-    ------
-    RunCacheNotFoundError:
-        if the stage is not cached.
-    """
-    with dvc.repo.lock_repo(repo):
-        with repo.scm_context():
-            repo.stage_cache.restore(stage=stage)
-            log.info(
-                f"Stage '{stage.name}' is cached - skipping run, checking out outputs "
-            )
 
+def get_all_queue_entries(
+    repo: dvc.repo.Repo,
+) -> typing.Dict[str, typing.Tuple[QueueEntry, str]]:
+    """Get QueueEntry and infofile from the queue.
 
-def submit_stage(
-    name: str, force: bool, successors: list, root_dir: str
-) -> typing.List[str]:
-    """Submit a stage to the Dask cluster."""
-    os.chdir(root_dir)
-    repo = dvc.repo.Repo(root_dir)
+    We do all at once, because doing it in parallel seems not to work probably.
+    """
+    queue = repo.experiments.celery_queue
+    return {
+        entry.name: (entry, queue.get_infofile_path(entry.stash_rev))
+        for entry in queue.iter_queued()
+    }
 
-    if force:
-        stages = [repo.stage.get_target(name)]
-    else:
-        # dvc reproduce returns the stages that are not checked out
-        stages = _run_locked_cmd(repo, repo.reproduce, name, dry=True, single_item=True)
 
-    if len(stages) == 0 and not force:
-        # if the stage is already checked out, we don't need to run it
-        log.info(f"Stage '{name}' didn't change, skipping")
+def exec_run(infofile: str, successors: list = None) -> None:
+    """Execute a queued experiment via its infofile."""
+    # ! Do not use dvc.cli.main
+    subprocess.check_call(["dvc", "exp", "exec-run", "--infofile", infofile])
 
-    else:
-        if len(stages) > 1:
-            # we use single-item, so it should never be more than 1
-            raise ValueError("Something went wrong")
-
-        for stage in stages:
-            if not force:
-                with contextlib.suppress(RunCacheNotFoundError):
-                    # check if the stage is already in the run cache
-                    _run_locked_cmd(repo, _load_run_cache, repo, stages[0])
-                    return name
-            # if not, run the stage
-            log.info(f"Running stage '{name}': \n > {stage.cmd}")
-            subprocess.check_call(stage.cmd, shell=True)
-            # add the stage to the run cache
-            _run_locked_cmd(repo, repo.commit, name, force=True)
 
-    return [x.name for x in stages]
+def remove_experiments(experiments: typing.List[str] = None) -> None:
+    """Remove queued experiments."""
+    print(f"Removing experiments: {experiments}")
+    repo = dvc.repo.Repo()
+    queue = repo.experiments.celery_queue
+    found_experiments = []
+    for msg in queue.celery.iter_queued():
+        if msg.headers.get("task") != tasks.run_exp.name:
+            continue
+        args, kwargs, _embed = msg.decode()
+        entry_dict = kwargs.get("entry_dict", args[0])
+        if (experiments is None and "-dask4dvc-" in entry_dict["name"]) or (
+            experiments is not None and entry_dict["name"] in experiments
+        ):
+            found_experiments.append(entry_dict["name"])
+            queue.celery.reject(msg.delivery_tag)
+    dvc.cli.main(["exp", "remove"] + found_experiments)
+
+
+def collect_and_cleanup(
+    future: dask.distributed.Future, entry_dict: dict, infofile: str
+) -> None:
+    """Collect the results of a finished experiment and clean up."""
+    try:
+        tasks.collect_exp(proc_dict=None, entry_dict=entry_dict)
+    finally:
+        entry = QueueEntry.from_dict(entry_dict)
+        with dvc.repo.Repo(entry.dvc_root) as repo:
+            executor = BaseStashQueue.init_executor(
+                repo.experiments,
+                entry,
+                TempDirExecutor,
+                location="dvc-task",
+            )
+            executor.cleanup(infofile)
 
 
-def reproduce(
-    repo: dvc.repo.Repo,
-    targets=None,
-    recursive=False,
-    pipeline=False,
-    all_pipelines=False,
-    after_repro_callback=None,  # TODO
-    client: dask.distributed.Client = None,
-    prefix: str = None,
-    **kwargs,
-) -> typing.List[dvc.stage.PipelineStage]:
-    """Parallel Exectuion drop-in replacement for 'dvc.repo.Repo.reproduce'.
+def submit_to_dask(
+    client: dask.distributed.Client, infofile: str, entry: QueueEntry, successors: list
+) -> dask.distributed.Future:
+    """Submit a queued experiment to run with Dask."""
+    future = client.submit(
+        exec_run,
+        infofile=infofile,
+        successors=successors,
+        pure=False,
+        key=entry.name,
+    )
 
-    Use with functools.partial to set the client and prefix
-    """
-    if targets is None:
-        targets = []
-    mapping = parallel_submit(
-        client,
-        targets,
-        force=kwargs.get("force", False),
-        root_dir=repo.root_dir,
-        prefix=prefix,
+    future.add_done_callback(
+        functools.partial(
+            collect_and_cleanup,
+            entry_dict=dataclasses.asdict(entry),
+            infofile=infofile,
+        )
     )
-    results: typing.Dict[str, list] = utils.dask.wait_for_futures(client, mapping)
-    result = []
-    for stages in results.values():
-        if isinstance(stages, str):  # TODO this should always be a list?
-            stages = [stages]
-        result.extend([repo.stage.get_target(x) for x in stages])
-    return result
+    return future
 
 
 def parallel_submit(
     client: dask.distributed.Client,
-    targets: list[str],
-    force: bool,
-    root_dir: str = None,
-    prefix: str = None,
-) -> typing.Dict[str, dask.distributed.Future]:
-    """Submit all stages to the Dask cluster."""
+    repo: dvc.repo.Repo,
+    stages: typing.Dict[PipelineStage, str],
+) -> typing.Tuple[typing.Dict[PipelineStage, dask.distributed.Future], typing.List[str],]:
+    """Submit experiments in parallel."""
     mapping = {}
-    repo = dvc.repo.Repo(root_dir)
-
-    if len(targets) == 0:
-        targets = repo.index.graph.nodes
-    else:
-        targets = [repo.stage.get_target(x) for x in targets]
+    queue_entries = get_all_queue_entries(repo)
+    experiments = []
 
-    nodes = _get_steps(repo.index.graph, targets, downstream=False, single_item=False)
+    for stage in stages:
+        log.debug(f"Preparing experiment '{stages[stage]}'")
+        entry, infofile = queue_entries[stages[stage]]
+        tasks.setup_exp(dataclasses.asdict(entry))
 
-    for node in nodes:
-        if node.cmd is None:
-            # if the stage doesn't have a command, e.g. a dvc tracked file
-            # we don't need to run it
-            mapping[node] = None
-            continue
+        # we use get here, because some stages won't be queued, such as dependency files
         successors = [
-            mapping[successor] for successor in repo.index.graph.successors(node)
+            mapping.get(successor) for successor in repo.index.graph.successors(stage)
         ]
+        mapping[stage] = submit_to_dask(client, infofile, entry, successors)
 
-        if len(successors) == 0 and prefix is not None:
-            successors = [dask.distributed.Variable(prefix).get()]
-        # https://docs.dask.org/en/stable/futures.html#distributed.Variable to connect to main graph
-
-        mapping[node] = client.submit(
-            submit_stage,
-            node.name,
-            force=force,
-            root_dir=repo.root_dir,
-            successors=successors,
-            pure=False,
-            key=f"{prefix}_{node.name}" if prefix else node.name,
-        )
+        experiments.append(entry.name)
 
-    mapping = {
-        node.name: future for node, future in mapping.items() if future is not None
-    }
+    return mapping, experiments
+
+
+def experiment_submit(
+    client: dask.distributed.Client, repo: dvc.repo.Repo, experiments: typing.List[str]
+) -> typing.Tuple[typing.Dict[str, dask.distributed.Future], typing.List[str]]:
+    """Submit experiments in parallel."""
+    queue_entries = get_all_queue_entries(repo)
+    if experiments is None:
+        experiments = list(queue_entries.keys())
+    mapping = {}
+    print(f"Submitting experiments: {experiments}")
+
+    for experiment in experiments:
+        log.critical(f"Preparing experiment '{experiment}'")
+        entry, infofile = queue_entries[experiment]
+        tasks.setup_exp(dataclasses.asdict(entry))
+
+        mapping[experiment] = submit_to_dask(client, infofile, entry, None)
 
-    return mapping
+    return mapping, list(mapping.keys())
```

### Comparing `dask4dvc-0.2.2/dask4dvc/utils/dask.py` & `dask4dvc-0.2.3/dask4dvc/utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.2/pyproject.toml` & `dask4dvc-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.2.2"
+version = "0.2.3"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

