# Comparing `tmp/toolforge_builds_cli-0.0.8.tar.gz` & `tmp/toolforge_builds_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge_builds_cli-0.0.8.tar", max compression
+gzip compressed data, was "toolforge_builds_cli-0.0.9.tar", max compression
```

## Comparing `toolforge_builds_cli-0.0.8.tar` & `toolforge_builds_cli-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35121 2023-12-08 10:28:04.017129 toolforge_builds_cli-0.0.8/LICENSE
--rw-r--r--   0        0        0     1162 2023-12-08 10:28:04.021129 toolforge_builds_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-08 10:28:04.053130 toolforge_builds_cli-0.0.8/toolforge_builds_cli/__init__.py
--rw-r--r--   0        0        0     2681 2023-12-08 10:28:04.021129 toolforge_builds_cli-0.0.8/toolforge_builds_cli/build.py
--rw-r--r--   0        0        0    13874 2023-12-08 10:28:04.021129 toolforge_builds_cli-0.0.8/toolforge_builds_cli/cli.py
--rw-r--r--   0        0        0     1434 2023-12-08 10:28:04.021129 toolforge_builds_cli-0.0.8/toolforge_builds_cli/config.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 toolforge_builds_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35121 2023-12-13 13:46:08.430377 toolforge_builds_cli-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1162 2023-12-13 13:46:08.434377 toolforge_builds_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-13 13:46:08.466377 toolforge_builds_cli-0.0.9/toolforge_builds_cli/__init__.py
+-rw-r--r--   0        0        0     2681 2023-12-13 13:46:08.434377 toolforge_builds_cli-0.0.9/toolforge_builds_cli/build.py
+-rw-r--r--   0        0        0    14680 2023-12-13 13:46:08.434377 toolforge_builds_cli-0.0.9/toolforge_builds_cli/cli.py
+-rw-r--r--   0        0        0     1434 2023-12-13 13:46:08.434377 toolforge_builds_cli-0.0.9/toolforge_builds_cli/config.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 toolforge_builds_cli-0.0.9/PKG-INFO
```

### Comparing `toolforge_builds_cli-0.0.8/LICENSE` & `toolforge_builds_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge_builds_cli-0.0.8/pyproject.toml` & `toolforge_builds_cli-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolforge-builds-cli"
-version = "0.0.8"
+version = "0.0.9"
 description = "Toolforge Build client"
 authors = ["David Caro <dcaro@wikimedia.org>", "Raymond Ndibe <rolisaemeka-ctr@wikimedia.org>"]
 license = "GPLv3"
 homepage = "https://gitlab.wikimedia.org/repos/cloud/toolforge/toolforge-builds-cli"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `toolforge_builds_cli-0.0.8/toolforge_builds_cli/build.py` & `toolforge_builds_cli-0.0.9/toolforge_builds_cli/build.py`

 * *Files identical despite different names*

### Comparing `toolforge_builds_cli-0.0.8/toolforge_builds_cli/cli.py` & `toolforge_builds_cli-0.0.9/toolforge_builds_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,52 +62,59 @@
     return ctx.obj["config"]
 
 
 def _format_build(build: Dict[str, Any]) -> Dict[str, Any]:
     start_time = build["start_time"] if build["start_time"] else "N/A"
     end_time = build["end_time"] if build["end_time"] else "N/A"
     ref = build["parameters"]["ref"] if build["parameters"]["ref"] else "N/A"
+    if build["parameters"].get("envvars"):
+        envvars = [f"{name}={value}" for name, value in build["parameters"]["envvars"].items()]
+    else:
+        envvars = ["N/A"]
     status = build["status"].split("_")[1].lower()
     if status == "success":
         status = "ok"
     elif status == "failure":
         status = "error"
 
     return {
         "build_id": build["build_id"],
         "start_time": start_time,
         "end_time": end_time,
         "status": status,
         "message": build["message"],
         "ref": ref,
+        "envvars": envvars,
         "source_url": build["parameters"]["source_url"],
         "destination_image": build["destination_image"],
     }
 
 
 def _builds_to_table(builds: List[Dict[str, Any]]) -> List[Any]:
     headers = [
         "build_id",
         "status",
         "start_time",
         "end_time",
         "source_url",
         "ref",
+        "envvars",
         "destination_image",
     ]
     headers = [click.style(header, bold=True) for header in headers]
     builds_values = []
     for build in builds:
         build_values = [
             build["build_id"],
             STATUS_STYLE[build["status"]],
             build["start_time"],
             build["end_time"],
             build["source_url"],
             build["ref"],
+            "\n".join(build["envvars"]),
             build["destination_image"],
         ]
         builds_values.append(build_values)
     return [headers, builds_values]
 
 
 def _get_formatted_build_str(build: Dict[str, Any]) -> str:
@@ -116,14 +123,16 @@
     build_str += f"{click.style('Start Time:', bold=True)} {build['start_time']}\n"
     build_str += f"{click.style('End Time:', bold=True)} {build['end_time']}\n"
     build_str += f"{click.style('Status:', bold=True)} {STATUS_STYLE[build['status']]}\n"
     build_str += f"{click.style('Message:', bold=True)} {build['message']}\n"
     build_str += click.style("Parameters:\n", bold=True)
     build_str += f"    {click.style('Source URL:', bold=True)} {build['source_url']}\n"
     build_str += f"    {click.style('Ref:', bold=True)} {build['ref']}\n"
+    envvars = "\n             ".join(build["envvars"])
+    build_str += f"    {click.style('Envvars:', bold=True)} {envvars}\n"
     build_str += f"{click.style('Destination Image:', bold=True)} {build['destination_image']}"
 
     return build_str
 
 
 @click.version_option(prog_name="Toolforge Builds CLI")
 @click.group(name="build", help="Toolforge build command line")
@@ -157,44 +166,55 @@
 @click.option(
     "--ref",
     help="Branch, tag or commit to build, by default will use the HEAD of the given repository.",
     show_default=True,
 )
 @click.option("-i", "--image-name", help="Name of the image to be built, by default will be the name of the tool.")
 @click.option(
+    "envvars",
+    "-e",
+    "--envvar",
+    help="Environment variable and value to set during build (format `NAME=value`)",
+    multiple=True,
+)
+@click.option(
     "--json",
     help="If set, will output in json format",
     is_flag=True,
 )
 @click.option("--detach", "-D", help="If set, will not stream build logs automatically", is_flag=True)
 @click.pass_context
 def build_start(
     ctx: click.Context,
     source_git_url: str,
     ref: Optional[str] = None,
     image_name: Optional[str] = None,
     json: bool = False,
     detach: bool = False,
+    envvars: Optional[List[str]] = None,
 ) -> None:
     if not source_git_url:
         message = (
             f"{click.style('Error:', bold=True, fg='red')} Please provide a git url for your source code.\n"
             + f"{click.style('Example:', bold=True)}"
             + " toolforge build start 'https://gitlab.wikimedia.org/toolforge-repos/my-tool'"
         )
         click.echo(message)
         sys.exit(1)
 
     config = _load_config_from_ctx()
     build_client = BuildClient.from_config(config=config)
-    data = {"source_url": source_git_url}
+    data: dict[str, Any] = {"source_url": source_git_url}
     if ref:
         data["ref"] = ref
     if image_name:
         data["image_name"] = image_name
+    if envvars:
+        # validation is done at the API, no need to duplicate logic
+        data["envvars"] = {envvar_str.split("=", 1)[0]: envvar_str.split("=", 1)[-1] for envvar_str in envvars}
 
     new_build = build_client.post("/build", json=data)
 
     if not detach:
         return ctx.invoke(build_logs, build_name=new_build["name"], follow=True)
 
     if json:
```

### Comparing `toolforge_builds_cli-0.0.8/toolforge_builds_cli/config.py` & `toolforge_builds_cli-0.0.9/toolforge_builds_cli/config.py`

 * *Files identical despite different names*

### Comparing `toolforge_builds_cli-0.0.8/PKG-INFO` & `toolforge_builds_cli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-builds-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolforge Build client
 Home-page: https://gitlab.wikimedia.org/repos/cloud/toolforge/toolforge-builds-cli
 License: GPLv3
 Author: David Caro
 Author-email: dcaro@wikimedia.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

