# Comparing `tmp/elasticsearch_curator-8.0.8.tar.gz` & `tmp/elasticsearch_curator-8.0.9.tar.gz`

## Comparing `elasticsearch_curator-8.0.8.tar` & `elasticsearch_curator-8.0.9.tar`

### file list

```diff
@@ -1,67 +1,61 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/_version.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/classdef.py
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/config_utils.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/curator_cli.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/exceptions.py
--rw-r--r--   0        0        0    65580 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/indexlist.py
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/logtools.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/repomgrcli.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/singletons.py
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/snapshotlist.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/alias.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/allocation.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/close.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/cluster_routing.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/cold2frozen.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/create_index.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/delete_indices.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/forcemerge.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/index_settings.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/open.py
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/reindex.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/replicas.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/rollover.py
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/shrink.py
--rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/actions/snapshot.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/__init__.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/alias.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/allocation.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/close.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/delete.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/forcemerge.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/object_class.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/open_indices.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/replicas.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/restore.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/rollover.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/show.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/shrink.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/snapshot.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/cli_singletons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/filter_elements.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/filtertypes.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/logging_defaults.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/option_defaults.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/defaults/settings.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/__init__.py
--rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/date_ops.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/getters.py
--rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/testers.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/utils.py
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/helpers/waiters.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/actions.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/filter_functions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/logconfig.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/options.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/curator/validators/schemacheck.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/.gitignore
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/NOTICE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/README.rst
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/pyproject.toml
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.8/PKG-INFO
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/_version.py
+-rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/classdef.py
+-rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/exceptions.py
+-rw-r--r--   0        0        0    65601 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/indexlist.py
+-rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/repomgrcli.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/singletons.py
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/snapshotlist.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/alias.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/allocation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/close.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/cluster_routing.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/cold2frozen.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/create_index.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/delete_indices.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/forcemerge.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/index_settings.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/open.py
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/reindex.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/replicas.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/rollover.py
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/shrink.py
+-rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/actions/snapshot.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/__init__.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/alias.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/allocation.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/close.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/delete.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/forcemerge.py
+-rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/object_class.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/open_indices.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/replicas.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/restore.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/rollover.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/show.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/shrink.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/snapshot.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/cli_singletons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/defaults/__init__.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/defaults/filter_elements.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/defaults/filtertypes.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/defaults/option_defaults.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/defaults/settings.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/__init__.py
+-rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/date_ops.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/getters.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/testers.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/utils.py
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/helpers/waiters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/validators/__init__.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/validators/actions.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/validators/filter_functions.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/curator/validators/options.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/.gitignore
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/LICENSE
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/NOTICE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/README.rst
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.9/PKG-INFO
```

### Comparing `elasticsearch_curator-8.0.8/curator/classdef.py` & `elasticsearch_curator-8.0.9/curator/classdef.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Other Classes"""
 import logging
-from es_client.exceptions import ConfigurationError as ESclient_ConfigError
+from es_client.exceptions import FailedValidation
+from es_client.helpers.schemacheck import password_filter
 from es_client.helpers.utils import get_yaml
 from curator import IndexList, SnapshotList
 from curator.actions import CLASS_MAP
 from curator.exceptions import ConfigurationError
-from curator.config_utils import password_filter
 from curator.helpers.testers import validate_actions
 
 # Let me tell you the story of the nearly wasted afternoon and the research that went into this
 # seemingly simple work-around. Actually, no. It's even more wasted time writing that story here.
 # Suffice to say that I couldn't use the CLASS_MAP with class objects to directly map them to class
 # instances. The Wrapper class and the ActionDef.instantiate method do all of the work for me,
 # allowing me to easily and cleanly pass *args and **kwargs to the individual action classes of
@@ -58,15 +58,15 @@
         :type action_file: str
 
         :returns: The result from passing ``action_file`` to
             :py:func:`~.curator.helpers.testers.validate_actions`
         """
         try:
             return validate_actions(get_yaml(action_file))
-        except (ESclient_ConfigError, UnboundLocalError) as err:
+        except (FailedValidation, UnboundLocalError) as err:
             self.logger.critical('Configuration Error: %s', err)
             raise ConfigurationError from err
 
     def parse_actions(self, all_actions):
         """Parse the individual actions found in ``all_actions['actions']``
 
         :param all_actions: All actions, each its own dictionary behind a numeric key. Making the
```

### Comparing `elasticsearch_curator-8.0.8/curator/exceptions.py` & `elasticsearch_curator-8.0.9/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/indexlist.py` & `elasticsearch_curator-8.0.9/curator/indexlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Index List Class"""
 import re
 import itertools
 import logging
 from elasticsearch8.exceptions import NotFoundError, TransportError
+from es_client.helpers.schemacheck import SchemaCheck
 from es_client.helpers.utils import ensure_list
 from curator.defaults import settings
 from curator.exceptions import ActionError, ConfigurationError, MissingArgument, NoIndices
 from curator.helpers.date_ops import (
     absolute_date_range, date_range, fix_epoch, get_date_regex, get_point_of_reference,
     get_unit_count_from_name, TimestringSearch
 )
 from curator.helpers.getters import byte_size, get_indices
 from curator.helpers.testers import verify_client_object
 from curator.helpers.utils import chunk_index_list, report_failure, to_csv
-from curator.validators import SchemaCheck
 from curator.validators.filter_functions import filterstructure
 
 class IndexList:
     """IndexList class"""
     def __init__(self, client):
         verify_client_object(client)
         self.loggit = logging.getLogger('curator.indexlist')
@@ -308,15 +308,17 @@
                 if 'routing' in wli['settings']['index']:
                     sii['routing'] = wli['settings']['index']['routing']
         self.loggit.debug('Getting index settings -- END')
 
     def get_index_state(self):
         """
         For each index in self.indices, populate ``index_info`` with:
+
             state (open or closed)
