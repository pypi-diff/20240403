# Comparing `tmp/taskara-0.1.2.tar.gz` & `tmp/taskara-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.2.tar", max compression
+gzip compressed data, was "taskara-0.1.3.tar", max compression
```

## Comparing `taskara-0.1.2.tar` & `taskara-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.2/LICENSE
--rw-r--r--   0        0        0      221 2024-04-02 20:40:49.884528 taskara-0.1.2/README.md
--rw-r--r--   0        0        0      392 2024-04-02 20:58:34.131602 taskara-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.2/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.2/taskara/db/conn.py
--rw-r--r--   0        0        0     1449 2024-04-02 20:36:27.320183 taskara-0.1.2/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.2/taskara/env.py
--rw-r--r--   0        0        0     1606 2024-04-02 20:58:29.041770 taskara-0.1.2/taskara/models.py
--rw-r--r--   0        0        0    20304 2024-04-02 20:38:39.122416 taskara-0.1.2/taskara/task.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 taskara-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.3/LICENSE
+-rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.3/README.md
+-rw-r--r--   0        0        0      392 2024-04-03 02:47:06.328910 taskara-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.3/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.3/taskara/db/conn.py
+-rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.3/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.3/taskara/env.py
+-rw-r--r--   0        0        0     1513 2024-04-03 02:25:02.082624 taskara-0.1.3/taskara/models.py
+-rw-r--r--   0        0        0    18840 2024-04-03 02:34:10.525445 taskara-0.1.3/taskara/task.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.3/PKG-INFO
```

### Comparing `taskara-0.1.2/LICENSE` & `taskara-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.2/taskara/db/conn.py` & `taskara-0.1.3/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.2/taskara/db/models.py` & `taskara-0.1.3/taskara/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 class TaskRecord(Base):
     __tablename__ = "tasks"
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=False)
     description = Column(String, nullable=False)
     url = Column(String, nullable=True)
-    thread_id = Column(String, nullable=False)
-    feed_id = Column(String, nullable=False)
     assigned_to = Column(String, nullable=True)
     status = Column(String, nullable=False)
     created = Column(Float, nullable=False)
     started = Column(Float, nullable=False, default=0.0)
     completed = Column(Float, nullable=False, default=0.0)
     error = Column(String, default="")
     output = Column(String, default="")
-    work_threads = Column(String, nullable=False)
+    threads = Column(String, nullable=False)
     version = Column(String, nullable=False)
 
 
 class UserRecord(Base):
     __tablename__ = "users"
 
     email = Column(String, unique=True, index=True, primary_key=True)
```

### Comparing `taskara-0.1.2/taskara/models.py` & `taskara-0.1.3/taskara/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     version: Optional[str] = None
 
 
 class TaskModel(BaseModel):
     id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     description: str
     status: Optional[str] = None
-    thread: Optional[RoleThreadModel] = None
-    feed: Optional[RoleThreadModel] = None
-    work_threads: Optional[List[RoleThreadModel]] = None
+    threads: Optional[List[RoleThreadModel]] = None
     assigned_to: Optional[str] = None
     url: Optional[str] = None
     created: float = Field(default_factory=time.time)
     started: float = 0.0
     completed: float = 0.0
     error: str = ""
     output: str = ""
```

### Comparing `taskara-0.1.2/taskara/task.py` & `taskara-0.1.3/taskara/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,49 +22,43 @@
     """An agent task"""
 
     def __init__(
         self,
         description: Optional[str] = None,
         owner_id: Optional[str] = None,
         id: str = None,
-        url: Optional[str] = None,
         status: str = "defined",
         created: float = None,
         started: float = 0.0,
         completed: float = 0.0,
-        feed: RoleThread = None,
-        thread: RoleThread = None,
-        work_threads: List[RoleThread] = None,
+        threads: List[RoleThread] = [],
         assigned_to: Optional[str] = None,
         error: str = "",
         output: str = "",
         remote: Optional[str] = None,
         version: Optional[str] = None,
     ):
         self._id = id if id is not None else str(uuid.uuid4())
         self._description = description
         self._owner_id = owner_id
