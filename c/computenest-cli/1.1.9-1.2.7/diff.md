# Comparing `tmp/computenest-cli-1.1.9.tar.gz` & `tmp/computenest-cli-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computenest-cli-1.1.9.tar", last modified: Tue Nov 14 03:45:06 2023, max compression
+gzip compressed data, was "computenest-cli-1.2.7.tar", last modified: Wed Apr  3 03:29:30 2024, max compression
```

## Comparing `computenest-cli-1.1.9.tar` & `computenest-cli-1.2.7.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.024255 computenest-cli-1.1.9/
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2023-11-14 03:45:06.023571 computenest-cli-1.1.9/PKG-INFO
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1669 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/README.md
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.007264 computenest-cli-1.1.9/computeNestSupplier/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     2838 2023-11-10 08:40:19.000000 computenest-cli-1.1.9/computeNestSupplier/main.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.007845 computenest-cli-1.1.9/computeNestSupplier/service_supplier/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/__init__.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.012993 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     7524 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/artifact_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      418 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/base_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      760 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/compute_nest_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      491 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/ecs_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     3171 2023-11-07 03:02:42.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/image_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)      492 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/oos_client.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     5707 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/service_client.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.015900 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1713 2023-11-10 08:40:19.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/constant.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1268 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/credentials.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     3027 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/file.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     2102 2023-11-10 08:40:19.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/util.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.018398 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/
--rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2023-10-23 13:35:01.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/__init__.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)    17935 2023-11-07 02:55:30.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/artifact_processor.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     3899 2023-10-25 01:49:49.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/check_processor.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)     6843 2023-11-07 02:55:30.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/image_processor.py
--rw-r--r--   0 xuhaoran   (502) staff       (20)    20568 2023-11-14 03:14:41.000000 computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/service_processor.py
-drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2023-11-14 03:45:06.022627 computenest-cli-1.1.9/computenest_cli.egg-info/
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/PKG-INFO
--rw-r--r--   0 xuhaoran   (502) staff       (20)     1449 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/SOURCES.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)        1 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/dependency_links.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)       66 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/entry_points.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)      216 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/requires.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)       20 2023-11-14 03:45:05.000000 computenest-cli-1.1.9/computenest_cli.egg-info/top_level.txt
--rw-r--r--   0 xuhaoran   (502) staff       (20)       38 2023-11-14 03:45:06.024430 computenest-cli-1.1.9/setup.cfg
--rw-r--r--   0 xuhaoran   (502) staff       (20)      788 2023-11-14 03:11:25.000000 computenest-cli-1.1.9/setup.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.038373 computenest-cli-1.2.7/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-04-03 03:29:30.037793 computenest-cli-1.2.7/PKG-INFO
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1669 2024-03-08 01:57:25.000000 computenest-cli-1.2.7/README.md
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.017685 computenest-cli-1.2.7/computenest_cli.egg-info/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1916 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/PKG-INFO
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1116 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        1 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       61 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/entry_points.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      230 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/requires.txt
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       15 2024-04-03 03:29:29.000000 computenest-cli-1.2.7/computenest_cli.egg-info/top_level.txt
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.018772 computenest-cli-1.2.7/computenestcli/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/__init__.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.022084 computenest-cli-1.2.7/computenestcli/client/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      418 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/base.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      785 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/computenest.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/ecs.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      525 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/client/oos.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.026754 computenest-cli-1.2.7/computenestcli/common/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1753 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/constant.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      146 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/context.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      236 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/credentials.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      670 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/decorator.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2102 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/common/util.py
+-rwxr-xr-x   0 xuhaoran   (502) staff       (20)     4130 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/main.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.031852 computenest-cli-1.2.7/computenestcli/processor/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)    17199 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/artifact.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     4448 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/check.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     6753 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/image.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2197 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/jinja2.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)    20467 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/processor/service.py
+drwxr-xr-x   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:29:30.036727 computenest-cli-1.2.7/computenestcli/service/
+-rw-r--r--   0 xuhaoran   (502) staff       (20)        0 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/__init__.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     8354 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/artifact.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      606 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/base.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     1002 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/credentials.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     2903 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/file.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     3253 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/image.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)     5508 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/computenestcli/service/supplier.py
+-rw-r--r--   0 xuhaoran   (502) staff       (20)       38 2024-04-03 03:29:30.038510 computenest-cli-1.2.7/setup.cfg
+-rw-r--r--   0 xuhaoran   (502) staff       (20)      783 2024-04-03 03:28:56.000000 computenest-cli-1.2.7/setup.py
```

### Comparing `computenest-cli-1.1.9/PKG-INFO` & `computenest-cli-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computenest-cli
-Version: 1.1.9
+Version: 1.2.7
 Summary: A command line interface for running the compute nest project
 Home-page: 
 Author: Chuan Lin
 Author-email: zhaoshuaibo.zsb@alibaba-inc.com
 Description-Content-Type: text/markdown
 
 # ComputeNest-CLI
```

### Comparing `computenest-cli-1.1.9/README.md` & `computenest-cli-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.1.9/computeNestSupplier/main.py` & `computenest-cli-1.2.7/computenestcli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 import json
 
 import yaml
 import click
-from computeNestSupplier.service_supplier.processor.service_processor import ServiceProcessor
-from computeNestSupplier.service_supplier.processor.check_processor import CheckProcesser
+from computenestcli.processor.service import ServiceProcessor
+from computenestcli.processor.check import CheckProcesser
+from computenestcli.processor.jinja2 import Jinja2Processor
+from computenestcli.common.context import Context
+from computenestcli.common.credentials import Credentials
 
 
 @click.group()
 def main():
     click.echo("Welcome to computenest-cli")
 
 
@@ -17,16 +20,17 @@
 @click.option('--service_name', default=None, help='Service name')
 @click.option('--version_name', default=None, help='Version name')
 @click.option('--icon', default=None, help='Icon Oss URL')
 @click.option('--desc', default=None, help='Service description')
 @click.option('--file_path', required=True, help='File path')
 @click.option('--access_key_id', required=True, help='Access Key ID')
 @click.option('--access_key_secret', required=True, help='Access Key Secret')
-@click.option('--parameters', default='{}', help='parameters')
-def import_command(update_artifact, service_name, version_name, icon, desc, file_path, access_key_id, access_key_secret, parameters):
+@click.option('--parameters', required=False, default='{}', help='Parameters')
+@click.option('--parameter_path', required=False, default='', help='Parameter file path, this option overrides parameters')
+def import_command(update_artifact, service_name, version_name, icon, desc, file_path, access_key_id, access_key_secret, parameters, parameter_path):
     if file_path is None:
         click.echo('Please provide the file_path')
         return
     if access_key_id is None:
         click.echo('Please provide the access_key_id')
         return
     if access_key_secret is None:
@@ -36,33 +40,56 @@
         service_name = None
     if version_name == 'None':
         version_name = None
     if icon == 'None':
         icon = None
     if desc == 'None':
         desc = None
+    if parameter_path:
+        with open(parameter_path, 'r') as stream:
+            parameter_json = yaml.load(stream, Loader=yaml.FullLoader)
+    else:
+        parameter_json = json.loads(parameters)
     with open(file_path, 'r') as stream:
         data = yaml.load(stream, Loader=yaml.FullLoader)
     region_id = data['Service']['RegionId']
-    service = ServiceProcessor(region_id, access_key_id, access_key_secret)
+    context = Context(region_id, Credentials(access_key_id, access_key_secret))
+    service = ServiceProcessor(context)
     check = CheckProcesser(data, file_path)
     check.processor()
     service.import_command(data_config=data, file_path=file_path, update_artifact=update_artifact, service_name=service_name,
-                           version_name=version_name, icon=icon, desc=desc, parameters=json.loads(parameters))
+                           version_name=version_name, icon=icon, desc=desc, parameters=parameter_json)
 
 
 @click.command(name='export')
 @click.option('--region_id', required=True, help='Region ID')
 @click.option('--service_name', required=True, help='Service name')
 @click.option('--file_path', required=True, help='File path')
 @click.option('--access_key_id', required=True, help='Access Key ID')
 @click.option('--access_key_secret', required=True, help='Access Key Secret')
 def export_command(region_id, service_name, file_path, access_key_id, access_key_secret):
-    service = ServiceProcessor(region_id, access_key_id, access_key_secret)
+    context = Context(region_id, Credentials(access_key_id, access_key_secret))
+    service = ServiceProcessor(context)
     service.export_command(service_name, file_path)
 
 
+@click.command(name='generate')
+@click.option('--file_path', required=True, help='File path')
+@click.option('--parameters', default='{}', help='Parameters')
+@click.option('--output_path', required=True, help='Output path')
+@click.option('--parameter_path', required=False, default='', help='Parameter file path, this option overrides parameters')
+def generate_command(file_path, parameters, output_path, parameter_path):
+    jinja2 = Jinja2Processor()
+    if parameter_path:
+        with open(parameter_path, 'r') as stream:
+            parameter_json = yaml.load(stream, Loader=yaml.FullLoader)
+    else:
+        parameter_json = json.loads(parameters)
+    jinja2.process(file_path, parameter_json, output_path)
+
+
 main.add_command(import_command)
 main.add_command(export_command)
+main.add_command(generate_command)
 
 if __name__ == '__main__':
     main()
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/artifact_client.py` & `computenest-cli-1.2.7/computenestcli/service/artifact.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 from alibabacloud_computenestsupplier20210521 import models as compute_nest_supplier_20210521_models
-from computeNestSupplier.service_supplier.client.compute_nest_client import ComputeNestClient
-from computeNestSupplier.service_supplier.common.util import Util
-from computeNestSupplier.service_supplier.common import constant
+from computenestcli.service.base import Service
+from computenestcli.common.util import Util
+from computenestcli.common import constant
+from computenestcli.common.decorator import retry_on_exception
 
 
-class ArtifactClient(ComputeNestClient):
+class ArtifactService(Service):
 
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        super().__init__(region_id, access_key_id, access_key_secret)
-        self.client = self.create_client_compute_nest()
-
-    def create_artifact(self, artifact_data, artifact_id=''):
+    @classmethod
+    def create_artifact(cls, context, artifact_data, artifact_id=''):
         artifact_type = artifact_data.get(constant.ARTIFACT_TYPE)
         version_name = Util.add_timestamp_to_version_name(artifact_data.get(constant.VERSION_NAME))
         supported_regions = artifact_data.get(constant.SUPPORT_REGION_IDS)
         if artifact_type == constant.ECS_IMAGE:
             artifact_property = compute_nest_supplier_20210521_models.CreateArtifactRequestArtifactProperty(
                 region_id=artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.REGION_ID),
                 image_id=artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.IMAGE_ID)
