# Comparing `tmp/pyorchestra-0.4.1.tar.gz` & `tmp/pyorchestra-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.4.1.tar", max compression
+gzip compressed data, was "pyorchestra-0.4.2.tar", max compression
```

## Comparing `pyorchestra-0.4.1.tar` & `pyorchestra-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     7652 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/LICENSE
--rwxr-xr-x   0        0        0    25622 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/README.md
--rwxr-xr-x   0        0        0       62 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     1045 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      208 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1170 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/main.py
--rwxr-xr-x   0        0        0     7208 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      519 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/backend.py
--rwxr-xr-x   0        0        0    19098 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/formatting.py
--rwxr-xr-x   0        0        0     1455 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/models.py
--rwxr-xr-x   0        0        0    10731 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-03 12:34:58.681928 pyorchestra-0.4.2/LICENSE
+-rwxr-xr-x   0        0        0    25622 2024-04-03 12:34:58.681928 pyorchestra-0.4.2/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     1045 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      208 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1294 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/main.py
+-rwxr-xr-x   0        0        0     7682 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      519 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/backend.py
+-rwxr-xr-x   0        0        0    19404 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/core.py
+-rwxr-xr-x   0        0        0      873 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/formatting.py
+-rwxr-xr-x   0        0        0     1455 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/models.py
+-rwxr-xr-x   0        0        0    10731 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-03 12:34:58.685928 pyorchestra-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.4.2/PKG-INFO
```

### Comparing `pyorchestra-0.4.1/LICENSE` & `pyorchestra-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/README.md` & `pyorchestra-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/api/dto/job.py` & `pyorchestra-0.4.2/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/api/dto/run.py` & `pyorchestra-0.4.2/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/api/dto/task.py` & `pyorchestra-0.4.2/orchestra/api/dto/task.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from orchestra.models import TimingAwareTask, Status
 
 
 class TaskDTO(BaseModel):
     id: int
     task_id: str
+    run_id: int
+    job_name: str
     status: Status
     result: Any
     date_done: datetime.datetime
     traceback: str | None
     args: list
     kwargs: dict
     worker: str