+        
         from the cat API
         """
         self.loggit.debug('Getting index state -- BEGIN')
         self.empty_list_check()
         fields = ['state']
         for lst in chunk_index_list(self.indices):
             # This portion here is to ensure that we're not polling for data unless we must
```

### Comparing `elasticsearch_curator-8.0.8/curator/repomgrcli.py` & `elasticsearch_curator-8.0.9/curator/repomgrcli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """es_repo_mgr CLI"""
 import sys
 import logging
 import pprint
 import click
 from elasticsearch8 import ApiError, NotFoundError
-from es_client.builder import ClientArgs, OtherArgs, Builder
-from es_client.helpers.utils import check_config, get_yaml, prune_nones, verify_url_schema
-from curator.defaults import settings
-from curator.config_utils import check_logging_config, set_logging
+from es_client.defaults import LOGGING_SETTINGS, SHOW_OPTION
+from es_client.builder import Builder
+from es_client.helpers.config import cli_opts, context_settings, get_config, get_args
+from es_client.helpers.logging import configure_logging
+from es_client.helpers.utils import option_wrapper, prune_nones
+from curator.defaults.settings import CLICK_DRYRUN, default_config_file, footer
 from curator.helpers.getters import get_repository
 from curator._version import __version__
-from curator.cli_singletons.utils import get_width
+
+ONOFF = {'on': '', 'off': 'no-'}
+click_opt_wrap = option_wrapper()
 
 # pylint: disable=unused-argument
 def delete_callback(ctx, param, value):
     """Callback if command ``delete`` called
 
     If the action is ``delete``, this is the :py:class:`click.Parameter` callback function if you
     used the ``--yes`` flag.
@@ -35,15 +39,17 @@
 def show_repos(client):
     """Show all repositories
 
     :param client: A client connection object
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
     :rtype: None
     """
+    logger = logging.getLogger(__name__)
     for repository in sorted(get_repository(client, '*').keys()):
+        logger.debug('REPOSITORY = %s', repository)
         click.echo(f'{repository}')
     sys.exit(0)
 
 def get_client(ctx):
     """
     :param ctx: The :py:class:`click` Context
     :type ctx: :py:class:`~.click.Context`
@@ -291,146 +297,126 @@
         'max_restore_bytes_per_sec': max_restore_rate,
         'max_snapshot_bytes_per_sec': max_snapshot_rate,
         'readonly': readonly,
     }
     create_repo(ctx, repo_name=name, repo_type='source', repo_settings=source_settings, verify=verify)
 
 
-# pylint: disable=unused-argument, redefined-builtin
-@click.group(context_settings=get_width())
-@click.option('--config', help='Path to configuration file.', type=click.Path(exists=True), default=settings.config_file())
-@click.option('--hosts', help='Elasticsearch URL to connect to', multiple=True)
-@click.option('--cloud_id', help='Shorthand to connect to Elastic Cloud instance')
-@click.option('--id', help='API Key "id" value', type=str)
-@click.option('--api_key', help='API Key "api_key" value', type=str)
-@click.option('--username', help='Username used to create "basic_auth" tuple')
-@click.option('--password', help='Password used to create "basic_auth" tuple')
-@click.option('--bearer_auth', type=str)
-@click.option('--opaque_id', type=str)
-@click.option('--request_timeout', help='Request timeout in seconds', type=float)
-@click.option('--http_compress', help='Enable HTTP compression', is_flag=True, default=None)
-@click.option('--verify_certs', help='Verify SSL/TLS certificate(s)', is_flag=True, default=None)
-@click.option('--ca_certs', help='Path to CA certificate file or directory')
-@click.option('--client_cert', help='Path to client certificate file')
-@click.option('--client_key', help='Path to client certificate key')
-@click.option('--ssl_assert_hostname', help='Hostname or IP address to verify on the node\'s certificate.', type=str)
-@click.option('--ssl_assert_fingerprint', help='SHA-256 fingerprint of the node\'s certificate. If this value is given then root-of-trust verification isn\'t done and only the node\'s certificate fingerprint is verified.', type=str)
-@click.option('--ssl_version', help='Minimum acceptable TLS/SSL version', type=str)
-@click.option('--master-only', help='Only run if the single host provided is the elected master', is_flag=True, default=None)
-@click.option('--skip_version_test', help='Do not check the host version', is_flag=True, default=None)
-@click.option('--dry-run', is_flag=True, help='Do not perform any changes. NON-FUNCTIONAL PLACEHOLDER! DO NOT USE!')
-@click.option('--loglevel', help='Log level', type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']))
-@click.option('--logfile', help='log file')
-@click.option('--logformat', help='Log output format', type=click.Choice(['default', 'logstash', 'json', 'ecs']))
-@click.version_option(version=__version__)
+# pylint: disable=unused-argument, redefined-builtin, too-many-arguments, too-many-locals
+@click.group('repo_mgr_cli', context_settings=context_settings(), epilog=footer(__version__))
+@click_opt_wrap(*cli_opts('config'))
+@click_opt_wrap(*cli_opts('hosts'))
+@click_opt_wrap(*cli_opts('cloud_id'))
+@click_opt_wrap(*cli_opts('api_token'))
+@click_opt_wrap(*cli_opts('id'))
+@click_opt_wrap(*cli_opts('api_key'))
+@click_opt_wrap(*cli_opts('username'))
+@click_opt_wrap(*cli_opts('password'))
+@click_opt_wrap(*cli_opts('bearer_auth'))
+@click_opt_wrap(*cli_opts('opaque_id'))
+@click_opt_wrap(*cli_opts('request_timeout'))
+@click_opt_wrap(*cli_opts('http_compress', onoff=ONOFF))
+@click_opt_wrap(*cli_opts('verify_certs', onoff=ONOFF))
+@click_opt_wrap(*cli_opts('ca_certs'))
+@click_opt_wrap(*cli_opts('client_cert'))
+@click_opt_wrap(*cli_opts('client_key'))
+@click_opt_wrap(*cli_opts('ssl_assert_hostname'))
+@click_opt_wrap(*cli_opts('ssl_assert_fingerprint'))
+@click_opt_wrap(*cli_opts('ssl_version'))
+@click_opt_wrap(*cli_opts('master-only', onoff=ONOFF))
+@click_opt_wrap(*cli_opts('skip_version_test', onoff=ONOFF))
+@click_opt_wrap(*cli_opts('dry-run', settings=CLICK_DRYRUN))
+@click_opt_wrap(*cli_opts('loglevel', settings=LOGGING_SETTINGS))
+@click_opt_wrap(*cli_opts('logfile', settings=LOGGING_SETTINGS))
+@click_opt_wrap(*cli_opts('logformat', settings=LOGGING_SETTINGS))
+@click.version_option(__version__, '-v', '--version', prog_name="es_repo_mgr")
 @click.pass_context
 def repo_mgr_cli(
-    ctx, config, hosts, cloud_id, id, api_key, username, password, bearer_auth,
+    ctx, config, hosts, cloud_id, api_token, id, api_key, username, password, bearer_auth,
     opaque_id, request_timeout, http_compress, verify_certs, ca_certs, client_cert, client_key,
     ssl_assert_hostname, ssl_assert_fingerprint, ssl_version, master_only, skip_version_test,
     dry_run, loglevel, logfile, logformat
 ):
-    """Repository manager for Elasticsearch Curator."""
-    # Ensure a passable ctx object
-    ctx.ensure_object(dict)
-
-    # Extract client args
-    client_args = ClientArgs()
-    other_args = OtherArgs()
-    if config:
-        from_yaml = get_yaml(config)
-        raw_config = check_config(from_yaml)
-        client_args.update_settings(raw_config['client'])
-        other_args.update_settings(raw_config['other_settings'])
-
-    # Check for log settings from config file
-    init_logcfg = check_logging_config(from_yaml)
-
-    # Override anything with options from the command-line
-    if loglevel:
-        init_logcfg['loglevel'] = loglevel
-    if logfile:
-        init_logcfg['logfile'] = logfile
-    if logformat:
-        init_logcfg['logformat'] = logformat
-
-    # Now enable logging with the merged settings
-    set_logging(check_logging_config({'logging': init_logcfg}))
-    logger = logging.getLogger(__name__)
-    logger.debug('Logging options validated.')
-
-    hostslist = []
-    if hosts:
-        for host in list(hosts):
-            hostslist.append(verify_url_schema(host))
-    else:
-        hostslist = None
-
-    cli_client = prune_nones({
-        'hosts': hostslist,
-        'cloud_id': cloud_id,
-        'bearer_auth': bearer_auth,
-        'opaque_id': opaque_id,
-        'request_timeout': request_timeout,
-        'http_compress': http_compress,
-        'verify_certs': verify_certs,
-        'ca_certs': ca_certs,
-        'client_cert': client_cert,
-        'client_key': client_key,
-        'ssl_assert_hostname': ssl_assert_hostname,
-        'ssl_assert_fingerprint': ssl_assert_fingerprint,
-        'ssl_version': ssl_version
-    })
-
-    cli_other = prune_nones({
-        'master_only': master_only,
-        'skip_version_test': skip_version_test,
-        'username': username,
-        'password': password,
-        'api_key': {
-            'id': id,
-            'api_key': api_key
-        }
-    })
+    """
+    Repository manager for Elasticsearch Curator
+    
+    The default $HOME/.curator/curator.yml configuration file (--config)
+    can be used but is not needed.
+    
+    Command-line settings will always override YAML configuration settings.
 