@@ -48,23 +46,27 @@
                 artifact_type=artifact_data.get(constant.ARTIFACT_TYPE),
                 name=artifact_data.get(constant.ARTIFACT_NAME),
                 version_name=version_name,
                 description=artifact_data.get(constant.DESCRIPTION),
                 artifact_property=artifact_property,
                 support_region_ids=supported_regions
             )
-        response = self.client.create_artifact(create_artifact_request)
+        client = cls._get_computenest_client(context)
+        response = client.create_artifact(create_artifact_request)
         return response
 
-    def release_artifact(self, artifact_id):
+    @classmethod
+    def release_artifact(cls, context, artifact_id):
         release_service_request = compute_nest_supplier_20210521_models.ReleaseArtifactRequest(artifact_id)
-        response = self.client.release_artifact(release_service_request)
+        client = cls._get_computenest_client(context)
+        response = client.release_artifact(release_service_request)
         return response
 
-    def update_artifact(self, artifact_data, artifact_id):
+    @classmethod
+    def update_artifact(cls, context, artifact_data, artifact_id):
         artifact_type = artifact_data.get(constant.ARTIFACT_TYPE)
         version_name = Util.add_timestamp_to_version_name(artifact_data.get(constant.VERSION_NAME))
         supported_regions = artifact_data.get(constant.SUPPORT_REGION_IDS)
         if artifact_type == constant.ECS_IMAGE:
             artifact_property = compute_nest_supplier_20210521_models.UpdateArtifactRequestArtifactProperty(
                 region_id=artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.REGION_ID),
                 image_id=artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.IMAGE_ID)
@@ -85,58 +87,77 @@
         update_artifact_request = compute_nest_supplier_20210521_models.UpdateArtifactRequest(
             artifact_id=artifact_id,
             version_name=version_name,
             description=artifact_data.get(constant.DESCRIPTION),
             artifact_property=artifact_property,
             support_region_ids=supported_regions
         )
-        response = self.client.update_artifact(update_artifact_request)
+        client = cls._get_computenest_client(context)
+        response = client.update_artifact(update_artifact_request)
         return response
 
-    def delete_artifact(self, artifact_id, artifact_version):
+    @classmethod
+    def delete_artifact(cls, context, artifact_id, artifact_version):
         delete_artifact_request = compute_nest_supplier_20210521_models.DeleteArtifactRequest(artifact_id,
                                                                                               artifact_version)
-        response = self.client.delete_artifact(delete_artifact_request)
+        client = cls._get_computenest_client(context)
+        response = client.delete_artifact(delete_artifact_request)
         return response
 
-    def list_artifact(self, artifact_name):
+    @classmethod
+    def list_artifact(cls, context, artifact_name):
         filter_first = compute_nest_supplier_20210521_models.ListArtifactsRequestFilter(
             name=constant.NAME,
             values=[artifact_name]
         )
         list_artifact_request = compute_nest_supplier_20210521_models.ListArtifactsRequest(
             filter=[
                 filter_first
             ]
         )
-        response = self.client.list_artifacts(list_artifact_request)
+        client = cls._get_computenest_client(context)
+        response = client.list_artifacts(list_artifact_request)
         return response
 
-    def list_acr_image_repositories(self, artifact_type, repo_name):
+    @classmethod
+    @retry_on_exception()
+    def list_acr_image_repositories(cls, context, artifact_type, repo_name):
+        print("list_acr_image_repositories artifact_type: %s repo_name: %s" % (artifact_type, repo_name))
         list_acr_image_repositories_request = compute_nest_supplier_20210521_models.ListAcrImageRepositoriesRequest(
             artifact_type=artifact_type,
             repo_name=repo_name
         )
-        response = self.client.list_acr_image_repositories(list_acr_image_repositories_request)
+        client = cls._get_computenest_client(context)
+        response = client.list_acr_image_repositories(list_acr_image_repositories_request)
+        print("list_acr_image_repositories response: %s" % response)
+        # 如果body不为空，且repositories数组为空的话就抛出异常
+        if response.body and not response.body.repositories:
+            raise Exception("No repositories found")
         return response
 
-    def list_acr_image_tags(self, repo_id, artifact_type):
+    @classmethod
+    def list_acr_image_tags(cls, context, repo_id, artifact_type):
         list_acr_image_tags_request = compute_nest_supplier_20210521_models.ListAcrImageTagsRequest(
             repo_id=repo_id,
             artifact_type=artifact_type
         )
-        response = self.client.list_acr_image_tags(list_acr_image_tags_request)
+        client = cls._get_computenest_client(context)
+        response = client.list_acr_image_tags(list_acr_image_tags_request)
         return response
 
-    def get_artifact(self, artifact_name, artifact_version='', artifact_id=''):
+    @classmethod
+    def get_artifact(cls, context, artifact_name, artifact_version='', artifact_id=''):
         get_artifact_request = compute_nest_supplier_20210521_models.GetArtifactRequest(
             artifact_version=artifact_version,
             artifact_name=artifact_name,
             artifact_id=artifact_id,
         )
-        response = self.client.get_artifact(get_artifact_request)
+        client = cls._get_computenest_client(context)
+        response = client.get_artifact(get_artifact_request)
         return response
 
-    def list_versions(self, artifact_id):
+    @classmethod
+    def list_versions(cls, context, artifact_id):
         list_artifact_versions_request = compute_nest_supplier_20210521_models.ListArtifactVersionsRequest(artifact_id)
-        response = self.client.list_artifact_versions(list_artifact_versions_request)
+        client = cls._get_computenest_client(context)
+        response = client.list_artifact_versions(list_artifact_versions_request)
         return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/image_client.py` & `computenest-cli-1.2.7/computenestcli/service/image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 # -*- coding: utf-8 -*-
 import json
-from computeNestSupplier.service_supplier.client.oos_client import OosClient
+
 from alibabacloud_oos20190601 import models as oos_20190601_models
-from computeNestSupplier.service_supplier.client.ecs_client import EcsClient
-from computeNestSupplier.service_supplier.common import constant
+from computenestcli.common import constant
 from alibabacloud_ecs20140526 import models as ecs_20140526_models
+from computenestcli.common.decorator import retry_on_exception
+from computenestcli.service.base import Service
+
+ACS_ECS_UPDATE_IMAGE = 'ACS-ECS-UpdateImage'
+ZONE = 'Zone'
+INSTANCE_TYPE = 'instanceType'
 
 
-class ImageClient(OosClient, EcsClient):
-    ACS_ECS_UPDATE_IMAGE = 'ACS-ECS-UpdateImage'
-    ZONE = 'Zone'
-    INSTANCE_TYPE = 'instanceType'
-
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        super().__init__(region_id, access_key_id, access_key_secret)
-        self.client = self.create_client_oos()
+class ImageService(Service):
 
-    def describe_available_resource(self, instance_type):
-        client = self.create_client_ecs()
+    @classmethod
+    def describe_available_resource(cls, context, instance_type):
+        client = cls._get_ecs_client(context)
         describe_available_resource_request = ecs_20140526_models.DescribeAvailableResourceRequest(
-            region_id=self.region_id,
-            destination_resource=self.ZONE,
+            region_id=context.region_id,
+            destination_resource=ZONE,
             instance_type=instance_type
         )
         response = client.describe_available_resource(describe_available_resource_request)
         return response
 
-    def get_available_zone_id(self, instance_type):
-        response = self.describe_available_resource(instance_type)
+    @classmethod
+    def get_available_zone_id(cls, context, instance_type):
+        response = cls.describe_available_resource(context, instance_type)
         zone_id = response.body.available_zones.available_zone[0].zone_id
         return zone_id
 
+    @classmethod
+    def start_update_Image_execution(cls, context, image_data):
 
-    def start_update_Image_execution(self, image_data):
-        instance_type = image_data.get(self.INSTANCE_TYPE)
+        instance_type = image_data.get(INSTANCE_TYPE)
         # 根据用户提供的实例类型和地域选择合适的可用区
-        zone_id = self.get_available_zone_id(instance_type)
+        zone_id = cls.get_available_zone_id(context, instance_type)
         image_data[constant.ZONE_ID] = zone_id
         # 默认用户选择新建vpc，无需用户指定vpc/vswitch
         image_data[constant.WHETHER_CREATE_VPC] = True
         image_data[constant.OOS_ASSUME_ROLE] = ""
         json_data = json.dumps(image_data)
         start_execution_request = oos_20190601_models.StartExecutionRequest(
-            region_id=self.region_id,
-            template_name=self.ACS_ECS_UPDATE_IMAGE,
+            region_id=context.region_id,
+            template_name=ACS_ECS_UPDATE_IMAGE,
             parameters=json_data
         )
-        response = self.client.start_execution(start_execution_request)
+        response = cls._get_oos_client(context).start_execution(start_execution_request)
         execution_id = response.body.execution.execution_id
 
         return execution_id
 
-    def list_execution(self, execution_id):
+    @classmethod
+    @retry_on_exception()
+    def list_execution(cls, context, execution_id):
         list_execution_request = oos_20190601_models.ListExecutionsRequest(execution_id=execution_id)
-        response = self.client.list_executions(list_execution_request)
+        response = cls._get_oos_client(context).list_executions(list_execution_request)
+        print("list_oos_execution execution_id: %s, response: %s" % (execution_id, response))
         return response
 
-    def list_task_executions(self, execution_id):
+    @classmethod
+    def list_task_executions(cls, context, execution_id):
         list_task_executions_request = oos_20190601_models.ListTaskExecutionsRequest(
-            region_id=self.region_id,
+            region_id=context.region_id,
             execution_id=execution_id
         )
-        response = self.client.list_task_executions(list_task_executions_request)
+        response = cls._get_oos_client(context).list_task_executions(list_task_executions_request)
         return response
 
-    def list_execution_logs(self, execution_id):
+    @classmethod
+    def list_execution_logs(cls, context, execution_id):
         list_execution_logs_request = oos_20190601_models.ListExecutionLogsRequest(
-            region_id=self.region_id,
+            region_id=context.region_id,
             execution_id=execution_id
         )
