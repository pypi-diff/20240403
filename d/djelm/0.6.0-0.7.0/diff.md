# Comparing `tmp/djelm-0.6.0.tar.gz` & `tmp/djelm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djelm-0.6.0.tar", max compression
+gzip compressed data, was "djelm-0.7.0.tar", max compression
```

## Comparing `djelm-0.6.0.tar` & `djelm-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1082 2024-03-27 00:34:17.033578 djelm-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0    23669 2024-03-27 00:34:17.033578 djelm-0.6.0/README_pypi.md
--rw-r--r--   0        0        0     1360 2024-03-27 00:34:17.037578 djelm-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      254 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/__init__.py
--rw-r--r--   0        0        0       83 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/apps.py
--rw-r--r--   0        0        0     1291 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/cookiecutter.py
--rw-r--r--   0        0        0      345 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/effect.py
--rw-r--r--   0        0        0     1659 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/elm.py
--rw-r--r--   0        0        0      179 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/__init__.py
--rw-r--r--   0        0        0      514 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/adapters.py
--rw-r--r--   0        0        0       65 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/form/__init__.py
--rw-r--r--   0        0        0      813 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/form/adapters.py
--rw-r--r--   0        0        0     2045 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/form/helpers.py
--rw-r--r--   0        0        0      444 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/form/primitives.py
--rw-r--r--   0        0        0      592 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/form/serializer.py
--rw-r--r--   0        0        0    21933 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/main.py
--rw-r--r--   0        0        0     1211 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/flags/primitives.py
--rw-r--r--   0        0        0       36 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/forms/widgets/main.py
--rw-r--r--   0        0        0    13914 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/generators.py
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/management/commands/__init__.py
--rw-r--r--   0        0        0     3376 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/management/commands/djelm.py
--rw-r--r--   0        0        0      105 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/model_template/cookiecutter.json
--rw-r--r--   0        0        0      432 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
--rw-r--r--   0        0        0     1384 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/npm.py
--rw-r--r--   0        0        0      112 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/cookiecutter.json
--rw-r--r--   0        0        0     1464 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
--rw-r--r--   0        0        0      791 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0       99 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0      375 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
--rw-r--r--   0        0        0      603 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
--rw-r--r--   0        0        0       75 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/cookiecutter.json
--rw-r--r--   0        0        0      430 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/hooks/post_gen_project.py
--rw-r--r--   0        0        0      167 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
--rw-r--r--   0        0        0      446 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
--rw-r--r--   0        0        0      475 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
--rw-r--r--   0        0        0      384 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
--rw-r--r--   0        0        0       92 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/include.html
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/{{cookiecutter.app_name}}/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
--rw-r--r--   0        0        0    21150 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/strategy.py
--rw-r--r--   0        0        0     1010 2024-03-27 00:34:17.037578 djelm-0.6.0/src/djelm/subprocess.py
--rw-r--r--   0        0        0     3348 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/utils.py
--rw-r--r--   0        0        0    20835 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/validate.py
--rw-r--r--   0        0        0      112 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/cookiecutter.json
--rw-r--r--   0        0        0     3912 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
--rw-r--r--   0        0        0      813 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0      429 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
--rw-r--r--   0        0        0      753 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
--rw-r--r--   0        0        0      105 2024-03-27 00:34:17.041578 djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0    24512 1970-01-01 00:00:00.000000 djelm-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-03 07:20:59.898015 djelm-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0    23669 2024-04-03 07:20:59.898015 djelm-0.7.0/README_pypi.md
+-rw-r--r--   0        0        0     1360 2024-04-03 07:20:59.898015 djelm-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      254 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/apps.py
+-rw-r--r--   0        0        0     1291 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/cookiecutter.py
+-rw-r--r--   0        0        0      345 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/effect.py
+-rw-r--r--   0        0        0     1659 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/elm.py
+-rw-r--r--   0        0        0      179 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/adapters.py
+-rw-r--r--   0        0        0       65 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/adapters.py
+-rw-r--r--   0        0        0     2045 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/helpers.py
+-rw-r--r--   0        0        0      444 2024-04-03 07:20:59.898015 djelm-0.7.0/src/djelm/flags/form/primitives.py
+-rw-r--r--   0        0        0      592 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/form/serializer.py
+-rw-r--r--   0        0        0    21933 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/main.py
+-rw-r--r--   0        0        0     1211 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/flags/primitives.py
+-rw-r--r--   0        0        0       36 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/forms/widgets/main.py
+-rw-r--r--   0        0        0    13914 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/generators.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/commands/__init__.py
+-rw-r--r--   0        0        0     3376 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/management/commands/djelm.py
+-rw-r--r--   0        0        0      105 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/model_template/cookiecutter.json
+-rw-r--r--   0        0        0      432 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
+-rw-r--r--   0        0        0     1384 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/npm.py
+-rw-r--r--   0        0        0      112 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/cookiecutter.json
+-rw-r--r--   0        0        0     1464 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
+-rw-r--r--   0        0        0      791 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0       99 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
+-rw-r--r--   0        0        0      375 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
+-rw-r--r--   0        0        0      603 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
+-rw-r--r--   0        0        0       75 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/cookiecutter.json
+-rw-r--r--   0        0        0      430 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      167 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
+-rw-r--r--   0        0        0      446 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
+-rw-r--r--   0        0        0      475 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
+-rw-r--r--   0        0        0      384 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
+-rw-r--r--   0        0        0       92 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/include.html
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/{{cookiecutter.app_name}}/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
+-rw-r--r--   0        0        0    21257 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/strategy.py
+-rw-r--r--   0        0        0     1010 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/subprocess.py
+-rw-r--r--   0        0        0     3348 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/utils.py
+-rw-r--r--   0        0        0    20835 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/validate.py
+-rw-r--r--   0        0        0      112 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/cookiecutter.json
+-rw-r--r--   0        0        0     3912 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
+-rw-r--r--   0        0        0      813 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0      429 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
+-rw-r--r--   0        0        0      753 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
+-rw-r--r--   0        0        0      105 2024-04-03 07:20:59.902015 djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
+-rw-r--r--   0        0        0    24512 1970-01-01 00:00:00.000000 djelm-0.7.0/PKG-INFO
```

### Comparing `djelm-0.6.0/LICENSE.txt` & `djelm-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/README_pypi.md` & `djelm-0.7.0/README_pypi.md`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/pyproject.toml` & `djelm-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.mypy]
 plugins = [ "mypy_django_plugin.main" ]
 
 [tool.poetry]
 name = "djelm"
-version = "0.6.0"
+version = "0.7.0"
 description = "A framework for using Elm programs in a Django project"
 authors = ["Confidenceman02"]
 readme = "README_pypi.md"
 keywords = ["django", "elm"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `djelm-0.6.0/src/djelm/cookiecutter.py` & `djelm-0.7.0/src/djelm/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/elm.py` & `djelm-0.7.0/src/djelm/elm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/adapters.py` & `djelm-0.7.0/src/djelm/flags/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/form/adapters.py` & `djelm-0.7.0/src/djelm/flags/form/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/form/helpers.py` & `djelm-0.7.0/src/djelm/flags/form/helpers.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/form/serializer.py` & `djelm-0.7.0/src/djelm/flags/form/serializer.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/main.py` & `djelm-0.7.0/src/djelm/flags/main.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/flags/primitives.py` & `djelm-0.7.0/src/djelm/flags/primitives.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/generators.py` & `djelm-0.7.0/src/djelm/generators.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/management/commands/djelm.py` & `djelm-0.7.0/src/djelm/management/commands/djelm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/npm.py` & `djelm-0.7.0/src/djelm/npm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm` & `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts` & `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py` & `djelm-0.7.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/strategy.py` & `djelm-0.7.0/src/djelm/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,19 @@
                 process = SubProcess(
                     ["node", "-e", COMPILE_PROGRAM],
                     os.path.join(src_path.value),
                     self.raise_error,
                 )
                 try:
                     process.open()
-                except Exception as _:
-                    return ExitSuccess(None)
+                except Exception as err:
+                    if self.raise_error:
+                        raise err
+                    else:
+                        return ExitSuccess(None)
                 return ExitSuccess(None)
             except subprocess.CalledProcessError:
                 sys.exit(1)
         return ExitFailure(None, StrategyError("Error"))
 
 
 @dataclass(slots=True)
```

### Comparing `djelm-0.6.0/src/djelm/subprocess.py` & `djelm-0.7.0/src/djelm/subprocess.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/utils.py` & `djelm-0.7.0/src/djelm/utils.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/validate.py` & `djelm-0.7.0/src/djelm/validate.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw` & `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts` & `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py` & `djelm-0.7.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py`

 * *Files identical despite different names*

### Comparing `djelm-0.6.0/PKG-INFO` & `djelm-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djelm
-Version: 0.6.0
+Version: 0.7.0
 Summary: A framework for using Elm programs in a Django project
 Keywords: django,elm
 Author: Confidenceman02
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