-    # Remove `api_key` root key if `id` and `api_key` are both None
-    if id is None and api_key is None:
-        del cli_other['api_key']
-
-    # If hosts are in the config file, but cloud_id is specified at the command-line,
-    # we need to remove the hosts parameter as cloud_id and hosts are mutually exclusive
-    if cloud_id:
-        click.echo('cloud_id provided at CLI, superseding any other configured hosts')
-        client_args.hosts = None
-        cli_client.pop('hosts', None)
-
-    # Likewise, if hosts are provided at the command-line, but cloud_id was in the config file,
-    # we need to remove the cloud_id parameter from the config file-based dictionary before merging
-    if hosts:
-        click.echo('hosts specified manually, superseding any other cloud_id or hosts')
-        client_args.hosts = None
-        client_args.cloud_id = None
-        cli_client.pop('cloud_id', None)
-
-    # Update the objects if we have settings after pruning None values
-    if cli_client:
-        client_args.update_settings(cli_client)
-    if cli_other:
-        other_args.update_settings(cli_other)
+    Some less-frequently used client configuration options are now hidden. To see the full list,
+    run:
 
-    # Build a "final_config" that reflects CLI args overriding anything from a config_file
-    final_config = {
+        es_repo_mgr show-all-options
+    """
+    ctx.obj = {}
+    # Ensure a passable ctx object
+    ctx.ensure_object(dict)
+    ctx.obj['dry_run'] = dry_run
+    cfg = get_config(ctx.params, default_config_file())
+    configure_logging(cfg, ctx.params)
+    logger = logging.getLogger('curator.repomgrcli')
+    client_args, other_args = get_args(ctx.params, cfg)
+    ctx.obj['esconfig'] = {
         'elasticsearch': {
             'client': prune_nones(client_args.asdict()),
             'other_settings': prune_nones(other_args.asdict())
         }
     }
-    ctx.obj['esconfig'] = final_config
-    ctx.obj['dry_run'] = dry_run
-    logger.debug('YOU HAVE REACHED THIS PHASE')
+    logger.debug('Exiting initial command function...')
+    
+
+@repo_mgr_cli.command(
+    'show-all-options',
+    context_settings=context_settings(),
+    short_help='Show all configuration options',
+    epilog=footer(__version__))
+@click_opt_wrap(*cli_opts('config'))
+@click_opt_wrap(*cli_opts('hosts'))
+@click_opt_wrap(*cli_opts('cloud_id'))
+@click_opt_wrap(*cli_opts('api_token'))
+@click_opt_wrap(*cli_opts('id'))
+@click_opt_wrap(*cli_opts('api_key'))
+@click_opt_wrap(*cli_opts('username'))
+@click_opt_wrap(*cli_opts('password'))
+@click_opt_wrap(*cli_opts('bearer_auth', override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('opaque_id', override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('request_timeout'))
+@click_opt_wrap(*cli_opts('http_compress', onoff=ONOFF, override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('verify_certs', onoff=ONOFF))
+@click_opt_wrap(*cli_opts('ca_certs'))
+@click_opt_wrap(*cli_opts('client_cert'))
+@click_opt_wrap(*cli_opts('client_key'))
+@click_opt_wrap(*cli_opts('ssl_assert_hostname', override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('ssl_assert_fingerprint', override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('ssl_version', override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('master-only', onoff=ONOFF, override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('skip_version_test', onoff=ONOFF, override=SHOW_OPTION))
+@click_opt_wrap(*cli_opts('dry-run', settings=CLICK_DRYRUN))
+@click_opt_wrap(*cli_opts('loglevel', settings=LOGGING_SETTINGS))
+@click_opt_wrap(*cli_opts('logfile', settings=LOGGING_SETTINGS))
+@click_opt_wrap(*cli_opts('logformat', settings=LOGGING_SETTINGS))
+@click.version_option(__version__, '-v', '--version', prog_name="es_repo_mgr")
+@click.pass_context
+def show_all_options(
+    ctx, config, hosts, cloud_id, api_token, id, api_key, username, password, bearer_auth,
+    opaque_id, request_timeout, http_compress, verify_certs, ca_certs, client_cert, client_key,
+    ssl_assert_hostname, ssl_assert_fingerprint, ssl_version, master_only, skip_version_test,
+    dry_run, loglevel, logfile, logformat
+):
+    """
+    ALL CLIENT OPTIONS
+    
+    The following is the full list of settings available for configuring a connection using
+    command-line options.
+    """
+    ctx = click.get_current_context()
+    click.echo(ctx.get_help())
+    ctx.exit()
 
 @repo_mgr_cli.group('create')
 @click.pass_context
 def _create(ctx):
     """Create an Elasticsearch repository"""
 _create.add_command(azure)
 _create.add_command(gcs)
```

### Comparing `elasticsearch_curator-8.0.8/curator/snapshotlist.py` & `elasticsearch_curator-8.0.9/curator/snapshotlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """SnapshotList"""
 import re
 import logging
+from es_client.helpers.schemacheck import SchemaCheck
 from curator.exceptions import ConfigurationError, FailedExecution, MissingArgument, NoSnapshots
 from curator.helpers.date_ops import (
     absolute_date_range, date_range, fix_epoch, get_date_regex, get_point_of_reference,
     TimestringSearch
 )
 from curator.helpers.getters import get_snapshot_data
 from curator.helpers.testers import repository_exists, verify_client_object
 from curator.helpers.utils import report_failure
 from curator.defaults import settings
-from curator.validators import SchemaCheck
 from curator.validators.filter_functions import filterstructure
 
 class SnapshotList:
     """Snapshot list object"""
     def __init__(self, client, repository=None):
         verify_client_object(client)
         if not repository:
```

### Comparing `elasticsearch_curator-8.0.8/curator/actions/__init__.py` & `elasticsearch_curator-8.0.9/curator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/alias.py` & `elasticsearch_curator-8.0.9/curator/actions/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/allocation.py` & `elasticsearch_curator-8.0.9/curator/actions/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/close.py` & `elasticsearch_curator-8.0.9/curator/actions/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/cluster_routing.py` & `elasticsearch_curator-8.0.9/curator/actions/cluster_routing.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/cold2frozen.py` & `elasticsearch_curator-8.0.9/curator/actions/cold2frozen.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/create_index.py` & `elasticsearch_curator-8.0.9/curator/actions/create_index.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/delete_indices.py` & `elasticsearch_curator-8.0.9/curator/actions/delete_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/forcemerge.py` & `elasticsearch_curator-8.0.9/curator/actions/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/index_settings.py` & `elasticsearch_curator-8.0.9/curator/actions/index_settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/open.py` & `elasticsearch_curator-8.0.9/curator/actions/open.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/reindex.py` & `elasticsearch_curator-8.0.9/curator/actions/reindex.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/replicas.py` & `elasticsearch_curator-8.0.9/curator/actions/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/rollover.py` & `elasticsearch_curator-8.0.9/curator/actions/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/shrink.py` & `elasticsearch_curator-8.0.9/curator/actions/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/actions/snapshot.py` & `elasticsearch_curator-8.0.9/curator/actions/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/__init__.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/alias.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/replicas.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,45 @@
-"""Alias Singleton"""
-import logging
+"""Change Replica Count Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, json_to_dict, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
-@click.command(context_settings=get_width())
-@click.option('--name', type=str, help='Alias name', required=True)
+@click.command(context_settings=context_settings())
+@click.option('--count', type=int, required=True, help='Number of replicas (max 10)')
 @click.option(
-    '--add',
-    callback=validate_filter_json,
-    help='JSON array of filters selecting indices to ADD to alias',
-    default=None
-)
-@click.option(
-    '--remove',
-    callback=validate_filter_json,
-    help='JSON array of filters selecting indices to REMOVE from alias',
-    default=None
+    '--wait_for_completion/--no-wait_for_completion',
+    default=False,
+    help='Wait for replication to complete',
+    show_default=True
 )
 @click.option(
-    '--warn_if_no_indices',
+    '--ignore_empty_list',
     is_flag=True,
-    help='Do not raise exception if there are no actionable indices in add/remove'
-)
-@click.option(
-    '--extra_settings',
-    help='JSON version of extra_settings (see documentation)',
-    callback=json_to_dict
+    help='Do not raise exception if there are no actionable indices'
 )
 @click.option(
     '--allow_ilm_indices/--no-allow_ilm_indices',
     help='Allow Curator to operate on Index Lifecycle Management monitored indices.',
     default=False,
     show_default=True
 )
+@click.option(
+    '--filter_list',
+    callback=validate_filter_json,
+    help='JSON array of filters selecting indices to act on.',
+    required=True
+)
 @click.pass_context
-def alias(ctx, name, add, remove, warn_if_no_indices, extra_settings, allow_ilm_indices):
+def replicas(ctx, count, wait_for_completion, ignore_empty_list, allow_ilm_indices, filter_list):
     """
-    Add/Remove Indices to/from Alias
+    Change Replica Count
     """
-    logger = logging.getLogger('cli.singleton.alias')
     manual_options = {
-        'name': name,
-        'extra_settings': extra_settings,
+        'count': count,
+        'wait_for_completion': wait_for_completion,
         'allow_ilm_indices': allow_ilm_indices,
     }
-    logger.debug('manual_options %s', manual_options)
     # ctx.info_name is the name of the function or name specified in @click.command decorator
-    ignore_empty_list = warn_if_no_indices
-    logger.debug('ctx.info_name %s', ctx.info_name)
-    logger.debug('ignore_empty_list %s', ignore_empty_list)
-    logger.debug('add %s', add)
-    logger.debug('remove %s', remove)
-    logger.debug('warn_if_no_indices %s', warn_if_no_indices)
-    logger.debug("ctx.obj['dry_run'] %s", ctx.obj['dry_run'])
     action = CLIAction(
-        ctx.info_name,
-        ctx.obj['config'],
-        manual_options,
-        [], # filter_list is empty in our case
-        ignore_empty_list,
-        add=add, remove=remove, warn_if_no_indices=warn_if_no_indices, # alias specific kwargs
-    )
-    logger.debug('We did not get here, did we?')
+        ctx.info_name, ctx.obj['config'], manual_options, filter_list, ignore_empty_list)
     action.do_singleton_action(dry_run=ctx.obj['dry_run'])
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/allocation.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/allocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Allocation Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--key', type=str, required=True, help='Node identification tag')
 @click.option('--value', type=str, default=None, help='Value associated with --key')
 @click.option('--allocation_type', type=click.Choice(['require', 'include', 'exclude']))
 @click.option(
     '--wait_for_completion/--no-wait_for_completion',
     default=False,
     help='Wait for the allocation to complete',
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/close.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/close.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Close Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--delete_aliases', is_flag=True, help='Delete all aliases from indices to be closed')
 @click.option('--skip_flush', is_flag=True, help='Skip flush phase for indices to be closed')
 @click.option(
     '--ignore_empty_list',
     is_flag=True,
     help='Do not raise exception if there are no actionable indices'
 )
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/delete.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Delete Index and Delete Snapshot Singletons"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
 #### Indices ####
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option(
     '--ignore_empty_list',
     is_flag=True,
     help='Do not raise exception if there are no actionable indices'
 )
 @click.option(
     '--allow_ilm_indices/--no-allow_ilm_indices',
@@ -34,15 +35,15 @@
         {'allow_ilm_indices':allow_ilm_indices},
         filter_list,
         ignore_empty_list
     )
     action.do_singleton_action(dry_run=ctx.obj['dry_run'])
 
 #### Snapshots ####
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--repository', type=str, required=True, help='Snapshot repository name')
 @click.option('--retry_count', type=int, help='Number of times to retry (max 3)')
 @click.option('--retry_interval', type=int, help='Time in seconds between retries')
 @click.option(
     '--ignore_empty_list',
     is_flag=True,
     help='Do not raise exception if there are no actionable snapshots'
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/forcemerge.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/forcemerge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ForceMerge Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option(
     '--max_num_segments',
     type=int,
     required=True,
     help='Maximum number of segments per shard (minimum of 1)'
 )
 @click.option(
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/object_class.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/object_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Object builder"""
 import logging
 import sys
 from voluptuous import Schema
 from es_client.builder import Builder
+from es_client.exceptions import FailedValidation
+from es_client.helpers.schemacheck import SchemaCheck
 from es_client.helpers.utils import prune_nones
 from curator import IndexList, SnapshotList
 from curator.actions import (
     Alias, Allocation, Close, ClusterRouting, CreateIndex, DeleteIndices, ForceMerge,
     IndexSettings, Open, Reindex, Replicas, Rollover, Shrink, Snapshot, DeleteSnapshots, Restore
 )
 from curator.defaults.settings import snapshot_actions
 from curator.exceptions import ConfigurationError, NoIndices, NoSnapshots
 from curator.helpers.testers import validate_filters
-from curator.validators import SchemaCheck, options
+from curator.validators import options
 from curator.validators.filter_functions import validfilters
 
 CLASS_MAP = {
     'alias' :  Alias,
     'allocation' : Allocation,
     'close' : Close,
     'cluster_routing' : ClusterRouting,
@@ -97,17 +99,16 @@
         elif action in ['cluster_routing', 'create_index', 'rollover']:
             self.action_kwargs = {}
             if action == 'rollover':
                 self.logger.debug('rollover option_dict = %s', option_dict)
         else:
             self.check_filters(filter_list)
 
-        builder = Builder(configdict=client_args)
-
         try:
+            builder = Builder(configdict=client_args)
             builder.connect()
         # pylint: disable=broad-except
         except Exception as exc:
             raise ConfigurationError(
                 f'Unable to connect to Elasticsearch as configured: {exc}') from exc
         # If we're here, we'll see the output from GET http(s)://hostname.tld:PORT
         self.logger.debug('Connection result: %s', builder.client.info())
@@ -135,30 +136,30 @@
                 'options',
                 f'{self.action} singleton action "options"'
             ).result()
             self.options = self.prune_excluded(_)
             # Remove this after the schema check, as the action class won't need it as an arg
             if self.action in ['delete_snapshots', 'restore']:
                 del self.options['repository']
-        except ConfigurationError as exc:
+        except FailedValidation as exc:
             self.logger.critical('Unable to parse options: %s', exc)
             sys.exit(1)
 
     def check_filters(self, filter_dict, loc='singleton', key='filters'):
         """Validate provided filters"""
         try:
             self.logger.debug('Validating provided filters: %s', filter_dict)
             _ = SchemaCheck(
                 filter_dict,
                 Schema(validfilters(self.action, location=loc)),
                 key,
                 f'{self.action} singleton action "{key}"'
             ).result()
             self.filters = validate_filters(self.action, _)
-        except ConfigurationError as exc:
+        except FailedValidation as exc:
             self.logger.critical('Unable to parse filters: %s', exc)
             sys.exit(1)
 
     def do_filters(self):
         """Actually run the filters"""
         self.logger.debug('Running filters and testing for empty list object')
         if self.allow_ilm:
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/open_indices.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/open_indices.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Open (closed) Index Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
-@click.command(name='open', context_settings=get_width())
+@click.command(name='open', context_settings=context_settings())
 @click.option(
     '--ignore_empty_list',
     is_flag=True,
     help='Do not raise exception if there are no actionable indices'
 )
 @click.option(
     '--allow_ilm_indices/--no-allow_ilm_indices',
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/restore.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/restore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Snapshot Restore Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, json_to_dict, validate_filter_json
+from curator.cli_singletons.utils import json_to_dict, validate_filter_json
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--repository', type=str, required=True, help='Snapshot repository')
 @click.option('--name', type=str, help='Snapshot name', required=False, default=None)
 @click.option('--index', multiple=True, help='Index name to restore. (Can invoke repeatedly for multiple indices)')
 @click.option('--rename_pattern', type=str, help='Rename pattern', required=False, default=None)
 @click.option('--rename_replacement', type=str, help='Rename replacement', required=False, default=None)
 @click.option('--extra_settings', type=str, help='JSON version of extra_settings (see documentation)', callback=json_to_dict)
 @click.option('--include_aliases', is_flag=True, show_default=True, help='Include aliases with restored indices.')
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/rollover.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/rollover.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Index Rollover Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from es_client.helpers.utils import prune_nones
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, json_to_dict
+from curator.cli_singletons.utils import json_to_dict
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--name', type=str, help='Alias name', required=True)
 @click.option('--max_age', type=str, help='max_age condition value (see documentation)')
 @click.option('--max_docs', type=str, help='max_docs condition value (see documentation)')
 @click.option('--max_size', type=str, help='max_size condition value (see documentation)')
 @click.option('--extra_settings', type=str, help='JSON version of extra_settings (see documentation)', callback=json_to_dict)
 @click.option( '--new_index', type=str, help='Optional new index name (see documentation)')
 @click.option('--wait_for_active_shards', type=int, default=1, show_default=True, help='Wait for number of shards to be active before returning')
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/show.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/show.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Show Index/Snapshot Singletons"""
 from datetime import datetime
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 from curator.helpers.getters import byte_size
+from curator.defaults.settings import footer
+from curator._version import __version__
 
 #### Indices ####
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings(), epilog=footer(__version__, tail='singleton-cli.html#_show_indicessnapshots'))
 @click.option('--verbose', help='Show verbose output.', is_flag=True, show_default=True)
 @click.option('--header', help='Print header if --verbose', is_flag=True, show_default=True)
 @click.option('--epoch', help='Print time as epoch if --verbose', is_flag=True, show_default=True)
 @click.option('--ignore_empty_list', is_flag=True, help='Do not raise exception if there are no actionable indices')
 @click.option('--allow_ilm_indices/--no-allow_ilm_indices', help='Allow Curator to operate on Index Lifecycle Management monitored indices.', default=False, show_default=True)
 @click.option('--filter_list', callback=validate_filter_json, default='{"filtertype":"none"}', help='JSON string representing an array of filters.')
 @click.pass_context
@@ -76,15 +79,15 @@
             )
         else:
             click.secho(f'{idx}')
 
 #### Snapshots ####
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings(), epilog=footer(__version__, tail='singleton-cli.html#_show_indicessnapshots'))
 @click.option('--repository', type=str, required=True, help='Snapshot repository name')
 @click.option('--ignore_empty_list', is_flag=True, help='Do not raise exception if there are no actionable snapshots')
 @click.option('--filter_list', callback=validate_filter_json, default='{"filtertype":"none"}', help='JSON string representing an array of filters.')
 @click.pass_context
 def show_snapshots(ctx, repository, ignore_empty_list, filter_list):
     """
     Show Snapshots
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/shrink.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/shrink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Shrink Index Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, json_to_dict, validate_filter_json
+from curator.cli_singletons.utils import json_to_dict, validate_filter_json
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--shrink_node', default='DETERMINISTIC', type=str, help='Named node, or DETERMINISTIC', show_default=True)
 @click.option('--node_filters', help='JSON version of node_filters (see documentation)', callback=json_to_dict)
 @click.option('--number_of_shards', default=1, type=int, help='Shrink to this many shards per index')
 @click.option('--number_of_replicas', default=1, type=int, help='Number of replicas for the target index', show_default=True)
 @click.option('--shrink_prefix', type=str, help='Prefix for the target index name')
 @click.option('--shrink_suffix', default='-shrink', type=str, help='Suffix for the target index name', show_default=True)
 @click.option('--copy_aliases', is_flag=True, help='Copy each source index aliases to target index')
```

### Comparing `elasticsearch_curator-8.0.8/curator/cli_singletons/snapshot.py` & `elasticsearch_curator-8.0.9/curator/cli_singletons/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Snapshot Singleton"""
 import click