-        response = self.client.list_execution_logs(list_execution_logs_request)
-        return response
+        response = cls._get_oos_client(context).list_execution_logs(list_execution_logs_request)
+        return response
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/client/service_client.py` & `computenest-cli-1.2.7/computenestcli/service/supplier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 # -*- coding: utf-8 -*-
 import json
 from alibabacloud_computenestsupplier20210521 import models as compute_nest_supplier_20210521_models
-from computeNestSupplier.service_supplier.client.compute_nest_client import ComputeNestClient
-from computeNestSupplier.service_supplier.common.util import Util
-from computeNestSupplier.service_supplier.common import constant
+from computenestcli.common.util import Util
+from computenestcli.common import constant
+from computenestcli.service.base import Service
 
 
-class ServiceClient(ComputeNestClient):
-
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        super().__init__(region_id, access_key_id, access_key_secret)
-        self.client = self.create_client_compute_nest()
-
-    def create_service(self, service_data, service_id=''):
-        service = service_data
-        service_info = service_data.get(constant.SERVICE_INFO)
-        deploy_meta_data = service_data.get(constant.DEPLOY_METADATA)
-        operation_metadata = service_data.get(constant.OPERATION_METADATA)
+class SupplierService(Service):
+
+    @classmethod
+    def create_service(cls, context, service_config, service_id=''):
+        service = service_config
+        service_info_config = service_config.get(constant.SERVICE_INFO)
+        deploy_metadata_config = service_config.get(constant.DEPLOY_METADATA)
+        operation_metadata = service_config.get(constant.OPERATION_METADATA)
         if operation_metadata is None:
             operation_metadata = '{}'
         else:
             operation_metadata = json.dumps(operation_metadata)
-        version_name = Util.add_timestamp_to_version_name(service_data.get(constant.VERSION_NAME))
-        for template in deploy_meta_data.get(constant.TEMPLATE_CONFIGS):
-            template[constant.PREDEFINED_PARAMETERS] = template.get(constant.PREDEFINED_PARAMETERS) or []
-            template[constant.HIDDEN_PARAMETER_KEYS] = template.get(constant.HIDDEN_PARAMETER_KEYS) or []
-        json_data = json.dumps(deploy_meta_data)
+        version_name = Util.add_timestamp_to_version_name(service_config.get(constant.VERSION_NAME))
+
+        deploy_metadata = json.dumps(deploy_metadata_config)
         service_info_init = compute_nest_supplier_20210521_models.CreateServiceRequestServiceInfo(
-            locale=service_info.get(constant.LOCALE),
-            short_description=service_info.get(constant.SHORT_DESCRIPTION),
-            image=service_info.get(constant.IMAGE),
-            name=service_info.get(constant.NAME)
+            locale=service_info_config.get(constant.LOCALE),
+            short_description=service_info_config.get(constant.SHORT_DESCRIPTION),
+            image=service_info_config.get(constant.IMAGE),
+            name=service_info_config.get(constant.NAME)
         )
         if service_id:
             create_service_request = compute_nest_supplier_20210521_models.CreateServiceRequest(
                 region_id=service.get(constant.REGION_ID),
                 service_id=service_id,
                 deploy_type=service.get(constant.DEPLOY_TYPE),
                 operation_metadata=operation_metadata,
                 version_name=version_name,
                 service_type=service.get(constant.SERVICE_TYPE),
                 service_info=[service_info_init],
-                deploy_metadata=json_data
+                deploy_metadata=deploy_metadata
             )
         else:
             create_service_request = compute_nest_supplier_20210521_models.CreateServiceRequest(
                 region_id=service.get(constant.REGION_ID),
                 deploy_type=service.get(constant.DEPLOY_TYPE),
                 operation_metadata=operation_metadata,
                 version_name=version_name,
                 service_type=service.get(constant.SERVICE_TYPE),
                 service_info=[service_info_init],
-                deploy_metadata=json_data
+                deploy_metadata=deploy_metadata
             )
-        response = self.client.create_service(create_service_request)
+        client = cls._get_computenest_client(context)
+        response = client.create_service(create_service_request)
         return response
 
-    def update_service(self, service_data, service_id):
+    @classmethod
+    def update_service(cls, context, service_data, service_id):
         service = service_data
         service_info = service_data.get(constant.SERVICE_INFO)
         deploy_meta_data = service_data.get(constant.DEPLOY_METADATA)
         operation_metadata = service_data.get(constant.OPERATION_METADATA)
         if operation_metadata is None:
             operation_metadata = '{}'
         else:
@@ -84,32 +81,37 @@
             operation_metadata=operation_metadata,
             version_name=version_name,
             service_id=service_id,
             service_info=[service_info_init],
             deploy_metadata=json_data,
             service_type=service.get(constant.SERVICE_TYPE)
         )
-        response = self.client.update_service(update_service_request)
+        client = cls._get_computenest_client(context)
+        response = client.update_service(update_service_request)
         return response
 
-    def list_service(self, service_name):
+    @classmethod
+    def list_service(cls, context, service_name):
         filter_first = compute_nest_supplier_20210521_models.ListServicesRequestFilter(
             name=constant.NAME,
             value=[service_name]
         )
         list_services_request = compute_nest_supplier_20210521_models.ListServicesRequest(
-            region_id=self.region_id,
+            region_id=context.region_id,
             filter=[
                 filter_first
             ]
         )
-        response = self.client.list_services(list_services_request)
+        client = cls._get_computenest_client(context)
+        response = client.list_services(list_services_request)
         return response
 
-    def get_service(self, service_id, service_version):
+    @classmethod
+    def get_service(cls, context, service_id, service_version):
         get_service_request = compute_nest_supplier_20210521_models.GetServiceRequest(
-            region_id=self.region_id,
+            region_id=context.region_id,
             service_id=service_id,
             service_version=service_version
         )
-        response = self.client.get_service(get_service_request)
+        client = cls._get_computenest_client(context)
+        response = client.get_service(get_service_request)
         return response
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/constant.py` & `computenest-cli-1.2.7/computenestcli/common/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,10 @@
 WHETHER_CREATE_VPC = 'whetherCreateVpc'
 OOS_ASSUME_ROLE = 'OOSAssumeRole'
 INSTANCE_TYPE = 'InstanceType'
 ALLOWED_REGIONS = 'AllowedRegions'
 ZONE_ID = 'zoneId'
 VERSION = 'Version'
 SHARE_TYPE = 'ShareType'
-APPROVAL_TYPE = 'ApprovalType'
+APPROVAL_TYPE = 'ApprovalType'
+MANAGED = 'managed'
+PRIVATE = 'private'
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/file.py` & `computenest-cli-1.2.7/computenestcli/service/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # -*- coding: utf-8 -*-
 import oss2
 import requests
 import hashlib
 import os
-from computeNestSupplier.service_supplier.common import constant
+from computenestcli.common import constant
+from computenestcli.service.base import Service
 
 
-class File:
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        self.region_id = region_id
-        self.access_key_id = access_key_id
-        self.access_key_secret = access_key_secret
+class FileService(Service):
 
-    def put_file(self, file_data, file_path, type):
+    @classmethod
+    def put_file(cls, file_data, file_path, type):
         file_name = os.path.basename(file_path)
         if type == 'file':
             sts_access_key_id = file_data.body.data.access_key_id
             sts_access_key_secret = file_data.body.data.access_key_secret
             security_token = file_data.body.data.security_token
             bucket_name = file_data.body.data.bucket_name
             object_name = file_data.body.data.key
@@ -35,15 +33,16 @@
             fileobj.seek(0, os.SEEK_SET)
             current = fileobj.tell()
             result = bucket.put_object(object_name, fileobj)
 
         url = "https://{}.{}/{}".format(bucket_name, endpoint, object_name)
         return url
 
