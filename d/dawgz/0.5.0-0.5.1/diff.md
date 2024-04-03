# Comparing `tmp/dawgz-0.5.0.tar.gz` & `tmp/dawgz-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgz-0.5.0.tar", last modified: Fri Jan 26 14:21:31 2024, max compression
+gzip compressed data, was "dawgz-0.5.1.tar", last modified: Wed Apr  3 20:58:35 2024, max compression
```

## Comparing `dawgz-0.5.0.tar` & `dawgz-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2024-01-26 14:21:31.567806 dawgz-0.5.0/
--rw-r--r--   0 francois  (1000) francois  (1000)     1072 2024-01-08 18:47:00.000000 dawgz-0.5.0/LICENSE
--rw-r--r--   0 francois  (1000) francois  (1000)     8400 2024-01-26 14:21:31.567806 dawgz-0.5.0/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)     7433 2024-01-26 14:19:11.000000 dawgz-0.5.0/README.md
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2024-01-26 14:21:31.567806 dawgz-0.5.0/dawgz/
--rw-r--r--   0 francois  (1000) francois  (1000)      826 2024-01-26 14:19:11.000000 dawgz-0.5.0/dawgz/__init__.py
--rw-r--r--   0 francois  (1000) francois  (1000)     1364 2024-01-08 18:47:00.000000 dawgz-0.5.0/dawgz/__main__.py
--rw-r--r--   0 francois  (1000) francois  (1000)    13749 2024-01-26 14:19:11.000000 dawgz-0.5.0/dawgz/schedulers.py
--rw-r--r--   0 francois  (1000) francois  (1000)     2371 2024-01-26 14:19:11.000000 dawgz-0.5.0/dawgz/utils.py
--rw-r--r--   0 francois  (1000) francois  (1000)     6431 2024-01-26 14:19:11.000000 dawgz-0.5.0/dawgz/workflow.py
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2024-01-26 14:21:31.567806 dawgz-0.5.0/dawgz.egg-info/
--rw-r--r--   0 francois  (1000) francois  (1000)     8400 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)      291 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/SOURCES.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        1 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/dependency_links.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       46 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/entry_points.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       35 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/requires.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        6 2024-01-26 14:21:31.000000 dawgz-0.5.0/dawgz.egg-info/top_level.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       38 2024-01-26 14:21:31.567806 dawgz-0.5.0/setup.cfg
--rw-r--r--   0 francois  (1000) francois  (1000)     1373 2024-01-26 14:20:12.000000 dawgz-0.5.0/setup.py
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/
+-rw-r--r--   0 francois  (1000) francois  (1000)     1072 2024-01-08 18:47:00.000000 dawgz-0.5.1/LICENSE
+-rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 20:58:35.574680 dawgz-0.5.1/PKG-INFO
+-rw-r--r--   0 francois  (1000) francois  (1000)     7433 2024-01-26 14:19:11.000000 dawgz-0.5.1/README.md
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/dawgz/
+-rw-r--r--   0 francois  (1000) francois  (1000)      849 2024-04-03 20:57:05.000000 dawgz-0.5.1/dawgz/__init__.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     1882 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/__main__.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)    14399 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/schedulers.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     2363 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/utils.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     6367 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/workflow.py
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/dawgz.egg-info/
+-rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1000) francois  (1000)      314 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        1 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       46 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/entry_points.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       35 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        6 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/top_level.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)     1019 2024-04-03 20:57:00.000000 dawgz-0.5.1/pyproject.toml
+-rw-r--r--   0 francois  (1000) francois  (1000)       35 2024-01-08 18:47:00.000000 dawgz-0.5.1/requirements.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       38 2024-04-03 20:58:35.574680 dawgz-0.5.1/setup.cfg
```

### Comparing `dawgz-0.5.0/LICENSE` & `dawgz-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.0/PKG-INFO` & `dawgz-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: dawgz
-Version: 0.5.0
+Version: 0.5.1
 Summary: Directed Acyclic Workflow Graph Scheduling
