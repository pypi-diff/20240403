# Comparing `tmp/starbot_executor-1.3.0.tar.gz` & `tmp/starbot_executor-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbot_executor-1.3.0.tar", max compression
+gzip compressed data, was "starbot_executor-1.4.0.tar", max compression
```

## Comparing `starbot_executor-1.3.0.tar` & `starbot_executor-1.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-11-22 07:55:21.658225 starbot_executor-1.3.0/LICENSE
--rw-r--r--   0        0        0      496 2023-11-28 14:57:26.816401 starbot_executor-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6243 2023-11-22 13:12:41.101337 starbot_executor-1.3.0/README.md
--rw-r--r--   0        0        0       37 2023-11-22 13:11:24.323082 starbot_executor-1.3.0/starbot_executor/__init__.py
--rw-r--r--   0        0        0        0 2023-11-21 13:46:16.485466 starbot_executor-1.3.0/starbot_executor/core/__init__.py
--rw-r--r--   0        0        0      142 2023-11-21 14:17:56.493192 starbot_executor-1.3.0/starbot_executor/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9771 2023-11-22 16:04:48.885302 starbot_executor-1.3.0/starbot_executor/core/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0        0        0     8697 2023-11-28 14:27:14.110411 starbot_executor-1.3.0/starbot_executor/core/executor.py
--rw-r--r--   0        0        0     6614 1970-01-01 00:00:00.000000 starbot_executor-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-11-22 07:55:21.658225 starbot_executor-1.4.0/LICENSE
+-rw-r--r--   0        0        0      496 2024-04-03 14:59:15.955676 starbot_executor-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6433 2023-12-05 15:23:46.381866 starbot_executor-1.4.0/README.md
+-rw-r--r--   0        0        0      195 2023-12-02 16:48:11.069533 starbot_executor-1.4.0/starbot_executor/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-21 13:46:16.485466 starbot_executor-1.4.0/starbot_executor/core/__init__.py
+-rw-r--r--   0        0        0      142 2023-11-21 14:17:56.493192 starbot_executor-1.4.0/starbot_executor/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9867 2023-12-04 09:50:43.185324 starbot_executor-1.4.0/starbot_executor/core/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0        0        0     9458 2023-12-09 12:38:53.896448 starbot_executor-1.4.0/starbot_executor/core/executor.py
+-rw-r--r--   0        0        0     6792 1970-01-01 00:00:00.000000 starbot_executor-1.4.0/PKG-INFO
```

### Comparing `starbot_executor-1.3.0/LICENSE` & `starbot_executor-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starbot_executor-1.3.0/README.md` & `starbot_executor-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     # 仅可被例 4 监听到
     executor.dispatch(None, "Message", channel="Private")
 
     # ——————————————————————————————————————————————————————————————————————
 
     # 排队执行示例
     await asyncio.sleep(1)
-    await executor.create_queue_task(test(), 3)
-    await executor.create_queue_task(test(), 3)
-    await executor.create_queue_task(test(), 3)
+    await executor.create_queue_task(test, 3)
+    await executor.create_queue_task(test, 3)
+    await executor.create_queue_task(test, 3)
 
 
 async def test():
     print(f"当前时间戳: {int(time.time())}")
 
 
 loop = executor.init()
@@ -147,79 +147,91 @@
 * func: 异步任务
 
 Returns:
 * Task，可用于进行 await 操作
 
 #### 3. create_queue_task
 ```
-create_queue_task(self, func: Coroutine, wait: Union[int, float] = 0) -> NoReturn
+create_queue_task(self, func: Callable, wait: Union[int, float] = 0) -> NoReturn
 ```
 向异步任务执行队列中添加新任务
 
 Args:
 * func: 异步任务
 * wait: 执行任务后的等待时间。默认：0
 
 Returns:
 * 无返回值
 
-#### 4. create_channel
+#### 4. remove_queue_task
+```
+remove_queue_task(self, func: Callable) -> bool
+```
+从异步任务执行队列中移除任务
+
+Args:
+* func: 异步任务
+
+Returns:
+* 是否移除成功
+
+#### 5. create_channel
 ```
 create_channel(self, channel: str) -> NoReturn
 ```
 显式创建消息频道，一般情况下可省略，注册事件监听器时若指定了不存在的消息频道会自动创建
 
 Args:
 * channel: 消息频道名
 
 Returns:
 * 无返回值
 