-    def check_file_repeat(self, file_url, file_path):
+    @classmethod
+    def check_file_repeat(cls, file_url, file_path):
         response = requests.get(file_url)
         if '?' in file_url:
             # 文件部署物的私有链接会包含token，服务的logo和模版链接不包含token
             file_url = file_url.split('?')[0]
         file_name = os.path.basename(file_url)
         file_url_path = os.path.join(constant.TEMP_PATH, file_name)
         # 创建文件夹（如果不存在）
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/common/util.py` & `computenest-cli-1.2.7/computenestcli/common/util.py`

 * *Files identical despite different names*

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/artifact_processor.py` & `computenest-cli-1.2.7/computenestcli/processor/artifact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,171 +1,166 @@
-import sys
 import time
 import json
 import os
 import re
-import datetime
 from Tea.exceptions import TeaException
-from computeNestSupplier.service_supplier.client.artifact_client import ArtifactClient
-from computeNestSupplier.service_supplier.common.file import File
-from computeNestSupplier.service_supplier.common.credentials import Credentials
-from computeNestSupplier.service_supplier.common.util import Util
-from computeNestSupplier.service_supplier.processor.image_processor import ImageProcessor
-from computeNestSupplier.service_supplier.common import constant
+from computenestcli.service.artifact import ArtifactService
+from computenestcli.service.file import FileService
+from computenestcli.service.credentials import CredentialsService
+from computenestcli.common.util import Util
+from computenestcli.processor.image import ImageProcessor
+from computenestcli.common import constant
+from computenestcli.common.context import Context
+
+TRUE = 'True'
+FALSE = 'False'
+UPDATE_ARTIFACT = 'UpdateArtifact'
+AVAILABLE = 'Available'
+DELIVERING = 'Delivering'
+DATA = 'data'
+RESULT = 'result'
+IMAGE_BUILDER = 'ImageBuilder'
+ACR_IMAGE_BUILDER = 'AcrImageBuilder'
+HELM_CHART_BUILDER = 'HelmChartBuilder'
+ARTIFACT = 'artifact'
+DRAFT = 'draft'
+REGION_ID = 'regionId'
+COMMAND_CONTENT = 'CommandContent'
+ENTITY_ALREADY_EXIST_DRAFT_ARTIFACT = 'EntityAlreadyExist.DraftArtifact'
+ARTIFACT_VERSION_NOT_FOUND = 'ArtifactVersionNotFound'
 
 
 class ArtifactProcessor:
-    TRUE = 'True'
-    FALSE = 'False'
-    UPDATE_ARTIFACT = 'UpdateArtifact'
-    AVAILABLE = 'Available'
-    DELIVERING = 'Delivering'
-    DATA = 'data'
-    RESULT = 'result'
-    IMAGE_BUILDER = 'ImageBuilder'
-    ACR_IMAGE_BUILDER = 'AcrImageBuilder'
-    HELM_CHART_BUILDER = 'HelmChartBuilder'
-    ARTIFACT = 'artifact'
-    DRAFT = 'draft'
-    REGION_ID = 'regionId'
-    COMMAND_CONTENT = 'CommandContent'
-    ENTITY_ALREADY_EXIST_DRAFT_ARTIFACT = 'EntityAlreadyExist.DraftArtifact'
-    ARTIFACT_VERSION_NOT_FOUND = 'ArtifactVersionNotFound'
-
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        self.region_id = region_id
-        self.access_key_id = access_key_id
-        self.access_key_secret = access_key_secret
-        self.artifact = ArtifactClient(self.region_id, self.access_key_id, self.access_key_secret)
+
+    def __init__(self, context):
+        self.context = context
 
     def _get_file_artifact_url(self, artifact_name):
-        get_artifact_data = json.loads(self.artifact.get_artifact(artifact_name).body.artifact_property)
+        get_artifact_data = json.loads(ArtifactService.get_artifact(self.context, artifact_name).body.artifact_property)
         url = get_artifact_data.get(constant.URL)
         return url
 
     def _create_image_from_image_builder(self, data, artifact_data):
-        data_image = data.get(self.IMAGE_BUILDER)
+        data_image = data.get(IMAGE_BUILDER)
         id_image = artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.IMAGE_ID)
         id_image_match = Util.regular_expression(id_image)
         data_image_oos = data_image.get(id_image_match[1])
         region_id = data_image_oos[constant.REGION_ID]
-        command_content = data_image_oos[self.COMMAND_CONTENT]
+        command_content = data_image_oos[COMMAND_CONTENT]
         # 识别命令语句中的占位符
         pattern = r'\$\{Artifact\.(.*?)\.ArtifactProperty\.Url\}'
         matches = re.findall(pattern, command_content)
         if matches:
             artifact_key = matches[0].strip()
             artifact_name = data[constant.ARTIFACT].get(artifact_key, {}).get(constant.ARTIFACT_NAME)
             url = self._get_file_artifact_url(artifact_name)
             parts = url.split("/")
             # 截取文件部署物下载链接的后半部分
             artifact_url = parts[-2] + "/" + parts[-1]
             placeholder = f'${{Artifact.{artifact_key}.ArtifactProperty.Url}}'
             # 替换真正的url
             command_content = command_content.replace(placeholder, artifact_url)
-            data_image_oos[self.COMMAND_CONTENT] = command_content
+            data_image_oos[COMMAND_CONTENT] = command_content
         data_image_oos = Util.lowercase_first_letter(data_image_oos)
-        region_id_image = data_image_oos[self.REGION_ID]
-        image_processor = ImageProcessor(region_id_image, self.access_key_id, self.access_key_secret)
+        region_id_image = data_image_oos[REGION_ID]
+        image_context = Context(region_id_image, self.context.credentials)
+        image_processor = ImageProcessor(image_context)
         return region_id, image_processor.process_image(data_image_oos)
 
     def _create_acrimage_from_acrimage_builder(self, data, artifact_data, file_path_config):
         artifact_type = artifact_data.get(constant.ARTIFACT_TYPE)
-        image = ImageProcessor(self.region_id, self.access_key_id, self.access_key_secret)
-        data_acr_image = data.get(self.ACR_IMAGE_BUILDER)
+        image = ImageProcessor(self.context)
+        data_acr_image = data.get(ACR_IMAGE_BUILDER)
         acr_image = artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.REPO_NAME)
         acr_image_match = Util.regular_expression(acr_image)
         data_acr_image = data_acr_image.get(acr_image_match[1])
-        file_path = os.path.join(os.path.dirname(file_path_config),data_acr_image[constant.DOCKER_FILE_PATH])
+        file_path = os.path.join(os.path.dirname(file_path_config), data_acr_image[constant.DOCKER_FILE_PATH])
         acr_image_name = data_acr_image[constant.REPO_NAME]
         acr_image_tag = data_acr_image[constant.TAG]
         # 如果DockerfilePath存在，运行Dockerfile并打标推送
         if data_acr_image[constant.DOCKER_FILE_PATH]:
             image.process_acr_image(acr_image_name, acr_image_tag, file_path)
-            repo_id = self.artifact.list_acr_image_repositories(artifact_type, acr_image_name).body.repositories[0].repo_id
+            repo_id = self._get_repo_id(artifact_type, acr_image_name)
         # 若不存在认为线上仓库已存在相关容器镜像
         else:
-            try:
-                # 根据repo_name查询repo_id，查询不到直接抛出错误
-                repo_id = self.artifact.list_acr_image_repositories(artifact_type, acr_image_name).body.repositories[0].repo_id
-            except TeaException as e:
-                raise e
+            repo_id = self._get_repo_id(artifact_type, acr_image_name)
             # 查到repo_id后检索所有已存在的tag，检查提供的tag是否存在
-            tags = self.artifact.list_acr_image_tags(repo_id, artifact_type).body.images
+            tags = ArtifactService.list_acr_image_tags(self.context, repo_id, artifact_type).body.images
             tag_values = []
             for item in tags:
                 tag_value = item.tag
                 tag_values.append(tag_value)
             if acr_image_tag in tag_values:
                 acr_image_tag = acr_image_tag
             else:
                 raise ValueError("Provided acr image tag does not exist")
         return acr_image_name, repo_id, acr_image_tag
 
+    def _get_repo_id(self, artifact_type, acr_image_name):
+        response_body = ArtifactService.list_acr_image_repositories(self.context, artifact_type, acr_image_name).body
+        if response_body and response_body.repositories:
+            return response_body.repositories[0].repo_id
+        else:
+            raise Exception("No Repo found")
+
     def _create_helmchart_from_helmchart_builder(self, data, artifact_data, file_path_config):
         artifact_type = artifact_data.get(constant.ARTIFACT_TYPE)
-        image = ImageProcessor(self.region_id, self.access_key_id, self.access_key_secret)
-        helm_chart_data = data.get(self.HELM_CHART_BUILDER)
+        image = ImageProcessor(self.context)
+        helm_chart_data = data.get(HELM_CHART_BUILDER)
         helm_chart = artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.REPO_NAME)
         helm_chart_match = Util.regular_expression(helm_chart)
         data_helm_chart = helm_chart_data.get(helm_chart_match[1])
         file_path = os.path.join(os.path.dirname(file_path_config), data_helm_chart[constant.HELM_CHART_PATH])
         helm_chart_name = data_helm_chart[constant.REPO_NAME]
         helm_chart_tag = data_helm_chart[constant.TAG]
 
         if data_helm_chart[constant.HELM_CHART_PATH]:
             image.process_helm_chart(file_path)
-            helm_chart_id = self.artifact.list_acr_image_repositories(artifact_type, helm_chart_name).body.repositories[0].repo_id
+            helm_chart_repo_id = self._get_repo_id(artifact_type, helm_chart_name)
         # 若不存在认为线上仓库已存在相关容器镜像
         else:
-            try:
-                # 根据repo_name查询repo_id，查询不到直接抛出错误
-                helm_chart_id = self.artifact.list_acr_image_repositories(artifact_type, helm_chart_name).body.repositories[0].repo_id
-            except TeaException as e:
-                raise e
+            helm_chart_repo_id = self._get_repo_id(artifact_type, helm_chart_name)
         # 查到repo_id后检索所有已存在的tag，检查提供的tag是否存在
-        tags = self.artifact.list_acr_image_tags(helm_chart_id, artifact_type).body.images
+        tags = ArtifactService.list_acr_image_tags(self.context, helm_chart_repo_id, artifact_type).body.images
+        print("_create_helmchart_from_helmchart_builder tags: ", tags)
         tag_values = []
         for item in tags:
             tag_value = item.tag
             tag_values.append(tag_value)
         if helm_chart_tag in tag_values:
             helm_chart_tag = helm_chart_tag
         else:
             raise ValueError("Invalid or non-existent Helm chart version provided.")
 
-        return helm_chart_name, helm_chart_id, helm_chart_tag
+        return helm_chart_name, helm_chart_repo_id, helm_chart_tag
 
     def _replace_artifact_file_path_with_url(self, file_path):
-        credentials = Credentials(self.region_id, self.access_key_id, self.access_key_secret)
-        file = File(self.region_id, self.access_key_id, self.access_key_secret)
-        data = credentials.get_artifact_repository_credentials(constant.FILE)
-        file_artifact_url = file.put_file(data, file_path, self.ARTIFACT)
+        data = CredentialsService.get_artifact_repository_credentials(self.context, constant.FILE)
+        file_artifact_url = FileService.put_file(data, file_path, ARTIFACT)
         return file_artifact_url
 
     def _release_artifact(self, artifact_id, artifact_name):
-        self.artifact.release_artifact(artifact_id)
+        ArtifactService.release_artifact(self.context, artifact_id)
         while True:
             # 定时检测部署物发布状态
             try:
-                data_response = self.artifact.get_artifact(artifact_name, 'draft')
+                data_response = ArtifactService.get_artifact(self.context, artifact_name, 'draft')
                 artifact_status = data_response.body.status
-                if artifact_status == self.DELIVERING:
+                if artifact_status == DELIVERING:
                     print('The artifact is being released...')
             except TeaException as e:
-                if e.code == self.ARTIFACT_VERSION_NOT_FOUND:
+                if e.code == ARTIFACT_VERSION_NOT_FOUND:
                     print('The release is complete')
                     break
                 else:
                     raise
             time.sleep(25)
 
     def get_artifact_detail(self, artifact_id, data_yaml, artifact_key):
-        artifact = ArtifactClient(self.region_id, self.access_key_id, self.access_key_secret)
-        response = artifact.get_artifact('', '', artifact_id)
+        response = ArtifactService.get_artifact(self.context, '', '', artifact_id)
         artifact_type = response.body.artifact_type
         artifact_name = response.body.name
         description = response.body.description
         support_region_ids = response.body.support_region_ids
         artifact_property = json.loads(response.body.artifact_property)
         parameters = {
             constant.ARTIFACT_TYPE: artifact_type,
@@ -176,117 +171,118 @@
         }
         data_yaml[constant.ARTIFACT][artifact_key] = parameters
         return data_yaml
 
     @Util.measure_time
     def process(self, data_config, file_path_config, update_artifact='', version_name=''):
         data_artifact = data_config.get(constant.ARTIFACT)
-        file = File(self.region_id, self.access_key_id, self.access_key_secret)
         for artifact_data in data_artifact.values():
             if constant.ARTIFACT_NAME in artifact_data:
                 artifact_type = artifact_data.get(constant.ARTIFACT_TYPE)
                 artifact_name = artifact_data.get(constant.ARTIFACT_NAME)
                 if version_name:
                     artifact_data[constant.VERSION_NAME] = version_name
-                if update_artifact == self.TRUE:
-                    artifact_data[self.UPDATE_ARTIFACT] = True
+                if update_artifact == TRUE:
+                    artifact_data[UPDATE_ARTIFACT] = True
                 else:
-                    artifact_data[self.UPDATE_ARTIFACT] = False
-                artifact_data_list = self.artifact.list_artifact(artifact_name)
+                    artifact_data[UPDATE_ARTIFACT] = False
+                artifact_data_list = ArtifactService.list_artifact(self.context, artifact_name)
                 if len(artifact_data_list.body.artifacts) == 0:
                     if artifact_type == constant.FILE:
                         # 将相对路径替换成绝对路径
                         file_path = os.path.join(os.path.dirname(file_path_config),
                                                  artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.URL))
                         # 将文件部署物的本地路径替换成Url
                         artifact_data[constant.ARTIFACT_PROPERTY][
                             constant.URL] = self._replace_artifact_file_path_with_url(file_path)
                     elif artifact_type == constant.ECS_IMAGE:
-                        if self.IMAGE_BUILDER in data_config:
+                        if IMAGE_BUILDER in data_config:
                             # 利用oos模版创建镜像
                             region_id, image_id = self._create_image_from_image_builder(data_config, artifact_data)
                             artifact_data[constant.ARTIFACT_PROPERTY][constant.REGION_ID] = region_id
                             artifact_data[constant.ARTIFACT_PROPERTY][constant.IMAGE_ID] = image_id
                     elif artifact_type == constant.ACR_IMAGE:
-                            acr_image_name, repo_id, acr_image_tag = self._create_acrimage_from_acrimage_builder(
-                                data_config, artifact_data, file_path_config)
-                            artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_NAME] = acr_image_name
-                            artifact_data[constant.ARTIFACT_PROPERTY][constant.TAG] = acr_image_tag
-                            artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_ID] = repo_id
+                        acr_image_name, repo_id, acr_image_tag = self._create_acrimage_from_acrimage_builder(
+                            data_config, artifact_data, file_path_config)
+                        artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_NAME] = acr_image_name
+                        artifact_data[constant.ARTIFACT_PROPERTY][constant.TAG] = acr_image_tag
+                        artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_ID] = repo_id
                     elif artifact_type == constant.HELM_CHART:
-                        helm_chart_name, helm_chart_id, helm_chart_tag = self._create_helmchart_from_helmchart_builder(data_config, artifact_data, file_path_config)
+                        helm_chart_name, helm_chart_id, helm_chart_tag = self._create_helmchart_from_helmchart_builder(
+                            data_config, artifact_data, file_path_config)
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_NAME] = helm_chart_name
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.TAG] = helm_chart_tag
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_ID] = helm_chart_id
-                    data_create_artifact = self.artifact.create_artifact(artifact_data)
+                    data_create_artifact = ArtifactService.create_artifact(self.context, artifact_data)
                     artifact_id = data_create_artifact.body.artifact_id
                     current_time = Util.get_current_time()
                     print("===========================")
                     print("Successfully created a new artifact!")
                     print("The artifact name: ", artifact_name)
                     print("The artifact id: ", artifact_id)
                     print("Completion time: ", current_time)
                     print("===========================")
                     self._release_artifact(artifact_id, artifact_name)
-                elif artifact_data.get(self.UPDATE_ARTIFACT) == False:
+                elif artifact_data.get(UPDATE_ARTIFACT) == False:
                     artifact_id = artifact_data_list.body.artifacts[0].artifact_id
                     current_time = Util.get_current_time()
                     print("===========================")
                     print("No need to update the artifact")
                     print("The artifact name: ", artifact_name)
                     print("The artifact id: ", artifact_id)
                     print("Completion time: ", current_time)
                     print("===========================")
                 else:
                     if artifact_type == constant.FILE:
                         file_url_existed = self._get_file_artifact_url(artifact_name)
                         # 将相对路径替换成绝对路径
                         file_path = os.path.join(os.path.dirname(file_path_config),
                                                  artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.URL))
-                        result_artifact = file.check_file_repeat(file_url_existed, file_path)
+                        result_artifact = FileService.check_file_repeat(file_url_existed, file_path)
                         # 检查文件部署物是否重复，重复则不再上传，使用现有Url
                         if result_artifact:
                             artifact_data[constant.ARTIFACT_PROPERTY][constant.URL] = file_url_existed.split('?')[0]
                         else:
                             artifact_data[constant.ARTIFACT_PROPERTY][
                                 constant.URL] = self._replace_artifact_file_path_with_url(file_path)
                     elif artifact_type == constant.ECS_IMAGE:
-                        if self.IMAGE_BUILDER in data_config:
+                        if IMAGE_BUILDER in data_config:
                             # 利用oos模版创建镜像
                             region_id, image_id = self._create_image_from_image_builder(data_config, artifact_data)
                             artifact_data[constant.ARTIFACT_PROPERTY][constant.REGION_ID] = region_id
                             artifact_data[constant.ARTIFACT_PROPERTY][constant.IMAGE_ID] = image_id
                     elif artifact_type == constant.ACR_IMAGE:
                         acr_image_name, repo_id, acr_image_tag = self._create_acrimage_from_acrimage_builder(
                             data_config, artifact_data, file_path_config)
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_NAME] = acr_image_name
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.TAG] = acr_image_tag
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_ID] = repo_id
                     elif artifact_type == constant.HELM_CHART:
-                        helm_chart_name, helm_chart_id, helm_chart_tag = self._create_helmchart_from_helmchart_builder(data_config, artifact_data, file_path_config)
+                        helm_chart_name, helm_chart_id, helm_chart_tag = self._create_helmchart_from_helmchart_builder(
+                            data_config, artifact_data, file_path_config)
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_NAME] = helm_chart_name
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.TAG] = helm_chart_tag
                         artifact_data[constant.ARTIFACT_PROPERTY][constant.REPO_ID] = helm_chart_id
                     artifact_id = artifact_data_list.body.artifacts[0].artifact_id
                     try:
-                        self.artifact.create_artifact(artifact_data, artifact_id)
+                        ArtifactService.create_artifact(self.context, artifact_data, artifact_id)
                     except TeaException as e:
-                        if e.code == self.ENTITY_ALREADY_EXIST_DRAFT_ARTIFACT:
-                            self.artifact.update_artifact(artifact_data, artifact_id)
+                        if e.code == ENTITY_ALREADY_EXIST_DRAFT_ARTIFACT:
+                            ArtifactService.update_artifact(self.context, artifact_data, artifact_id)
                         else:
                             raise
                     current_time = Util.get_current_time()
                     print("===========================")
                     print("Successfully updated the artifact!")
                     print("The artifact name: ", artifact_name)
                     print("The artifact id: ", artifact_id)
                     print("Completion time: ", current_time)
                     print("===========================")
                     self._release_artifact(artifact_id, artifact_name)
-                data_response = self.artifact.list_artifact(artifact_name)
+                data_response = ArtifactService.list_artifact(self.context, artifact_name)
                 max_version = int(data_response.body.artifacts[0].max_version)
                 if artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.VERSION):
                     version = artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.VERSION)
                     if version == 'back':
                         artifact_version = max_version - 1
                     elif int(version) <= max_version:
                         artifact_version = artifact_data.get(constant.ARTIFACT_PROPERTY).get(constant.VERSION)
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/check_processor.py` & `computenest-cli-1.2.7/computenestcli/processor/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,59 @@
 import yaml
 import os
-from computeNestSupplier.service_supplier.common import constant
-from computeNestSupplier.service_supplier.common.util import Util
+from computenestcli.common import constant
+from computenestcli.common.util import Util
+
 
 class CheckProcesser:
     def __init__(self, config, file_path):
         self.config = config
         self.file_path = file_path
         self.checks = [self.validate_allowed_regions, self.validate_image_key]
         self.errors = []
 
     def validate_allowed_regions(self):
         support_regions = []
+        if constant.ARTIFACT not in self.config:
+            return True
+        deploy_metadata = self.config[constant.SERVICE][constant.DEPLOY_METADATA]
+        if self.config[constant.SERVICE][constant.SERVICE_TYPE] == constant.MANAGED:
+            template_configs = deploy_metadata[constant.SUPPLIER_DEPLOY_METADATA][constant.SUPPLIER_TEMPLATE_CONFIGS]
+        else:
+            template_configs = deploy_metadata[constant.TEMPLATE_CONFIGS]
+
         for artifact in self.config[constant.ARTIFACT]:
             if self.config[constant.ARTIFACT][artifact][constant.ARTIFACT_TYPE] == constant.ECS_IMAGE:
                 support_regions.extend(self.config[constant.ARTIFACT][artifact][constant.SUPPORT_REGION_IDS])
-                template_configs = self.config[constant.SERVICE][constant.DEPLOY_METADATA][constant.TEMPLATE_CONFIGS]
                 for config in template_configs:
                     allowed_regions = config[constant.ALLOWED_REGIONS]
                     if set(allowed_regions).issubset(set(support_regions)):
                         continue
                     else:
                         self.errors.append("The AllowedRegions in TemplateConfigs are beyond the scope of SupportRegionIds in Artifact.")
                         return False
         return True
 
     def validate_image_key(self):
         deploy_metadata = self.config[constant.SERVICE][constant.DEPLOY_METADATA]
-        for template in deploy_metadata.get(constant.TEMPLATE_CONFIGS):
+
+        if self.config[constant.SERVICE][constant.SERVICE_TYPE] == constant.MANAGED:
+            template_configs = deploy_metadata[constant.SUPPLIER_DEPLOY_METADATA][constant.SUPPLIER_TEMPLATE_CONFIGS]
+        else:
+            template_configs = deploy_metadata[constant.TEMPLATE_CONFIGS]
+
+        for template in template_configs:
             # 将相对路径替换成绝对路径
             template_path = os.path.join(os.path.dirname(self.file_path), template.get(constant.URL))
             template = self.read_yaml_file(template_path)
             template_image_ids = self.get_image_ids(template)
-            if constant.ARTIFACT_RELATION not in self.config[constant.SERVICE][constant.DEPLOY_METADATA][constant.SUPPLIER_DEPLOY_METADATA]:
+            if constant.ARTIFACT_RELATION not in deploy_metadata[constant.SUPPLIER_DEPLOY_METADATA]:
                 return True
-            config_image_ids = set(self.config[constant.SERVICE][constant.DEPLOY_METADATA][constant.SUPPLIER_DEPLOY_METADATA][constant.ARTIFACT_RELATION].keys())
+            config_image_ids = set(self.config[constant.SERVICE][constant.DEPLOY_METADATA][
+                                       constant.SUPPLIER_DEPLOY_METADATA][constant.ARTIFACT_RELATION].keys())
             if not config_image_ids.issubset(template_image_ids):
                 self.errors.append("The ImageId in template.yaml does not match the image identifier in config.yaml.")
                 return False
         return True
 
     @staticmethod
     def read_yaml_file(file):
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/image_processor.py` & `computenest-cli-1.2.7/computenestcli/processor/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 import os
-import sys
 import time
 import json
-import datetime
-from computeNestSupplier.service_supplier.client.image_client import ImageClient
-from computeNestSupplier.service_supplier.common.util import Util
-from computeNestSupplier.service_supplier.common import constant
-from computeNestSupplier.service_supplier.common.credentials import Credentials
+from computenestcli.service.image import ImageService
+from computenestcli.common.util import Util
+from computenestcli.common import constant
+from computenestcli.service.credentials import CredentialsService
+
+IMAGEID = 'imageId'
+RUNNING = 'Running'
+WAITING = 'Waiting'
+QUEUED = 'Queued'
+FAILED = 'Failed'
+SUCCESS = 'Success'
+RESPONSE = 'Response'
+INVOCATIONS = 'Invocations'
+INVOCATION = 'Invocation'
+INVOKEINSTANCES = 'InvokeInstances'
+INVOKEINSTANCE = 'InvokeInstance'
+INVOCATIONRESULTS = 'InvocationResults'
+INVOCATIONRESULT = 'InvocationResult'
+OUTPUT = 'Output'
+ACS_ECS_RUNCOMMAND = 'ACS::ECS::RunCommand'
+MAX_RETRIES = 3
+MAX_WAIT_TIME_SECOND = 1
 
 
 class ImageProcessor:
-    IMAGEID = 'imageId'
-    RUNNING = 'Running'
-    WAITING = 'Waiting'
-    QUEUED = 'Queued'
-    FAILED = 'Failed'
-    SUCCESS = 'Success'
-    RESPONSE = 'Response'
-    INVOCATIONS = 'Invocations'
-    INVOCATION = 'Invocation'
-    INVOKEINSTANCES = 'InvokeInstances'
-    INVOKEINSTANCE = 'InvokeInstance'
-    INVOCATIONRESULTS = 'InvocationResults'
-    INVOCATIONRESULT = 'InvocationResult'
-    OUTPUT = 'Output'
-    ACS_ECS_RUNCOMMAND = 'ACS::ECS::RunCommand'
-
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        self.region_id = region_id
-        self.access_key_id = access_key_id
-        self.access_key_secret = access_key_secret
-        self.image = ImageClient(self.region_id, self.access_key_id, self.access_key_secret)
+
+    def __init__(self, context):
+        self.context = context
 
     def get_execution_logs(self, execution_id):
-        response = self.image.list_task_executions(execution_id).body.task_executions
+        response = ImageService.list_task_executions(self.context, execution_id).body.task_executions
         for task_execution in response:
-            if task_execution.task_action == self.ACS_ECS_RUNCOMMAND and (task_execution.status == self.FAILED or task_execution.status == self.SUCCESS):
+            if task_execution.task_action == ACS_ECS_RUNCOMMAND and (task_execution.status == FAILED or task_execution.status == SUCCESS):
                 child_execution_id = task_execution.task_execution_id
-                execution_logs = json.loads(self.image.list_execution_logs(child_execution_id).body.execution_logs[2].message)
-                if task_execution.status == self.FAILED:
-                    execution_log = execution_logs[self.RESPONSE][self.INVOCATIONS][self.INVOCATION][0][self.INVOKEINSTANCES][self.INVOKEINSTANCE][0][self.OUTPUT]
-                elif task_execution.status == self.SUCCESS:
-                    execution_log = execution_logs[self.RESPONSE][self.INVOCATION][self.INVOCATIONRESULTS][self.INVOCATIONRESULT][0][self.OUTPUT]
+                execution_logs = json.loads(ImageService.list_execution_logs(self.context, child_execution_id).body.execution_logs[2].message)
+                if task_execution.status == FAILED:
+                    execution_log = execution_logs[RESPONSE][INVOCATIONS][INVOCATION][0][INVOKEINSTANCES][INVOKEINSTANCE][0][OUTPUT]
+                elif task_execution.status == SUCCESS:
+                    execution_log = execution_logs[RESPONSE][INVOCATION][INVOCATIONRESULTS][INVOCATIONRESULT][0][OUTPUT]
                 message = Util.decode_base64(execution_log)
-            elif task_execution.status == self.FAILED:
+            elif task_execution.status == FAILED:
                 message = task_execution.status_message
         return message
 
     @Util.measure_time
     def process_image(self, image_data):
-        execution_id = self.image.start_update_Image_execution(image_data)
+        retry_times = 0
+        execution_id = ImageService.start_update_Image_execution(self.context, image_data)
         current_time = Util.get_current_time()
         print("===========================")
         print("The task to create an image has started executing")
         print("The execution id: ", execution_id)
         print("Start time: ", current_time)
         print("===========================")
         while True:
-            image_data = self.image.list_execution(execution_id)
-            status = image_data.body.executions[0].status
-            if status == self.RUNNING or status == self.WAITING or status == self.QUEUED:
-                current_task = image_data.body.executions[0].current_tasks[0].task_name
-                print('executing...The current task is :', current_task)
-            elif status == self.FAILED:
-                status_message = image_data.body.executions[0].status_message
-                print('Execution failed')
-                print("The failed status message: ", status_message)
-                try:
-                    execution_log = self.get_execution_logs(execution_id)
-                    print("The detailed execution log: \n", execution_log)
-                except Exception as e:
-                    print('get execution log failed', e)
-                sys.exit(1)
-            elif status == self.SUCCESS:
-                image_data = self.image.list_execution(execution_id)
+            image_data = ImageService.list_execution(self.context, execution_id)
+            execution = image_data.body.executions[0]
+            status = execution.status
+            if status == RUNNING or status == WAITING or status == QUEUED:
+                current_tasks = execution.current_tasks
+                if current_tasks is None or len(current_tasks) == 0:
+                    if retry_times < MAX_RETRIES:
+                        retry_times += 1
+                        time.sleep(MAX_WAIT_TIME_SECOND)
+                        continue
+                    if retry_times >= MAX_RETRIES:
+                        raise Exception("Build image failed, error message: ", execution.status_message)
+                current_task = current_tasks[0].task_name
+                print('Executing...The current task is :', current_task)
+            elif status == FAILED:
+                raise Exception("Execution failed, Error message: ", execution.status_message)
+                # try:
+                #     execution_log = self.get_execution_logs(execution_id)
+                #     print("The detailed execution log: \n", execution_log)
+                # except Exception as e:
+                #     print('get execution log failed', e)
+            elif status == SUCCESS:
+                image_data = ImageService.list_execution(self.context, execution_id)
                 outputs = json.loads(image_data.body.executions[0].outputs)
-                image_id = outputs[self.IMAGEID]
+                image_id = outputs[IMAGEID]
                 current_time = Util.get_current_time()
                 try:
-                    execution_log = self.get_execution_logs(execution_id)
+                    execution_log = ImageService.get_execution_logs(self.context, execution_id)
                     # print("The detailed execution log: \n", execution_log)
                 except Exception as e:
                     print('get execution log failed', e)
                 print("===========================")
                 print("Successfully created a new image!")
                 print("The image id: ", image_id)
                 print("Completion time: ", current_time)
@@ -90,16 +95,15 @@
                 break
             time.sleep(100)
 
         return image_id
 
     @Util.measure_time
     def process_acr_image(self, acr_image_name, acr_image_tag, file_path):
-        credentials = Credentials(self.region_id, self.access_key_id, self.access_key_secret)
-        response = credentials.get_artifact_repository_credentials(constant.ACR_IMAGE)
+        response = CredentialsService.get_artifact_repository_credentials(self.context, constant.ACR_IMAGE)
         username = response.body.credentials.username
         password = response.body.credentials.password
         repository_name = response.body.available_resources[0].repository_name
         docker_path = os.path.dirname(response.body.available_resources[0].path)
         file_path = os.path.dirname(file_path)
         commands = [
             f"docker build -t {acr_image_name}:{acr_image_tag} .",
@@ -110,19 +114,19 @@
         for command in commands:
             try:
                 output, error = Util.run_cli_command(command, file_path)
                 print(output.decode())
                 print(error.decode())
             except Exception as e:
                 print(f"Error occurred: {e}")
+                raise e
 
     @Util.measure_time
     def process_helm_chart(self, file_path):
-        credentials = Credentials(self.region_id, self.access_key_id, self.access_key_secret)
-        response = credentials.get_artifact_repository_credentials(constant.HELM_CHART)
+        response = CredentialsService.get_artifact_repository_credentials(self.context, constant.HELM_CHART)
         username = response.body.credentials.username
         password = response.body.credentials.password
         repository_name = response.body.available_resources[0].repository_name
         chart_path = os.path.dirname(response.body.available_resources[0].path)
         file_name = file_path.split("/")[-1]
         file_path = os.path.dirname(file_path)
         commands = [
@@ -132,7 +136,8 @@
         for command in commands:
             try:
                 output, error = Util.run_cli_command(command, file_path)
                 print(output.decode())
                 print(error.decode())
             except Exception as e:
                 print(f"Error occurred: {e}")
+                raise e
```