-Home-page: https://github.com/francois-rozet/dawgz
-Author: François Rozet, Joeri Hermans
-Author-email: francois.rozet@outlook.com
-License: MIT license
-Project-URL: Documentation, https://github.com/francois-rozet/dawgz
-Project-URL: Source, https://github.com/francois-rozet/dawgz
-Project-URL: Tracker, https://github.com/francois-rozet/dawgz/issues
-Keywords: acyclic workflow graph scheduling reproducible-science slurm hpc hpc-tools
+Author: Joeri Hermans
+Author-email: François Rozet <francois.rozet@outlook.com>
+Project-URL: documentation, https://github.com/francois-rozet/dawgz
+Project-URL: source, https://github.com/francois-rozet/dawgz
+Project-URL: tracker, https://github.com/francois-rozet/dawgz/issues
+Keywords: workflow,scheduling,slurm,hpc
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `dawgz-0.5.0/README.md` & `dawgz-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.0/dawgz/schedulers.py` & `dawgz-0.5.1/dawgz/schedulers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 r"""Scheduling backends"""
 
+from __future__ import annotations
+
 import asyncio
 import concurrent.futures as cf
 import csv
 import os
 import re
 import shutil
 import subprocess
@@ -20,14 +22,15 @@
 from typing import *
 
 from .utils import comma_separated, eprint, future, pickle, runpickle, trace, slugify
 from .workflow import Job, cycles, prune as _prune
 
 
 DIR = os.environ.get('DAWGZ_DIR', '.dawgz')
+DIR = Path(DIR).resolve()
 
 
 class Scheduler(ABC):
     r"""Abstract workflow scheduler"""
 
     backend = None
 
@@ -39,40 +42,45 @@
     ):
         super().__init__()
 
         self.name = name
         self.date = datetime.now().replace(microsecond=0)
         self.uuid = uuid.uuid4().hex
 
-        self.path = Path(DIR).resolve() / self.uuid
+        self.path = DIR / self.uuid
         self.path.mkdir(parents=True)
 
         # Settings
         self.settings = settings.copy()
         self.settings.update(kwargs)
 
         # Jobs
         self.order = {}
         self.results = {}
         self.traces = {}
 
-    def dump(self) -> None:
+    def dump(self):
         with open(self.path / 'dump.pkl', 'wb') as f:
             pickle.dump(self, f)
 
         with open(self.path.parent / 'workflows.csv', 'a', newline='') as f:
             csv.writer(f).writerow((
                 self.name,
                 self.uuid,
                 self.date,
                 self.backend,
                 len(self.order),
                 len(self.traces),
             ))
 
+    @staticmethod
+    def load(path: Path) -> Scheduler:
+        with open(path / 'dump.pkl', 'rb') as f:
+            return pickle.load(f)
+
     def tag(self, job: Job) -> str:
         if job in self.order:
             i = self.order[job]
         else:
             i = self.order[job] = len(self.order)
 
         return f'{i:04d}_{slugify(job.name)}'
@@ -111,26 +119,29 @@
                 rows = [
                     (f'{job.name}[{i}]', self.state(job, i), self.output(job, i))
                     for i in array
                 ]
 
             return tabulate(rows, headers, showindex=array)
 
+    def cancel(self, job: Job = None) -> str:
+        raise NotImplementedError(f"'cancel' is not implemented for the {self.backend} backend.")
+
     @contextmanager
-    def context(self) -> None:
+    def context(self):
         try:
             yield None
         finally:
             pass
 
-    def wait(self, *jobs: Job) -> None:
+    def wait(self, *jobs: Job):
         with self.context():
             asyncio.run(self._wait(*jobs))
 
-    async def _wait(self, *jobs: Job) -> None:
+    async def _wait(self, *jobs: Job):
         if jobs:
             await asyncio.wait(map(asyncio.create_task, map(self.submit, jobs)))
             await asyncio.wait(map(asyncio.create_task, map(self.submit, self.order)))
 
     async def submit(self, job: Job) -> Any:
         if job in self.results:
             result = self.results[job]
@@ -153,15 +164,15 @@
                 raise DependencyNeverSatisfiedError(str(job))
         finally:
             self.tag(job)
 
         return await self.exec(job)
 
     @abstractmethod
-    async def satisfy(self, job: Job) -> None:
+    async def satisfy(self, job: Job):
         pass
 
     @abstractmethod
     async def exec(self, job: Job) -> Any:
         pass
 
 
@@ -204,26 +215,26 @@
 
     def __init__(self, pools: int = None, **kwargs):
         super().__init__(**kwargs)
 
         self.pools = pools
 
     @contextmanager
-    def context(self) -> None:
+    def context(self):
         if self.pools is None:
             self.executor = cf.ThreadPoolExecutor()
         else:
             self.executor = cf.ProcessPoolExecutor(self.pools)
 
         try:
             yield None
         finally:
             del self.executor
 
-    async def satisfy(self, job: Job) -> None:
+    async def satisfy(self, job: Job):
         pending = [
             asyncio.gather(self.submit(dep), future(status))
             for dep, status in job.dependencies.items()
         ]
 
         while pending:
             done, pending = await asyncio.wait(pending, return_when=asyncio.FIRST_COMPLETED)
@@ -271,15 +282,15 @@
 
 
 class DummyScheduler(AsyncScheduler):
     r"""Dummy scheduler"""
 
     backend = 'dummy'
 
-    async def exec(self, job: Job) -> None:
+    async def exec(self, job: Job):
         print(f"START {job}")
         await asyncio.sleep(random())
         print(f"END   {job}")
 
         return None if job.array is None else {}
 
 
@@ -377,14 +388,28 @@
 
                 rows.append((str(job), jobid, self.state(job)))
 
             return tabulate(rows, headers, showindex=True)
         else:
             return super().report(job)
 
+    def cancel(self, job: Job = None) -> str:
+        if job is None:
+            jobids = list(self.results.values())
+        else:
+            jobid = self.results[job]
+            jobids = [jobid]
+
+        return subprocess.run(
+            ['scancel', '-v', *jobids],
+            capture_output=True,
+            check=True,
+            text=True,
+        ).stderr.strip('\n')
+
     async def satisfy(self, job: Job) -> str:
         results = await asyncio.gather(*map(self.submit, job.dependencies))
 
         for result in results:
             if isinstance(result, Exception):
                 raise DependencyNeverSatisfiedError(str(job)) from result
```

