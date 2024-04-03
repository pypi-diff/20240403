# Comparing `tmp/starbot_bilibili_datasource-1.0.0.tar.gz` & `tmp/starbot_bilibili_datasource-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbot_bilibili_datasource-1.0.0.tar", max compression
+gzip compressed data, was "starbot_bilibili_datasource-1.1.0.tar", max compression
```

## Comparing `starbot_bilibili_datasource-1.0.0.tar` & `starbot_bilibili_datasource-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0    35184 2022-08-20 15:36:38.000000 starbot_bilibili_datasource-1.0.0/LICENSE
--rw-r--r--   0        0        0      569 2023-11-29 15:15:26.288926 starbot_bilibili_datasource-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1785 2023-11-29 16:05:33.698516 starbot_bilibili_datasource-1.0.0/README.md
--rw-r--r--   0        0        0      201 2023-11-29 15:28:55.460967 starbot_bilibili_datasource-1.0.0/starbot_datasource/__init__.py
--rw-r--r--   0        0        0        0 2023-11-29 15:05:36.521370 starbot_bilibili_datasource-1.0.0/starbot_datasource/core/__init__.py
--rw-r--r--   0        0        0     6831 2023-11-29 15:24:29.007748 starbot_bilibili_datasource-1.0.0/starbot_datasource/core/datasource.py
--rw-r--r--   0        0        0      552 2023-11-29 15:24:08.586640 starbot_bilibili_datasource-1.0.0/starbot_datasource/core/event.py
--rw-r--r--   0        0        0    10608 2023-11-29 15:21:47.251220 starbot_bilibili_datasource-1.0.0/starbot_datasource/core/model.py
--rw-r--r--   0        0        0        0 2023-11-29 15:05:43.778052 starbot_bilibili_datasource-1.0.0/starbot_datasource/exception/__init__.py
--rw-r--r--   0        0        0      264 2023-11-13 15:14:18.053679 starbot_bilibili_datasource-1.0.0/starbot_datasource/exception/ApiException.py
--rw-r--r--   0        0        0      214 2023-11-29 15:09:01.325994 starbot_bilibili_datasource-1.0.0/starbot_datasource/exception/DataSourceException.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 starbot_bilibili_datasource-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-08-20 15:36:38.000000 starbot_bilibili_datasource-1.1.0/LICENSE
+-rw-r--r--   0        0        0      569 2024-04-03 15:03:55.794350 starbot_bilibili_datasource-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1755 2024-04-03 15:04:59.121495 starbot_bilibili_datasource-1.1.0/README.md
+-rw-r--r--   0        0        0      156 2024-03-28 15:56:51.771419 starbot_bilibili_datasource-1.1.0/starbot_datasource/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-29 15:05:36.521370 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__init__.py
+-rw-r--r--   0        0        0      154 2024-03-31 17:12:02.466642 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      638 2024-03-31 17:12:02.863577 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     7880 2024-03-31 17:22:19.969065 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__pycache__/datasource.cpython-310.pyc
+-rw-r--r--   0        0        0      778 2024-03-31 17:12:02.467665 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__pycache__/event.cpython-310.pyc
+-rw-r--r--   0        0        0     7873 2024-03-31 17:12:02.666405 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0      335 2024-04-03 14:52:03.679583 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/config.json
+-rw-r--r--   0        0        0     2630 2024-04-03 14:52:03.674593 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/config.py
+-rw-r--r--   0        0        0     7131 2024-04-03 14:56:54.518659 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/datasource.py
+-rw-r--r--   0        0        0      552 2023-11-29 15:24:08.586640 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/event.py
+-rw-r--r--   0        0        0    10672 2024-03-10 17:32:23.632686 starbot_bilibili_datasource-1.1.0/starbot_datasource/core/model.py
+-rw-r--r--   0        0        0        0 2023-11-29 15:05:43.778052 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-31 17:12:02.859493 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      770 2024-03-31 17:12:02.861536 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/__pycache__/ApiException.cpython-310.pyc
+-rw-r--r--   0        0        0      632 2024-03-31 17:12:02.860533 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/__pycache__/DataSourceException.cpython-310.pyc
+-rw-r--r--   0        0        0      264 2023-11-13 15:14:18.053679 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/ApiException.py
+-rw-r--r--   0        0        0      214 2023-11-29 15:09:01.325994 starbot_bilibili_datasource-1.1.0/starbot_datasource/exception/DataSourceException.py
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 starbot_bilibili_datasource-1.1.0/PKG-INFO
```

### Comparing `starbot_bilibili_datasource-1.0.0/LICENSE` & `starbot_bilibili_datasource-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.0.0/pyproject.toml` & `starbot_bilibili_datasource-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbot-bilibili-datasource"
-version = "1.0.0"
+version = "1.1.0"
 description = "StarBot 推送配置数据源"
 keywords = ["starbot", "bilibili", "bot"]
 license = "AGPL-3.0-only"
 authors = ["Starlwr <lwr1104@qq.com>"]
 readme = "README.md"
 repository = "https://github.com/Starlwr/StarBotDataSource"
 packages = [{ include = "starbot_datasource" }]