### Comparing `computenest-cli-1.1.9/computeNestSupplier/service_supplier/processor/service_processor.py` & `computenest-cli-1.2.7/computenestcli/processor/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 import os
 import sys
 import json
 from ruamel.yaml import YAML
 from Tea.exceptions import TeaException
-from computeNestSupplier.service_supplier.client.service_client import ServiceClient
-from computeNestSupplier.service_supplier.common import constant
-from computeNestSupplier.service_supplier.common.util import Util
-from computeNestSupplier.service_supplier.processor.artifact_processor import ArtifactProcessor
-from computeNestSupplier.service_supplier.common.file import File
-from computeNestSupplier.service_supplier.common.credentials import Credentials
+from computenestcli.service.supplier import SupplierService
+from computenestcli.common import constant
+from computenestcli.common.util import Util
+from computenestcli.processor.artifact import ArtifactProcessor
+from computenestcli.service.file import FileService
+from computenestcli.service.credentials import CredentialsService
+
+FILE = 'file'
+DRAFT = 'draft'
+SERVICE_NOT_FOUND = 'ServiceNotFound'
+CUSTOM_OPERATIONS = 'CustomOperations'
+ACTIONS = 'Actions'
+TEMPLATE_URL = 'TemplateUrl'
+SHARE_TYPE = 'ShareType'
+APPROVAL_TYPE = 'ApprovalType'
+ALWAYS_LATEST = 'AlwaysLatest'
+SECURITY_GROUPS = 'SecurityGroups'
+HIDDEN_PARAMETER_KEYS = 'HiddenParameterKeys'
+PREDEFINED_PARAMETERS = 'PredefinedParameters'
+NETWORK_METADATA = 'NetworkMetadata'
+DEPLOY_TIME_OUT = 'DeployTimeout'
+UPDATE_INFO = 'UpdateInfo'
 
 
 class ServiceProcessor:
