# Comparing `tmp/gcp-sphinx-docfx-yaml-3.0.1.tar.gz` & `tmp/gcp-sphinx-docfx-yaml-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-sphinx-docfx-yaml-3.0.1.tar", last modified: Wed Mar 13 03:57:05 2024, max compression
+gzip compressed data, was "gcp-sphinx-docfx-yaml-3.1.0.tar", last modified: Wed Apr  3 17:57:11 2024, max compression
```

## Comparing `gcp-sphinx-docfx-yaml-3.0.1.tar` & `gcp-sphinx-docfx-yaml-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-13 03:57:05.596870 gcp-sphinx-docfx-yaml-3.0.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/LICENSE
--rw-r--r--   0 root         (0)     1003      796 2024-03-13 03:57:05.596870 gcp-sphinx-docfx-yaml-3.0.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2625 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-13 03:57:05.592870 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/
--rw-rw-r--   0 root         (0)     1003      576 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/__init__.py
--rw-rw-r--   0 root         (0)     1003     1262 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/directives.py
--rw-rw-r--   0 root         (0)     1003    77958 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/extension.py
--rw-rw-r--   0 root         (0)     1003     5154 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/extract_nodes.py
--rw-rw-r--   0 root         (0)     1003    14975 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/markdown_utils.py
--rw-rw-r--   0 root         (0)     1003    20734 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/monkeypatch.py
--rw-rw-r--   0 root         (0)     1003      988 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/nodes.py
--rw-rw-r--   0 root         (0)     1003      727 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/settings.py
--rw-rw-r--   0 root         (0)     1003     1731 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/utils.py
--rw-rw-r--   0 root         (0)     1003    33366 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-13 03:57:05.596870 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/
--rw-r--r--   0 root         (0)     1003      796 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      640 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      289 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       11 2024-03-13 03:57:05.000000 gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-13 03:57:05.596870 gcp-sphinx-docfx-yaml-3.0.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     1756 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-13 03:57:05.596870 gcp-sphinx-docfx-yaml-3.0.1/tests/
--rw-rw-r--   0 root         (0)     1003    15861 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/tests/test_helpers.py
--rw-rw-r--   0 root         (0)     1003     1588 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/tests/test_inspect.py
--rw-rw-r--   0 root         (0)     1003    10011 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/tests/test_markdown.py
--rw-rw-r--   0 root         (0)     1003    32326 2024-03-13 03:54:43.000000 gcp-sphinx-docfx-yaml-3.0.1/tests/test_unit.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/LICENSE
+-rw-r--r--   0 root         (0)     1003      796 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2625 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.223463 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/
+-rw-rw-r--   0 root         (0)     1003      576 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1262 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/directives.py
+-rw-rw-r--   0 root         (0)     1003    84402 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extension.py
+-rw-rw-r--   0 root         (0)     1003     5154 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extract_nodes.py
+-rw-rw-r--   0 root         (0)     1003    16722 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/markdown_utils.py
+-rw-rw-r--   0 root         (0)     1003    20734 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/monkeypatch.py
+-rw-rw-r--   0 root         (0)     1003      988 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/nodes.py
+-rw-rw-r--   0 root         (0)     1003      727 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/settings.py
+-rw-rw-r--   0 root         (0)     1003     1731 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/utils.py
+-rw-rw-r--   0 root         (0)     1003    33366 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.223463 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/
+-rw-r--r--   0 root         (0)     1003      796 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      640 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      289 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       11 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     1756 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/tests/
+-rw-rw-r--   0 root         (0)     1003    15861 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1588 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_inspect.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_markdown.py
+-rw-rw-r--   0 root         (0)     1003    32326 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_unit.py
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/LICENSE` & `gcp-sphinx-docfx-yaml-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.0.1
+Version: 3.1.0
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/README.rst` & `gcp-sphinx-docfx-yaml-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/__init__.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/directives.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/directives.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/extension.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 
 # -*- coding: utf-8 -*-
 """
 Sphinx DocFX YAML Top-level Extension.
 
 This extension allows you to automagically generate DocFX YAML from your Python AutoAPI docs.
 """
-import ast
-import os
-import inspect
-import re
-import copy
-import shutil
-import black
-import logging
 
+import ast
 from collections import defaultdict
-from collections.abc import MutableSet
-from pathlib import Path
+from collections.abc import Mapping, MutableSet, Sequence
+import copy
 from functools import partial
+import inspect
 from itertools import zip_longest