-#### 5. add_event_listener
+#### 6. add_event_listener
 ```
 add_event_listener(self, func: Callable, *subjects: Any, channel: str = "Default") -> NoReturn
 ```
 注册事件监听器
 
 Args:
 * func: 回调异步函数
 * subjects: 订阅消息主题，可传入多个值
 * channel: 注册监听的消息频道。默认：Default
 
 Returns:
 * 无返回值
 
-#### 6. remove_event_listener
+#### 7. remove_event_listener
 ```
 remove_event_listener(self, *subjects: Any, func: Optional[Callable] = None, channel: str = "Default") -> bool
 ```
 移除事件监听器回调函数
 
 Args:
 * subjects: 订阅消息主题，可传入多个值
 * func: 要移除的回调异步函数，参数为 None 时，移除监听此消息主题的全部回调函数。默认：None
 * channel: 移除监听的消息频道。默认：Default
 
 Returns:
 * 是否移除成功
 
-#### 7. on
+#### 8. on
 ```
 on(self, *subjects: Any, channel: str = "Default") -> Callable
 ```
 注册事件监听器装饰器
 
 Args:
 * subjects: 订阅消息主题，可传入多个值
 * channel: 注册监听的消息频道。默认：Default
 
 Returns:
 * 装饰后的函数
 
-#### 8. dispatch
+#### 9. dispatch
 ```
 dispatch(self, data: Any, *subjects: Any, recursion: bool = True, channel: str = "Default") -> NoReturn
 ```
 发布消息主题
 
 Args:
 * data: 事件附加数据
```

### Comparing `starbot_executor-1.3.0/starbot_executor/core/executor.py` & `starbot_executor-1.4.0/starbot_executor/core/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import inspect
 from asyncio import AbstractEventLoop, Task, Queue
+from collections import deque
 from typing import Dict, Coroutine, Set, Optional, Any, NoReturn, Tuple, Union, List, Callable
 
 
 class Handler:
     """
     订阅消息主题回调处理器
     """
@@ -78,26 +79,29 @@
     """
     __loop: Optional[AbstractEventLoop]
     """asyncio 事件循环"""
 
     __running_tasks: Set[Task]
     """执行中的任务"""
 
-    __task_queue: Queue[Tuple[Coroutine, int]]
+    __task_queue: Queue[Tuple[Callable, int]]
     """排队执行队列"""
 
     __handlers: Dict[str, Handler]
     """订阅-发布回调方法"""
 
     def __init__(self):
         self.__loop = None
         self.__running_tasks = set()
         self.__task_queue = Queue()
         self.__handlers = {"Default": Handler()}
 
+    def __contains__(self, item):
+        return item in list(map(lambda task: task[0], self.__task_queue.__getattribute__("_queue")))
+
     def init(self, loop: Optional[AbstractEventLoop] = None) -> AbstractEventLoop:
         """
         初始化异步任务执行器
 
         Args:
             loop: 事件循环，未传入时自动创建新事件循环。默认：None
 
@@ -136,31 +140,55 @@
             raise RuntimeError("在执行任务之前先使用 executor.init() 或 executor.init(loop) 方法初始化异步执行器")
 
         task = self.__loop.create_task(func)
         self.__running_tasks.add(task)
         task.add_done_callback(lambda t: self.__running_tasks.remove(t))
         return task
 
-    async def create_queue_task(self, func: Coroutine, wait: Union[int, float] = 0) -> NoReturn:
+    async def create_queue_task(self, func: Callable, wait: Union[int, float] = 0) -> NoReturn:
         """
         向异步任务执行队列中添加新任务
 
         Args:
             func: 异步任务
             wait: 执行任务后的等待时间。默认：0
         """
         await self.__task_queue.put((func, wait))
 
+    def remove_queue_task(self, func: Callable) -> bool:
+        """
+        从异步任务执行队列中移除任务
+
+        Args:
+            func: 异步任务
+
+        Returns:
+            是否移除成功
+        """
+        if func not in self:
+            return False
+
+        async def empty():
+            pass
+
+        queue: deque = self.__task_queue.__getattribute__("_queue")
+        for index, (task, _) in enumerate(queue):
+            if task == func:
+                queue[index] = (empty, 0)
+                return True
+
+        return False
+
     async def __queue_task_executor(self) -> NoReturn:
         """
         异步任务队列调度执行器，随异步任务执行器初始化自动启动
         """
         while True:
             func, wait = await self.__task_queue.get()