+from es_client.helpers.config import context_settings
 from curator.cli_singletons.object_class import CLIAction
-from curator.cli_singletons.utils import get_width, validate_filter_json
+from curator.cli_singletons.utils import validate_filter_json
 
 # pylint: disable=line-too-long
-@click.command(context_settings=get_width())
+@click.command(context_settings=context_settings())
 @click.option('--repository', type=str, required=True, help='Snapshot repository')
 @click.option('--name', type=str, help='Snapshot name', show_default=True, default='curator-%Y%m%d%H%M%S')
 @click.option('--ignore_unavailable', is_flag=True, show_default=True, help='Ignore unavailable shards/indices.')
 @click.option('--include_global_state', is_flag=True, show_default=True, help='Store cluster global state with snapshot.')
 @click.option('--partial', is_flag=True, show_default=True, help='Do not fail if primary shard is unavailable.')
 @click.option('--wait_for_completion/--no-wait_for_completion', default=True, show_default=True, help='Wait for the snapshot to complete')
 @click.option('--wait_interval', default=9, type=int, help='Seconds to wait between completion checks.')
```

### Comparing `elasticsearch_curator-8.0.8/curator/defaults/filter_elements.py` & `elasticsearch_curator-8.0.9/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/defaults/filtertypes.py` & `elasticsearch_curator-8.0.9/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/defaults/option_defaults.py` & `elasticsearch_curator-8.0.9/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/defaults/settings.py` & `elasticsearch_curator-8.0.9/curator/defaults/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 """Utilities/Helpers for defaults and schemas"""
 from os import path
 from six import string_types
 from voluptuous import Any, Boolean, Coerce, Optional