+import json
+import logging
+import os
+from pathlib import Path
+import re
+import shutil
 from typing import Any, Dict, Iterable, List, Optional
+import black
 from black import InvalidInput
 
 try:
     from subprocess import getoutput
 except ImportError:
     from commands import getoutput
 
@@ -130,19 +131,60 @@
     OBJECTIVE: 'Objective',
     SUCCESS: 'Success',
     BETA: 'Beta',
     PREVIEW: 'Preview',
     DEPRECATED: 'deprecated',
 }
 
+_SUMMARY_TYPE_BY_ITEM_TYPE = {
+    # Modules and Classes are similar types.
+    MODULE: CLASS,
+    CLASS: CLASS,
+    # Methods and Functions are similar types.
+    METHOD: METHOD,
+    FUNCTION: METHOD,
+    # Properties and Attributes are similar types.
+    PROPERTY: PROPERTY,
+    ATTRIBUTE: PROPERTY,
+}
+# Construct a mapping of name and content for each unique summary type entry.
+_ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE = {
+    summary_type: [[], []]  # entry name then entry content
+    for summary_type in set(_SUMMARY_TYPE_BY_ITEM_TYPE.values())
+}
+# Mapping for each summary page entry's file name and entry name.
+_FILE_NAME_AND_ENTRY_NAME_BY_SUMMARY_TYPE = {
+    CLASS: ('summary_class.yml', "Classes"),
+    METHOD: ('summary_method.yml', "Methods"),
+    PROPERTY: ('summary_property.yml', "Properties and Attributes"),
+}
+
 # Disable blib2to3 output that clutters debugging log.
 logging.getLogger("blib2to3").setLevel(logging.ERROR)
 
 
+def _grab_repo_metadata() -> Mapping[str, str] | None:
+    """Retrieves the repository's metadata info if found."""
+    try:
+        with open('.repo-metadata.json', 'r') as metadata_file:
+            json_content = json.load(metadata_file)
+        # Return outside of context manager for safe close
+        return json_content
+    except Exception:
+        return None
+
+
 def build_init(app):
+    print("Retrieving repository metadata.")
+    if not (repo_metadata := _grab_repo_metadata()):
+        print("Failed to retrieve repository metadata.")
+        app.env.library_shortname = ""
+    else:
+        print("Successfully retrieved repository metadata.")
+        app.env.library_shortname = repo_metadata["name"]
     print("Running sphinx-build with Markdown first...")
     markdown_utils.run_sphinx_markdown()
     print("Completed running sphinx-build with Markdown files.")
 
     """
     Set up environment data
     """
@@ -1344,14 +1386,110 @@
     # Retrieve only the package name
     split_name = package_group.split(".")[-1]
     # Capitalize the first letter of each package name part
     capitalized_name = [part.capitalize() for part in split_name.split("_")]
     return " ".join(capitalized_name)
 
 