### Comparing `dawgz-0.5.0/dawgz/utils.py` & `dawgz-0.5.1/dawgz/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         intervals.append((i, j))
 
     fmt = lambda i, j: f'{i}' if i == j else f'{i}-{j}'
 
     return ','.join(map(fmt, *zip(*intervals)))
 
 
-def eprint(*args, **kwargs) -> None:
+def eprint(*args, **kwargs):
     r"""Prints to the standard error stream."""
 
     print(*args, file=sys.stderr, **kwargs)
 
 
 def every(conditions: Iterable[Callable]) -> Callable:
     r"""Combines a list of conditions into a single condition."""
```

### Comparing `dawgz-0.5.0/dawgz/workflow.py` & `dawgz-0.5.1/dawgz/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
     def __init__(self):
         super().__init__()
 
         self.children = {}
         self.parents = {}
 
-    def add_child(self, node: Node, edge: Any = None) -> None:
+    def add_child(self, node: Node, edge: Any = None):
         self.children[node] = edge
         node.parents[self] = edge
 
-    def add_parent(self, node: Node, edge: Any = None) -> None:
+    def add_parent(self, node: Node, edge: Any = None):
         node.add_child(self, edge)
 
-    def rm_child(self, node: Node) -> None:
+    def rm_child(self, node: Node):
         del self.children[node]
         del node.parents[self]
 
-    def rm_parent(self, node: Node) -> None:
+    def rm_parent(self, node: Node):
         node.rm_child(self)
 
 
 class Job(Node):
     r"""Job node"""
 
     def __init__(
@@ -106,35 +106,35 @@
         else:
             return self.name + '[' + comma_separated(self.array) + ']'
 
     @property
     def dependencies(self) -> Dict[Job, str]:
         return self.parents
 
-    def after(self, *deps: Job, status: str = 'success') -> None:
+    def after(self, *deps: Job, status: str = 'success'):
         assert status in ['success', 'failure', 'any']
 
         for dep in deps:
             self.add_parent(dep, status)
 
-    def detach(self, *deps: Job) -> None:
+    def detach(self, *deps: Job):
         for dep in deps:
             self.rm_parent(dep)
 
     @property
     def waitfor(self) -> str:
         return self._waitfor
 
     @waitfor.setter
-    def waitfor(self, mode: str = 'all') -> None:
+    def waitfor(self, mode: str = 'all'):
         assert mode in ['all', 'any']
 
         self._waitfor = mode
 
-    def ensure(self, condition: Callable) -> None:
+    def ensure(self, condition: Callable):
         if self.array is None:
             assert accepts(condition), "postcondition should not expect arguments"
         else:
             assert accepts(condition, 0), "postcondition should expect an argument"
 
         self._postconditions.append(pickle.dumps(condition))
```

### Comparing `dawgz-0.5.0/dawgz.egg-info/PKG-INFO` & `dawgz-0.5.1/dawgz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: dawgz
-Version: 0.5.0
+Version: 0.5.1
 Summary: Directed Acyclic Workflow Graph Scheduling
-Home-page: https://github.com/francois-rozet/dawgz
-Author: François Rozet, Joeri Hermans
-Author-email: francois.rozet@outlook.com
-License: MIT license
-Project-URL: Documentation, https://github.com/francois-rozet/dawgz
-Project-URL: Source, https://github.com/francois-rozet/dawgz
-Project-URL: Tracker, https://github.com/francois-rozet/dawgz/issues
-Keywords: acyclic workflow graph scheduling reproducible-science slurm hpc hpc-tools
+Author: Joeri Hermans
+Author-email: François Rozet <francois.rozet@outlook.com>
+Project-URL: documentation, https://github.com/francois-rozet/dawgz
+Project-URL: source, https://github.com/francois-rozet/dawgz
+Project-URL: tracker, https://github.com/francois-rozet/dawgz/issues
+Keywords: workflow,scheduling,slurm,hpc
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