-        self._url = url
         self._status = status
         self._created = created if created is not None else time.time()
         self._started = started
         self._completed = completed
-        self._feed = feed if feed is not None else RoleThread()
-        self._thread = (
-            thread
-            if thread is not None
-            else RoleThread(owner_id=self._owner_id, name="feed")
-        )
-        self._work_threads = work_threads if work_threads is not None else []
         self._assigned_to = assigned_to
         self._error = error
         self._output = output
         self._remote = remote
         self._version = version if version is not None else self.generate_version_hash()
 
+        self._threads = []
+        self.create_thread("feed")
+        if threads:
+            self._threads.extend(threads)
+
         if not self._version:
             self._version = self.generate_version_hash()
         if not self._remote and not self._description:
             raise ValueError("Task must have a description or a remote task")
         if self._remote:
             if not self._id:
                 raise ValueError("ID must be set for remote tasks")
@@ -155,20 +149,20 @@
         return self._thread
 
     @thread.setter
     def thread(self, value: RoleThread):
         self._thread = value
 
     @property
-    def work_threads(self) -> List[RoleThread]:
-        return self._work_threads
+    def threads(self) -> List[RoleThread]:
+        return self._threads
 
-    @work_threads.setter
-    def work_threads(self, value: List[RoleThread]):
-        self._work_threads = value
+    @threads.setter
+    def threads(self, value: List[RoleThread]):
+        self._threads = value
 
     @property
     def assigned_to(self) -> Optional[str]:
         return self._assigned_to
 
     @assigned_to.setter
     def assigned_to(self, value: Optional[str]):
@@ -206,40 +200,36 @@
             started=self._started,
             completed=self._completed,
             thread_id=self._thread._id,
             assigned_to=self._assigned_to,
             feed_id=self._feed._id,
             error=self._error,
             output=self._output,
-            work_threads=json.dumps([t._id for t in self._work_threads]),
+            threads=json.dumps([t._id for t in self._threads]),
             version=self._version,
         )
 
     @classmethod
     def from_record(cls, record: TaskRecord) -> "Task":
-        work_threads_ids = json.loads(record.work_threads)
-        work_threads = [
-            RoleThread.find(id=thread_id)[0] for thread_id in work_threads_ids
-        ]
+        thread_ids = json.loads(record.threads)
+        threads = [RoleThread.find(id=thread_id)[0] for thread_id in thread_ids]
 
         obj = cls.__new__(cls)
         obj._id = record.id
         obj._owner_id = record.owner_id
         obj._description = record.description
         obj._url = record.url
         obj._status = record.status
         obj._created = record.created
         obj._started = record.started
         obj._completed = record.completed
-        obj._thread = RoleThread.find(id=record.thread_id)[0]
-        obj._feed = RoleThread.find(id=record.feed_id)[0]
         obj._assigned_to = record.assigned_to
         obj._error = record.error
         obj._output = record.output
