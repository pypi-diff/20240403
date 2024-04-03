# Comparing `tmp/galaxy-navigation-23.2.1.tar.gz` & `tmp/galaxy-navigation-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/navigation/dist/.tmp-btg03zo6/galaxy-navigation-23.2.1.tar", last modified: Thu Feb 22 03:52:27 2024, max compression
+gzip compressed data, was "galaxy-navigation-24.0.0.tar", last modified: Wed Apr  3 02:44:34 2024, max compression
```

## Comparing `galaxy-navigation-23.2.1.tar` & `galaxy-navigation-24.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/navigation/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/navigation/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44049 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/navigation/navigation.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/galaxy_navigation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-22 03:52:27.000000 galaxy-navigation-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-navigation-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.930742 galaxy-navigation-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.930742 galaxy-navigation-24.0.0/galaxy/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44962 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-navigation-23.2.1/HISTORY.rst` & `galaxy-navigation-24.0.0/HISTORY.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-navigation-23.2.1/LICENSE.txt` & `galaxy-navigation-24.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-23.2.1/PKG-INFO` & `galaxy-navigation-24.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy client DOM navigation framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: galaxy-util
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-naivgation.svg
    :target: https://pypi.org/project/galaxy-naivgation/
 
 
 
@@ -44,14 +46,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-navigation-23.2.1/galaxy/navigation/components.py` & `galaxy-navigation-24.0.0/galaxy/navigation/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,16 +251,15 @@
 
     def resolve_component_locator(self, path: Optional[str] = None) -> LocatorT:
         if not path:
             return self._selectors["_"].resolve_component_locator()
 
         def arguments() -> Tuple[str, Optional[Dict[str, str]], Optional[str]]:
             assert path
-            match = CALL_ARGUMENTS_RE.match(path)
-            if match:
+            if match := CALL_ARGUMENTS_RE.match(path):
                 component_name = match.group("SUBCOMPONENT")
                 expression = match.group("ARGS")
                 rest = match.group("REST")
                 if expression:
                     parts = expression.split(",")
                     parameters = {}
                     for part in parts:
```

### Comparing `galaxy-navigation-23.2.1/galaxy/navigation/navigation.yml` & `galaxy-navigation-24.0.0/galaxy/navigation/navigation.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 
 _:  # global stuff
 
   selectors:
     editable_text: '.editable-text'
     tooltip_balloon: '.tooltip'
     tooltip_inner: .tooltip-inner
-    left_panel_drag: '#left-drag'
-    left_panel_collapse: '#left-collapse'
-    right_panel_drag: '#right-drag'
-    right_panel_collapse: '#right-collapse'
+    left_panel_drag: '.flex-panel.left .drag-handle'
+    left_panel_collapse: '.collapse-button.left'
+    right_panel_drag: '.flex-panel.right .drag-handle'
+    right_panel_collapse: '.collapse-button.right'
     by_attribute: '${scope} [${name}="${value}"]'
 
+    confirm_button:
+      type: xpath
+      selector: '//button[contains(text(), "${name}")]'
+
   messages:
     selectors:
       all: '[class*="alert"]'
       error: '.alert-danger'
       warning: '.alert-warning'
       done: '.alert-success'
       info: '.alert-info'
@@ -49,35 +53,32 @@
     logged_out_only: '.loggedout-only'
     storage_dashboard_link:
       selector: 'storage dashboard link'
       type: data-description
 
   labels:
     # top-level menus
+    admin: 'Admin'
     analyze: 'Analyze Data'
-    workflow: 'Workflow'
-    shared_data: 'Shared Data'
-    visualization: 'Visualization'
+    data: 'Data'
     help: 'Help'
     user: 'User'
-    admin: 'Admin'
+    visualization: 'Visualization'
+    workflow: 'Workflow'
 
     # user menu
     logout: 'Sign Out'
     preferences: 'Preferences'
+
+    # data menu
+    libraries: 'Data Libraries'
     histories: 'Histories'
     invocations: 'Workflow Invocations'
     pages: 'Pages'
-    histories_shared_with_me: 'Histories shared with me'
-
-    # Shared data
-    libraries: 'Data Libraries'
-    published_workflows: 'Workflows'
-    published_histories: 'Histories'
-    published_pages: 'Pages'
+    workflows: 'Workflows'
 
 preferences:
   selectors:
     sign_out: "#edit-preferences-sign-out"
     change_password: "#edit-preferences-password"
     manage_information: '#edit-preferences-information'
     toolbox_filters: '#edit-preferences-toolbox-filters'
@@ -233,15 +234,15 @@
   # history tags
   tag_editor:
     selectors:
       _: '${scope} .details .stateless-tags'
       toggle: '${_} .toggle-link'
       display: '${_} .tag span'
       input: '${_} input'