+# Type alias used for yaml entries.
+_yaml_type_alias = dict[str, any]
+
+
+def _find_and_add_summary_details(
+    yaml_data: _yaml_type_alias,
+    summary_type: str,
+    cgc_url: str,
+) -> None:
+    """Finds the summary details to add for a given entry."""
+    uid = yaml_data.get("uid", "")
+    item_to_add = uid if summary_type == CLASS else f"{uid}-summary"
+
+    if item_to_add not in _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE[summary_type][0]:
+        _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE[summary_type][0].append(
+            item_to_add
+        )
+
+    if summary_type in [CLASS]:
+        name_to_use = f"[{uid}]({cgc_url}{uid})"
+
+        _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE[summary_type][1].append({
+            "uid": uid,
+            "name": name_to_use,
+            "fullName": uid,
+            "isExternal": False,
+        })
+        return
+
+    # if summary_type in [METHOD, PROPERTY]:
+    short_name = yaml_data.get("name", "")
+    name_to_use = uid
+    if not (class_name := yaml_data.get("class", "")):
+        class_name = yaml_data.get("module", "")
+    anchor_name = f"#{class_name.replace('.', '_')}_{short_name}"
+    # Extract the first summary line by attempting to detect the first sentence.
+    summary = yaml_data.get("summary", "")
+    first_summary_line = min(
+        summary.split(". ")[0],
+        summary.split(".\n")[0],
+        summary.split("\n\n")[0],
+        key=len,
+    )
+    if first_summary_line and first_summary_line[-1] != ".":
+      first_summary_line += "."
+
+    summary_to_use = (
+        f"{first_summary_line}\n\n"
+        f"See more: [{name_to_use}]({cgc_url}{class_name}{anchor_name})"
+    )
+
+    fields = {
+        "uid": f"{uid}-summary",
+        "name": name_to_use,
+        "summary": summary_to_use,
+        "fullName": uid,
+        "type": 'method',
+    }
+
+    if summary_type == METHOD:
+        fields["syntax"] = {
+            "content": yaml_data.get("syntax").get("content") if yaml_data.get("syntax") else ""
+        }
+    _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE[summary_type][1].append(
+        fields
+    )
+
+
+def _render_summary_content(
+    children_name_and_summary_content: Sequence[Sequence[str | _yaml_type_alias]],
+    entry_name: str,
+    summary_type: str,
+    library_name: str,
+) -> _yaml_type_alias:
+    """Returns the summary content in appropriate YAML format to write."""
+    summary_content = {
+        "items": [{
+            'uid': f'{summary_type.lower()}-summary',
+            'name': entry_name,
+            'fullName': f'{entry_name} Summary',
+            'langs': ['python'],
+            'type': 'package',
+            'summary': f'Summary of entries of {entry_name} for {library_name}.',
+            'children': children_name_and_summary_content[0],
+        }]
+    }
+
+    if summary_type in [CLASS]:
+        summary_content["references"] = children_name_and_summary_content[1]
+
+    if summary_type in [METHOD, PROPERTY]:
+        summary_content["items"].extend(children_name_and_summary_content[1])
+
+    return summary_content
+
+
 def find_uid_to_convert(
     current_word: str,
     words: List[str],
     index: int,
     known_uids: List[str],
     current_object_name: str,
     processed_words: List[str],
@@ -1571,36 +1709,33 @@
                     current_object_name,
                     known_uids
                 )
                 attribute["var_type"] = (
                     markdown_utils.reformat_markdown_to_html(attribute_type))
 
 
-# Type alias used for toc_yaml entries.
-_toc_yaml_type_alias = dict[str, any]
-
 def merge_markdown_and_package_toc(
-    pkg_toc_yaml: list[_toc_yaml_type_alias],
-    markdown_toc_yaml: _toc_yaml_type_alias,
+    pkg_toc_yaml: list[_yaml_type_alias],
+    markdown_toc_yaml: _yaml_type_alias,
     known_uids: set[str],
-) -> tuple[MutableSet[str], list[_toc_yaml_type_alias]]:
+) -> tuple[MutableSet[str], list[_yaml_type_alias]]:
     """
     Merges the markdown and package table of contents.
 
     Args:
         pkg_toc_yaml: table of content for package files.
         markdown_toc_yaml: table fo content for markdown files.
 
     Returns:
         A set of markdown pages that has been added, and the merged table of
         contents file, with files in the correct position.
     """
     def _flatten_toc(
-        toc_yaml_entry: list[_toc_yaml_type_alias],
-    ) -> list[_toc_yaml_type_alias]:
+        toc_yaml_entry: list[_yaml_type_alias],
+    ) -> list[_yaml_type_alias]:
         """Flattens and retrieves all children within pkg_toc_yaml."""
         entries = list(toc_yaml_entry)
         for entry in toc_yaml_entry:
             if (children := entry.get('items')):
                 entries.extend(_flatten_toc(children))
         return entries
 
@@ -1893,26 +2028,46 @@
         pkg_toc_yaml, app.env.markdown_pages, known_uids)
 
     # Remove unused pages after merging the table of contents.
     if added_pages:
         markdown_utils.remove_unused_pages(
             added_pages, app.env.moved_markdown_pages, normalized_outdir)
 
+    if app.env.library_shortname:
+        # Add summary pages as the second entry into the table of contents.
+        pkg_toc_yaml.insert(
+            1,
+            {
+                "name": f"{app.env.library_shortname} APIs",
+                "items": [
+                    {"name": "Overview", "href": "summary_overview.md"},
+                    {"name": "Classes", "href": "summary_class.yml"},
+                    {"name": "Methods", "href": "summary_method.yml"},
+                    {"name": "Properties and Attributes", "href": "summary_property.yml"},
+                ],
+            }
+        )
+
     toc_file = os.path.join(normalized_outdir, 'toc.yml')
     with open(toc_file, 'w') as writable:
         writable.write(
             dump(
                 [{
                     'name': app.config.project,
                     'items': pkg_toc_yaml
                 }],
                 default_flow_style=False,
             )
         )
 