-        obj._work_threads = work_threads
+        obj._threads = threads
         obj._version = record.version
         return obj
 
     def post_message(
         self,
         role: str,
         msg: str,
@@ -267,23 +257,25 @@
                 raise
 
         if thread:
             threads = RoleThread.find(id=thread)
             if threads:
                 thread: RoleThread = threads[0]
                 thread.post(role, msg, images, private, metadata)
+                return
             threads = self.find(name=thread)
             if threads:
                 thread: RoleThread = threads[0]
                 thread.post(role, msg, images, private, metadata)
+                return
             raise ValueError(f"Thread by name or id {thread} not found")
 
-        self._thread.post(role, msg, images, private, metadata)
+        self._threads[0].post(role, msg, images, private, metadata)
 
-    def create_work_thread(
+    def create_thread(
         self,
         name: Optional[str] = None,
         public: bool = False,
         metadata: Optional[dict] = None,
         id: Optional[str] = None,
     ) -> None:
         if hasattr(self, "_remote") and self._remote:
@@ -295,32 +287,32 @@
                 {"name": name, "public": public, "metadata": metadata, "id": id},
             )
             print("removed remote work thread")
             return
 
         print("creating local work thread")
         thread = RoleThread(self.owner_id, public, name, metadata)
-        self._work_threads.append(thread)
+        self._threads.append(thread)
         self.save()
         print("created local work thread")
         return
 
-    def remove_work_thread(self, thread_id: str) -> None:
+    def remove_thread(self, thread_id: str) -> None:
         if hasattr(self, "_remote") and self._remote:
             print("removing remote thread")
             self._remote_request(
                 self._remote,
                 "DELETE",
                 f"/v1/tasks/{self._id}/threads",
                 {"id": thread_id},
             )
             print("removed remote thread")
             return
 
-        self._work_threads = [t for t in self._work_threads if t._id != thread_id]
+        self._threads = [t for t in self._threads if t._id != thread_id]
         self.save()
 
     def save(self) -> None:
         print("\n!saving task", self._id)
         # Generate the new version hash
         new_version = self.generate_version_hash()
 
@@ -422,17 +414,15 @@
                     db.commit()
 
     def to_schema(self) -> TaskModel:
         return TaskModel(
             id=self._id,
             description=self._description,
             url=self._url,
-            thread=self._thread.to_schema(),
-            feed=self._feed.to_schema(),
-            work_threads=[t.to_schema() for t in self._work_threads],
+            threads=[t.to_schema() for t in self._threads],
             status=self._status,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
             error=self._error,
             output=self._output,
@@ -468,30 +458,18 @@
         obj._completed = schema.completed
         obj._assigned_to = schema.assigned_to
         obj._error = schema.error
         obj._output = schema.output
         obj._version = schema.version
         obj._remote = remote
 
-        # For thread and feed, use from_schema or create a new instance with owner_id
-        obj._thread = (
-            RoleThread.from_schema(schema.thread)
-            if schema.thread
-            else RoleThread(owner_id=owner_id)
-        )
-        obj._feed = (
-            RoleThread.from_schema(schema.feed)
-            if schema.feed
-            else RoleThread(owner_id=owner_id)
-        )
-
-        if schema.work_threads:
-            obj._work_threads = [RoleThread.from_schema(s) for s in schema.work_threads]
+        if schema.threads:
+            obj._threads = [RoleThread.from_schema(s) for s in schema.threads]
         else:
-            obj._work_threads = []
+            obj._threads = []
 
         return obj
 
     def refresh(self, auth_token: Optional[str] = None) -> None:
         print("\n!refreshing task", self._id)
         if hasattr(self, "_remote") and self._remote:
             print("\n!refreshing remote task", self._id)
@@ -509,26 +487,16 @@
                     self._created = schema.created
                     self._started = schema.started
                     self._completed = schema.completed
                     self._assigned_to = schema.assigned_to
                     self._error = schema.error
                     self._output = schema.output
                     self._version = schema.version
-                    self._thread = (
-                        RoleThread.from_schema(schema.thread)
-                        if schema.thread
-                        else RoleThread(owner_id=self._owner_id)
-                    )
-                    self._feed = (
-                        RoleThread.from_schema(schema.feed)
-                        if schema.feed
-                        else RoleThread(owner_id=self._owner_id)
-                    )
-                    self._work_threads = [
-                        RoleThread.from_schema(wt) for wt in schema.work_threads
+                    self._threads = [
+                        RoleThread.from_schema(wt) for wt in schema.threads
                     ]
                     print("\nrefreshed remote task", self._id)
             except requests.RequestException as e:
                 raise e
         else:
             raise ValueError("Refresh is only supported for remote tasks")
```

