# Comparing `tmp/pih-0.32.tar.gz` & `tmp/pih-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.32.tar", last modified: Fri Mar 29 05:55:10 2024, max compression
+gzip compressed data, was "pih-0.33.tar", last modified: Tue Apr  2 23:28:02 2024, max compression
```

## Comparing `pih-0.32.tar` & `pih-0.33.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:10.727903 pih-0.32/
--rw-rw-rw-   0        0        0      247 2024-03-29 05:55:10.695608 pih-0.32/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:08.431805 pih-0.32/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.32/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:08.811509 pih-0.32/pih/collections/
--rw-rw-rw-   0        0        0    27985 2024-03-25 23:03:49.000000 pih-0.32/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-02-21 00:45:01.000000 pih-0.32/pih/collections/service.py
--rw-rw-rw-   0        0        0   104106 2024-03-27 00:18:20.000000 pih-0.32/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.32/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:10.243010 pih-0.32/pih/consts/
--rw-rw-rw-   0        0        0    25132 2024-03-29 05:54:03.000000 pih-0.32/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3650 2024-03-11 05:53:16.000000 pih-0.32/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1584 2024-03-22 01:07:28.000000 pih-0.32/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.32/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.32/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.32/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29270 2024-03-13 12:22:09.000000 pih-0.32/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.32/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.32/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.32/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.32/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.32/pih/consts/password.py
--rw-rw-rw-   0        0        0    11276 2024-03-29 04:57:29.000000 pih-0.32/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.32/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.32/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.32/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.32/pih/consts/rpc.py
--rw-rw-rw-   0        0        0      924 2024-02-15 03:33:44.000000 pih-0.32/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.32/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.32/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13234 2024-03-26 00:15:02.000000 pih-0.32/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.32/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.32/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   546111 2024-03-28 10:54:33.000000 pih-0.32/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:10.414902 pih-0.32/pih/rpc/
--rw-rw-rw-   0        0        0    34084 2024-02-21 13:10:29.000000 pih-0.32/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.32/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.32/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.32/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:10.601860 pih-0.32/pih/tools/
--rw-rw-rw-   0        0        0    51255 2024-03-28 11:42:14.000000 pih-0.32/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-02-26 05:50:04.000000 pih-0.32/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.32/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:55:10.664384 pih-0.32/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-03-29 05:55:07.000000 pih-0.32/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-03-29 05:55:07.000000 pih-0.32/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 05:55:07.000000 pih-0.32/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-29 05:55:07.000000 pih-0.32/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-29 05:55:07.000000 pih-0.32/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 05:55:10.743524 pih-0.32/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:02.157410 pih-0.33/
+-rw-rw-rw-   0        0        0      247 2024-04-02 23:28:02.093831 pih-0.33/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 23:27:59.489820 pih-0.33/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.33/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:00.165710 pih-0.33/pih/collections/
+-rw-rw-rw-   0        0        0    28133 2024-04-02 01:24:26.000000 pih-0.33/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-02-21 00:45:01.000000 pih-0.33/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104106 2024-04-02 01:12:34.000000 pih-0.33/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.33/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.590188 pih-0.33/pih/consts/
+-rw-rw-rw-   0        0        0    25132 2024-04-02 23:24:59.000000 pih-0.33/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3650 2024-03-11 05:53:16.000000 pih-0.33/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1584 2024-03-22 01:07:28.000000 pih-0.33/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.33/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.33/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.33/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29270 2024-03-13 12:22:09.000000 pih-0.33/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.33/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.33/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.33/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.33/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.33/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11276 2024-03-29 04:57:29.000000 pih-0.33/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.33/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.33/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.33/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.33/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0      924 2024-02-15 03:33:44.000000 pih-0.33/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.33/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.33/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13234 2024-03-26 00:15:02.000000 pih-0.33/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.33/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.33/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   546859 2024-04-02 08:28:41.000000 pih-0.33/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.794353 pih-0.33/pih/rpc/
+-rw-rw-rw-   0        0        0    34084 2024-02-21 13:10:29.000000 pih-0.33/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.33/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.33/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.33/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:01.968305 pih-0.33/pih/tools/
+-rw-rw-rw-   0        0        0    51249 2024-03-30 01:04:09.000000 pih-0.33/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3958 2024-02-26 05:50:04.000000 pih-0.33/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.33/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:28:02.046938 pih-0.33/pih.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 23:27:58.000000 pih-0.33/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 23:28:02.173033 pih-0.33/setup.cfg
```

### Comparing `pih-0.32/pih/collections/__init__.py` & `pih-0.33/pih/collections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,29 +690,32 @@
 class RobocopyJobDescription:
     name: str | None = None
     start_datetime: str | None = None
     host: str | None = None
     run_from_system_account: bool = False
     run_with_elevetion: bool = False
     live: bool = False