+from curator.exceptions import CuratorException
 
-# Elasticsearch versions supported
-def version_max():
-    """
-    :returns: The maximum Elasticsearch version Curator supports: ``(8, 99, 99)``
-    """
-    return (8, 99, 99)
-def version_min():
-    """
-    :returns: The minimum Elasticsearch version Curator supports: ``(8, 99, 99)``
+CURATOR_DOCS = 'https://www.elastic.co/guide/en/elasticsearch/client/curator'
+CLICK_DRYRUN = {
+    'dry-run': {'help': 'Do not perform any changes.', 'is_flag': True},
+}
+
+# Click specifics
+
+def footer(version, tail='index.html'):
     """
-    return (8, 0, 0)
+    Generate a footer linking to Curator docs based on Curator version
+
+    :param version: The Curator version
+
+    :type version: str
+    
+    :returns: An epilog/footer suitable for Click
+    """
+    if not isinstance(version, str):
+        raise CuratorException('Parameter version is not a string: {type(version)}')
+    majmin = ''
+    try:
+        ver = version.split('.')
+        majmin = f'{ver[0]}.{ver[1]}'
+    except Exception as exc:
+        msg = f'Could not determine Curator version from provided value: {version}'
+        raise CuratorException(msg) from exc
+    return f'Learn more at {CURATOR_DOCS}/{majmin}/{tail}'
 
 # Default Config file location
-def config_file():
+def default_config_file():
     """
     :returns: The default configuration file location:
         ``path.join(path.expanduser('~'), '.curator', 'curator.yml')``
     """
-    return path.join(path.expanduser('~'), '.curator', 'curator.yml')
+    default = path.join(path.expanduser('~'), '.curator', 'curator.yml')
+    if path.isfile(default):
+        return default
 
 # Default filter patterns (regular expressions)
 def regex_map():
     """
     :returns: A dictionary of pattern filter 'kind's with their associated regular expression:
         ``{'timestring': r'^.*{0}.*$', 'regex': r'{0}', 'prefix': r'^{0}.*$', 'suffix': r'^.*{0}$'}``
     """
```

### Comparing `elasticsearch_curator-8.0.8/curator/helpers/date_ops.py` & `elasticsearch_curator-8.0.9/curator/helpers/date_ops.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/helpers/getters.py` & `elasticsearch_curator-8.0.9/curator/helpers/getters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Utility functions that get things"""
-# :pylint disable=
 import logging
 import re
 from elasticsearch8 import exceptions as es8exc
