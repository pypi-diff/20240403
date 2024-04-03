# Comparing `tmp/jcci-0.0.9.tar.gz` & `tmp/jcci-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.9.tar", last modified: Tue Jul 11 13:55:43 2023, max compression
+gzip compressed data, was "jcci-0.1.0.tar", last modified: Wed Apr  3 09:29:42 2024, max compression
```

## Comparing `jcci-0.0.9.tar` & `jcci-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.631126 jcci-0.0.9/
--rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     3031 2023-07-11 13:55:43.630126 jcci-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.9/README.md
--rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.9/README.pypi.md
--rw-rw-rw-   0        0        0      710 2023-07-11 13:55:34.000000 jcci-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 13:55:43.631126 jcci-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.615131 jcci-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.624126 jcci-0.0.9/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.9/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.9/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    44672 2023-07-11 13:52:41.000000 jcci-0.0.9/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.629125 jcci-0.0.9/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     3031 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.948499 jcci-0.1.0/
+-rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3087 2024-04-03 09:29:42.946500 jcci-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3412 2024-04-03 09:26:49.000000 jcci-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1186 2023-12-15 07:51:52.000000 jcci-0.1.0/README.pypi.md
+-rw-rw-rw-   0        0        0      763 2024-04-03 09:18:17.000000 jcci-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:29:42.948499 jcci-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.912501 jcci-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.934500 jcci-0.1.0/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.0/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    38366 2024-04-03 09:21:22.000000 jcci-0.1.0/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.0/src/jcci/config.py
+-rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.0/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.0/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7847 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    38308 2024-04-03 09:15:40.000000 jcci-0.1.0/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4117 2023-08-07 08:01:30.000000 jcci-0.1.0/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.0/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.945500 jcci-0.1.0/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0     3087 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 09:29:42.000000 jcci-0.1.0/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 09:29:42.942499 jcci-0.1.0/test/
+-rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.0/test/test_case.py
```

### Comparing `jcci-0.0.9/LICENSE` & `jcci-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.0.9/PKG-INFO` & `jcci-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.9
-Summary: Java code commit impact analyze in pure Python
+Version: 0.1.0
+Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,17 +26,19 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: javalang>=0.13.0
+Requires-Dist: unidiff>=0.7.4
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
 #### Installation
 ```
@@ -45,22 +47,19 @@
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci import jcci
 
+# Compare different commits on the same branch
 jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+
 ```
 