-    FILE = 'file'
-    DRAFT = 'draft'
-    SERVICE_NOT_FOUND = 'ServiceNotFound'
-    CUSTOM_OPERATIONS = 'CustomOperations'
-    ACTIONS = 'Actions'
-    TEMPLATE_URL = 'TemplateUrl'
-    SHARE_TYPE = 'ShareType'
-    APPROVAL_TYPE = 'ApprovalType'
-    ALWAYS_LATEST = 'AlwaysLatest'
-    SECURITY_GROUPS = 'SecurityGroups'
-    HIDDEN_PARAMETER_KEYS = 'HiddenParameterKeys'
-    PREDEFINED_PARAMETERS = 'PredefinedParameters'
-    NETWORK_METADATA = 'NetworkMetadata'
-    DEPLOY_TIME_OUT = 'DeployTimeout'
-    UPDATE_INFO = 'UpdateInfo'
-
-    def __init__(self, region_id, access_key_id, access_key_secret):
-        self.region_id = region_id
-        self.access_key_id = access_key_id
-        self.access_key_secret = access_key_secret
-        self.service = ServiceClient(self.region_id, self.access_key_id, self.access_key_secret)
+
+    def __init__(self, context):
+        self.context = context
 
     def _get_service_logo_url(self, service_name):