-from es_client.defaults import VERSION_MAX, VERSION_MIN
-from es_client.builder import Builder
-from curator.exceptions import ClientException, CuratorException, FailedExecution, MissingArgument
+from curator.exceptions import CuratorException, FailedExecution, MissingArgument
 
 def byte_size(num, suffix='B'):
     """
     :param num: The number of byte
     :param suffix: An arbitrary suffix, like ``Bytes``
 
     :type num: int
@@ -41,54 +38,14 @@
     """
     actions = []
     for alias in aliases.keys():
         actions.append({'remove': {'index': oldidx, 'alias': alias}})
         actions.append({'add': {'index': newidx, 'alias': alias}})
     return actions
 
-def get_client(
-    configdict=None, configfile=None, autoconnect=False, version_min=VERSION_MIN,
-    version_max=VERSION_MAX):
-    """Get an Elasticsearch Client using :py:class:`es_client.Builder`
-
-    Build a client out of settings from `configfile` or `configdict`
-    If neither `configfile` nor `configdict` is provided, empty defaults will be used.
-    If both are provided, `configdict` will be used, and `configfile` ignored.
-
-    :param configdict: A configuration dictionary
-    :param configfile: A configuration file
-    :param autoconnect: Connect to client automatically
-    :param verion_min: Minimum acceptable version of Elasticsearch (major, minor, patch)
-    :param verion_max: Maximum acceptable version of Elasticsearch (major, minor, patch)
-
-    :type configdict: dict
-    :type configfile: str
-    :type autoconnect: bool
-    :type version_min: tuple
-    :type version_max: tuple
-
-    :returns: A client connection object
-    :rtype: :py:class:`~.elasticsearch.Elasticsearch`
-    """
-    logger = logging.getLogger(__name__)
-    logger.info('Creating client object and testing connection')
-
-    builder = Builder(
-        configdict=configdict, configfile=configfile, autoconnect=autoconnect,
-        version_min=version_min, version_max=version_max
-    )
-
-    try:
-        builder.connect()
-    except Exception as exc:
-        logger.critical('Exception encountered: %s', exc)
-        raise ClientException from exc
-
-    return builder.client
-
 def get_data_tiers(client):
     """
     Get all valid data tiers from the node roles of each node in the cluster by polling each node
 
     :param client: A client connection object
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
```

### Comparing `elasticsearch_curator-8.0.8/curator/helpers/testers.py` & `elasticsearch_curator-8.0.9/curator/helpers/testers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Utility functions that get things"""
 import logging
 from voluptuous import Schema
 from elasticsearch8 import Elasticsearch
 from elasticsearch8.exceptions import NotFoundError
