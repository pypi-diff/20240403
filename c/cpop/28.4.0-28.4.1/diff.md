# Comparing `tmp/cpop-28.4.0.tar.gz` & `tmp/cpop-28.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.4.0.tar", last modified: Wed Apr  3 06:25:08 2024, max compression
+gzip compressed data, was "cpop-28.4.1.tar", last modified: Wed Apr  3 15:28:43 2024, max compression
```

## Comparing `cpop-28.4.0.tar` & `cpop-28.4.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.123296 cpop-28.4.0/
--rw-r--r--   0 akmod     (1000) akmod     (1001)    11348 2024-03-24 19:10:42.000000 cpop-28.4.0/LICENSE
--rw-r--r--   0 akmod     (1000) akmod     (1001)      111 2024-04-03 00:52:36.000000 cpop-28.4.0/MANIFEST.in
--rw-r--r--   0 akmod     (1000) akmod     (1001)     4996 2024-04-03 06:25:08.123296 cpop-28.4.0/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1001)     4411 2024-04-02 01:31:22.000000 cpop-28.4.0/README.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.119962 cpop-28.4.0/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1001)     4996 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1001)      535 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/SOURCES.txt
--rw-r--r--   0 akmod     (1000) akmod     (1001)        1 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/dependency_links.txt
--rw-r--r--   0 akmod     (1000) akmod     (1001)       42 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/entry_points.txt
--rw-r--r--   0 akmod     (1000) akmod     (1001)      128 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/requires.txt
--rw-r--r--   0 akmod     (1000) akmod     (1001)        8 2024-04-03 06:25:08.000000 cpop-28.4.0/cpop.egg-info/top_level.txt
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.119962 cpop-28.4.0/hub/
--rw-r--r--   0 akmod     (1000) akmod     (1001)        0 2024-04-02 01:31:22.000000 cpop-28.4.0/hub/__init__.py
--rwxr-xr-x   0 akmod     (1000) akmod     (1001)     4277 2024-04-03 06:23:16.000000 cpop-28.4.0/hub/__main__.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.123296 cpop-28.4.0/pop/
--rw-r--r--   0 akmod     (1000) akmod     (1001)     2465 2024-04-03 03:10:06.000000 cpop-28.4.0/pop/config.yaml
--rw-r--r--   0 akmod     (1000) akmod     (1001)    10479 2024-04-02 03:55:01.000000 cpop-28.4.0/pop/contract.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     4417 2024-04-02 03:49:55.000000 cpop-28.4.0/pop/dirs.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     1573 2024-03-24 19:10:42.000000 cpop-28.4.0/pop/exc.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)    23470 2024-04-03 02:51:14.000000 cpop-28.4.0/pop/hub.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)    11349 2024-04-03 00:52:34.000000 cpop-28.4.0/pop/loader.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.123296 cpop-28.4.0/pop/log/
--rw-r--r--   0 akmod     (1000) akmod     (1001)     5219 2024-04-02 06:29:03.000000 cpop-28.4.0/pop/log/async.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.119962 cpop-28.4.0/pop/mods/
-drwxr-xr-x   0 akmod     (1000) akmod     (1001)        0 2024-04-03 06:25:08.123296 cpop-28.4.0/pop/mods/pop/
--rw-r--r--   0 akmod     (1000) akmod     (1001)    10500 2024-04-03 06:22:41.000000 cpop-28.4.0/pop/mods/pop/config.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)      570 2024-03-29 03:49:42.000000 cpop-28.4.0/pop/mods/pop/contract.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)      234 2024-03-27 21:35:46.000000 cpop-28.4.0/pop/mods/pop/dyne.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     6993 2024-04-02 01:31:22.000000 cpop-28.4.0/pop/mods/pop/sub.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)      861 2024-04-02 01:31:22.000000 cpop-28.4.0/pop/mods/pop/test.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)   878343 2024-04-03 06:25:08.000000 cpop-28.4.0/pop/pop.data.c
--rw-r--r--   0 akmod     (1000) akmod     (1001)     6101 2024-04-02 01:31:22.000000 cpop-28.4.0/pop/pop.data.pyx
--rw-r--r--   0 akmod     (1000) akmod     (1001)      555 2024-04-02 01:31:22.000000 cpop-28.4.0/pop/ref.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     1176 2024-04-02 03:50:19.000000 cpop-28.4.0/pop/scanner.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     7642 2024-03-26 00:13:31.000000 cpop-28.4.0/pop/verify.py
--rw-r--r--   0 akmod     (1000) akmod     (1001)     1315 2024-04-03 03:04:24.000000 cpop-28.4.0/pyproject.toml
--rw-r--r--   0 akmod     (1000) akmod     (1001)       38 2024-04-03 06:25:08.123296 cpop-28.4.0/setup.cfg
--rw-r--r--   0 akmod     (1000) akmod     (1001)     1263 2024-04-02 01:31:22.000000 cpop-28.4.0/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.414366 cpop-28.4.1/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.4.1/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      111 2024-04-03 15:09:20.000000 cpop-28.4.1/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-03 15:28:43.414366 cpop-28.4.1/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.4.1/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.410366 cpop-28.4.1/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-03 15:28:43.000000 cpop-28.4.1/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.410366 cpop-28.4.1/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.4.1/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     4277 2024-04-03 15:09:20.000000 cpop-28.4.1/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.414366 cpop-28.4.1/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2465 2024-04-03 15:09:20.000000 cpop-28.4.1/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.4.1/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.4.1/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.4.1/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.4.1/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    23470 2024-04-02 21:09:20.000000 cpop-28.4.1/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11349 2024-04-02 21:09:20.000000 cpop-28.4.1/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.414366 cpop-28.4.1/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.4.1/pop/log/async.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.410366 cpop-28.4.1/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-03 15:28:43.414366 cpop-28.4.1/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7501 2024-04-03 15:16:56.000000 cpop-28.4.1/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.4.1/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.4.1/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.4.1/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.4.1/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-03 15:28:25.000000 cpop-28.4.1/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-02 20:52:24.000000 cpop-28.4.1/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.4.1/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.4.1/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.4.1/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-03 15:27:53.000000 cpop-28.4.1/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-03 15:28:43.414366 cpop-28.4.1/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.4.1/setup.py
```

### Comparing `cpop-28.4.0/LICENSE` & `cpop-28.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/PKG-INFO` & `cpop-28.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.4.0
+Version: 28.4.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.4.0/README.rst` & `cpop-28.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/cpop.egg-info/PKG-INFO` & `cpop-28.4.1/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.4.0
+Version: 28.4.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.4.0/cpop.egg-info/SOURCES.txt` & `cpop-28.4.1/cpop.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 cpop.egg-info/entry_points.txt
 cpop.egg-info/requires.txt
 cpop.egg-info/top_level.txt
 hub/__init__.py
 hub/__main__.py
 pop/config.yaml
 pop/contract.py