```

### Comparing `starbot_bilibili_datasource-1.0.0/README.md` & `starbot_bilibili_datasource-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![STARS](https://img.shields.io/github/stars/Starlwr/StarBotDataSource?color=yellow&label=Stars)](https://github.com/Starlwr/StarBotDataSource/stargazers)
 
 **StarBot 推送配置数据源**
 </div>
 
 ## 用途
 
-* 已内置 字典数据源(DictDataSource) 和 JSON 数据源(JsonDataSource) 实现
+* 已内置 JSON 数据源(JsonDataSource) 实现
 * 可自行实现其他来源的推送配置数据源
 
 ## 快速开始
 ### 安装
 
 ```shell
 pip install starbot-bilibili-datasource
@@ -49,10 +49,10 @@
         
         # 在此实现初始化逻辑
         pass
 
         logger.success(f"成功从 自定义来源 中导入了 {len(self.ups)} 个 UP 主")
 ```
 
-## 鸣谢
+## 相关项目
 
 * [StarBotExecutor](https://github.com/Starlwr/StarBotExecutor): 一个基于订阅发布模式的异步执行器
```

### Comparing `starbot_bilibili_datasource-1.0.0/starbot_datasource/core/datasource.py` & `starbot_bilibili_datasource-1.1.0/starbot_datasource/core/datasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import abc
 import asyncio
 import json
-from typing import List, Dict, Union, Optional, NoReturn, Set
+import os
+from json import JSONDecodeError
+from typing import Dict, NoReturn, Set
 
 from loguru import logger
 from pydantic import ValidationError
 from starbot_executor import executor
 
+from .. import config
 from ..core.event import EventType, DataSourceEvent
 from ..core.model import Up
 from ..exception.DataSourceException import DataSourceException
 
 
 class DataSource(metaclass=abc.ABCMeta):
     """
@@ -18,14 +21,17 @@
     """
 
     def __init__(self):
         self.ups: Set[Up] = set()
         self.uids: Set[int] = set()
         self.__up_map: Dict[int, Up] = {}
 
+    def __getitem__(self, key):
+        return self.__up_map[key]
+
     @abc.abstractmethod
     async def load(self) -> NoReturn:
         """
         读取配置，基类空实现
         """
         pass
 
@@ -79,80 +85,49 @@
         self.ups.add(up)
         self.uids.add(up.uid)
         self.__up_map[up.uid] = up
 
         executor.dispatch(up, EventType.DataSourceEvent, DataSourceEvent.DataSourceUpdated)
 
 
-class DictDataSource(DataSource):
-    """
-    使用字典初始化的推送配置数据源
-    """
-
-    def __init__(self, dict_config: Union[List[Dict], Dict]):
-        super().__init__()
-        self.__config = dict_config
-
-        if isinstance(self.__config, dict):
-            self.__config = [self.__config]
-
-    async def load(self) -> NoReturn:
-        """
-        从字典中初始化配置
-        """
-        if self.ups:
-            return
-
-        logger.info("已选用 Dict 作为 Bot 数据源")
-        logger.info("开始从 Dict 中初始化 Bot 配置")
-
-        for up in self.__config:
-            try:
-                self.add(Up(**up))
-            except ValidationError as ex:
-                raise DataSourceException(f"提供的配置字典中缺少必须的 {ex.errors()[0].get('loc')[-1]} 参数")
-
-        logger.success(f"成功从 Dict 中导入了 {len(self.ups)} 个 UP 主")
-
-
 class JsonDataSource(DataSource):
     """
     使用 JSON 初始化的推送配置数据源
     """
-    def __init__(self, json_file: str, auto_reload: Optional[bool] = True, auto_reload_interval: Optional[int] = 5):
+    def __init__(self):
         super().__init__()
         self.__config = None
-        self.__content = ""
 
-        self.__json_file = json_file
-        self.__auto_reload = auto_reload
-        self.__auto_reload_interval = auto_reload_interval
+        self.__json_file = config.get("datasource.json_datasource.file_path", str, "推送配置.json")
+        self.__auto_reload = config.get("datasource.json_datasource.auto_reload", bool, True)
+        self.__auto_reload_interval = config.get("datasource.json_datasource.auto_reload_interval", int, 5)
 
     async def load(self) -> NoReturn:
         """
         从 JSON 字符串中初始化配置
         """
         if self.ups:
             return
 
         logger.info("已选用 JSON 作为 Bot 数据源")
         logger.info("开始从 JSON 中初始化 Bot 配置")
 
         try:
+            modify_time = os.path.getmtime(self.__json_file)
             with open(self.__json_file, encoding="utf-8") as file:
-                self.__content = file.read()
+                content = file.read()
         except FileNotFoundError:
             raise DataSourceException("JSON 文件不存在, 请检查文件路径是否正确")
         except UnicodeDecodeError:
             raise DataSourceException("JSON 文件编码不正确, 请将其转换为 UTF-8 格式编码后重试")
         except Exception as ex:
             raise DataSourceException(f"读取 JSON 文件异常 {ex}")
 
         try:
-            self.__config = json.loads(self.__content)
+            self.__config = json.loads(content)
         except Exception:
             raise DataSourceException("JSON 文件内容格式不正确")
 
         if isinstance(self.__config, dict):
             self.__config = [self.__config]
 
         for up in self.__config:
@@ -160,53 +135,75 @@
                 self.add(Up(**up))
             except ValidationError as ex:
                 raise DataSourceException(f"提供的配置字典中缺少必须的 {ex.errors()[0].get('loc')[-1]} 参数")
 
         logger.success(f"成功从 JSON 中导入了 {len(self.ups)} 个 UP 主")
 
         if self.__auto_reload:
-            executor.create_task(self.__auto_reload_task())
+            executor.create_task(self.__auto_reload_task(modify_time))
 
-    async def __auto_reload_task(self) -> NoReturn:
+    async def __auto_reload_task(self, modify_time: float) -> NoReturn:
         """
         JSON 文件内容发生变化时自动重载配置
+
+        Args:
+            modify_time: 配置文件修改时间
         """
         while True:
             await asyncio.sleep(self.__auto_reload_interval)
             try:
-                with open(self.__json_file, encoding="utf-8") as file:
-                    content = file.read()
+                new_modify_time = os.path.getmtime(self.__json_file)
 
-                if content == self.__content:
+                if new_modify_time == modify_time:
                     continue
 
+                modify_time = new_modify_time
+
+                logger.info(f"数据源配置已更新, 开始重载配置")
+
+                with open(self.__json_file, encoding="utf-8") as file:
+                    content = file.read()
+
                 conf = json.loads(content)
                 if isinstance(conf, dict):
                     conf = [conf]
 
                 new_ups = []
                 for up in conf:
                     new_ups.append(Up(**up))
 
                 new_up_set = set(new_ups)
                 if len(new_up_set) != len(new_ups):
                     raise DataSourceException("数据源中不可含有重复的主播")
 
-                self.__content = content
                 self.__config = conf
 
                 added_ups = new_up_set - self.ups
                 removed_ups = self.ups - new_up_set
 
-                logger.info(f"""检测到数据源配置中 {', '.join([
-                    f'{action}了 {len(ups)} 个主播' for action, ups in [('新增', added_ups), ('移除', removed_ups)] if ups
-                ])}""")
+                tip = [f'{act}了 {len(ups)} 个主播' for act, ups in [('新增', added_ups), ('移除', removed_ups)] if ups]
+                if tip:
+                    logger.info(f"检测到 {', '.join(tip)}")
+                else:
+                    logger.info("未检测到新增或移除的主播, 开始重载已存在主播的配置")
 
-                for up in new_up_set:
+                for up in new_up_set.union(self.ups):
                     if up in added_ups:
                         self.add(up)
                     elif up in removed_ups:
                         self.remove(up.uid)
                     else:
                         self.update(up)
-            except Exception:
+
+                logger.success("数据源配置重载成功")
+            except FileNotFoundError:
+                logger.error("数据源配置 JSON 文件不存在")
+            except UnicodeDecodeError:
+                logger.error("数据源配置 JSON 文件编码不正确, 请将其转换为 UTF-8 格式编码")
+            except JSONDecodeError:
+                logger.error("数据源配置 JSON 文件内容格式不正确")
+            except DataSourceException as ex:
+                logger.error(ex.msg)
+            except Exception as ex:
+                logger.error(f"数据源自动重载任务异常 {ex}")
+            finally:
                 continue
```

### Comparing `starbot_bilibili_datasource-1.0.0/starbot_datasource/core/event.py` & `starbot_bilibili_datasource-1.1.0/starbot_datasource/core/event.py`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.0.0/starbot_datasource/core/model.py` & `starbot_bilibili_datasource-1.1.0/starbot_datasource/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
     enabled: bool = False
     """是否启用开播推送。默认：False"""
 
     message: str = ""
     """
     开播推送内容模板。
-    专用占位符：{uname} 主播昵称，{title} 直播间标题，{url} 直播间链接，{cover} 直播间封面图。
-    通用占位符：{next} 消息分条，{atall} @全体成员，{at114514} @指定QQ号，{urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
+    专用占位符: {uname} 主播昵称，{title} 直播间标题，{url} 直播间链接，{cover} 直播间封面图。
+    通用占位符: {next} 消息分条，{atall} @全体成员，{at=114514} @指定成员，
+              {urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
     默认：""
     """
 
     @classmethod
     def default(cls):
         """
         获取功能全部开启的默认 LiveOn 实例
@@ -39,16 +40,17 @@
 
     enabled: bool = False
     """是否启用下播推送。默认：False"""
 
     message: str = ""
     """
     下播推送内容模板。
-    专用占位符：{uname} 主播昵称。
-    通用占位符：{next} 消息分条，{atall} @全体成员，{at114514} @指定QQ号，{urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
+    专用占位符: {uname} 主播昵称。
+    通用占位符: {next} 消息分条，{atall} @全体成员，{at=114514} @指定成员，
+              {urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
     默认：""
     """
 
     @classmethod
     def default(cls):
         """
         获取功能全部开启的默认 LiveOff 实例
@@ -170,16 +172,18 @@
 
     enabled: bool = False
     """是否启用动态推送。默认：False"""
 
     message: str = ""
     """
     动态推送内容模板。
-    专用占位符：{uname} 主播昵称，{action} 动态操作类型（发表了新动态，转发了新动态，投稿了新视频...），{url} 动态链接（若为发表视频、专栏等则为视频、专栏等对应的链接），{picture} 动态图片。
-    通用占位符：{next} 消息分条，{atall} @全体成员，{at114514} @指定QQ号，{urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
+    专用占位符: {uname} 主播昵称，{action} 动态操作类型（发表了新动态，转发了新动态，投稿了新视频...），
+              {url} 动态链接（若为发表视频、专栏等则为视频、专栏等对应的链接），{picture} 动态图片。
+    通用占位符: {next} 消息分条，{atall} @全体成员，{at=114514} @指定成员，
+              {urlpic=链接} 网络图片，{pathpic=路径} 本地图片，{base64pic=base64字符串} base64图片。
     默认：""
     """
 
     @classmethod
     def default(cls):
         """
         获取功能全部开启的默认 DynamicUpdate 实例
```

### Comparing `starbot_bilibili_datasource-1.0.0/PKG-INFO` & `starbot_bilibili_datasource-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbot-bilibili-datasource
-Version: 1.0.0
+Version: 1.1.0
 Summary: StarBot 推送配置数据源
 Home-page: https://github.com/Starlwr/StarBotDataSource
 License: AGPL-3.0-only
 Keywords: starbot,bilibili,bot
 Author: Starlwr
 Author-email: lwr1104@qq.com
 Requires-Python: >=3.10,<4.0
@@ -28,15 +28,15 @@
 [![STARS](https://img.shields.io/github/stars/Starlwr/StarBotDataSource?color=yellow&label=Stars)](https://github.com/Starlwr/StarBotDataSource/stargazers)
 
 **StarBot 推送配置数据源**
 </div>
 
 ## 用途
 
-* 已内置 字典数据源(DictDataSource) 和 JSON 数据源(JsonDataSource) 实现
+* 已内置 JSON 数据源(JsonDataSource) 实现
 * 可自行实现其他来源的推送配置数据源
 
 ## 快速开始
 ### 安装
 
 ```shell
 pip install starbot-bilibili-datasource
@@ -69,11 +69,11 @@
         
         # 在此实现初始化逻辑
         pass
 
         logger.success(f"成功从 自定义来源 中导入了 {len(self.ups)} 个 UP 主")
 ```
 
-## 鸣谢
+## 相关项目
 
 * [StarBotExecutor](https://github.com/Starlwr/StarBotExecutor): 一个基于订阅发布模式的异步执行器
```