+from es_client.helpers.schemacheck import SchemaCheck
 from es_client.helpers.utils import prune_nones
 from curator.helpers.getters import get_repository, get_write_index
 from curator.exceptions import (
     ConfigurationError, MissingArgument, RepositoryException, SearchableSnapshotException)
 from curator.defaults.settings import index_filtertypes, snapshot_actions, snapshot_filtertypes
-from curator.validators import SchemaCheck, actions, options
+from curator.validators import actions, options
 from curator.validators.filter_functions import validfilters
 from curator.helpers.utils import report_failure
 
 def has_lifecycle_name(idx_settings):
     """
     :param idx_settings: The settings for an index being tested
     :type idx_settings: dict
```

### Comparing `elasticsearch_curator-8.0.8/curator/helpers/utils.py` & `elasticsearch_curator-8.0.9/curator/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/helpers/waiters.py` & `elasticsearch_curator-8.0.9/curator/helpers/waiters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/curator/validators/actions.py` & `elasticsearch_curator-8.0.9/curator/validators/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Validate root ``actions`` and individual ``action`` Schemas"""
 from voluptuous import Any, In, Schema, Optional, Required
 from six import string_types
+from es_client.helpers.schemacheck import SchemaCheck
 from curator.defaults import settings
-from curator.validators import SchemaCheck
 
 def root():
     """
     Return a valid :py:class:`~.voluptuous.schema_builder.Schema` definition which is a dictionary
     with ``actions`` :py:class:`~.voluptuous.schema_builder.Required` to be the root key with
     another dictionary as the value.
     """