-
+    exclude: bool = False
+    
     def clone(
         self,
         job_name: str,
         start_datetime: str | None = None,
         host: str | None = None,
         live: bool | None = None,
+        exclude: bool = False
     ):
         return RobocopyJobDescription(
             job_name,
             start_datetime,
             host or self.host,
             self.run_from_system_account,
             self.run_with_elevetion,
             self.live if live is None else live,
+            self.exclude if exclude is None else exclude,
         )
 
 
 @dataclass
 class RobocopyJobItem(RobocopyJobDescription):
     source: str | None = None
     destination: str | None = None
@@ -724,14 +727,15 @@
     source: str | None = None
     destination: str | None = None
     active: bool = False
     last_created: str | None = None
     last_status: int | None = None
     live: bool = False
     pid: int = -1
+    exclude: bool = False
 
 
 @dataclass
 class PrinterADInformation:
     driverName: str | None = None
     adminDescription: str | None = None
     description: str | None = None
```

### Comparing `pih-0.32/pih/collections/service.py` & `pih-0.33/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/console_api.py` & `pih-0.33/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -777,15 +777,15 @@
                     report_list: list[str] = []
                     admin_description_list: list[str] = (
                         printer_report.adminDescription or ""
                     ).split(",")
                     name: str = A.D_F.host_name(printer_report.ip)
                     description_list: list[str] = A.D_F.format(
                         printer_report.description, use_python=True
-                    ).splitlines()
+                    ).split("\\n")
                     report_list.append(
                         j(
                             (
                                 self.bold("Модель"),
                                 ": ",
                                 nl(printer_report.model),
                                 self.bold("Название"),
```

### Comparing `pih-0.32/pih/console_api_wrapper.py` & `pih-0.33/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/__init__.py` & `pih-0.33/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.32"
+VERSION: str = "0.33"
 
 EMAIL_SPLITTER: str = "@"
 ISOLATED_ARG_NAME: str = "isolated"
 ARGUMENT_PREFIX: str = "--"
 SPLITTER: str = ":"
 UNKNOWN: str = "?"
```

### Comparing `pih-0.32/pih/consts/ad.py` & `pih-0.33/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/addresses.py` & `pih-0.33/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/date_time.py` & `pih-0.33/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/errors.py` & `pih-0.33/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/events.py` & `pih-0.33/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/hosts.py` & `pih-0.33/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/names.py` & `pih-0.33/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/password.py` & `pih-0.33/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/paths.py` & `pih-0.33/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/polibase.py` & `pih-0.33/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/service.py` & `pih-0.33/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/service_commands.py` & `pih-0.33/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/service_roles.py` & `pih-0.33/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/consts/settings.py` & `pih-0.33/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/pih.py` & `pih-0.33/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -2535,14 +2535,15 @@
             PIH.input: Input = input
         else:
             self.input: Input = input
         if n(session):
             PIH.session: Session = Session(input, output)
         else:
             self.session: Session = session
+        PIH.output.init()
 
     class VERSION:
         value: str = VERSION
 
         @staticmethod
         def need_update() -> bool:
             return False
@@ -3444,15 +3445,15 @@
             output: str = result.stdout
             return PIH.DATA.CHECK.returncode(result) and (
                 output.count("(TTL)") < count or output.count("TTL=") < count
             )
 
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
-            return PIH.PATH.adapt_for_windows(
+            return PIH.PATH.for_windows(
                 PIH.PATH.join(PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
             )
 
         @staticmethod
         def create_command_for_executor(
             executor_name: str,
             command: tuple[str, ...] | str,
@@ -4631,30 +4632,39 @@
         ) -> None:
             PIH.EVENT.send(
                 Events.IT_NOTIFY_ABOUT_TEMPORARY_MARK_RETURN,
                 (mark.FullName, temporary_tab_number),
             )
 
         @staticmethod
-        def backup_notify_about_polibase_creation_db_dumb_start() -> None:
-            PIH.EVENT.send(Events.POLIBASE_CREATION_DB_DUMP_START)
+        def backup_notify_about_polibase_creation_db_dumb_start(
+            save: bool = True,
+        ) -> None:
+            event: Events = Events.POLIBASE_CREATION_DB_DUMP_START
+            PIH.EVENT.send(
+                event, flags=None if save else PIH.DATA.EVENT.remove_save_flag(event)
+            )
 
         @staticmethod
-        def backup_notify_about_polibase_creation_db_dumb_complete(size: int) -> None:
-            PIH.EVENT.send(Events.POLIBASE_CREATION_DB_DUMP_COMPLETE, (size,))
+        def backup_notify_about_polibase_creation_db_dumb_complete(size: int, save: bool = True) -> None:
+            event: Events = Events.POLIBASE_CREATION_DB_DUMP_COMPLETE
+            PIH.EVENT.send(Events.POLIBASE_CREATION_DB_DUMP_COMPLETE, (size,), None if save else PIH.DATA.EVENT.remove_save_flag(event))
 
         @staticmethod
         def backup_notify_about_polibase_creation_archived_db_dumb_start() -> None:
             PIH.EVENT.send(Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_START)
 
         @staticmethod
         def backup_notify_about_polibase_creation_archived_db_dumb_complete(
-            size: int,
+            size: int, save: bool = True
         ) -> None:
-            PIH.EVENT.send(Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE, size)
+            event: Events = Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE
+            PIH.EVENT.send(
+                event, size, None if save else PIH.DATA.EVENT.remove_save_flag(event)
+            )
 
         @staticmethod
         def backup_notify_about_polibase_coping_archived_db_dumb_start(
             destination: str,
         ) -> None:
             PIH.EVENT.send(
                 Events.POLIBASE_COPING_ARCHIVED_DB_DUMP_START, (destination,)
@@ -5743,14 +5753,21 @@
         StringTool,
         ListTool,
         DateTimeTool,
         EnumTool,
         FullNameTool,
         ServiceRoleTool,
     ):
+
+        class EVENT:
+
+            @staticmethod
+            def remove_save_flag(value: Events) -> int:
+                return BM.remove(EnumTool.get(value).flags, LogMessageFlags.SAVE)
+
         class JOURNAL:
             @staticmethod
             def type_by_any(
                 value: str | int | None, full_equaliment: bool = True
             ) -> list[JournalType] | None:
                 result: list[JournalType] = []
                 if n(value):
@@ -10317,33 +10334,35 @@
                 return False
 
         class EMAIL:
             @staticmethod
             def accessability(
                 value: str,
                 cached: bool = True,
-                verification_method: EmailVerificationMethods | None = None
+                verification_method: EmailVerificationMethods | None = None,
             ) -> bool:
                 def internal_accessability(
                     value: str, verification_method: EmailVerificationMethods
                 ) -> bool:
                     domain: str = value.split(EMAIL_SPLITTER)[1]
                     if domain == "icloud.com":
                         verification_method = EmailVerificationMethods.NORMAL
                     return DataTool.rpc_unrepresent(
                         PIH.SERVICE.call_command(
                             ServiceCommands.check_email_accessibility,
                             (value, verification_method, cached),
                         )
                     )
 
-                #if not internal_accessability(value, verification_method):
-                verification_method = verification_method or EmailVerificationMethods.DEFAULT
+                # if not internal_accessability(value, verification_method):
+                verification_method = (
+                    verification_method or EmailVerificationMethods.DEFAULT
+                )
                 return internal_accessability(value, verification_method)
-                #return True
+                # return True
 
         class FILE:
             @staticmethod
             def excel_file(path: str) -> bool:
                 return os.path.isfile(path) and PathTool.get_extension(path) in [
                     FILE.EXTENSION.EXCEL_OLD,
                     FILE.EXTENSION.EXCEL_NEW,
@@ -12802,19 +12821,20 @@
                         (value, person.pin, test),
                     )
                 )
 
             class DB:
                 @staticmethod
                 def backup(
-                    dump_file_name: str | None = None, test: bool | None = None
+                    dump_file_name: str | None = None,
+                    test: bool | None = None,
                 ) -> bool:
                     PIH.SERVICE.call_command(
                         ServiceCommands.create_polibase_database_backup,
-                        (dump_file_name, test),
+                        (dump_file_name, test,),
                     )
                     return True
 
             class VISIT:
                 class DATA_STORAGE:
                     @staticmethod
                     def update(value: PolibasePersonVisitDS) -> bool:
```

### Comparing `pih-0.32/pih/rpc/__init__.py` & `pih-0.33/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.33/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.33/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/tools/__init__.py` & `pih-0.33/pih/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1310,15 +1310,15 @@
 
     
     @staticmethod
     def path(value: str) -> str:
         return value.replace("\\", "/")
 
     @staticmethod
-    def adapt_for_windows(value: str) -> str:
+    def for_windows(value: str) -> str:
         separator: str = "\\"
         value = value.replace("/", separator)
         if value.find(":") == -1 and not value.startswith(separator * 2):
             value = j((separator*2, value))
         return value
 
     @staticmethod
```

### Comparing `pih-0.32/pih/tools/service.py` & `pih-0.33/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih/widgets.py` & `pih-0.33/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.32/pih.egg-info/SOURCES.txt` & `pih-0.33/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