-      tag_area: '${_} .multiselect__tags'
+      tag_area: '${_} .interactive-tags'
       tag_close_btn: '${_} .tag-delete-button'
 
   multi_operations:
     selectors:
       show_button: '.show-history-content-selectors-btn'
       action_button: '.history-contents-list-action-menu-btn'
       action_menu: '.list-action-menu .dropdown-menu'
@@ -258,33 +259,33 @@
       nav_menu: '[data-description="collection breadcrumbs menu"]'
       back_button: '[data-description="collection breadcrumbs menu"] :last'
       back: '.navigation .back'
       title: '.dataset-collection-panel .controls .title .editable-text'
       title_input: '.dataset-collection-panel .controls .title input'
       subtitle: '.dataset-collection-panel .controls .title .subtitle'
       elements_warning: '.dataset-collection-panel .controls .elements-warning'
-      tag_area_button: '.details .stateless-tags .multiselect button'
-      tag_area_input: '.details .stateless-tags .multiselect input'
-      list_items: '.dataset-collection-panel .listing .content-item'
+      tag_area_button: '.details .stateless-tags .toggle-button'
+      tag_area_input: '.details .stateless-tags .headless-multiselect input'
+      list_items: '.dataset-collection-panel .listing-layout .content-item'
       back_to_history: svg[data-description="back to history"]
 
   selectors:
     _: '#current-history-panel'
     search: '#current-history-panel input.search-query'
     refresh_button: '.history-refresh-button'
     name: '.history-title span:last-child'
     name_edit_input:
       selector: 'name input'
       type: data-description
     contents: '.history-index .content-item'
-    empty_message: '.empty-message'
+    empty_message: '#empty-history-message'
     size: '.history-size'
     tag_area: '.details .stateless-tags'
-    tag_area_button: '.details .stateless-tags .multiselect button'
-    tag_area_input: '.details .stateless-tags .multiselect input'
+    tag_area_button: '.details .stateless-tags .toggle-button'
+    tag_area_input: '.details .stateless-tags .headless-multiselect input'
     tag_close_btn: '.tags-display .tag-delete-button'
     tags: '.tag span'
 
     annotation_icon: '.actions .history-annotate-btn'
     annotation_area: '.details .history-annotation'
     annotation_editable_text:
       selector: 'annotation value'
@@ -377,15 +378,15 @@
   selectors:
     _: '.multi-history-panel .content-item${suffix}'
     item: '.multi-history-panel #${history_content_type}-${id}'
     histories: '.multi-history-panel .history-layout'
     current_label: '.details .name'
     switch_history: '.switch-to'
     current_history_check: '#history-column-${history_id} .details .name'
-    empty_message_check: '.empty-message'
+    empty_message_check: '#empty-history-message'
     switch_button: '#history-column-${history_id} .switch-to'
   history_dropdown_menu:
     selectors:
       _: '[history-dropdown-menu="${history_id}"]'
       delete:  '[history-dropdown-menu="${history_id}"] > .delete-history'
       purge:  '[history-dropdown-menu="${history_id}"] > .purge-history'
   copy_history_modal:
@@ -393,27 +394,27 @@
       _: '.modal-dialog'
       copy_btn:
         type: xpath
         selector: '//button[contains(text(), "Copy")]'
 
 published_histories:
   selectors:
-    histories: '#published-histories-table tbody tr'
-    search_input: '#published-histories input.search-query[data-description="filter text input"]'
-    advanced_search_toggle: '#published-histories [data-description="toggle advanced search"]'
-    advanced_search_name_input: '#published-histories-advanced-filter-name'
-    advanced_search_tag_input: '#published-histories-advanced-filter-tag'
-    advanced_search_submit: '#published-histories-advanced-filter-submit'
-    tag_content: '#published-histories-table tbody tr .tag span'
-    column_header: '#published-histories-table thead tr th:nth-child(${column_number})'
+    histories: '#grid-histories-published tbody tr'
+    advanced_search_name_input: '#histories-advanced-filter-name'
+    advanced_search_tag_area: '#histories-advanced-filter-tag .stateless-tags button'
+    advanced_search_tag_input: '#histories-advanced-filter-tag .stateless-tags input'
+    advanced_search_toggle: '#histories-published-grid [data-description="toggle advanced search"]'
+    search_input: '#histories-published-grid input.search-query[data-description="filter text input"]'
+    tab: '#histories-published-tab'
 
 shared_histories:
   selectors:
-    _: ".histories-shared-with-you-by-others"
-    histories: "#grid-table-body tr"
+    _: '#histories-shared-grid'
+    histories: '.grid-table tr'
+    tab: '#histories-shared-tab'
 
 history_copy_elements:
   selectors:
     # Following two don't really work as CSS would only work as jQuery/sizzle I think
     # since the page is dynamically generated.
     # https://stackoverflow.com/questions/10645552/is-it-possible-to-use-an-input-value-attribute-as-a-css-selector
     dataset_checkbox: "input[id='dataset|${id}']"