+    cgc_url = (
+        "https://cloud.google.com/python/docs/reference/"
+        f"{app.env.library_shortname}/latest/"
+    )
+    yaml_entry_line = "### YamlMime:UniversalReference\n"
     # Output files
     for uid, data in iter(yaml_map.items()):
 
         for yaml_item in data:
             for obj in yaml_item:
                 # If the entry was disambiguated, update here:
                 obj_full_name = obj['fullName']
@@ -1931,15 +2086,15 @@
 
         out_file = os.path.join(normalized_outdir, '%s.yml' % filename)
         ensuredir(os.path.dirname(out_file))
         if app.verbosity >= 1:
             app.info(bold('[docfx_yaml] ') + darkgreen('Outputting %s' % filename))
 
         with open(out_file, 'w') as out_file_obj:
-            out_file_obj.write('### YamlMime:UniversalReference\n')
+            out_file_obj.write(yaml_entry_line)
             try:
                 dump(
                     {
                         'items': yaml_data,
                         'references': references,
                         'api_name': [],  # Hack around docfx YAML
                     },
@@ -1947,14 +2102,49 @@
                     default_flow_style=False
                 )
             except Exception as e:
                 raise ValueError("Unable to dump object\n{0}".format(yaml_data)) from e
 
         file_name_set.add(filename)
 
