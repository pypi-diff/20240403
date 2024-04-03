# Comparing `tmp/dopelemon-0.0.4.tar.gz` & `tmp/dopelemon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopelemon-0.0.4.tar", max compression
+gzip compressed data, was "dopelemon-0.0.5.tar", max compression
```

## Comparing `dopelemon-0.0.4.tar` & `dopelemon-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      534 2024-03-23 12:45:54.113893 dopelemon-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/__init__.py
--rw-r--r--   0        0        0     1406 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/cli.py
--rw-r--r--   0        0        0     1838 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/client.py
--rw-r--r--   0        0        0      110 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/exceptions.py
--rw-r--r--   0        0        0     1391 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/manager/controller.py
--rw-r--r--   0        0        0      743 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/manager/registry.py
--rw-r--r--   0        0        0     3003 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/manager/work_manager.py
--rw-r--r--   0        0        0     2981 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/service.py
--rw-r--r--   0        0        0      955 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/utils.py
--rw-r--r--   0        0        0     1142 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/worker/ex_thread.py
--rw-r--r--   0        0        0     1432 2024-03-23 12:45:54.113893 dopelemon-0.0.4/service_sdk/worker/worker.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 dopelemon-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      546 2024-04-03 19:14:05.283518 dopelemon-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/__init__.py
+-rw-r--r--   0        0        0     2633 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/cli.py
+-rw-r--r--   0        0        0     2256 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/client.py
+-rw-r--r--   0        0        0      222 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/exceptions.py
+-rw-r--r--   0        0        0     1391 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/manager/controller.py
+-rw-r--r--   0        0        0     1493 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/manager/registry.py
+-rw-r--r--   0        0        0     3368 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/manager/work_manager.py
+-rw-r--r--   0        0        0     3758 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/service.py
+-rw-r--r--   0        0        0      955 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/utils.py
+-rw-r--r--   0        0        0     1142 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/worker/ex_thread.py
+-rw-r--r--   0        0        0     1790 2024-04-03 19:14:05.283518 dopelemon-0.0.5/service_sdk/worker/worker.py
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 dopelemon-0.0.5/PKG-INFO
```

### Comparing `dopelemon-0.0.4/pyproject.toml` & `dopelemon-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dopelemon"
-version = "0.0.4"
-description = "tools for microservices"
+version = "0.0.5"
+description = "Service framework with built-in API"
 authors = ["limonyellow"]
 packages = [{include = "service_sdk"}]
 
 [tool.poetry.scripts]
 dope = 'service_sdk.cli:cli'
 
 [tool.poetry.dependencies]
```

### Comparing `dopelemon-0.0.4/service_sdk/client.py` & `dopelemon-0.0.5/service_sdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,25 +35,34 @@
             return "server is still up"
         except requests.exceptions.ConnectionError:
             return "server was stopped successfully"
 
     def stop_all(self, force: Optional[bool] = None, wait: Optional[bool] = None):
         params = {}
         if force is not None:
-            params.update(dict(force=force))
+            params["force"] = force
         if wait is not None:
-            params.update(dict(wait=force))
+            params["wait"] = wait
 
         self.post(path="stop_all", params=params)
 
     def kill_service(self) -> str:
+        """
+        WARNING: Killing the service does not kill the running workers processes.
+        """
         try:
             self.post(path="kill_service")
             return "server is still up"
         except requests.exceptions.ConnectionError:
             return "server was stopped successfully"
 
-    def start_worker(self):
-        return self.post(path="start_worker")
+    def start_worker(self, name: Optional[str] = None, data: Optional[dict] = None):
+        params = dict(name=name) if name else None
+        return self.post(path="start_worker", data=data, params=params)
 
-    def stop_worker(self, uid: str):
-        return self.post(path=f"stop_worker/{uid}")
+    def stop_worker(self, uid: Optional[str] = None, name: Optional[str] = None):
+        params = {}
+        if uid is not None:
+            params["uid"] = uid
+        if name is not None:
+            params["name"] = name
+        return self.post(path=f"stop_worker", params=params)
```

### Comparing `dopelemon-0.0.4/service_sdk/manager/controller.py` & `dopelemon-0.0.5/service_sdk/manager/controller.py`

 * *Files identical despite different names*

### Comparing `dopelemon-0.0.4/service_sdk/manager/work_manager.py` & `dopelemon-0.0.5/service_sdk/manager/work_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import getLogger, Logger
 from time import sleep, time
 from typing import Optional, Callable, Any
 