-        data_list_service = self.service.list_service(service_name)
+        data_list_service = SupplierService.list_service(self.context, service_name)
         service_id = data_list_service.body.services[0].service_id
         service_version = data_list_service.body.services[0].version
-        data_get_service = self.service.get_service(service_id, service_version)
+        data_get_service = SupplierService.get_service(self.context, service_id, service_version)
         url = data_get_service.body.service_infos[0].image
         return url
 
     def _get_template_url_data(self, service_name):
-        data_list_service = self.service.list_service(service_name)
+        data_list_service = SupplierService.list_service(self.context, service_name)
         service_id = data_list_service.body.services[0].service_id
         service_version = data_list_service.body.services[0].version
-        data_get_service = self.service.get_service(service_id, service_version)
+        data_get_service = SupplierService.get_service(self.context, service_id, service_version)
         deploy_metadata = data_get_service.body.deploy_metadata
         return deploy_metadata
 
     def _replace_artifact_data(self, artifact_relations, data_artifact):
         for artifact_info in artifact_relations.values():
             id_file = artifact_info.get(constant.ARTIFACT_ID)
             version_file = artifact_info.get(constant.ARTIFACT_VERSION)
@@ -60,77 +58,74 @@
             artifact_id_file = data_artifact.get(id_match[1]).get(id_match[2])
             # [0][1][2]为刚才解析出得占位符的分解，即Artifact，Artifact_x，ArtifactId
             artifact_version_file = data_artifact.get(version_match[1]).get(version_match[2])
             artifact_info[constant.ARTIFACT_ID] = artifact_id_file
             artifact_info[constant.ARTIFACT_VERSION] = artifact_version_file
 
     def _replace_file_path_with_url(self, file_path):
-        file = File(self.region_id, self.access_key_id, self.access_key_secret)
-        credentials = Credentials(self.region_id, self.access_key_id, self.access_key_secret)
         file_name = os.path.basename(file_path)
-        data_file = credentials.get_upload_credentials(file_name)
-        file_url = file.put_file(data_file, file_path, self.FILE)
+        data_file = CredentialsService.get_upload_credentials(self.context, file_name)
+        file_url = FileService.put_file(data_file, file_path, FILE)
         return file_url
 
     def _replace_parameters(self, content, parameters):
-        new_content = None
+        new_content = content
         if isinstance(content, dict):
             new_content = {}
             for key, value in content.items():
                 new_key = self._replace_parameters(key, parameters)
                 new_value = self._replace_parameters(value, parameters)
                 new_content[new_key] = new_value
         elif isinstance(content, list):
             new_content = []
             for value in content:
                 new_value = self._replace_parameters(value, parameters)
                 new_content.append(new_value)
         elif isinstance(content, str):
             parameter_match = Util.regular_expression(content)
-            if parameter_match and len(parameter_match) == 1:
-                if parameter_match[0] in parameters:
-                    new_content = parameters.get(parameter_match[0])
+            if parameter_match and len(parameter_match) == 1 and parameter_match[0] in parameters:
+                new_content = parameters.get(parameter_match[0])
             else:
                 new_content = content
-
+        elif isinstance(content, bool):
+            new_content = content
         return new_content
 
     def _delete_field(self, data, field):
         if isinstance(data, dict):
             for key in list(data.keys()):
                 if key == field:
                     del data[key]
                 else:
                     self._delete_field(data[key], field)
         elif isinstance(data, list):
             for item in data:
                 self._delete_field(item, field)
 
     def _get_service_detail(self, region_id, service_name):
-        service = ServiceClient(self.region_id, self.access_key_id, self.access_key_secret)
-        response = service.list_service(service_name)
+        response = SupplierService.list_service(self.context, service_name)
         if len(response.body.services) == 0:
             print("Service does not exist, please check the region_id and service_name")
             sys.exit(1)
         service_id = response.body.services[0].service_id
         version = response.body.services[0].version
-        data = service.get_service(service_id, version)
+        data = SupplierService.get_service(self.context, service_id, version)
         deploy_metadata = json.loads(data.body.deploy_metadata)
         approval_type = data.body.approval_type
         share_type = data.body.share_type
         service_type = data.body.service_type
         deploy_type = data.body.deploy_type
-        # self._delete_field(deploy_metadata, self.NETWORK_METADATA)
-        # self._delete_field(deploy_metadata, self.DEPLOY_TIME_OUT)
-        self._delete_field(deploy_metadata, self.ALWAYS_LATEST)
+        # self._delete_field(deploy_metadata, NETWORK_METADATA)
+        # self._delete_field(deploy_metadata, DEPLOY_TIME_OUT)
+        self._delete_field(deploy_metadata, ALWAYS_LATEST)
         for config in deploy_metadata[constant.TEMPLATE_CONFIGS]:
-            self._delete_field(config, self.SECURITY_GROUPS)
-            # self._delete_field(config, self.HIDDEN_PARAMETER_KEYS)
-            # self._delete_field(config, self.PREDEFINED_PARAMETERS)
-            self._delete_field(config, self.UPDATE_INFO)
+            self._delete_field(config, SECURITY_GROUPS)
+            # self._delete_field(config, HIDDEN_PARAMETER_KEYS)
+            # self._delete_field(config, PREDEFINED_PARAMETERS)
+            self._delete_field(config, UPDATE_INFO)
         service_info_pre = data.body.service_infos[0]
         image = service_info_pre.image
         name = service_info_pre.name
         locale = service_info_pre.locale
         short_description = service_info_pre.short_description
         service_info = {
             constant.LOCALE: locale,
@@ -156,17 +151,16 @@
     @Util.measure_time
     def import_command(self, data_config, file_path, update_artifact, service_name='', version_name='', icon='',
                        desc='', parameters={}):
         if parameters:
             data_config = self._replace_parameters(data_config, parameters)
         service_config = data_config[constant.SERVICE]
         deploy_metadata_config = service_config[constant.DEPLOY_METADATA]
-        file = File(self.region_id, self.access_key_id, self.access_key_secret)
         if data_config.get(constant.ARTIFACT):
-            artifact_processor = ArtifactProcessor(self.region_id, self.access_key_id, self.access_key_secret)
+            artifact_processor = ArtifactProcessor(self.context)
             data_artifact = artifact_processor.process(data_config, file_path, update_artifact, version_name)
             # 遍历部署物关联映射，进行部署物替换
             support_artifact_relation_types = [constant.ARTIFACT_RELATION, constant.FILE_ARTIFACT_RELATION,
                                                constant.ACR_IMAGE_ARTIFACT_RELATION,
                                                constant.HELM_CHART_ARTIFACT_RELATION]
             for relation_type, artifact_relations in \
                     deploy_metadata_config.get(constant.SUPPLIER_DEPLOY_METADATA, {}).items():
@@ -176,155 +170,162 @@
             # 如果有service_name传入，那么覆盖yaml文件中的服务名称
             service_config[constant.SERVICE_INFO][constant.NAME] = service_name
         if version_name:
             service_config[constant.VERSION_NAME] = version_name
         if desc:
             service_config[constant.SERVICE_INFO][constant.SHORT_DESCRIPTION] = desc
         service_name = service_config.get(constant.SERVICE_INFO).get(constant.NAME)
-        data_list = self.service.list_service(service_name)
+        data_list = SupplierService.list_service(self.context, service_name)
         # 将相对路径替换成绝对路径
         image_path = os.path.join(os.path.dirname(file_path),
                                   service_config.get(constant.SERVICE_INFO).get(constant.IMAGE))
         if service_config.get(constant.OPERATION_METADATA):
-            for operation_template in service_config[constant.OPERATION_METADATA][self.CUSTOM_OPERATIONS][self.ACTIONS]:
-                # 将相对路径替换成绝对路径
-                operation_template_path = os.path.join(os.path.dirname(file_path),
-                                                       operation_template.get(self.TEMPLATE_URL))
-                operation_template[self.TEMPLATE_URL] = self._replace_file_path_with_url(operation_template_path)
+            # 判断CUSTOM_OPERATIONS是否存在
+            if CUSTOM_OPERATIONS in service_config[constant.OPERATION_METADATA]:
+                for operation_template in service_config[constant.OPERATION_METADATA][CUSTOM_OPERATIONS][ACTIONS]:
+                    # 将相对路径替换成绝对路径
+                    operation_template_path = os.path.join(os.path.dirname(file_path),
+                                                           operation_template.get(TEMPLATE_URL))
+                    operation_template[TEMPLATE_URL] = self._replace_file_path_with_url(operation_template_path)
         # 将部署物的id和version替换成正确的值
         if len(data_list.body.services) == 0:
             if icon:
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = icon
             else:
                 # 将服务logo的本地路径替换成Url
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = self._replace_file_path_with_url(image_path)
             # 将模版文件的本地路径替换成url
             for template in deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
                 # 将相对路径替换成绝对路径
-                template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
-                template[constant.URL] = self._replace_file_path_with_url(template_path)
+                if template.get(constant.URL):
+                    template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
+                    template[constant.URL] = self._replace_file_path_with_url(template_path)
             # 将SupplierDeployMetadata的路径做替换
             if constant.SUPPLIER_DEPLOY_METADATA in deploy_metadata_config:
                 supplier_deploy_metadata = deploy_metadata_config.get(constant.SUPPLIER_DEPLOY_METADATA)
                 if constant.SUPPLIER_TEMPLATE_CONFIGS in supplier_deploy_metadata:
                     for supplier_template_config in supplier_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS):
                         template_path = os.path.join(os.path.dirname(file_path),
                                                      supplier_template_config.get(constant.URL))
                         supplier_template_config[constant.URL] = self._replace_file_path_with_url(template_path)