+        for entry in yaml_data:
+            if not app.env.library_shortname:
+                break
+            summary_type = _SUMMARY_TYPE_BY_ITEM_TYPE.get(entry.get("type"))
+            if not (summary_type):
+                continue
+
+            _find_and_add_summary_details(entry, summary_type, cgc_url)
+
+    for summary_type in _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE:
+        children_names_and_content = (
+            _ENTRY_NAME_AND_ENTRY_CONTENT_BY_SUMMARY_TYPE[summary_type]
+        )
+        if not all(children_names_and_content):
+            continue
+
+        file_name, entry_name = _FILE_NAME_AND_ENTRY_NAME_BY_SUMMARY_TYPE[summary_type]
+
+        dump_content = _render_summary_content(
+            children_names_and_content,
+            entry_name,
+            summary_type,
+            app.env.library_shortname,
+        )
+
+        file_path_to_use = os.path.join(normalized_outdir, file_name)
+        with open(file_path_to_use, "w") as summary_file_obj:
+            summary_file_obj.write(yaml_entry_line)
+            dump(
+                dump_content,
+                summary_file_obj,
+                default_flow_style=False,
+            )
+
+
     index_file = os.path.join(normalized_outdir, 'index.yml')
     index_children = []
     index_references = []
     for package in pkg_toc_yaml_with_uid:
         for item in package.get("items"):
             index_children.append(item.get('uidname', ''))
             index_references.append({
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/extract_nodes.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/markdown_utils.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/markdown_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -255,14 +255,49 @@
     """
     file_content = f'# {filename}\n\n' + mdfile.read()
     # Reset file position to the beginning to write
     mdfile.seek(0)
     mdfile.write(file_content)
 
 
+def _merge_markdown_content(
+    *,
+    base_file: str,
+    additional_content_file: str,
+    prepend_additional_content: bool = False,
+) -> None:
+    """Merges the Markdown file contents.
+
+    The additional_content_file's contents get appended to the base_file's
+    content.
+
+    Args:
+        base_file: The base content to append content to.
+        additional_content_file: The additional content to be appended to
+            the base file.
+        prepend_additional_content: Optional. If specified, puts the additional
+            content before the base file content.
+    """
+    try:
+        with (
+            open(base_file, 'r+') as base,
+            open(additional_content_file, 'r') as additional_content
+        ):
+            file_content = (
+                f'{additional_content.read()}\n{base.read()}'
+                if prepend_additional_content
+                else f'{base.read()}\n{additional_content.read()}'
+            )
+            base.seek(0)
+            base.write(file_content)
+    except OSError:
+        print("Could not open the given files.")
+        return
+
+
 def move_markdown_pages(
     app: sphinx.application,
     outdir: Path,
     cwd: Optional[List[str]] = [],
 ) -> None:
     """Moves markdown pages to be added to the generated reference documentation.
 
@@ -276,14 +311,21 @@
     """
     # Use this to ignore markdown files that are unnecessary.
     files_to_ignore = [
         "index.md",     # use readme.md instead
 
         "reference.md", # Reference docs overlap with Overview. Will try and incorporate this in later.
                         # See https://github.com/googleapis/sphinx-docfx-yaml/issues/106.
+        "overview_content.md",  # Content will be merged into summary_overview page.
+    ]
+
+    # Use this to move the page but do not add them in the TOC.
+    ignore_in_toc = [
+        "summary_overview.md",  # Already included in the TOC with other
+                                # summary pages.
     ]
 
     files_to_rename = {
         'readme.md': 'index.md',
     }
 
     base_markdown_dir = Path(app.builder.outdir).parent / "markdown"
@@ -307,78 +349,95 @@
     }
 
     # If there is an index.md and no readme.md, use the index.md. Otherwise, we ignore the index.md.
     if ("index.md" in markdown_file_names and
         "readme.md" not in markdown_file_names):
         files_to_ignore.remove("index.md")
 
+    if (
+        "summary_overview.md" in markdown_file_names and
+        "overview_content.md" in markdown_file_names
+    ):
+        # Keep the summary_overview file, prepend the additioanl content.
+        _merge_markdown_content(
+            base_file=markdown_dir/"summary_overview.md",
+            additional_content_file=markdown_dir/"overview_content.md",
+            prepend_additional_content=True,
+        )
+
     # For each file, if it is a markdown file move to the top level pages.
     for mdfile in markdown_dir.iterdir():
         if mdfile.is_dir():
             cwd.append(mdfile.name)
             move_markdown_pages(app, outdir, cwd)
             # Restore the original cwd after finish working on the directory.
             cwd.pop()
 
-        if mdfile.is_file() and mdfile.name.lower() not in files_to_ignore:
-            mdfile_name = ""
+        if not mdfile.is_file() or mdfile.name.lower() in files_to_ignore:
+            continue
 
-            _remove_license(mdfile)
+        mdfile_name = ""
 
-            # Extract the header name for TOC.
-            with open(mdfile) as mdfile_iterator:
-                name = _extract_header_from_markdown(mdfile_iterator)
+        _remove_license(mdfile)
 
-            if not name:
-                with open(mdfile, 'r+') as mdfile_iterator:
-                    mdfile_name = mdfile_iterator.name.split("/")[-1].split(".")[0].capitalize()
+        # Extract the header name for TOC.
+        with open(mdfile) as mdfile_iterator:
+            name = _extract_header_from_markdown(mdfile_iterator)
 
-                    print(f"Could not find a title for {mdfile_iterator.name}. Using {mdfile_name} as the title instead.")
-                    name = mdfile_name
+        if not name:
+            with open(mdfile, 'r+') as mdfile_iterator:
+                mdfile_name = mdfile_iterator.name.split("/")[-1].split(".")[0].capitalize()
 
-                    _prepend_markdown_header(name, mdfile_iterator)
+                print(f"Could not find a title for {mdfile_iterator.name}. Using {mdfile_name} as the title instead.")
+                name = mdfile_name
 
+                _prepend_markdown_header(name, mdfile_iterator)
 
-            mdfile_name_to_use = mdfile.name.lower()
-            if mdfile_name_to_use in files_to_rename:
-                mdfile_name_to_use = files_to_rename[mdfile_name_to_use]
 
-            if cwd and mdfile_name_to_use == "index.md":
-                mdfile_name_to_use = f"{'_'.join(cwd)}_{mdfile_name_to_use}"
+        mdfile_name_to_use = mdfile.name.lower()
+        if mdfile_name_to_use in files_to_rename:
+            mdfile_name_to_use = files_to_rename[mdfile_name_to_use]
 
-            mdfile_outdir = f"{outdir}/{mdfile_name_to_use}"
+        if cwd and mdfile_name_to_use == "index.md":
+            mdfile_name_to_use = f"{'_'.join(cwd)}_{mdfile_name_to_use}"
 
-            shutil.copy(mdfile, mdfile_outdir)
-            app.env.moved_markdown_pages.add(mdfile_name_to_use)
+        mdfile_outdir = f"{outdir}/{mdfile_name_to_use}"
 
-            _highlight_md_codeblocks(mdfile_outdir)
-            _clean_image_links(mdfile_outdir)
+        shutil.copy(mdfile, mdfile_outdir)
 
-            if not cwd:
-                # Use Overview as the name for top-level index file.
-                if 'index.md' in mdfile_name_to_use:
-                    # Save the index page entry.
-                    index_page_entry = {
-                        'name': 'Overview',
-                        'href': 'index.md',
-                    }
-                    continue
+        _highlight_md_codeblocks(mdfile_outdir)
+        _clean_image_links(mdfile_outdir)
 
-                # Use '/' to reserve for top level pages.
-                app.env.markdown_pages['/'].append({
-                    'name': name,
-                    'href': mdfile_name_to_use,
-                })
+        if mdfile.name.lower() in ignore_in_toc:
+            continue
+
+        app.env.moved_markdown_pages.add(mdfile_name_to_use)
+
+        if not cwd:
+            # Use Overview as the name for top-level index file.
+            if 'index.md' in mdfile_name_to_use:
+                # Save the index page entry.
+                index_page_entry = {
+                    'name': 'Overview',
+                    'href': 'index.md',
+                }
                 continue
 
-            # Add the file to the TOC later.
-            app.env.markdown_pages[cwd[-1]].append({
+            # Use '/' to reserve for top level pages.
+            app.env.markdown_pages['/'].append({
                 'name': name,
                 'href': mdfile_name_to_use,
             })
+            continue
+
+        # Add the file to the TOC later.
+        app.env.markdown_pages[cwd[-1]].append({
+            'name': name,
+            'href': mdfile_name_to_use,
+        })
 
     if app.env.markdown_pages.get('/'):
         # Sort the top level pages. Other pages will be sorted when they're
         # added to package level files accordingly.
         app.env.markdown_pages['/'] = sorted(
             app.env.markdown_pages['/'],
             key=lambda entry: entry['href'],
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/monkeypatch.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/nodes.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/settings.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/settings.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/utils.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/docfx_yaml/writer.py` & `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/writer.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.0.1
+Version: 3.1.0
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt` & `gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/setup.py` & `gcp-sphinx-docfx-yaml-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import codecs
 import setuptools
 
 name = 'gcp-sphinx-docfx-yaml'
 description = 'Sphinx Python Domain to DocFX YAML Generator'
-version = '3.0.1'
+version = '3.1.0'
 dependencies = [
     'black',
     'gcp-docuploader',
     'PyYAML',
     'recommonmark',
     'sphinxcontrib-applehelp==1.0.4',
     'sphinxcontrib-devhelp==1.0.2',
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/tests/test_helpers.py` & `gcp-sphinx-docfx-yaml-3.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/tests/test_inspect.py` & `gcp-sphinx-docfx-yaml-3.1.0/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/tests/test_markdown.py` & `gcp-sphinx-docfx-yaml-3.1.0/tests/test_markdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -302,9 +302,53 @@
             markdown_utils._remove_license(test_file.name)
             test_file.seek(0)
 
             with open(want_filename) as mdfile_want:
                 self.assertEqual(test_file.read(), mdfile_want.read())
 
 
+    test_markdown_filenames = [
+        [
+            "tests/markdown_example_base.md",
+            "tests/markdown_example_additional_content.md",
+            "tests/markdown_example_base_expected.md",
+        ],
+        [
+            # The content should be the same as base, and not throw any errors.
+            "tests/markdown_example_base.md",
+            "tests/markdown_example_does_not_exist.md",
+            "tests/markdown_example_base.md",
+        ],
+        [
+            # The content should be the same as base, and not throw any errors.
+            "tests/markdown_example_base.md",
+            "tests/markdown_example_additional_content.md",
+            "tests/markdown_example_prepended_base.md",
+            True,
+        ],
+    ]
+    @parameterized.expand(test_markdown_filenames)
+    def test_merges_markdown_content(
+        self,
+        base_file,
+        additional_file,
+        expected_file,
+        prepend_additional_content=False,
+    ):
+        with tempfile.NamedTemporaryFile(mode='w+', delete=False) as test_file:
+            with open(base_file) as base:
+                test_file.write(base.read())
+                test_file.flush()
+                test_file.seek(0)
+
+            markdown_utils._merge_markdown_content(
+                base_file=test_file.name,
+                additional_content_file=additional_file,
+                prepend_additional_content=prepend_additional_content,
+            )
+            test_file.seek(0)
+
+            with open(expected_file) as mdfile_expected:
+                self.assertEqual(test_file.read(), mdfile_expected.read())
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gcp-sphinx-docfx-yaml-3.0.1/tests/test_unit.py` & `gcp-sphinx-docfx-yaml-3.1.0/tests/test_unit.py`

 * *Files identical despite different names*