-            self.create_task(func)
+            self.create_task(func())
             await asyncio.sleep(wait)
             self.__task_queue.task_done()
 
     def create_channel(self, channel: str) -> NoReturn:
         """
         显式创建消息频道，一般情况下可省略，注册事件监听器时若指定了不存在的消息频道会自动创建
```

### Comparing `starbot_executor-1.3.0/PKG-INFO` & `starbot_executor-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbot-executor
-Version: 1.3.0
+Version: 1.4.0
 Summary: 一个基于订阅发布模式的异步执行器
 Home-page: https://github.com/Starlwr/StarBotExecutor
 License: MIT
 Keywords: starbot,async,executor
 Author: Starlwr
 Author-email: lwr1104@qq.com
 Requires-Python: >=3.10,<4.0
@@ -105,17 +105,17 @@
     # 仅可被例 4 监听到
     executor.dispatch(None, "Message", channel="Private")
 
     # ——————————————————————————————————————————————————————————————————————
 
     # 排队执行示例
     await asyncio.sleep(1)
-    await executor.create_queue_task(test(), 3)
-    await executor.create_queue_task(test(), 3)
-    await executor.create_queue_task(test(), 3)
+    await executor.create_queue_task(test, 3)
+    await executor.create_queue_task(test, 3)
+    await executor.create_queue_task(test, 3)
 
 
 async def test():
     print(f"当前时间戳: {int(time.time())}")
 
 
 loop = executor.init()
@@ -164,79 +164,91 @@
 * func: 异步任务
 
 Returns:
 * Task，可用于进行 await 操作
 
 #### 3. create_queue_task
 ```
-create_queue_task(self, func: Coroutine, wait: Union[int, float] = 0) -> NoReturn
+create_queue_task(self, func: Callable, wait: Union[int, float] = 0) -> NoReturn
 ```
 向异步任务执行队列中添加新任务
 
 Args:
 * func: 异步任务
 * wait: 执行任务后的等待时间。默认：0
 
 Returns:
 * 无返回值
 
-#### 4. create_channel
+#### 4. remove_queue_task
+```
+remove_queue_task(self, func: Callable) -> bool
+```
+从异步任务执行队列中移除任务
+
+Args:
+* func: 异步任务
+
+Returns:
+* 是否移除成功
+
+#### 5. create_channel
 ```
 create_channel(self, channel: str) -> NoReturn
 ```
 显式创建消息频道，一般情况下可省略，注册事件监听器时若指定了不存在的消息频道会自动创建
 
 Args:
 * channel: 消息频道名
 
 Returns:
 * 无返回值
 
-#### 5. add_event_listener
+#### 6. add_event_listener
 ```
 add_event_listener(self, func: Callable, *subjects: Any, channel: str = "Default") -> NoReturn
 ```
 注册事件监听器
 
 Args:
 * func: 回调异步函数
 * subjects: 订阅消息主题，可传入多个值
 * channel: 注册监听的消息频道。默认：Default
 
 Returns:
 * 无返回值
 
-#### 6. remove_event_listener
+#### 7. remove_event_listener
 ```
 remove_event_listener(self, *subjects: Any, func: Optional[Callable] = None, channel: str = "Default") -> bool
 ```
 移除事件监听器回调函数
 
 Args:
 * subjects: 订阅消息主题，可传入多个值
 * func: 要移除的回调异步函数，参数为 None 时，移除监听此消息主题的全部回调函数。默认：None
 * channel: 移除监听的消息频道。默认：Default
 
 Returns:
 * 是否移除成功
 
-#### 7. on
+#### 8. on
 ```
 on(self, *subjects: Any, channel: str = "Default") -> Callable
 ```
 注册事件监听器装饰器
 
 Args:
 * subjects: 订阅消息主题，可传入多个值
 * channel: 注册监听的消息频道。默认：Default
 
 Returns:
 * 装饰后的函数
 
-#### 8. dispatch
+#### 9. dispatch
 ```
 dispatch(self, data: Any, *subjects: Any, recursion: bool = True, channel: str = "Default") -> NoReturn
 ```
 发布消息主题
 
 Args:
 * data: 事件附加数据
```

