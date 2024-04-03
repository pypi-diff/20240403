# Comparing `tmp/octostar_streamlit-0.1.3.tar.gz` & `tmp/octostar_streamlit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit-0.1.3.tar", max compression
+gzip compressed data, was "octostar_streamlit-0.1.4.tar", max compression
```

## Comparing `octostar_streamlit-0.1.3.tar` & `octostar_streamlit-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1074 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/LICENSE
--rw-r--r--   0        0        0      324 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/README.md
--rw-r--r--   0        0        0     1884 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/desktop/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/desktop/method_call.py
--rw-r--r--   0        0        0     7821 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/desktop/params.py
--rw-r--r--   0        0        0     6134 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/entities.py
--rw-r--r--   0        0        0      281 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/method_call.py
--rw-r--r--   0        0        0        0 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/ontology/__init__.py
--rw-r--r--   0        0        0      673 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/ontology/method_call.py
--rw-r--r--   0        0        0     1766 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/ontology/params.py
--rw-r--r--   0        0        0      222 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/params_base_model.py
--rw-r--r--   0        0        0      867 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/core/streamlit_executor.py
--rw-r--r--   0        0        0    10049 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/desktop.py
--rw-r--r--   0        0        0      253 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/.gitignore
--rw-r--r--   0        0        0      357 2024-04-03 15:34:45.491160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/index.html
--rw-r--r--   0        0        0    42450 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/package-lock.json
--rw-r--r--   0        0        0      413 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/package.json
--rw-r--r--   0        0        0     1497 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/public/vite.svg
--rw-r--r--   0        0        0      835 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/core.ts
--rw-r--r--   0        0        0    15318 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/desktop.ts
--rw-r--r--   0        0        0     2373 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/main.ts
--rw-r--r--   0        0        0     4177 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/ontology.ts
--rw-r--r--   0        0        0       38 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      527 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/frontend/tsconfig.json
--rw-r--r--   0        0        0      396 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/main.py
--rw-r--r--   0        0        0     3984 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/octostar_streamlit/ontology.py
--rw-r--r--   0        0        0      677 2024-04-03 15:34:45.495160 octostar_streamlit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/LICENSE
+-rw-r--r--   0        0        0      324 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/README.md
+-rw-r--r--   0        0        0     1948 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/desktop/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/desktop/method_call.py
+-rw-r--r--   0        0        0     7821 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/desktop/params.py
+-rw-r--r--   0        0        0     6134 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/entities.py
+-rw-r--r--   0        0        0      281 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/method_call.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/ontology/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/ontology/method_call.py
+-rw-r--r--   0        0        0     1766 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/ontology/params.py
+-rw-r--r--   0        0        0      222 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/params_base_model.py
+-rw-r--r--   0        0        0      867 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/core/streamlit_executor.py
+-rw-r--r--   0        0        0    10049 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/desktop.py
+-rw-r--r--   0        0        0      253 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/.gitignore
+-rw-r--r--   0        0        0      356 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/index.html
+-rw-r--r--   0        0        0    42450 2024-04-03 16:26:28.999745 octostar_streamlit-0.1.4/octostar_streamlit/frontend/package-lock.json
+-rw-r--r--   0        0        0      413 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/package.json
+-rw-r--r--   0        0        0     1497 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/public/vite.svg
+-rw-r--r--   0        0        0      835 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/core.ts
+-rw-r--r--   0        0        0    14114 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/desktop.ts
+-rw-r--r--   0        0        0     2373 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/main.ts
+-rw-r--r--   0        0        0     4166 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/ontology.ts
+-rw-r--r--   0        0        0       38 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      527 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/tsconfig.json
+-rw-r--r--   0        0        0       86 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/frontend/vite.config.ts
+-rw-r--r--   0        0        0     3984 2024-04-03 16:26:09.767471 octostar_streamlit-0.1.4/octostar_streamlit/ontology.py
+-rw-r--r--   0        0        0      677 2024-04-03 16:26:09.771471 octostar_streamlit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.4/PKG-INFO
```

### Comparing `octostar_streamlit-0.1.3/LICENSE` & `octostar_streamlit-0.1.4/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Oleksandr Korzhov
+Copyright (c) 2024 Octostar Limited
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/__init__.py` & `octostar_streamlit-0.1.4/octostar_streamlit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import streamlit.components.v1 as components
 
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = os.environ.get("OCTOSTAR_STREAMLIT_RELEASE", "false").lower() == "true"
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
 # It's worth noting that this call to `declare_component` is the
 # *only thing* you need to do to create the binding between Streamlit and
 # your component frontend. Everything else we do in this file is simply a
 # best practice.
-component_name = "octostar_streamlit_communication_bridge"
+component_name = "octostar_streamlit_comunication_bridge"
 
 if not _RELEASE:
     _component_func = components.declare_component(
         # We give the component a simple, descriptive name ("my_component"
         # does not fit this bill, so please choose something better for your
         # own component :)
         component_name,
@@ -32,9 +32,9 @@
         url="http://localhost:5173",
     )
 else:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend/build")