-At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
+At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , upload analyze result file end with .cci, then can be displayed through the view.
 
 ##### CCI result
 ![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
 
 ##### CCI result tree view
 ![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
-
-#### Communication
-Communicate via Wechat:
-
-![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jcci-0.0.9/README.pypi.md` & `jcci-0.1.0/README.pypi.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,19 @@
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci import jcci
 
+# Compare different commits on the same branch
 jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+
 ```
 
-At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
+At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , upload analyze result file end with .cci, then can be displayed through the view.
 
 ##### CCI result
 ![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
 
 ##### CCI result tree view
 ![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
-
-#### Communication
-Communicate via Wechat:
-
-![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

### Comparing `jcci-0.0.9/pyproject.toml` & `jcci-0.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
-description = "Java code commit impact analyze in pure Python"
+description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
-requires-python = ">=3.5"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "javalang >= 0.13.0",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jcci-0.0.9/src/jcci/jcci.py` & `jcci-0.1.0/src/jcci/java_parse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,782 +1,655 @@
-# -*- coding: UTF-8 -*-
-import datetime
+import logging
 import json
-import os
-import sys
-import time
 import javalang
-from unidiff import PatchSet
-from .java_analyzer import JavaAnalyzer, JavaImports, JavaMethods, JavaDeclarators, JavaDiffResult
-import atexit
-
-sep = os.sep
-
-
-# get all java files
-def _get_java_files(dir_path):
-    file_lists = []
-    file_or_dir_list = os.walk(dir_path)
-    for filepath, dir_names, file_names in file_or_dir_list:
-        if '.git' in filepath or 'src' + sep + 'test' + sep in filepath:
-            continue
-        for filename in file_names:
-            if filename.endswith('.java'):
-                full_file_path = filepath + sep + filename
-                file_lists.append(full_file_path)
-    return file_lists
-
-
-# analyze and return：{
-# 	'filepath': '/path',
-# 	'package_name': 'com.tal.wangxiao.conan.admin.controller',
-# 	'imports': {
-# 		'start': 3,
-# 		'end': 10,
-# 		'imports': ['com.tal.wangxiao.conan.common.domain.ApiInfo',
-# 			'com.tal.wangxiao.conan.common.service.ApiService'
-# 		]
-# 	},
-# 	'class_name': 'ApiController',
-# 	'extends': 'ConanBaseController',
-# 	'implements': ['a', 'b'],
-# 	'declarators': [{
-# 		'type': 'ApiService',
-# 		'name': 'apiService',
-#       'line': 46,
-#       'contains_class': 'com.tal.wangxiao.conan.common.service.ApiService'
-# 	}],
-# 	'methods': [{
-# 		'name': 'list',
-# 		'start': 55,
-# 		'end': 62,
-# 		'content': 'public ApiResponse<PageInfoResponse<List<ApiInfo>>> list(ApiInfo api).....'
-#       'contains_class': {
-#           'com.tal.wangxiao.conan.common.service.ApiService': {
-#               'methods': ['selectApiList']
-#            }
-#        }
-#       'contains_declarators': ['abc','def']
-# 	}]
-# }
-#
-def _analyze_java_file(filepath, folder_name):
-    print(filepath)
-    import_list = []
-    with open(filepath, encoding='UTF-8') as fp:
-        file_content = fp.read()
-    lines = file_content.split('\n')
-    try:
-        tree = javalang.parse.parse(file_content)
-        package_name = tree.package.name
-        types = tree.types[0]
-        class_name = types.name
-    except Exception as e:
-        print(e.args)
-        print(str(e))
-        print(repr(e))
-        return None
-    # is controller or not
-    is_controller = False
-    base_request = ''
-    annotations = types.annotations
-    for annotation in annotations:
-        if 'Controller' in annotation.name:
-            is_controller = True
-        if 'RequestMapping' == annotation.name:
-            if type(annotation.element) != type([]):
-                if annotation.element is not None:
-                    if 'value' in annotation.element.attrs:
-                        base_request = annotation.element.value.replace('"', '')
-                    elif 'values' in annotation.element.attrs:
-                        # print(annotation.element.values)
-                        base_request = ' || '.join([literal.value for literal in annotation.element.values])
-            else:
-                base_request_list = []
-                for annotation_element in annotation.element:
-                    if annotation_element.name == 'value' or annotation_element.name == 'path':
-                        if 'values' in annotation_element.value.attrs:
-                            base_request_list += _get_element_with_values(annotation_element.value)
-                        else:
-                            base_request_list = [annotation_element.value.value.replace('"', '')]
-                if len(base_request_list) > 0:
-                    base_request = base_request_list[0]
-    if is_controller and not base_request.endswith('/'):
-        base_request += '/'
-    class_path = package_name + '.' + class_name
-    extends_name = types.extends.name \
-        if 'extends' in types.attrs and types.extends is not None \
-           and type(types.extends) != type([]) else None
-    extends_name_path = extends_name
-    implements_names = [implement.name for implement in types.implements] \
-        if 'implements' in types.attrs and types.implements is not None else None
-    implements_names_list = []
-    import_path_class_map = {}
-    for import_Obj in tree.imports:
-        import_path = import_Obj.path
-        if not import_path.startswith('com.'):
-            continue
-        if not import_Obj.wildcard and not import_Obj.static:
-            import_path_class = import_path.split('.')[-1]
-            import_path_class_map[import_path_class] = import_path
-            import_list.append(import_path)
-            if extends_name and import_path.endswith(extends_name):
-                extends_name_path = import_path
-            if implements_names and import_path_class in implements_names:
-                implements_names_list.append(import_path)
-    imports = JavaImports(
-        tree.imports[0].position.line if tree.imports else None,
-        tree.imports[-1].position.line if tree.imports else None,
-        tree.imports
-    )
-    fields = types.fields
-    fields_list = []
-    for field_obj in fields:
-        field_type = field_obj.type.name
-        field_declarators = field_obj.declarators[0].name
-        field_map = JavaDeclarators(field_type, field_declarators, field_obj.position.line)
-        if field_type in import_path_class_map.keys():
-            field_map.contains_class = import_path_class_map[field_type]
-        fields_list.append(field_map)
-
-    methods_list = []
-    methods_name_list = [method.name for method in types.methods]
-    for method_obj in types.methods:
-        method_name = method_obj.name
-        method_start_line = method_obj.position.line
-        if method_obj.annotations:
-            method_start_line = method_obj.annotations[0].position.line
-        method_end_line = _get_method_end_line_new(method_obj)
-        method_content = lines[method_start_line - 1: method_end_line]
-        # method is api or not
-        is_api = False
-        api_path_list = []
-        if is_controller:
-            method_annotations = method_obj.annotations
-            req_method_list = []
-            method_api_path = []
-            for method_annotation in method_annotations:
-                if 'Mapping' in method_annotation.name:
-                    is_api = True
-                    if method_annotation.name != 'RequestMapping':
-                        req_method_list.append(method_annotation.name.replace('Mapping', ''))
-                    else:
-                        if type(method_annotation.element) == type([]):
-                            for method_annotation_element in method_annotation.element:
-                                if 'name' in method_annotation_element.attrs and method_annotation_element.name == 'method':
-                                    method_annotation_element_value = method_annotation_element.value
-                                    if 'member' in method_annotation_element_value.attrs:
-                                        req_method_list.append(method_annotation_element_value.member)
-                                    elif 'values' in method_annotation_element_value.attrs:
-                                        method_annotation_element_values = method_annotation_element_value.values
-                                        req_method_list += [method_annotation_element_temp.member for
-                                                            method_annotation_element_temp in
-                                                            method_annotation_element_values
-                                                            if 'member' in method_annotation_element_temp.attrs]
-                    if type(method_annotation.element) != type([]):
-                        if method_annotation.element is not None and method_annotation.element.value is not None:
-                            method_api_path += [method_annotation.element.value.replace('"', '')]
-                    else:
-                        method_api_path_list = [method_annotation_element.value for method_annotation_element in
-                                                method_annotation.element
-                                                if
-                                                method_annotation_element.name == 'path' or method_annotation_element.name == 'value']
-                        if len(method_api_path_list) > 0:
-                            method_api_path_obj = method_api_path_list[0]
-                            if 'value' in method_api_path_obj.attrs:
-                                method_api_path += [method_api_path_obj.value.replace('"', '')]
-                            else:
-                                if 'values' in method_api_path_obj.attrs:
-                                    for method_api_value in method_api_path_obj.values:
-                                        if type(method_api_value).__name__ == "BinaryOperation":
-                                            operandl = method_api_value.operandl
-                                            operandr = method_api_value.operandr
-                                            operandl_str = _get_api_part_route(operandl)
-                                            operandr_str = _get_api_part_route(operandr)
-                                            method_api_path += [operandl_str + operandr_str]
-                                        else:
-                                            method_api_path += [method_api_value.value.replace('"', '')]
-                                else:
-                                    method_api_path += [method_name + '/cci-unknown']
-            if len(method_api_path) == 0:
-                method_api_path = ['/']
-            for method_api_path_obj in method_api_path:
-                if method_api_path_obj.startswith('/'):
-                    method_api_path_obj = method_api_path_obj[1:]
-                api_path = base_request + method_api_path_obj
-                if api_path.endswith('/'):
-                    api_path = api_path[0:-1]
-                for req_method_temp in req_method_list:
-                    full_api = '[' + req_method_temp + ']' + api_path
-                    api_path_list.append(full_api)
-        method_map = JavaMethods(method_name, method_start_line, method_end_line, method_content, is_api, api_path_list)
-        # imports in this method or not
-        for import_path_class in import_path_class_map.keys():
-            if import_path_class in method_content:
-                if import_path_class_map[import_path_class] not in method_map['contains_class']:
-                    method_map.contains_class[import_path_class_map[import_path_class]] = {}
-        # declarator in this method or not
-        declarator_tmp_final = None
-        for declarator_tmp in fields_list:
-            declarator_tmp_final = declarator_tmp
-            if declarator_tmp.name in str(method_content):
-                if declarator_tmp.contains_class != '':
-                    class_method_list = []
-                    if declarator_tmp.contains_class not in method_map.contains_class.keys():
-                        method_map.contains_class[declarator_tmp.contains_class] = {}
-                    else:
-                        if 'methods' in method_map.contains_class[declarator_tmp.contains_class].keys():
-                            class_method_list = method_map.contains_class[declarator_tmp.contains_class]['methods']
-                    for method_content_line in method_content:
-                        if declarator_tmp.name in method_content_line and len(
-                                method_content_line.split(declarator_tmp.name + '.')) > 1:
-                            class_method = method_content_line.split(declarator_tmp.name + '.')[1].split('(')[0]
-                            if class_method not in class_method_list:
-                                class_method_list.append(class_method)
-                    method_map.contains_class[declarator_tmp.contains_class]['methods'] = class_method_list
-                else:
-                    method_map.add_declarators(declarator_tmp_final.__dict__)
-        # class method used in this class
-        for methods_name in methods_name_list:
-            for method_content_line in method_content:
-                if ' ' + methods_name + '(' in method_content_line and not method_content_line.endswith("{"):
-                    if class_path not in method_map.contains_class.keys():
-                        method_map.contains_class[class_path] = {'methods': [methods_name]}
+from src.jcci.database import SqliteHelper
+from src.jcci.constant import ENTITY, RETURN_TYPE, PARAMETERS, BODY, METHODS, FIELDS, PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN, JAVA_BASIC_TYPE
+
+logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
+
+class JavaParse(object):
+    def __init__(self, db_path, project_id):
+        self.project_id = project_id
+        self.sqlite = SqliteHelper(db_path)
+
+    def _handle_extends(self, extends, import_list: list, package_name):
+        if isinstance(extends, list):
+            extends_package_class_list = []
+            extends_class = extends[0].name
+            extends_package_class = self._get_extends_class_full_package(extends_class, import_list, package_name)
+            extends_package_class_list.append(extends_package_class)
+            if 'arguments' in extends[0].attrs and extends[0].arguments:
+                extends_arguments = extends[0].arguments
+                extends_argument_classes = []
+                for extends_argument in extends_arguments:
+                    if type(extends_argument) == javalang.tree.TypeArgument:
+                        extends_argument_class = extends_argument.type.name
                     else:
-                        if 'methods' in method_map.contains_class[class_path].keys():
-                            method_map.contains_class[class_path]['methods'].append(methods_name)
-                        else:
-                            method_map.contains_class[class_path] = {'methods': [methods_name]}
-        if 'body' in method_obj.attrs and method_obj.body is not None:
-            for method_body in method_obj.body:
-                if str(type(method_body)) == "<class 'javalang.tree.LocalVariableDeclaration'>":
-                    if 'type' in method_body.attrs and 'name' in method_body.type.attrs \
-                            and method_body.type.name in import_path_class_map.keys() \
-                            and 'declarators' in method_body.attrs \
-                            and type(method_body.declarators) == type([]) \
-                            and len(method_body.declarators) > 0:
-                        class_method_list = []
-                        if import_path_class_map.get(method_body.type.name) not in method_map.contains_class.keys():
-                            method_map.contains_class[import_path_class_map.get(method_body.type.name)] = {}
-                        else:
-                            if 'methods' in method_map.contains_class[
-                                import_path_class_map.get(method_body.type.name)].keys():
-                                class_method_list = \
-                                    method_map.contains_class[import_path_class_map.get(method_body.type.name)][
-                                        'methods']
-                        for method_content_line in method_content:
-                            if method_body.declarators[0].name in method_content_line and len(
-                                    method_content_line.split(method_body.declarators[0].name + '.')) > 1:
-                                class_method = \
-                                    method_content_line.split(method_body.declarators[0].name + '.')[1].split('(')[0]
-                                if class_method not in class_method_list:
-                                    class_method_list.append(class_method)
-                        method_map.contains_class[import_path_class_map.get(method_body.type.name)][
-                            'methods'] = class_method_list
-                        # method_obj.append(method_body.declarators[0].name)
-        methods_list.append(method_map)
-    file_analyze = JavaAnalyzer(filepath.replace(sep, '/').replace(folder_name + '/', ''), package_name, class_name,
-                                extends_name_path, is_controller)
-    file_analyze.imports = imports
-    file_analyze.implements = implements_names_list
-    file_analyze.declarators = fields_list
-    file_analyze.methods = methods_list
-    return file_analyze
-
-
-def _get_element_with_values(method_api_path_obj):
-    method_api_path = []
-    for method_api_value in method_api_path_obj.values:
-        if type(method_api_value).__name__ == "BinaryOperation":
-            operandl = method_api_value.operandl
-            operandr = method_api_value.operandr
-            operandl_str = _get_api_part_route(operandl)
-            operandr_str = _get_api_part_route(operandr)
-            method_api_path += [operandl_str.replace('"', '') + operandr_str.replace('"', '')]
+                        extends_argument_class = extends_argument.name
+                    extends_argument_package_class = self._get_extends_class_full_package(extends_argument_class, import_list, package_name)
+                    extends_argument_classes.append(extends_argument_package_class)
+                extends_package_class_list += extends_argument_classes
+                return extends_package_class + '<' + ','.join(extends_argument_classes) + '>', extends_package_class_list
+            else:
+                return extends_package_class, [extends_package_class]
         else:
-            method_api_path += [method_api_value.value.replace('"', '')]
-    return method_api_path
-
+            extends_class = self._get_extends_class_full_package(extends.name, import_list, package_name)
+            return extends_class, [extends_class]
 
-def _get_api_part_route(part):
-    part_class = type(part).__name__
-    if part_class == 'MemberReference':
-        return part.member
-    elif part_class == 'Literal':
-        return part.value
-
-
-def _get_method_end_line_new(method_obj):
-    method_end_line = method_obj.position.line
-    while True:
-        if isinstance(method_obj, list):
-            if None in method_obj:
-                method_obj.remove(None)
-            if len(method_obj) == 0:
-                break
-            length = len(method_obj)
-            for i in range(0, length):
-                temp = method_obj[length-1-i]
-                if temp is not None:
-                    method_obj = temp
-                    break
-            if method_obj is None:
-                break
-        if isinstance(method_obj, list):
-            continue
-        if hasattr(method_obj, 'position') \
-                and method_obj.position is not None \
-                and method_obj.position.line > method_end_line:
-            method_end_line = method_obj.position.line
-        if hasattr(method_obj, 'children'):
-            method_obj = method_obj.children
+    def _get_extends_class_full_package(self, extends_class, import_list, package_name):
+        extends_in_imports = [import_obj for import_obj in import_list if extends_class in import_obj['import_path']]
+        return extends_in_imports[0]['import_path'] if extends_in_imports else package_name + '.' + extends_class
+
+    def _parse_class(self, node, filepath: str, package_name: str, import_list: list, commit_or_branch: str):
+        # 处理class信息
+        documentation = node.documentation
+        class_name = node.name
+        package_class = package_name + '.' + node.name
+        class_type = type(node).__name__.replace('Declaration', '')
+        access_modifier = [m for m in list(node.modifiers) if m.startswith('p')][0] if list([m for m in list(node.modifiers) if m.startswith('p')]) else 'public'
+        annotations_json = json.dumps(node.annotations, default=lambda obj: obj.__dict__)
+        is_controller, controller_base_url = self._judge_is_controller(node.annotations)
+        extends_package_class = None
+        if 'extends' in node.attrs and node.extends:
+            extends_package_class, extends_package_class_list = self._handle_extends(node.extends, import_list, package_name)
+            package_path = package_class.replace('.', '/') + '.java'
+            base_filepath = filepath.replace(package_path, '')
+            for extends_package_class_item in extends_package_class_list:
+                extends_package = '.'.join(extends_package_class_item.split('.')[0: -1])
+                extends_class_name = extends_package_class_item.split('.')[-1]
+                extends_class_filepath = base_filepath + extends_package_class_item.replace('.', '/') + '.java'
+                extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id={self.project_id} and package_name = "{extends_package}" and class_name = "{extends_class_name}" and filepath= "{extends_class_filepath}"')
+                # if not extends_class_db:
+                # self.parse_java_file(extends_class_filepath, commit_or_branch)
+        implements = ','.join([implement.name for implement in node.implements]) if 'implements' in node.attrs and node.implements else None
+        class_id, new_add = self.sqlite.add_class(filepath.replace('\\', '/'), access_modifier, class_type, class_name, package_name, extends_package_class, self.project_id, implements, annotations_json, documentation, is_controller, controller_base_url, commit_or_branch)
+        return class_id, new_add
+
+    def _parse_imports(self, imports):
+        import_list = []
+        for import_decl in imports:
+            import_obj = {
+                'import_path': import_decl.path,
+                'is_static': import_decl.static,
+                'is_wildcard': import_decl.wildcard,
+                'start_line': import_decl.position.line,
+                'end_line': import_decl.position.line
+            }
+            import_list.append(import_obj)
+        return import_list
+
+    def _parse_fields(self, fields, package_name, class_id, import_map):
+        field_list = []
+        for field_obj in fields:
+            field_annotations = json.dumps(field_obj.annotations, default=lambda obj: obj.__dict__)
+            access_modifier = [m for m in list(field_obj.modifiers) if m.startswith('p')][0] if list([m for m in list(field_obj.modifiers) if m.startswith('p')]) else 'public'
+            field_name = field_obj.declarators[0].name
+            field_type: str = field_obj.type.name
+            if field_type.lower() not in JAVA_BASIC_TYPE:
+                if field_type in import_map.keys():
+                    field_type = import_map.get(field_type)
+                else:
+                    import_map[field_obj.type.name] = package_name + '.' + field_obj.type.name
+                    field_type = package_name + '.' + field_type
+            is_static = 'static' in list(field_obj.modifiers)
+            documentation = field_obj.documentation
+            start_line = field_obj.position.line if not field_obj.annotations else field_obj.annotations[0].position.line
+            end_line = field_obj.position.line
+            field_obj = {
+                'class_id': class_id,
+                'project_id': self.project_id,
+                'annotations': field_annotations,
+                'access_modifier': access_modifier,
+                'field_type': field_type,
+                'field_name': field_name,
+                'is_static': is_static,
+                'documentation': documentation,
+                'start_line': start_line,
+                'end_line': end_line
+            }
+            field_list.append(field_obj)
+        self.sqlite.update_data(f'DELETE FROM field where class_id={class_id}')
+        self.sqlite.insert_data('field', field_list)
+        return field_list
+
+    def _parse_method(self, methods, lines, class_id, import_map, field_map):
+        # 处理 methods
+        all_method = []
+        class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
+        base_url = class_db['controller_base_url'] if class_db['controller_base_url'] else ''
+        method_name_entity_map = {method.name: method for method in methods}
+        for method_obj in methods:
+            method_invocation = {}
+            variable_map = {}
+            method_name = method_obj.name
+            documentation = method_obj.documentation  # document
+            annotations = json.dumps(method_obj.annotations, default=lambda obj: obj.__dict__)  # annotations
+            is_api, api_path = self._judge_is_api(method_obj.annotations, base_url, method_name)
+            access_modifier = [m for m in list(method_obj.modifiers) if m.startswith('p')][0] if list([m for m in list(method_obj.modifiers) if m.startswith('p')]) else 'public'
+            is_static = 'static' in list(method_obj.modifiers)
+            is_abstract = 'abstract' in list(method_obj.modifiers)
+            # 处理返回对象
+            return_type = self._deal_declarator_type(method_obj.return_type, import_map, method_invocation, RETURN_TYPE)
+            method_start_line = method_obj.position.line
+            if method_obj.annotations:
+                method_start_line = method_obj.annotations[0].position.line
+            method_end_line = self._get_method_end_line(method_obj)
+            method_body = lines[method_start_line - 1: method_end_line + 1]
+            # 处理参数
+            parameters = []
+            for parameter in method_obj.parameters:
+                parameter_obj = {
+                    'parameter_type': self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS),
+                    'parameter_name': parameter.name,
+                    'parameter_varargs': parameter.varargs
+                }
+                parameters.append(parameter_obj)
+            parameters_map = {parameter['parameter_name']: parameter['parameter_type'] for parameter in parameters}
+
+            # 处理方法体
+            if method_obj.body:
+                for body in method_obj.body:
+                    for path, node in body.filter(javalang.tree.VariableDeclaration):
+                        var_declarator = node.declarators[0].name
+                        var_declarator_type = self._deal_declarator_type(node.type, import_map, method_invocation, BODY)
+                        variable_map[var_declarator] = var_declarator_type
+                    for path, node in body.filter(javalang.tree.MethodInvocation):
+                        qualifier = node.qualifier
+                        member = node.member
+                        # 类静态方法调用
+                        if not qualifier and not member[0].islower():
+                            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            # todo a.b.c
+                            if node.selectors is None:
+                                continue
+                            for selector in node.selectors:
+                                selector_member = selector.member
+                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                                selector_line = selector.position.line
+                                selector_method = f'{selector_member}({",".join(selector_arguments)})'
+                                self._add_method_used_to_method_invocation(method_invocation, qualifier_type, selector_method, [selector_line])
+                        elif qualifier:
+                            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            node_line = node.position.line
+                            node_method = f'{member}({",".join(node_arguments)})'
+                            self._add_method_used_to_method_invocation(method_invocation, qualifier_type, node_method, [node_line])
+                        # 在一个类的方法或父类方法
+                        elif member:
+                            class_db = self.sqlite.select_data(f'SELECT * FROM class where class_id={class_id} limit 1')[0]
+                            package_class = class_db['package_name'] + '.' + class_db['class_name']
+                            node_line = node.position.line
+                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            # todo 同级方法, 判断参数长度，不精确
+                            if method_name_entity_map.get(member):
+                                same_class_method = None
+                                max_score = -float('inf')
+                                for method_item in methods:
+                                    if method_item.name != member or len(node.arguments) != len(method_item.parameters):
+                                        continue
+                                    method_item_param_types = [self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS) for parameter in method_item.parameters]
+                                    score = self._calculate_similar_score_method_params(node_arguments, method_item_param_types)
+                                    if score > max_score:
+                                        max_score = score
+                                        same_class_method = method_item
+                                if same_class_method:
+                                    node_arguments = self._deal_var_type(same_class_method.parameters, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                                    node_method = f'{member}({",".join(node_arguments)})'
+                                    self._add_method_used_to_method_invocation(method_invocation, package_class, node_method, [node_line])
+                            # todo 继承方法
+                            elif class_db['extends_class']:
+                                extends_package_class, method_params = self._find_method_in_extends(class_db['extends_class'], member, node_arguments)
+                                if not extends_package_class:
+                                    self._add_method_used_to_method_invocation(method_invocation, extends_package_class, method_params, [node_line])
+
+                    # for path, node in body.filter(javalang.tree.SuperMethodInvocation):
+                    #     print(node)
+                    # for path, node in body.filter(javalang.tree.TypeArgument):
+                    #     print(node)
+                    # for path, node in body.filter(javalang.tree.TypeParameter):
+                    #     print(node)
+                    # for path, node in body.filter(javalang.tree.FieldDeclaration):
+                    #     print(node)
+            method_db = {
+                'class_id': class_id,
+                'project_id': self.project_id,
+                'annotations': annotations,
+                'access_modifier': access_modifier,
+                'return_type': return_type,
+                'method_name': method_name,
+                'parameters': json.dumps(parameters),
+                'body': json.dumps(method_body),
+                'method_invocation_map': json.dumps(method_invocation),
+                'is_static': is_static,
+                'is_abstract': is_abstract,
+                'is_api': is_api,
+                'api_path': json.dumps(api_path),
+                'start_line': method_start_line,
+                'end_line': method_end_line,
+                'documentation': documentation
+            }
+            all_method.append(method_db)
+        self.sqlite.update_data(f'DELETE FROM methods where class_id={class_id}')
+        self.sqlite.insert_data('methods', all_method)
+
+    def _find_method_in_extends(self, extend_package_class: str, method_name: str, method_arguments):
+        if not extend_package_class:
+            return None, None
+        # 查表有没有记录
+        extend_package = '.'.join(extend_package_class.split('.')[0: -1])
+        extend_class = extend_package_class.split('.')[-1]
+        extend_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name="{extend_package}" '
+                                                  f'AND class_name="{extend_class}" '
+                                                  f'AND project_id={self.project_id} limit 1')
+
+        if not extend_class_db:
+            return None, None
+        extend_class_entity = extend_class_db[0]
+        extend_class_id = extend_class_entity['class_id']
+        methods_db_list = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id={extend_class_id} and method_name = "{method_name}"')
+        if not methods_db_list and not extend_class_entity['extends_class']:
+            return None, None
+        if not methods_db_list:
+            return self._find_method_in_extends(extend_class_entity['extends_class'], method_name, method_arguments)
         else:
-            break
-    return method_end_line
+            filter_methods = [method for method in methods_db_list if len(json.loads(method['parameters'])) == len(method_arguments)]
+            if not filter_methods:
+                return self._find_method_in_extends(extend_class_entity['extends_class'], method_name, method_arguments)
+            package_class = extend_class_entity['package_name'] + '.' + extend_class_entity['class_name']
+            if len(filter_methods) == 1:
+                method_db = filter_methods[0]
+                method_params = f'{method_db["method_name"]}({",".join([param["parameter_type"] for param in json.loads(method_db["parameters"])])})'
+                return package_class, method_params
+            else:
+                max_score = -float('inf')
+                max_score_method = None
+                for method_db in filter_methods:
+                    method_db_params = [param["parameter_type"] for param in json.loads(method_db["parameters"])]
+                    score = self._calculate_similar_score_method_params(method_arguments, method_db_params)
+                    if score > max_score:
+                        max_score = score
+                        max_score_method = method_db
+                if max_score_method is None:
+                    max_score_method = filter_methods[0]
+                method_params = f'{max_score_method["method_name"]}({",".join([param["parameter_type"] for param in json.loads(max_score_method["parameters"])])})'
+                return package_class, method_params
+
+    def _calculate_similar_score_method_params(self, except_method_param_list, method_param_list):
+        score = 0
+        positions = {}
+
+        # 记录list1中每个元素的位置
+        for i, item in enumerate(except_method_param_list):
+            positions[item] = i
+
+        # 遍历list2,计算分数
+        for i, item in enumerate(method_param_list):
+            if item in positions:
+                score += 1
+                score -= abs(i - positions[item])
 
+        return score
 
-def _get_method_end_line(method_obj):
-    method_end_line = method_obj.position.line
-    if method_obj.body is not None and len(method_obj.body) > 0:
-        method_end_line = method_obj.body[-1].position.line
-        method_body = method_obj.body[-1]
+    def _get_method_end_line(self, method_obj):
+        method_end_line = method_obj.position.line
         while True:
-            method_obj_dict = method_body.__dict__
-            method_last_attr = method_body.attrs[-1]
-            if type(method_obj_dict[method_last_attr]) == type([]):
-                if len(method_obj_dict[method_last_attr]) < 1:
+            if isinstance(method_obj, list):
+                if None in method_obj:
+                    method_obj.remove(None)
+                if len(method_obj) == 0:
+                    break
+                length = len(method_obj)
+                for i in range(0, length):
+                    temp = method_obj[length - 1 - i]
+                    if temp is not None:
+                        method_obj = temp
+                        break
+                if method_obj is None:
                     break
-                method_body = method_obj_dict[method_last_attr][-1]
-                if type(method_body.__dict__[method_body.attrs[-1]]) == type([]) \
-                        and len(method_body.__dict__[method_body.attrs[-1]]) == 0 \
-                        and len(method_obj_dict[method_last_attr]) > 1:
-                    method_body = method_obj_dict[method_last_attr][-2]
-            elif type(method_obj_dict[method_last_attr]) == type(''):
-                return method_end_line + 1
+            if isinstance(method_obj, list):
+                continue
+            if hasattr(method_obj, 'position') \
+                    and method_obj.position is not None \
+                    and method_obj.position.line > method_end_line:
+                method_end_line = method_obj.position.line
+            if hasattr(method_obj, 'children'):
+                method_obj = method_obj.children
             else:
-                if method_obj_dict[method_last_attr] is None:
-                    if '_position' in method_obj_dict.keys():
-                        method_end_line = method_obj_dict['_position'].line
-                    return method_end_line + 1
-                method_obj_dict_dict = method_obj_dict[method_last_attr].__dict__
-                method_body = method_obj_dict[method_last_attr]
-                if '_position' in method_obj_dict_dict.keys():
-                    method_end_line = method_obj_dict[method_last_attr].position.line
-                else:
-                    return method_end_line + 1
-    return method_end_line + 1
+                break
+        return method_end_line
 
+    def _get_element_value(self, method_element):
+        method_api_path = []
+        if type(method_element).__name__ == 'BinaryOperation':
+            operandl = method_element.operandl
+            operandr = method_element.operandr
+            operandl_str = self._get_api_part_route(operandl)
+            operandr_str = self._get_api_part_route(operandr)
+            method_api_path = [operandl_str + operandr_str]
+        elif type(method_element).__name__ == 'MemberReference':
+            method_api_path = [method_element.member.replace('"', '')]
+        elif type(method_element).__name__ == 'ElementArrayValue':
+            method_api_path = self._get_element_with_values(method_element)
+        elif method_element.value is not None:
+            method_api_path = [method_element.value.replace('"', '')]
+        return method_api_path
+
+    def _get_element_with_values(self, method_api_path_obj):
+        result = []
+        for method_api_value in method_api_path_obj.values:
+            result += self._get_element_value(method_api_value)
+        return result
+
+    def _get_api_part_route(self, part):
+        part_class = type(part).__name__
+        if part_class == 'MemberReference':
+            return part.member.replace('"', '')
+        elif part_class == 'Literal':
+            return part.value.replace('"', '')
+
+    def _judge_is_controller(self, annotation_list):
+        is_controller = any('Controller' in annotation.name for annotation in annotation_list)
+        base_request = ''
+        if not is_controller:
+            return is_controller, base_request
+        for annotation in annotation_list:
+            if 'RequestMapping' != annotation.name:
+                continue
+            if annotation.element is None:
+                continue
+            if isinstance(annotation.element, list):
+                base_request_list = []
+                for annotation_element in annotation.element:
+                    if annotation_element.name != 'value' and annotation_element.name != 'path':
+                        continue
+                    if 'values' in annotation_element.value.attrs:
+                        base_request_list += self._get_element_with_values(annotation_element.value)
+                    else:
+                        base_request_list += self._get_element_value(annotation_element.value)
+                if len(base_request_list) > 0:
+                    base_request = base_request_list[0]
+            else:
+                if 'value' in annotation.element.attrs:
+                    base_request = annotation.element.value.replace('"', '')
+                elif 'values' in annotation.element.attrs:
+                    base_request = ' || '.join([literal.value for literal in annotation.element.values])
+        if is_controller and not base_request.endswith('/'):
+            base_request += '/'
+        return is_controller, base_request
 
-# handle diff result text
-def _get_diff_results(diff_file, head_java_file_analyze_result, base_java_file_analyze_result):
-    with open(diff_file, encoding='UTF-8') as f:
-        diff_text = f.read()
-    patch_set = PatchSet(diff_text)
-    patch_results = []
-    for patch in patch_set:
-        patch_result = _analyze_diff_patch(patch, head_java_file_analyze_result, base_java_file_analyze_result)
-        if patch_result is not None:
-            patch_results.append(patch_result)
-    return patch_results
-
-
-def _analyze_diff_patch(patch, head_java_file_analyze_result, base_java_file_analyze_result):
-    if '.git' in patch.path or 'src' + sep + 'test' + sep in patch.path or not patch.path.endswith('.java'):
-        return None
-    line_num_added, line_content_added, line_num_removed, line_content_removed = _diff_patch_lines(patch)
-    java_file_path = patch.path
-    methods_impacted = {}
-    declarators_impacted = {}
-    _diff_patch_impact(methods_impacted, declarators_impacted, head_java_file_analyze_result, java_file_path,
-                       line_num_added, 'ADD')
-    _diff_patch_impact(methods_impacted, declarators_impacted, base_java_file_analyze_result, java_file_path,
-                       line_num_removed, 'DEL')
-    diff_result = JavaDiffResult(patch.path, line_num_added, line_content_added, line_num_removed, line_content_removed)
-    diff_result.changed_methods = methods_impacted
-    diff_result.changed_declarators = declarators_impacted
-    return diff_result
-
-
-def _diff_patch_impact(methods_impacted, declarators_impacted, java_file_analyze_result, java_file_path, line_num_mode,
-                       mode):
-    java_analyze = java_file_analyze_result[
-        java_file_path] if java_file_path in java_file_analyze_result.keys() else None
-    if java_analyze is not None:
-        java_methods = java_analyze.methods
-        for line_num_index in range(0, len(line_num_mode)):
-            line_num = line_num_mode[line_num_index]
-            line_num_in_method = False
-            for method in java_methods:
-                if method.start <= line_num <= method.end:
-                    line_num_in_method = True
-                    if method.name not in methods_impacted.keys():
-                        method.diff_impact = mode
-                        methods_impacted[method.name] = method.__dict__
-            if not line_num_in_method:
-                java_declarators = java_analyze.declarators
-                for declarator in java_declarators:
-                    if line_num == declarator.line:
-                        declarator.diff_impact = mode
-                        declarators_impacted[declarator.name] = declarator.__dict__
-
-
-def _diff_patch_lines(patch):
-    line_num_added = []
-    line_num_removed = []
-    line_content_added = []
-    line_content_removed = []
-    for hunk in patch:
-        if hunk.added > 0:
-            targets = hunk.target
-            target_start = hunk.target_start
-            for i in range(0, len(targets)):
-                if targets[i].startswith('+') \
-                        and not targets[i][1:].strip().startswith('*') \
-                        and not targets[i][1:].strip().startswith('//') \
-                        and not targets[i][1:].strip().startswith('import '):
-                    line_num_added.append(target_start + i + 1)
-                    line_content_added.append(targets[i][1:])
-        if hunk.removed > 0:
-            sources = hunk.source
-            source_start = hunk.source_start
-            for i in range(0, len(sources)):
-                if sources[i].startswith('-') \
-                        and not sources[i][1:].strip().startswith('*') \
-                        and not sources[i][1:].strip().startswith('//') \
-                        and not sources[i][1:].strip().startswith('import '):
-                    line_num_removed.append(source_start + i + 1)
-                    line_content_removed.append(sources[i][1:])
-    return line_num_added, line_content_added, line_num_removed, line_content_removed
-
-
-# judge in imports, java_analyze类是不是再java_file_analyze里面
-def _in_import(java_analyze, java_file_analyze):
-    if java_file_analyze is None or java_file_analyze.imports is None \
-            or java_file_analyze.imports.imports is None:
-        return False, False
-    class_path = java_analyze.package_name + '.' + java_analyze.class_name
-    implements = java_analyze.implements
-    imports = java_file_analyze.imports.imports
-    class_path_analyze = java_file_analyze.package_name + '.' + java_file_analyze.class_name
-    if class_path_analyze == class_path:
-        return True, True
-    if java_file_analyze.package_name == java_analyze.package_name:
-        return True, True
-    for import_obj in imports:
-        if not import_obj.wildcard:
-            if class_path == import_obj.path or import_obj.path in implements:
-                return True, True
-        else:
-            class_path_parent = '.'.join(class_path.split('.')[0: -1])
-            if class_path_parent == import_obj.path:
-                return True, False
-    for declarator in java_file_analyze.declarators:
-        if declarator.type == java_analyze.class_name:
-            return True, False
-    return False, False
-
-
-def _get_commit_project_files(commit_id, folder_name):
-    java_file_analyze_result = {}
-    git_bash = 'cd ' + folder_name + ' && ' + 'git reset --hard ' + commit_id
-    os.system(git_bash)
-    time.sleep(1)
-    commit_files = _get_java_files(folder_name)
-
-    for commit_file in commit_files:
-        commit_file_result = _analyze_java_file(commit_file, folder_name)
-        if commit_file_result is not None:
-            java_file_analyze_result[commit_file.replace(folder_name + sep, '').replace(sep, '/')] = commit_file_result
-    return java_file_analyze_result
-
-
-def _gen_treemap_data(diff_results, commit_first, commit_second):
-    flare = {'name': commit_second + '..' + commit_first, 'children': []}
-    api_list = []
-    diff_results.reverse()
-    diff_filepath = []
-    for diff_result in diff_results:
-        if diff_result.filepath in diff_filepath:
-            continue
-        diff_filepath.append(diff_result.filepath)
-        class_name = diff_result.filepath.split('/')[-1].split('.')[0]
-        flare_children = {'name': class_name, 'children': [], 'collapsed': True}
-        flare_children_list = []
-        changed_methods = diff_result.changed_methods
-        for key in changed_methods.keys():
-            if changed_methods[key]['is_api']:
-                flare_children_children = {'name': 'methods.' + key + '(' + str(changed_methods[key]['api_path']) + ')',
-                                           'children': [], 'collapsed': True}
-                api_list_item = {'name': str(changed_methods[key]['api_path'])}
-                if api_list_item not in api_list:
-                    api_list.append(api_list_item)
+    def _judge_is_api(self, method_annotations, base_request, method_name):
+        api_path_list = []
+        req_method_list = []
+        method_api_path = []
+        is_api = False
+        for method_annotation in method_annotations:
+            if 'Mapping' not in method_annotation.name:
+                continue
+            is_api = True
+            if method_annotation.name != 'RequestMapping':
+                req_method_list.append(method_annotation.name.replace('Mapping', ''))
             else:
-                flare_children_children = {'name': 'methods.' + key, 'children': [], 'collapsed': True}
-            flare_children_list.append(flare_children_children)
-        changed_declarators = diff_result.changed_declarators
-        for key in changed_declarators.keys():
-            flare_children_children = {'name': 'declarators.' + key, 'children': [], 'collapsed': True}
-            flare_children_list.append(flare_children_children)
-        impact = diff_result.impact
-        for key in impact.keys():
-            tmp_impact_class_name = key.split('.')[-1]
-            if 'methods' in impact[key].keys():
-                impact_methods = impact[key]['methods']
-                for impact_method in impact_methods:
-                    impact_method_name = impact_method['name']
-                    if impact_method['is_api']:
-                        flare_children_children = {
-                            'name': 'impacted.' + tmp_impact_class_name + '.' + impact_method_name + '(' + str(
-                                impact_method['api_path']) + ')',
-                            'children': [], 'collapsed': True}
-                        api_list_item = {'name': str(impact_method['api_path'])}
-                        if api_list_item not in api_list:
-                            api_list.append(api_list_item)
-                    else:
-                        flare_children_children = {
-                            'name': 'impacted.' + tmp_impact_class_name + '.' + impact_method_name,
-                            'children': [], 'collapsed': True}
-                    if 'contains_class' in impact_method.keys() and len(impact_method['contains_class'].keys()) > 0:
-                        for impact_method_cc_key in impact_method['contains_class'].keys():
-                            if 'methods' in impact_method['contains_class'][impact_method_cc_key].keys():
-                                for impact_method_cc_m in impact_method['contains_class'][impact_method_cc_key][
-                                    'methods']:
-                                    if impact_method_cc_m in changed_methods.keys():
-                                        for flare_children_list_item in flare_children_list:
-                                            if 'methods.' + impact_method_cc_m in flare_children_list_item['name']:
-                                                flare_children_list_item_index = flare_children_list.index(
-                                                    flare_children_list_item)
-                                                if impact_method['is_api']:
-                                                    flare_children_list_item_children = {
-                                                        'name': 'impacted.' + tmp_impact_class_name + '.' + impact_method_name + '(' + str(
-                                                            impact_method['api_path']) + ')',
-                                                        'children': [], 'collapsed': True}
-                                                    api_list_item = {'name': str(impact_method['api_path'])}
-                                                    if api_list_item not in api_list:
-                                                        api_list.append(api_list_item)
-                                                else:
-                                                    flare_children_list_item_children = {
-                                                        'name': 'impacted.' + tmp_impact_class_name + '.' + impact_method_name,
-                                                        'children': [], 'collapsed': True}
-                                                if flare_children_list_item_children not in flare_children_list_item[
-                                                    'children']:
-                                                    flare_children_list_item['children'].append(
-                                                        flare_children_list_item_children)
-                                                flare_children_list[
-                                                    flare_children_list_item_index] = flare_children_list_item
-                                            else:
-                                                if flare_children_children not in flare_children_list:
-                                                    flare_children_list.append(flare_children_children)
-                                    else:
-                                        if flare_children_children not in flare_children_list:
-                                            flare_children_list.append(flare_children_children)
-                            else:
-                                if flare_children_children not in flare_children_list:
-                                    flare_children_list.append(flare_children_children)
+                for method_annotation_element in method_annotation.element:
+                    if type(method_annotation_element) == tuple:
+                        req_method_list = ['ALL']
+                        break
+                    if 'name' not in method_annotation_element.attrs or method_annotation_element.name != 'method':
+                        continue
+                    method_annotation_element_value = method_annotation_element.value
+                    if 'member' in method_annotation_element_value.attrs:
+                        req_method_list.append(method_annotation_element_value.member)
+                    elif 'values' in method_annotation_element_value.attrs:
+                        method_annotation_element_values = method_annotation_element_value.values
+                        req_method_list += [method_annotation_element_temp.member for
+                                            method_annotation_element_temp in
+                                            method_annotation_element_values
+                                            if 'member' in method_annotation_element_temp.attrs]
+            if not isinstance(method_annotation.element, list):
+                if method_annotation.element is None:
+                    continue
+                method_api_path += self._get_element_value(method_annotation.element)
+            else:
+                method_api_path_list = [method_annotation_element.value for method_annotation_element in method_annotation.element
+                                        if method_annotation_element.name == 'path' or method_annotation_element.name == 'value']
+                if len(method_api_path_list) == 0:
+                    continue
+                method_api_path_obj = method_api_path_list[0]
+                if 'value' in method_api_path_obj.attrs:
+                    method_api_path += [method_api_path_obj.value.replace('"', '')]
+                else:
+                    if 'values' in method_api_path_obj.attrs:
+                        for method_api_value in method_api_path_obj.values:
+                            method_api_path += self._get_element_value(method_api_value)
                     else:
-                        if flare_children_children not in flare_children_list:
-                            flare_children_list.append(flare_children_children)
+                        method_api_path += [method_name + '/cci-unknown']
+        if len(method_api_path) == 0:
+            method_api_path = ['/']
+        for method_api_path_obj in method_api_path:
+            if method_api_path_obj.startswith('/'):
+                method_api_path_obj = method_api_path_obj[1:]
+            api_path = base_request + method_api_path_obj
+            if api_path.endswith('/'):
+                api_path = api_path[0:-1]
+            if len(req_method_list) > 0:
+                api_path_list += ['[' + req_method_temp + ']' + api_path for req_method_temp in req_method_list]
             else:
-                flare_children_children = {'name': 'impacted.' + tmp_impact_class_name, 'children': [],
-                                           'collapsed': True}
-                if flare_children_children not in flare_children_list:
-                    flare_children_list.append(flare_children_children)
-        flare_children['children'] = flare_children_list
-        flare['children'].append(flare_children)
-    flare['children'].reverse()
-    flare['children'].insert(0, {'name': 'Impact_Apis', 'children': api_list})
-    return flare
-
-
-def _clean_occupy(occupy_path):
-    if os.path.exists(occupy_path):
-        os.remove(occupy_path)
-
-
-def _class_in_method(class_name, method):
-    if method.contains_declarators is not None:
-        dcl_in_method = [d for d in method.contains_declarators if d['type'] == class_name]
-        if len(dcl_in_method) > 0:
-            return True
-    method_content = str(method.content)
-    if class_name + ' ' in method_content \
-            or '<' + class_name + '>' in method_content \
-            or class_name + '.' in method_content:
-        return True
-    else:
-        return False
-
-
-def _diff_result_impact(diff_result_item_index, diff_results_list, which_java_file_analyze_result, mode):
-    diff_result_item = diff_results_list[diff_result_item_index]
-    diff_result_filepath = diff_result_item.filepath
-    if diff_result_filepath in which_java_file_analyze_result.keys():
-        which_java_analyze = which_java_file_analyze_result[diff_result_filepath]
-        which_class_name = which_java_analyze.class_name
-        which_class_path = which_java_analyze.package_name + '.' + which_java_analyze.class_name
-        which_implements = which_java_analyze.implements
-        head_extends = which_java_analyze.extends
-        which_implements.append(which_class_path)
-        for which_java_file_analyze_key in which_java_file_analyze_result.keys():
-            which_java_file_analyze = which_java_file_analyze_result[which_java_file_analyze_key]
-            if which_java_file_analyze.extends is not None:
-                which_java_file_analyze_extends = which_java_file_analyze.extends
-                if '.' in which_java_file_analyze_extends:
-                    which_java_file_analyze_extends = '/'.join(which_java_file_analyze_extends.split('.'))
-                extends_analyzer_list = [which_java_file_analyze_result[obj] for obj in
-                                         which_java_file_analyze_result.keys()
-                                         if which_java_file_analyze_extends in obj]
-                if len(extends_analyzer_list) > 0:
-                    extends_analyzer = extends_analyzer_list[0]
-                    which_java_file_analyze.methods = list(
-                        set(which_java_file_analyze.methods + extends_analyzer.methods))
-                    which_java_file_analyze.declarators = list(
-                        set(which_java_file_analyze.declarators + extends_analyzer.declarators))
-                    which_java_file_analyze.imports.imports = list(
-                        set(which_java_file_analyze.imports.imports + extends_analyzer.imports.imports))
-            is_in, directly = _in_import(which_java_analyze, which_java_file_analyze)
-            if not is_in:
+                api_path_list.append('[ALL]' + api_path)
+        return is_api, api_path_list
+
+    def _add_entity_used_to_method_invocation(self, method_invocation, package_class, section):
+        if package_class not in method_invocation.keys():
+            method_invocation[package_class] = {ENTITY: {section: True}}
+        elif ENTITY not in method_invocation[package_class].keys():
+            method_invocation[package_class][ENTITY] = {section: True}
+        elif section not in method_invocation[package_class][ENTITY].keys():
+            method_invocation[package_class][ENTITY][section] = True
+
+    def _add_method_used_to_method_invocation(self, method_invocation, package_class, method, lines):
+        if package_class not in method_invocation.keys():
+            method_invocation[package_class] = {METHODS: {method: lines}}
+        elif METHODS not in method_invocation[package_class].keys():
+            method_invocation[package_class][METHODS] = {method: lines}
+        elif method not in method_invocation[package_class][METHODS].keys():
+            method_invocation[package_class][METHODS][method] = lines
+        else:
+            method_invocation[package_class][METHODS][method] += lines
+
+    def _add_field_used_to_method_invocation(self, method_invocation, package_class, field, lines):
+        if package_class not in method_invocation.keys():
+            method_invocation[package_class] = {FIELDS: {field: lines}}
+        elif FIELDS not in method_invocation[package_class].keys():
+            method_invocation[package_class][FIELDS] = {field: lines}
+        elif field not in method_invocation[package_class][FIELDS].keys():
+            method_invocation[package_class][FIELDS][field] = lines
+        else:
+            method_invocation[package_class][FIELDS][field] += lines
+
+    def _deal_declarator_type(self, node_type, import_map, method_invocation, section):
+        if node_type is None:
+            return node_type
+        if type(node_type) == javalang.tree.BasicType:
+            return node_type.name
+        var_declarator_type = node_type.name
+        if var_declarator_type in import_map.keys():
+            var_declarator_type = import_map.get(var_declarator_type)
+            self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type, section)
+        var_declarator_type_arguments = self._deal_arguments_type(node_type.arguments, import_map, method_invocation, section)
+        if var_declarator_type_arguments:
+            var_declarator_type = var_declarator_type + '<' + '#'.join(var_declarator_type_arguments) + '>'
+        return var_declarator_type
+
+    def _deal_arguments_type(self, arguments, import_map, method_invocation, section):
+        var_declarator_type_arguments_new = []
+        if not arguments:
+            return var_declarator_type_arguments_new
+        var_declarator_type_arguments = []
+        for argument in arguments:
+            if type(argument) == javalang.tree.MethodInvocation:
+                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
                 continue