+pop/data.c
 pop/dirs.py
 pop/exc.py
 pop/hub.py
 pop/loader.py
 pop/pop.data.c
 pop/pop.data.pyx
 pop/ref.py
```

### Comparing `cpop-28.4.0/hub/__main__.py` & `cpop-28.4.1/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/config.yaml` & `cpop-28.4.1/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/contract.py` & `cpop-28.4.1/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/dirs.py` & `cpop-28.4.1/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/exc.py` & `cpop-28.4.1/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/hub.py` & `cpop-28.4.1/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/loader.py` & `cpop-28.4.1/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/log/async.py` & `cpop-28.4.1/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/mods/pop/config.py` & `cpop-28.4.1/pop/mods/pop/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -95,100 +95,14 @@
     if not cli:
         return {}
 
     # Create the main parser for the CLI
     parser = hub.lib.argparse.ArgumentParser(
         description=f"{cli.title().replace('_', ' ')} CLI Parser"
     )
-
-    # Initialize subparsers
-    sparser = parser.add_subparsers(dest="SUBPARSER")
-    subparsers = {
-        subcommand: sparser.add_parser(
-            subcommand,
-            description=f"{cli.title().replace('_', ' ')} {subcommand.title().replace('_', ' ')} CLI Parser",
-            **opts,
-        )
-        for subcommand, opts in subcommands.items()
-    }
-
-    # Initialize groups for organizing arguments
-    groups = {}
-    subparser_groups = {subcommand: {} for subcommand in subparsers}
-
-    # Add CLI options to the parser
-    for name, opts in active_cli.items():
-        opts = opts.copy()
-        positional = opts.pop("positional", False)
-        cli_name = name if positional else f"--{name.lower().replace('_', '-')}"
-
-        # If choices is a string then assume it is a referenc eon the hub
-        choices = opts.pop("choices", ())
-        if isinstance(choices, str):
-            opts["choices"] = tuple(hub[choices]._loaded.keys())
-
-        # Pass a list of possible options for each cli
-        options = opts.pop("options", [])
-
-        # Determine the target group for the argument
-        group_name = opts.pop("group", None)
-        target_group = (
-            groups.setdefault(group_name, parser.add_argument_group(group_name))
-            if group_name
-            else parser
-        )
-
-        # Add the argument to the top-level parser if it's global or has no subcommands
-        arg_subparsers = opts.pop("subcommands", [])
-        if "__global__" in arg_subparsers or not arg_subparsers:
-            target_group.add_argument(cli_name, *options, **opts)
-
-        # Add the argument to the specified subparsers
-        for subcommand in arg_subparsers:
-            if subcommand in subparsers:
-                subparser_group = (
-                    subparser_groups[subcommand].setdefault(
-                        group_name,
-                        subparsers[subcommand].add_argument_group(group_name),
-                    )
-                    if group_name
-                    else subparsers[subcommand]
-                )
-                subparser_group.add_argument(cli_name, *options, **opts)
-
-    # Parse the CLI arguments and return them as a NamespaceDict
-    return pop.data.NamespaceDict(parser.parse_args(args=parser_args).__dict__)
-
-
-async def parse_cli(
-    hub,
-    cli: str,
-    active_cli: dict[str, object],
-    subcommands: dict[str, object],
-    parser_args: tuple = None,
-) -> dict[str, object]:
-    """
-    Create a parser and parse all the CLI options.
-
-    Args:
-        hub: The POP hub instance.
-        cli (str): The name of the CLI being parsed.
-        active_cli (dict): The active CLI configuration.
-        subcommands (dict): The subcommands configuration.
-
-    Returns:
-        argparse.Namespace: The parsed CLI options.
-    """
-    if not cli:
-        return {}
-
-    # Create the main parser for the CLI
-    parser = hub.lib.argparse.ArgumentParser(
-        description=f"{cli.title().replace('_', ' ')} CLI Parser"
-    )
     sparser = None
     subparsers = {}
 
     # Add subcommands to the parser
     for subcommand, opts in subcommands.items():
         if sparser is None:
             sparser = parser.add_subparsers(dest="SUBPARSER")