+    build_dir = os.path.join(parent_dir, "frontend/dist")
     _component_func = components.declare_component(component_name, path=build_dir)
```

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/desktop/method_call.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/desktop/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/desktop/params.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/desktop/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/entities.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/entities.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/ontology/method_call.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/ontology/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/ontology/params.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/ontology/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/core/streamlit_executor.py` & `octostar_streamlit-0.1.4/octostar_streamlit/core/streamlit_executor.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/desktop.py` & `octostar_streamlit-0.1.4/octostar_streamlit/desktop.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/package-lock.json` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/public/vite.svg` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/core.ts` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/core.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/desktop.ts` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/desktop.ts`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,23 @@
   Desktop,
   DesktopActionOptions,
   DesktopStylerContext,
   Entity,
   ExportOptions,
   FileTreeOptions,
   GetAttachmentOptions,
-  GraphSpec,
   IDataTransfer,
   ImportZipOptions,
   OsTag,
   Relationship,
   SaveOptions,
   TagAttributes,
   TagInfo,
   Watcher,
-  Workspace,
   WorkspaceItem,
-  WorkspaceItemIdentifier,
   WorkspacePermissionValue,
   WorkspaceRecordIdentifier,
   WorkspaceRecordInfo,
   WorkspaceRecordWithRelationships,
 } from "@octostar/platform-types";
 import {
   MethodCallDef,
@@ -41,70 +38,14 @@
   "desktop",
   M,
   P
 >;
 
 type InternalWorkspaceItemIdentifier = { id: string } | WorkspaceItem;
 
-type RefreshMethodCall = DesktopApiMethodCall<"refresh", never>;
-
-type OpenWorkspaceMethodCall = DesktopApiMethodCall<
-  "openWorkspace",
-  InternalWorkspaceItemIdentifier
->;
-
-type GetActiveWorkspaceMethodCall = DesktopApiMethodCall<
-  "getActiveWorkspace",
-  {
-    prompt: boolean;
-  }
->;
-
-// TODO: seems this method deviates from the baseline of other methods for working with worksapce
-type SetActiveWorkspaceMethodCall = DesktopApiMethodCall<
-  "setActiveWorkspace",
-  { id: string }
->;
-
-type CloseWorkspaceMethodCall = DesktopApiMethodCall<
-  "closeWorkspace",
-  InternalWorkspaceItemIdentifier
->;
-
-type CopyMethodCall = DesktopApiMethodCall<
-  "copy",
-  {
-    source: WorkspaceItem;
-    target: WorkspaceItem;
-  }
->;
-
-type ListWorkspacesMethodCall = DesktopApiMethodCall<
-  "listAllWorkspaces",
-  never
->;
-
-type GetOpenWorkspacesMethodCall = DesktopApiMethodCall<
-  "getOpenWorkspaces",
-  never
->;
-
-type GetAttachmentMethodCall = DesktopApiMethodCall<
-  "getAttachment",
-  {
-    entity: Entity;
-    options?: GetAttachmentOptions<AttachmentType>;
-  }
->;
-
-type GetStylerOptionsMethodCall = DesktopApiMethodCall<
-  "getStylerOptions",
-  never
->;
-
 type BridgedDesktop = Omit<
   Desktop,
   | "withProgressBar"
   | "getPasteContext"
   | "showModalTemplate"
   | "getOpenWorkspaceIds"
   | "setOpenWorkspaceIds"
```

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/main.ts` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/src/ontology.ts` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/src/ontology.ts`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             lowPriority: noneToUndefined(params.options.low_priority),
           }
     );
   },
   getSysInheritance: function (): Promise<Inheritance[]> {
     return ontologyApi().getSysInheritance();
   },
-  subscribe: function (params: any): Promise<Unsubscribe> {
+  subscribe: function (): Promise<Unsubscribe> {
     throw new Error("Function not implemented.");
   },
   consistentUUID: function (params: {
     name: string;
     namespace: string | None;
   }): Promise<string> {
     return ontologyApi().consistentUUID(
```

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/frontend/tsconfig.json` & `octostar_streamlit-0.1.4/octostar_streamlit/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/octostar_streamlit/ontology.py` & `octostar_streamlit-0.1.4/octostar_streamlit/ontology.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.3/pyproject.toml` & `octostar_streamlit-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octostar-streamlit"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 license = "MIT"
 authors = ["Oleksandr Korzhov <another.fullstack.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.mypy]
 python_version = ">=3.9,<3.9.7 || >3.9.7,<4.0"
```

### Comparing `octostar_streamlit-0.1.3/PKG-INFO` & `octostar_streamlit-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Oleksandr Korzhov
 Author-email: another.fullstack.dev@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