-            data_create = self.service.create_service(service_config)
-            service_id = data_create.body.service_id
+            create_service_instance_result = SupplierService.create_service(self.context, service_config)
+            service_id = create_service_instance_result.body.service_id
             current_time = Util.get_current_time()
             print("===========================")
             print("Successfully created a new service!")
             print("The service name:", service_name)
             print("The service id:", service_id)
             print("Completion time:", current_time)
             print("===========================")
         else:
             service_id = data_list.body.services[0].service_id
             if icon:
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = icon
             else:
                 image_url_existed = self._get_service_logo_url(service_name)
-                result_image = file.check_file_repeat(image_url_existed, image_path)
+                result_image = FileService.check_file_repeat(image_url_existed, image_path)
                 # 检查服务logo是否重复，重复则不再上传，直接使用原有Url
                 if result_image:
                     image_url = image_url_existed
                 else:
                     image_url = self._replace_file_path_with_url(image_path)
                 service_config[constant.SERVICE_INFO][constant.IMAGE] = image_url
+
             service_deploy_metadata = json.loads(self._get_template_url_data(service_name))
             if service_deploy_metadata and service_deploy_metadata.get(constant.TEMPLATE_CONFIGS):
                 name_url_mapping = {template[constant.NAME]: template[constant.URL] for template in
                                     service_deploy_metadata.get(constant.TEMPLATE_CONFIGS)}
                 # 检查模版文件是否重复，重复则不再上传，直接使用原有Url
                 for template in service_config[constant.DEPLOY_METADATA][constant.TEMPLATE_CONFIGS]:
                     if template[constant.NAME] in name_url_mapping:
                         # 将相对路径替换成绝对路径
                         template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
-                        result_template = file.check_file_repeat(name_url_mapping[template[constant.NAME]],
+                        result_template = FileService.check_file_repeat(name_url_mapping[template[constant.NAME]],
                                                                  template_path)
                         if result_template:
                             template[constant.URL] = name_url_mapping.get(template[constant.NAME])
                         else:
                             template[constant.URL] = self._replace_file_path_with_url(template_path)
                     else:
-                        template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
-                        template[constant.URL] = self._replace_file_path_with_url(template_path)
+                        if template.get(constant.URL):
+                            template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
+                            template[constant.URL] = self._replace_file_path_with_url(template_path)
             else:
                 for template in deploy_metadata_config.get(constant.TEMPLATE_CONFIGS):
                     # 将相对路径替换成绝对路径
-                    template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
-                    template[constant.URL] = self._replace_file_path_with_url(template_path)
+                    if template.get(constant.URL):
+                        template_path = os.path.join(os.path.dirname(file_path), template.get(constant.URL))
+                        template[constant.URL] = self._replace_file_path_with_url(template_path)
 
             # 将SupplierDeployMetadata的路径做替换
             if constant.SUPPLIER_DEPLOY_METADATA in deploy_metadata_config:
                 supplier_deploy_metadata = deploy_metadata_config.get(constant.SUPPLIER_DEPLOY_METADATA)
                 # 已存在的服务的supplier_template_configs
                 service_supplier_template_configs = service_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS)
                 if service_supplier_template_configs:
                     name_url_mapping = {template[constant.NAME]: template[constant.URL] for template in
                                         service_supplier_template_configs}
                     for supplier_template_config in supplier_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS):
                         if supplier_template_config[constant.NAME] in name_url_mapping:
                             template_path = os.path.join(os.path.dirname(file_path),
                                                          supplier_template_config.get(constant.URL))
-                            result_template = file.check_file_repeat(
+                            result_template = FileService.check_file_repeat(
                                 name_url_mapping[supplier_template_config[constant.NAME]],
                                 template_path)
                             if result_template:
                                 supplier_template_config[constant.URL] = name_url_mapping.get(
                                     supplier_template_config[constant.NAME])
                             else:
                                 supplier_template_config[constant.URL] = self._replace_file_path_with_url(
                                     template_path)
                         else:
                             supplier_template_config[constant.URL] = self._replace_file_path_with_url(
                                 template_path)
                 else:
                     # 已有服务中没有对应的SUPPLIER_TEMPLATE_CONFIGS
-                    for supplier_template_config in supplier_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS):
-                        template_path = os.path.join(os.path.dirname(file_path),
-                                                     supplier_template_config.get(constant.URL))
-                        supplier_template_config[constant.URL] = self._replace_file_path_with_url(template_path)
+                    if supplier_deploy_metadata and constant.SUPPLIER_TEMPLATE_CONFIGS in supplier_deploy_metadata:
+                        for supplier_template_config in supplier_deploy_metadata.get(constant.SUPPLIER_TEMPLATE_CONFIGS):
+                            template_path = os.path.join(os.path.dirname(file_path),
+                                                         supplier_template_config.get(constant.URL))
+                            supplier_template_config[constant.URL] = self._replace_file_path_with_url(template_path)
 
             # 状态为Draft或者Creating时，更新服务
             service_status = data_list.body.services[0].status
             if service_status == 'Draft' or service_status == 'Creating':
-                self.service.update_service(service_config, service_id)
+                SupplierService.update_service(self.context, service_config, service_id)
                 service_name = service_config.get(constant.SERVICE_INFO).get(constant.NAME)
                 current_time = Util.get_current_time()
                 print("===========================")
                 print("Successfully updated the service!")
                 print("The service name: ", service_name)
                 print("The service id: ", service_id)
                 print("Completion time: ", current_time)
                 print("===========================")
             else:
                 service_id = data_list.body.services[0].service_id
                 try:
-                    self.service.get_service(service_id, self.DRAFT)
+                    SupplierService.get_service(self.context, service_id, DRAFT)
                 except TeaException as e:
-                    if e.code == self.SERVICE_NOT_FOUND:
-                        self.service.create_service(service_config, service_id)
+                    if e.code == SERVICE_NOT_FOUND:
+                        SupplierService.create_service(self.context, service_config, service_id)
                     else:
                         raise
                 else:
-                    self.service.update_service(service_config, service_id)
+                    SupplierService.update_service(self.context, service_config, service_id)
                 current_time = Util.get_current_time()
                 print("===========================")
                 print("Successfully updated the service!")
                 print("The service name: ", service_name)
                 print("The service id: ", service_id)
                 print("Completion time: ", current_time)
                 print("===========================")
 
     def export_command(self, service_name, file_path, parameters):
-        artifact = ArtifactProcessor(self.region_id, self.access_key_id, self.access_key_secret)
-        data_yaml, deploy_metadata = self._get_service_detail(self.region_id, service_name)
+        artifact = ArtifactProcessor(self.context)
+        data_yaml, deploy_metadata = self._get_service_detail(self.context.region_id, service_name)
         supplier_deploy_metadata = deploy_metadata[constant.SUPPLIER_DEPLOY_METADATA]
         if data_yaml[constant.SERVICE][constant.DEPLOY_METADATA][constant.SUPPLIER_DEPLOY_METADATA]:
             data_yaml.setdefault(constant.ARTIFACT, {})
             i = 1
             for artifact_metadata in supplier_deploy_metadata:
                 if artifact_metadata == constant.ARTIFACT_RELATION:
                     relation = constant.ARTIFACT_RELATION
```

### Comparing `computenest-cli-1.1.9/computenest_cli.egg-info/PKG-INFO` & `computenest-cli-1.2.7/computenest_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computenest-cli
-Version: 1.1.9
+Version: 1.2.7
 Summary: A command line interface for running the compute nest project
 Home-page: 
 Author: Chuan Lin
 Author-email: zhaoshuaibo.zsb@alibaba-inc.com
 Description-Content-Type: text/markdown
 
 # ComputeNest-CLI
```

### Comparing `computenest-cli-1.1.9/setup.py` & `computenest-cli-1.2.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
 
 setup(
     name='computenest-cli',
-    version='1.1.9',
+    version='1.2.7',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'computenest-cli = computeNestSupplier.main:main'
+            'computenest-cli = computenestcli.main:main'
         ]
     },
     install_requires=requirements,
     description='A command line interface for running the compute nest project',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Chuan Lin',
```