@@ -426,16 +427,23 @@
   selectors:
     clear_filters: "a.clear-filters-link"
     forward_datasets: ".forward-column .column-datasets"
     reverse_datasets: ".reverse-column .column-datasets"
     name: "input.collection-name"
 
 histories:
-  labels:
-    import_button: 'Import history'
+  selectors:
+    advanced_search_toggle: '#histories-grid [data-description="toggle advanced search"]'
+    advanced_search_name_input: '#histories-advanced-filter-name'
+    advanced_search_tag_area: '#histories-advanced-filter-tag .stateless-tags button'
+    advanced_search_tag_input: '#histories-advanced-filter-tag .stateless-tags input'
+    histories: '.grid-table tr'
+    import_button: '[data-description="grid action import new history"]'
+    reset_input: '#histories-grid [data-description="reset query"]'
+    search_input: '#histories-grid input.search-query[data-description="filter text input"]'
   sharing:
     selectors:
       unshare_user_button: '.share_with_view .multiselect__tag-icon'
       unshare_with_user_button: '.share_with_view [data-email="${email}"] .multiselect__tag-icon'
       user_email_input: '.user-email-input-form'
       submit_sharing_with: '.submit-sharing-with'
       share_with_multiselect: '.share_with_view > .multiselect'
@@ -497,24 +505,17 @@
     running: '.history-import-component .loading-icon'
     success_message: '.history-import-component .alert-success'
 
 pages:
   selectors:
     create: '#page-create'
     submit: '#submit'
-    drop: '.page-dropdown'
-    drop_edit: '.dropdown-item-edit'
-    drop_view: '.dropdown-item-view'
     create_title_input: '#form-element-title input'
     create_slug_input: '#form-element-slug input'
     export: '.markdown-pdf-export'
-    dropdown: '[data-page-dropdown*="${id}"]'
-    index_table: "#page-table"
-    index_rows: "#page-table > tbody > tr:not(.b-table-empty-row, [style*='display: none'])"
-    delete_modal_confirm: '#delete-page-modal-${id}___BV_modal_footer_ .btn-primary'
 
   editor:
     selectors:
       save: '#save-button'
       embed_dataset: '.toolTitle .title-link[data-tool-id="history_dataset_embedded"]'
       embed_workflow_display: '.toolTitle .title-link[data-tool-id="workflow_display"]'
       history_link: '.toolTitle .title-link[data-tool-id="history_link"]'
@@ -570,37 +571,52 @@
     drilldown_expand: '.fa-plus-square'
 
   labels:
     generate_tour: 'Generate Tour'
 
 workflows:
   selectors:
+    shared_with_me_tab: '#shared-with-me'
+    published_tab: '#published a'
     new_button: '#workflow-create'
     import_button: '#workflow-import'
     save_button: '#workflow-save-button'
     search_box: '.workflows-list input.search-query[data-description="filter text input"]'
     clear_filter: '.workflows-list [data-description="reset query"]'
     advanced_search_toggle: '.workflows-list [data-description="toggle advanced search"]'
     advanced_search_name_input: '#workflows-advanced-filter-name'
     advanced_search_tag_input: '#workflows-advanced-filter-tag .stateless-tags'
-    advanced_search_submit: '#workflows-advanced-filter-submit'
-    workflow_table: "#workflow-table"
     workflow_rows: "#workflow-table > tbody > tr:not(.b-table-empty-row, [style*='display: none'])"
+    workflows_list: '#workflows-list'
+    workflows_list_empty: '#workflow-list-empty'
+    workflow_not_found_message: '#no-workflow-found'
+    workflow_card: '.workflow-card'
+    workflow_cards: '#workflow-cards'
     external_link: '.workflow-external-link'
     trs_icon: '.workflow-trs-icon'
     pager: '.gx-workflows-grid-pager'
     pager_page: '.gx-workflows-grid-pager .gx-grid-pager-page [aria-posinset=${page}]'
     pager_page_next: '.gx-workflows-grid-pager .gx-grid-pager-next button'
     pager_page_first: '.gx-workflows-grid-pager .gx-grid-pager-first button'
     pager_page_last: '.gx-workflows-grid-pager .gx-grid-pager-last button'
     pager_page_previous: '.gx-workflows-grid-pager .gx-grid-pager-prev button'
     pager_page_active: '.gx-workflows-grid-pager .gx-grid-pager-page.active button'