-            which_java_file_methods = which_java_file_analyze.methods
-            which_java_file_declarators = [declarator for declarator in which_java_file_analyze.declarators if
-                                           declarator.type == which_class_name]
-            for which_java_file_method in which_java_file_methods:
-                classname_in_method = False
-                tmp = []
-                if diff_result_item.changed_declarators != {}:
-                    classname_in_method = _class_in_method(which_class_name, which_java_file_method)
-                if which_java_file_method.contains_class is not None:
-                    for implement in which_implements:
-                        if implement in which_java_file_method.contains_class.keys() and 'methods' in \
-                                which_java_file_method.contains_class[implement].keys():
-                            java_file_method_includes_methods = which_java_file_method.contains_class[implement][
-                                'methods']
-                            tmp = [j for j in diff_result_item.changed_methods.keys() if
-                                   mode in diff_result_item.changed_methods[j][
-                                       'diff_impact'] and j in java_file_method_includes_methods]
-                if len(tmp) == 0:
-                    method_content_str = str(which_java_file_method.content)
-                    if len(which_java_file_declarators) > 0:
-                        for declarator in which_java_file_declarators:
-                            tmp += [j for j in diff_result_item.changed_methods.keys() if
-                                    mode in diff_result_item.changed_methods[j]['diff_impact']
-                                    and ('(' + j + '(' in method_content_str
-                                         or '=' + j + '(' in method_content_str
-                                         or '=' + j + '(' in method_content_str
-                                         or '= ' + j + '(' in method_content_str
-                                         or declarator.name + '.' + j + '(' in method_content_str
-                                         )
-                                    ]
-                    else:
-                        tmp += [j for j in diff_result_item.changed_methods.keys() if
-                                mode in diff_result_item.changed_methods[j]['diff_impact']
-                                and ('(' + j + '(' in method_content_str
-                                     or '=' + j + '(' in method_content_str
-                                     or '=' + j + '(' in method_content_str
-                                     or '= ' + j + '(' in method_content_str
-                                     )
-                                ]
-                if len(tmp) > 0 or classname_in_method:
-                    if which_java_file_method.diff_impact is None or which_java_file_method.diff_impact != '':
-                        which_java_file_method.diff_impact = mode
-                    else:
-                        which_java_file_method.diff_impact = which_java_file_method.diff_impact + '_' + mode
-                    java_file_class_path = which_java_file_analyze.package_name + '.' + which_java_file_analyze.class_name
-                    if java_file_class_path not in diff_result_item.impact.keys():
-                        diff_result_item.impact[java_file_class_path] = {'methods': [which_java_file_method.__dict__]}
-                    elif which_java_file_method.__dict__ not in diff_result_item.impact[java_file_class_path][
-                        'methods']:
-                        diff_result_item.impact[java_file_class_path]['methods'].append(which_java_file_method.__dict__)
-                    diff_result_need_add = JavaDiffResult(which_java_file_analyze_key, None, None, None, None)
-                    index = -1
-                    for i in range(len(diff_results_list) - 1, -1, -1):
-                        if diff_results_list[i] is None:
-                            continue
-                        if diff_results_list[i].filepath == which_java_file_analyze_key:
-                            diff_result_need_add = JavaDiffResult(diff_results_list[i].filepath,
-                                                                  diff_results_list[i].added_line_nums,
-                                                                  diff_results_list[i].added_line_contents,
-                                                                  diff_results_list[i].removed_line_nums,
-                                                                  diff_results_list[i].removed_line_contents)
-                            diff_result_need_add.impact = diff_results_list[i].impact.copy()
-                            diff_result_need_add.changed_methods = diff_results_list[i].changed_methods.copy()
-                            diff_result_need_add.changed_declarators = diff_results_list[i].changed_declarators.copy()
-                            index = i
-                            break
-                    if which_java_file_method.name not in diff_result_need_add.changed_methods.keys():
-                        # or diff_result_need_add.changed_methods[
-                        #         which_java_file_method.name] != which_java_file_method.__dict__:
-                        diff_result_need_add.changed_methods[
-                            which_java_file_method.name] = which_java_file_method.__dict__
-                        if index > diff_result_item_index:
-                            diff_results_list[index] = diff_result_need_add
-                        else:
-                            diff_results_list.append(diff_result_need_add)
-
-
-# Press the green button in the gutter to run the script.
-def analyze(project_git_url, branch_name, commit_first, commit_second, request_user):
-    t1 = datetime.datetime.now()
-    print(datetime.datetime.now(), ':', 'Start At:', datetime.datetime.now(), flush=True)
-    cur_dir = os.getcwd()
-    project_name = project_git_url.split("/")[-1].split('.git')[0]
-    folder_name = cur_dir + sep + project_name
-    git_clone_bash = 'git clone -b ' + branch_name + ' ' + project_git_url + ' ' + folder_name
-    git_pull_base = 'cd ' + folder_name + ' && git checkout ' + branch_name + ' && git pull'
-    diff_base = 'cd ' + folder_name + ' && ' \
-                + 'git diff ' + commit_second + '..' + commit_first + ' > diff_' + commit_second + '..' + commit_first + '.txt'
-    atexit.register(_clean_occupy, folder_name + sep + 'Occupy.ing')
-    if not os.path.exists(folder_name):
-        print(datetime.datetime.now(), ':', 'Clone from git', flush=True)
-        os.system(git_clone_bash)
-    else:
-        # had analyze result, skip
-        if os.path.exists(folder_name + sep + commit_second + '..' + commit_first + '.cci'):
-            print(datetime.datetime.now(), ':', 'Has analyze result, skip!', flush=True)
-            with open(folder_name + sep + commit_second + '..' + commit_first + '.cci', 'r') as read:
-                print(datetime.datetime.now(), ':', read.read(), flush=True)
-            sys.exit(0)
+            var_declarator_type_argument = self._deal_type(argument)
+            if var_declarator_type_argument in import_map.keys():
+                var_declarator_type_argument = import_map.get(var_declarator_type_argument)
+                self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type_argument, section)
+            var_declarator_type_arguments.append(var_declarator_type_argument)
+        return var_declarator_type_arguments
+
+    def _deal_type(self, argument):
+        if not argument:
+            return None
+        argument_type = type(argument)
+        if argument_type == javalang.tree.MemberReference:
+            var_declarator_type_argument = argument.member
+        elif argument_type == javalang.tree.Literal:
+            var_declarator_type_argument = self._deal_literal_type(argument.value)
+        elif argument_type == javalang.tree.This:
+            var_declarator_type_argument = 'This'
+        elif argument_type == javalang.tree.LambdaExpression:
+            var_declarator_type_argument = 'LambdaExpression'
+        elif argument_type == javalang.tree.BinaryOperation:
+            # todo BinaryOperation temp set string
+            var_declarator_type_argument = 'String'
+        elif argument_type == javalang.tree.MethodReference or argument_type == javalang.tree.TernaryExpression:
+            # todo MethodReference temp set unknown
+            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+        elif argument_type == javalang.tree.SuperMethodInvocation:
+            logging.info(argument_type)
+            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+        elif argument_type == javalang.tree.Assignment:
+            var_declarator_type_argument = self._deal_type(argument.value)
+        elif argument_type == javalang.tree.Cast:
+            var_declarator_type_argument = argument.type.name
+        # todo
+        elif argument_type == javalang.tree.SuperMemberReference:
+            var_declarator_type_argument = 'String'
+        elif argument.type is not None:
+            var_declarator_type_argument = argument.type.name
+        else:
+            logging.info(f'argument type is None：{argument}')
+            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+        return var_declarator_type_argument
+
+    def _deal_literal_type(self, text):
+        if 'true' == text or 'false' == text:
+            return 'boolean'
+        if text.isdigit():
+            return 'int'
+        return 'String'
+
+    def _deal_var_type(self, arguments, parameters_map, variable_map, field_map, import_map, method_invocation, section):
+        var_declarator_type_arguments_new = []
+        if not arguments:
+            return var_declarator_type_arguments_new
+        var_declarator_type_arguments = []
+        for argument in arguments:
+            argument_type = type(argument)
+            if argument_type == javalang.tree.MethodInvocation:
+                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
+                continue
+            var_declarator_type_argument = self._deal_type(argument)
+            var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section)
+            type_arguments = self._deal_arguments_type(argument.type.arguments, import_map, method_invocation, section) \
+                if 'type' in argument.attrs \
+                   and not isinstance(argument.type, str) \
+                   and 'arguments' in argument.type.attrs \
+                   and argument.type.arguments \
+                else []
+            if type_arguments:
+                var_declarator_type_argument = var_declarator_type_argument + '<' + '#'.join(type_arguments) + '>'
+            var_declarator_type_arguments.append(var_declarator_type_argument)
+        return var_declarator_type_arguments
+
+    def _get_var_type(self, var, parameters_map, variable_map, field_map, import_map, method_invocation, section):
+        if not var:
+            return var
+        if var in parameters_map.keys():
+            return parameters_map.get(var)
+        if var in variable_map.keys():
+            return variable_map.get(var)
+        if var in field_map.keys():
+            field_type = field_map.get(var)['field_type']
+            package_class = field_map.get(var)['package_class']
+            start_line = field_map.get(var)['start_line']
+            self._add_field_used_to_method_invocation(method_invocation, package_class, var, [start_line])
+            return field_type
+        if var in import_map.keys():
+            var_type = import_map.get(var)
+            self._add_entity_used_to_method_invocation(method_invocation, var_type, section)
+            return var_type
+        return var
+
+    def _get_extends_class_fields_map(self, class_id: int):
+        class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
+        extend_package_class = class_db['extends_class']
+        if not extend_package_class:
+            return {}
+        extend_package = '.'.join(extend_package_class.split('.')[0: -1])
+        extend_class = extend_package_class.split('.')[-1]
+        extend_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name="{extend_package}" '
+                                                  f'AND class_name="{extend_class}" '
+                                                  f'AND project_id={self.project_id} limit 1')
+        if not extend_class_db:
+            return {}
+        extend_class_entity = extend_class_db[0]
+        extend_class_id = extend_class_entity['class_id']
+        extend_class_fields = self.sqlite.select_data(f'SELECT * FROM field WHERE class_id = {extend_class_id}')
+        extend_class_fields_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': extend_package_class, 'start_line': field_obj['start_line']} for field_obj in extend_class_fields}
+        if not extend_class_entity['extends_class']:
+            return extend_class_fields_map
         else:
-            # analyzing, wait
-            wait_index = 0
-            while os.path.exists(folder_name + sep + 'Occupy.ing') and wait_index < 30:
-                print(datetime.datetime.now(), ':', 'Analyzing by others, waiting......', flush=True)
-                time.sleep(3)
-                wait_index += 1
-    print(datetime.datetime.now(), ':', 'Start occupying project, and others can not analyze until released',
-          flush=True)
-    with open(folder_name + sep + 'Occupy.ing', 'w') as ow:
-        ow.write('Occupy by ' + request_user)
-    time.sleep(1)
-    print(datetime.datetime.now(), ':', 'Git pull project to HEAD', flush=True)
-    os.system(git_pull_base)
-    time.sleep(1)
-    print(datetime.datetime.now(), ':', 'Git diff between ' + commit_second + ' and ' + commit_first, flush=True)
-    os.system(diff_base)
-    time.sleep(1)
-    print(datetime.datetime.now(), ':', 'Get all ' + commit_second + ' files', flush=True)
-    base_java_file_analyze_result = _get_commit_project_files(commit_second, folder_name)
-    print(datetime.datetime.now(), ':', 'Get all ' + commit_first + ' files', flush=True)
-    head_java_file_analyze_result = _get_commit_project_files(commit_first, folder_name)
-    diff_txt = folder_name + sep + 'diff_' + commit_second + '..' + commit_first + '.txt'
-    print(datetime.datetime.now(), ':', 'Get all diff file', flush=True)
-    diff_results = _get_diff_results(diff_txt, head_java_file_analyze_result, base_java_file_analyze_result)
-    diff_result_index = 0
-    for diff_result in diff_results:
-        if diff_result is None:
-            continue
-        print(datetime.datetime.now(), ':', 'Analyzing diff/impact file:' + diff_result.filepath, flush=True)
-        _diff_result_impact(diff_result_index, diff_results, head_java_file_analyze_result, 'ADD')
-        _diff_result_impact(diff_result_index, diff_results, base_java_file_analyze_result, 'DEL')
-        diff_result_index = diff_result_index + 1
-    print(datetime.datetime.now(), ':', 'Analyze success, generating......', flush=True)
-    flare = _gen_treemap_data(diff_results, commit_first, commit_second)
-    print(json.dumps(flare), flush=True)
-    with open(folder_name + sep + flare['name'] + '.cci', 'w') as w:
-        w.write(json.dumps(flare))
-    t2 = datetime.datetime.now()
-    try:
-        print(datetime.datetime.now(), ':', 'Analyze done, remove occupy, others can analyze now', flush=True)
-        os.remove(folder_name + sep + 'Occupy.ing')
-    except:
-        pass
-    print(datetime.datetime.now(), ':', 'Analyze done, spend: ', t2 - t1, flush=True)
+            extend_new_map = self._get_extends_class_fields_map(extend_class_id)
+            extend_new_map.update(extend_class_fields_map)
+            return extend_new_map
+
+    def parse_java_file(self, filepath, commit_or_branch):
+        if not filepath.endswith('.java'):
+            return
+        try:
+            with open(filepath, encoding='UTF-8') as fp:
+                file_content = fp.read()
+        except:
+            return
+        logging.info(f'Parsing java file: {filepath}')
+        lines = file_content.split('\n')
+        try:
+            tree = javalang.parse.parse(file_content)
+            if not tree.types:
+                return
+        except Exception as e:
+            logging.error(f"Error parsing {filepath}: {e}")
+            return
+        # 处理包信息
+        package_name = tree.package.name if tree.package else None
+        class_name = tree.types[0].name
+        package_class = package_name + '.' + tree.types[0].name
+        # 处理 import 信息
+        import_list = self._parse_imports(tree.imports)
+        import_map = {import_obj['import_path'].split('.')[-1]: import_obj['import_path'] for import_obj in import_list}
+
+        # 处理 class 信息
+        class_id, new_add = self._parse_class(tree.types[0], filepath, package_name, import_list, commit_or_branch)
+        # 已经处理过了，返回
+        # if not new_add:
+        #     return
+        # 导入import
+        imports = [dict(import_obj, class_id=class_id, project_id=self.project_id) for import_obj in import_list]
+        self.sqlite.update_data(f'DELETE FROM import WHERE class_id={class_id}')
+        self.sqlite.insert_data('import', imports)
+
+        # 处理 field 信息
+        field_list = self._parse_fields(tree.types[0].fields, package_name, class_id, import_map)
+        field_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': package_class, 'start_line': field_obj['start_line']} for field_obj in field_list}
+        import_map = dict((k, v) for k, v in import_map.items() if v.startswith('com.patsnap'))
+
+        # 将extend class的field导进来
+        extends_class_fields_map = self._get_extends_class_fields_map(class_id)
+        extends_class_fields_map.update(field_map)
+        # 处理 methods 信息
+        self._parse_method(tree.types[0].methods, lines, class_id, import_map, extends_class_fields_map)
+
+    def parse_java_file_list(self, filepath_list: list, commit_or_branch: str):
+        for file_path in filepath_list:
+            self.parse_java_file(file_path, commit_or_branch)
+
+
+if __name__ == '__main__':
+    print('jcci')
```

### Comparing `jcci-0.0.9/src/jcci.egg-info/PKG-INFO` & `jcci-0.1.0/src/jcci.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.9
-Summary: Java code commit impact analyze in pure Python
+Version: 0.1.0
+Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,17 +26,19 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: javalang>=0.13.0
+Requires-Dist: unidiff>=0.7.4
 
 #### Description
 Java code commit impact analysis, is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data.
 
 Github: [jcci](https://github.com/baikaishuipp/jcci)
 #### Installation
 ```
@@ -45,22 +47,19 @@
 
 #### Instructions
 Start a new python project, add a new python file, code example:
 
 ```
 from jcci import jcci
 
+# Compare different commits on the same branch
 jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
+
 ```
 
-At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.
+At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, download [jcci-result.html](https://github.com/baikaishuipp/jcci/blob/main/jcci-result.html) , upload analyze result file end with .cci, then can be displayed through the view.
 
 ##### CCI result
 ![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cci-result.png)
 
 ##### CCI result tree view
 ![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/cii-result-tree.png)
-
-#### Communication
-Communicate via Wechat:
-
-![communicate via Wechat](https://raw.githubusercontent.com/baikaishuipp/jcci/main/images/wechat.jpg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