```

### Comparing `elasticsearch_curator-8.0.8/curator/validators/filter_functions.py` & `elasticsearch_curator-8.0.9/curator/validators/filter_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions validating the ``filter`` Schema of an ``action``"""
 import logging
 from voluptuous import Any, In, Required, Schema
+from es_client.helpers.schemacheck import SchemaCheck
 from es_client.helpers.utils import prune_nones
 from curator.defaults import settings, filtertypes
 from curator.exceptions import ConfigurationError
-from curator.validators import SchemaCheck
 
 logger = logging.getLogger(__name__)
 
 def filtertype():
     """
     Return a :py:class:`~.voluptuous.schema_builder.Schema` object that uses
     :py:func:`~.curator.defaults.settings.all_filtertypes` to populate acceptable values
```

### Comparing `elasticsearch_curator-8.0.8/curator/validators/options.py` & `elasticsearch_curator-8.0.9/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/LICENSE` & `elasticsearch_curator-8.0.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2011–2023 Elasticsearch <http://elastic.co> and contributors.
+Copyright 2011–2024 Elasticsearch <http://elastic.co> and contributors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `elasticsearch_curator-8.0.8/NOTICE` & `elasticsearch_curator-8.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/README.rst` & `elasticsearch_curator-8.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.8/pyproject.toml` & `elasticsearch_curator-8.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,36 +24,29 @@
 keywords = [
     'elasticsearch',
     'time-series',
     'indexed',
     'index-expiry'
 ]
 dependencies = [
-    "elasticsearch8==8.8.2",
-    "es_client==8.8.2.post1",
-    "ecs-logging==2.0.2",
-    "click==8.1.4",
-    "pyyaml==6.0.1",
-    "voluptuous>=0.13.1",
-    "certifi>=2023.5.7",
-    "six>=1.16.0",
+    "es_client==8.12.3"
 ]
 
 [project.optional-dependencies]
 test = [
     "mock",
     "requests",
     "pytest >=7.2.1",
     "pytest-cov",
 ]
 doc = ["sphinx", "sphinx_rtd_theme"]
 
 [project.scripts]
 curator = "curator.cli:cli"
-curator_cli = "curator.curator_cli:main"
+curator_cli = "curator.singletons:curator_cli"
 es_repo_mgr = "curator.repomgrcli:repo_mgr_cli"
 
 [project.urls]
 "Homepage" = "https://github.com/elastic/curator"
 "Bug Tracker" = "https://github.com/elastic/curator/issues"
 
 [tool.hatch.version]
@@ -89,25 +82,25 @@
     "requests",
     "pytest >=7.2.1",
     "pytest-cov",
 ]
 
 [tool.hatch.envs.test.scripts]
 step0 = "$(docker_test/scripts/destroy.sh 2&>1 /dev/null)"
-step1 = "step0 ; echo 'Starting test environment in Docker...' ; $(AUTO_EXPORT=y docker_test/scripts/create.sh 8.6.1 2&>1 /dev/null)"
+step1 = "step0 ; echo 'Starting test environment in Docker...' ; $(AUTO_EXPORT=y docker_test/scripts/create.sh 8.12.1 2&>1 /dev/null)"
 step2 = "step1 ; source docker_test/curatortestenv; echo 'Running tests:'"
 step3 = "step2 ; pytest ; EXITCODE=$?"
 step4 = "step3 ; echo 'Tests complete! Destroying Docker test environment...' "
 full = "step4 ; $(docker_test/scripts/destroy.sh 2&>1 /dev/null ) ;  exit $EXITCODE"
 run-coverage = "pytest --cov-config=pyproject.toml --cov=curator --cov=tests"
 run = "run-coverage --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.9", "3.10", "3.11"]
-version = ["8.0.5"]
+version = ["8.0.9"]
 
 [tool.pytest.ini_options]
 pythonpath = [".", "curator"]
 minversion = "7.2"
 addopts = "-ra -q"
 testpaths = [
     "tests/unit",
```

### Comparing `elasticsearch_curator-8.0.8/PKG-INFO` & `elasticsearch_curator-8.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-curator
-Version: 8.0.8
+Version: 8.0.9
 Summary: Tending your Elasticsearch indices and snapshots
 Project-URL: Homepage, https://github.com/elastic/curator
 Project-URL: Bug Tracker, https://github.com/elastic/curator/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -15,22 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: certifi>=2023.5.7
-Requires-Dist: click==8.1.4
-Requires-Dist: ecs-logging==2.0.2
-Requires-Dist: elasticsearch8==8.8.2
-Requires-Dist: es-client==8.8.2.post1
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: six>=1.16.0
-Requires-Dist: voluptuous>=0.13.1
+Requires-Dist: es-client==8.12.3
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.2.1; extra == 'test'
```