-    dropdown: '[data-workflow-dropdown*="${id}"]'
-    run_button: '[data-workflow-run*="${id}"]'
-    bookmark_link: '.workflow-bookmark-link'
+    dropdown: '[data-workflow-actions-dropdown="${id}"]'
+    share_button: '#workflow-share-button'
+    download_button: '#workflow-download-button'
+    run_button: '[data-workflow-run]'
+    edit_button: '.workflow-edit-button'
+    rename_input: '#workflow-name-input'
+    workflow_drop_down: '[data-workflow-actions-dropdown]'
+    delete_button: '.workflow-delete-button'
+    view_button: '.workflow-view-button'
+    workflow_preview_container: '.workflow-preview-container'
+    workflow_preview_information: '.workflow-information'
+    view_external_link: ".workflow-view-external-link-button"
+    bookmark_link: '.workflow-bookmark-button-${action}'
     import_file: '.workflow-import-file'
     import_trs_search: '.workflow-import-trs-search'
     import_trs_id: '.workflow-import-trs-id'
     import_file_link: '.workflow-import-file-link'
     import_trs_search_link: '.workflow-import-trs-search-link'
     import_trs_id_link: '.workflow-import-trs-id-link'
 
@@ -625,27 +641,27 @@
       type: xpath
       selector: "//td[contains(text(), '${workflow_name}')]"
     import_button: ".workflow-import"
     select_server_button: "#dropdownTrsServer"
     import_version: '[data-version-name*="${version}"]'
     select_server:
       type: xpath
-      selector: "//a[contains(@class, 'dropdown-item') and text() = '${server}']"
+      selector: "//a[contains(@class, 'dropdown-item') and normalize-space(text()) = '${server}']"
 
 trs_import:
   selectors:
     input: "#trs-id-input"
     # *= means attribute value contains "${version}"
     # needed because dockstore uses branch or git tag, while workflowhub
     # concatenates name and version
     import_version: '[data-version-name*="${version}"]'
     select_server_button: "#dropdownTrsServer"
     select_server:
       type: xpath
-      selector: "//a[contains(@class, 'dropdown-item') and text() = '${server}']"
+      selector: "//a[contains(@class, 'dropdown-item') and normalize-space(text()) = '${server}']"
     url_input: "#trs-import-url-input"
     url_import_button: "#trs-url-import-button"
 
 workflow_run:
   selectors:
     warning: ".ui-form-composite-messages .alert-warning"
     input_div: "[step-label='${label}']"
@@ -906,16 +922,16 @@
     selectors:
       repo_search: '#toolshed-repo-search'
       search_results: '#shed-search-results'
       upgrade_notification: '#repository-table .badge'
 
   quota:
     selectors:
-      add_new: '.quotas .manage-table-actions .action-button'
-      items: '.quotas #grid-table-body tr'
+      add_new: '[data-description="grid action create new quota"]'
+      items: '#quotas-grid table tr'
       add_form: "[url='/admin/create_quota']"
       add_form_submit: "[url='/admin/create_quota'] #submit"
 
   index:
     selectors:
       datatypes: '#admin-link-datatypes'
       dependencies: '#admin-link-manage-dependencies'
@@ -951,16 +967,16 @@
     dm_job: '#job-${job_id}'
     dm_job_breadcrumb: '#breadcrumb'
     dm_job_data_manager_card: '#data-manager-card'
     dm_job_data_card: '#data-card-${hda_index}'
     dm_table_button: '#${data_table}-table'
     dm_table_card: '#data-table-card'
     users_grid: '#users-grid'
-    users_grid_create_button: '.manage-table-actions .action-button'
-    groups_grid_create_button: '.manage-table-actions .action-button'
+    users_grid_create_button: '[data-description="grid action create new user"]'
+    groups_grid_create_button: '[data-description="grid action create new group"]'
     registration_form: 'form#registration'
     groups_grid: '#groups-grid'
     roles_grid: '#roles-grid'
     groups_create_view: '#submit'
 
 libraries:
 
@@ -1039,16 +1055,16 @@
   dataset:
     selectors:
       table: '.dataset_table'
       table_rows: '.dataset_table tbody tr'
 
 grids:
   selectors:
-    body: '#grid-table-body'
-    free_text_search: '#input-free-text-search-filter'
+    body: '.grid-table'
+    free_text_search: '[data-description="filter text input"]'
 
 gies:
   jupyter:
     selectors:
       body: 'body.notebook_app'
       trusted_notification: '#notification_trusted'
```

### Comparing `galaxy-navigation-23.2.1/galaxy_navigation.egg-info/PKG-INFO` & `galaxy-navigation-24.0.0/galaxy_navigation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy client DOM navigation framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: galaxy-util
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-naivgation.svg
    :target: https://pypi.org/project/galaxy-naivgation/
 
 
 
@@ -44,14 +46,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-navigation-23.2.1/setup.cfg` & `galaxy-navigation-24.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy client DOM navigation framework
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-navigation
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	PyYAML
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