```

### Comparing `cpop-28.4.0/pop/mods/pop/contract.py` & `cpop-28.4.1/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/mods/pop/sub.py` & `cpop-28.4.1/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/mods/pop/test.py` & `cpop-28.4.1/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/pop.data.c` & `cpop-28.4.1/pop/pop.data.c`

 * *Files 0% similar despite different names*

```diff
@@ -1498,19 +1498,19 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "pop/pop.data.pyx",
-  ".venv/lib/python3.11/site-packages/Cython/Includes/cpython/contextvars.pxd",
+  "contextvars.pxd",
   "<stringsource>",
-  ".venv/lib/python3.11/site-packages/Cython/Includes/cpython/type.pxd",
-  ".venv/lib/python3.11/site-packages/Cython/Includes/cpython/bool.pxd",
-  ".venv/lib/python3.11/site-packages/Cython/Includes/cpython/complex.pxd",
+  "type.pxd",
+  "bool.pxd",
+  "complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
```

### Comparing `cpop-28.4.0/pop/pop.data.pyx` & `cpop-28.4.1/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/ref.py` & `cpop-28.4.1/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/scanner.py` & `cpop-28.4.1/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pop/verify.py` & `cpop-28.4.1/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.4.0/pyproject.toml` & `cpop-28.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.4.0"
+version = "28.4.1"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-28.4.0/setup.py` & `cpop-28.4.1/setup.py`

 * *Files identical despite different names*