@@ -22,14 +24,16 @@
     date_created: datetime.datetime
     date_started: datetime.datetime
 
     @classmethod
     def map(cls, task: TimingAwareTask) -> "TaskDTO":
         return TaskDTO(id=task.id,
                        task_id=task.task_id,
+                       run_id=task.run_id,
+                       job_name=task.job_name,
                        status=Status[task.status.lower()],
                        result=task.result,
                        date_done=task.date_done,
                        traceback=task.traceback,
                        args=json.loads(task.args.decode("utf-8")),
                        kwargs=json.loads(task.kwargs.decode("utf-8")),
                        worker=task.worker,
```

### Comparing `pyorchestra-0.4.1/orchestra/api/main.py` & `pyorchestra-0.4.2/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/api/routers/jobs.py` & `pyorchestra-0.4.2/orchestra/api/routers/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,23 @@
 @router.post("/jobs/resume", tags=["jobs"])
 async def resume_scheduled_jobs_matching_tags(tags: Annotated[str | None, Query(description="Comma separated tags to filter scheduled jobs")] = None,
                                               any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = True) -> list[JobDTO]:
     tags: set[str] = set(tags.split(",")) if tags else set()
     return list(map(lambda job: JobDTO.map(job), instance.resume_jobs_with_tags(tags, any_tag)))
 
 
+@router.get("/jobs/{job_name}", tags=["jobs"], status_code=status.HTTP_200_OK)
+async def get_job_by_name(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")], response: Response) -> JobDTO | str:
+    if instance.job_exists(job_name):
+        return JobDTO.map(instance.get_job_by_name(job_name, include_paused=True))
+    else:
+        response.status_code = status.HTTP_404_NOT_FOUND
+        return f"Job {job_name} does not exist"
+
+
 @router.get("/jobs/{job_name}/runs", tags=["jobs"], status_code=status.HTTP_200_OK)
 async def get_runs_of_job(job_name: Annotated[str, Path(description="The name of the job to for which to fetch runs")], response: Response, page_size: int = 50, page: int = 1) -> list[RunDTO] | str:
     if instance.job_exists(job_name):
         return list(map(lambda run: RunDTO.map(run), instance.get_runs_of_a_job(job_name, page_size, page)))
     else:
         response.status_code = status.HTTP_404_NOT_FOUND
         return f"Job {job_name} does not exist"
```

### Comparing `pyorchestra-0.4.1/orchestra/api/routers/tags.py` & `pyorchestra-0.4.2/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/api/routers/tasks.py` & `pyorchestra-0.4.2/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/backend.py` & `pyorchestra-0.4.2/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/core.py` & `pyorchestra-0.4.2/orchestra/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
             await asyncio.wait(pending_tasks)
 
         except (asyncio.CancelledError, KeyboardInterrupt):
             logger.warning("User-requested shutdown.")
 
     def get_job_by_name(self, job_name: str, include_paused: bool = False) -> Job | None:
-        for job in self.scheduler.jobs.union(self.paused_jobs if include_paused else []):
+        for job in self.apply_state_to_jobs(self.scheduler.jobs.union(self.paused_jobs if include_paused else [])):
             if job.alias == job_name:
                 return job
 
     def wrap_celery_task(self, job_name: str, task: celery.Task, additional_options: dict):
         async def celery_task():
             task_meta = task.apply_async(**additional_options)
             logger.debug(f"Triggered job {job_name}")
@@ -276,15 +276,15 @@
 
     def apply_state_to_jobs(self, jobs: set[Job]) -> set[Job]:
         return set([self.set_job_state_property(job, is_paused=True if job in self.paused_jobs else False) for job in jobs])
 
     def get_jobs(self, tags: set[str], any_tag: bool, include_paused: bool = True):
         # contrary to what get_jobs' docstring says, get_job will not return all jobs when tag is an empty set
         if len(tags) == 0:
-            active_jobs = self.scheduler.get_jobs()
+            active_jobs = self.scheduler.jobs
         else:
             active_jobs = set(filter(lambda job: job.tags.intersection(tags) if any_tag else job.tags == tags, self.scheduler.jobs))
 
         paused_jobs = set()
         if include_paused:
             paused_jobs = self.get_paused_jobs(tags, any_tag=any_tag)
 
@@ -383,15 +383,21 @@
         with session_cleanup(session):
             run: Run = next(session.scalars(select(Run).where(Run.job == job_name, Run.id == run_id).limit(1).options(joinedload(Run.task_object))), None)
             return run
 
     def get_task_by_id(self, task_id: str) -> TimingAwareTask | None:
         session = self.backend.ResultSession()
         with session_cleanup(session):
-            return next(session.scalars(select(TimingAwareTask).where(TimingAwareTask.task_id == task_id).limit(1)), None)
+            run_of_task = next(session.scalars(select(Run).where(Run.task_object.has(TimingAwareTask.task_id == task_id)).limit(1).options(joinedload(Run.task_object))), None)
+            if run_of_task is None:
+                return None
+            task: TimingAwareTask = run_of_task.task_object
+            task.run_id = run_of_task.id
+            task.job_name = run_of_task.job
+            return task
 
     def get_scheduler_status_table(self) -> Table:
         grid = Table.grid(expand=True)
         grid.add_column()
 
         table = Table(expand=True)
         table.border_style = "bright_yellow"
```

### Comparing `pyorchestra-0.4.1/orchestra/formatting.py` & `pyorchestra-0.4.2/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/models.py` & `pyorchestra-0.4.2/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/orchestra/scheduling.py` & `pyorchestra-0.4.2/orchestra/scheduling.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.1/pyproject.toml` & `pyorchestra-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.4.1"
+version = "0.4.2"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.4.1/PKG-INFO` & `pyorchestra-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.4.1
+Version: 0.4.2
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
```