-from service_sdk.exceptions import TimeoutWaitingForWorkerToStop
+from service_sdk.exceptions import TimeoutWaitingForWorkerToStop, CannotExceedMaxWorkersLimit
 from service_sdk.manager.controller import Controller
 from service_sdk.manager.registry import Registry
 from service_sdk.worker.worker import Worker
 
 
 class WorkManager:
     def __init__(
@@ -18,38 +18,43 @@
     ):
         self.name = name
         self.logger = logger or getLogger(__name__)
         self.work_callback = work_callback or (lambda **_: None)
         self.max_workers = max_workers
         self._registry = Registry(max_workers=max_workers)
 
-    def start_worker(self, **kwargs):
+    def start_worker(self, name: Optional[str] = None, data: Optional[dict] = None, **kwargs):
         self._update_workers_status()
         self.logger.info("Starting worker")
 
         if self._registry.counter >= self.max_workers:
-            self.logger.info("Max worker capacity reached.")
-            return
+            self.logger.warning("Max workers capacity reached")
+            raise CannotExceedMaxWorkersLimit("Max workers capacity reached")
 
-        worker = Worker(controller=Controller(), work_callback=self.work_callback)
+        worker = Worker(controller=Controller(), work_callback=self.work_callback, name=name, data=data)
         self._registry.add(worker=worker)
         worker.start()
         self.logger.info(f"Worker started. uid={worker.uid}, pid={worker.get_pid()}.")
 
     def stop_all(self, wait: bool = True, timeout: int = 10):
         for worker in self._registry.all():
             worker.controller.set_stop()
 
         if wait:
             self._wait_for_workers_to_stop(timeout=timeout)
 
-    def stop_by_uid(self, uid: str) -> Optional[str]:
-        worker = self._registry.get(id_=uid)
+    def stop_worker(self, uid: Optional[str] = None, name: Optional[str] = None) -> Optional[str]:
+        worker = None
+        if name is not None:
+            worker = self._registry.get_by_name(name=name)
+        if uid is not None:
+            worker = self._registry.get_by_uid(uid=uid)
         if not worker:
             return
+
         worker.controller.set_stop()
         self._update_workers_status()
         return worker.uid
 
     def kill_all(self, wait: bool = True, timeout: int = 10):
         for worker in self._registry.all():
             worker.process.kill()
@@ -80,8 +85,8 @@
     def restart(self):
         self.stop_all()
         self.start_worker()
 
     def _update_workers_status(self):
         for worker in self._registry.all():
             if not worker.process.is_alive():
-                self._registry.remove(id_=worker.uid)
+                self._registry.remove(uid=worker.uid)
```

### Comparing `dopelemon-0.0.4/service_sdk/service.py` & `dopelemon-0.0.5/service_sdk/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from logging import Logger
 from typing import Optional, Callable, Any
 
 import uvicorn
 from fastapi import FastAPI, APIRouter, HTTPException
 from starlette.routing import Route
 
+from service_sdk.exceptions import WorkerNameAlreadyUsed, CannotExceedMaxWorkersLimit
 from service_sdk.utils import force_kill_process, setup_logger
 from service_sdk.manager.work_manager import WorkManager
 
 
 DEFAULT_SERVICE_HOST = "127.0.0.1"
 DEFAULT_SERVICE_PORT = "8080"
 
@@ -30,56 +31,69 @@
         self.api = api or FastAPI()
         self.manager = manager or WorkManager(work_callback=worker_callback)
 
         router = APIRouter()
         router.add_api_route(path="/", endpoint=self.root, methods=["GET"])
         router.add_api_route(path="/exit", endpoint=self.exit, methods=["POST"])
         router.add_api_route(path="/kill_service", endpoint=self.kill_service, methods=["POST"])
-        router.add_api_route(path="/stop_all", endpoint=self.stop_all_worker, methods=["POST"])
+        router.add_api_route(path="/stop_all", endpoint=self.stop_all_workers, methods=["POST"])
         router.add_api_route(path="/start_worker", endpoint=self.start_worker, methods=["POST"])
-        router.add_api_route(path="/stop_worker/{uid}", endpoint=self.stop_worker, methods=["POST"])
+        router.add_api_route(path="/stop_worker", endpoint=self.stop_worker, methods=["POST"])
         self.api.include_router(router=router)
 
     def run(self, start_worker: bool = True):
         if start_worker:
             self.manager.start_worker()
         try:
             uvicorn.run(self.api, host=self.host, port=self.port, log_level="info")
         finally:
-            self.exit()
+            self.stop_all_workers(force=True, wait=True)
 
     def exit(self, force: bool = False, wait: bool = True):
         try:
-            self.stop_all_worker(force=force, wait=wait)
+            self.stop_all_workers(force=force, wait=wait)
         finally:
             self.kill_service()
 
-    def stop_all_worker(self, force: bool = False, wait: bool = True):
+    def stop_all_workers(self, force: bool = False, wait: bool = True):
         if force:
             self.manager.kill_all(wait=wait)
         else:
             self.manager.stop_all(wait=wait)
 
     @staticmethod
     def kill_service():
         force_kill_process(os.getpid())
 
-    def start_worker(self):
-        self.manager.start_worker()
+    def start_worker(self, name: Optional[str] = None, data: Optional[dict] = None):
+        try:
+            self.manager.start_worker(name=name, data=data)
+        except WorkerNameAlreadyUsed as error:
+            raise HTTPException(
+                status_code=400,
+                detail=f"Worker {name=} is already used.",
+                headers={"X-Error": str(error)},
+            )
+        except CannotExceedMaxWorkersLimit as error:
+            raise HTTPException(
+                status_code=400,
+                detail=f"Cannot exceed max workers limit={self.manager.max_workers}",
+                headers={"X-Error": str(error)},
+            )
         return {"message": "worker started"}
 
-    def stop_worker(self, uid: str):
-        result = self.manager.stop_by_uid(uid=uid)
-        if result is None:
+    def stop_worker(self, uid: Optional[str] = None, name: Optional[str] = None):
+        stopped_uid = self.manager.stop_worker(uid=uid, name=name)
+        if stopped_uid is None:
             raise HTTPException(
                 status_code=404,
                 detail="Worker not found",
-                headers={"X-Error": f"Worker {uid=} is not exist."},
+                headers={"X-Error": f"Worker is not exist."},
             )
-        return {"message": "worker stopped", "uid": result}
+        return {"message": "worker stopped", "uid": stopped_uid}
 
     def root(self):
         return {
             "name": self.manager.name,
             "status": self.manager.get_status(),
             "paths": [route.path for route in self.api.routes if isinstance(route, Route)]
         }
```

### Comparing `dopelemon-0.0.4/service_sdk/utils.py` & `dopelemon-0.0.5/service_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `dopelemon-0.0.4/service_sdk/worker/ex_thread.py` & `dopelemon-0.0.5/service_sdk/worker/ex_thread.py`

 * *Files identical despite different names*

### Comparing `dopelemon-0.0.4/service_sdk/worker/worker.py` & `dopelemon-0.0.5/service_sdk/worker/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,36 +9,43 @@
 
 
 class Worker:
     def __init__(
             self,
             controller: Controller,
             work_callback: Callable[[Any], Any],
+            name: Optional[str] = None,
             uid: Optional[str] = None,
+            data: Optional[dict] = None,
             **kwargs
     ):
         self.work_callback = work_callback
         self.controller = controller
         self.uid = uid or generate_id()
+        self.name = name or self.uid
+        self.data = data or {}
         self.process = Process(target=self.handle_work, kwargs=kwargs)
-        self.context = {"id": self.uid}
+        self.context = dict(uid=self.uid, name=self.name, data=self.data)
 
     def get_pid(self) -> Optional[int]:
         return self.process.pid
 
     def start(self):
         self.process.start()
 
     def handle_work(self, **kwargs):
         logger = setup_logger()
         counter = 0
         logger.info("Starting work")
 
         working_thread = ExThread(target=self.work_callback, daemon=True, kwargs=dict(context=self.context))
         working_thread.start()
-        while not self.controller.get_stop():
-            counter += 1
-            self.controller.set_status(counter)
-            sleep(1)
-
-        logger.info("Stop command received. Shutting worker down.")
-        working_thread.raise_exception(exception=StopGracefullyException)
+        try:
+            while not self.controller.get_stop():
+                counter += 1
+                self.controller.set_status(counter)
+                sleep(1)
+
+            logger.info("Stop command received. Shutting worker down.")
+            working_thread.raise_exception(exception=StopGracefullyException)
+        except KeyboardInterrupt as exception:
+            logger.info(f"{exception.__class__.__name__} received. Shutting worker down.")
```

### Comparing `dopelemon-0.0.4/PKG-INFO` & `dopelemon-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dopelemon
-Version: 0.0.4
-Summary: tools for microservices
+Version: 0.0.5
+Summary: Service framework with built-in API
 Author: limonyellow
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

