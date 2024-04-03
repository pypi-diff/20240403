# Comparing `tmp/pycti-6.0.8.tar.gz` & `tmp/pycti-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.0.8.tar", last modified: Sun Mar 24 13:40:27 2024, max compression
+gzip compressed data, was "pycti-6.0.9.tar", last modified: Wed Apr  3 11:21:10 2024, max compression
```

## Comparing `pycti-6.0.8.tar` & `pycti-6.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.936387 pycti-6.0.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-03-24 13:40:15.000000 pycti-6.0.8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-03-24 13:40:27.936387 pycti-6.0.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-03-24 13:40:15.000000 pycti-6.0.8/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.928387 pycti-6.0.8/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4691 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.928387 pycti-6.0.8/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28980 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.928387 pycti-6.0.8/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    55835 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.936387 pycti-6.0.8/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18331 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27005 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17392 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20904 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33037 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48728 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   103971 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    77998 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14610 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.936387 pycti-6.0.8/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7915 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112190 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-03-24 13:40:15.000000 pycti-6.0.8/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-24 13:40:27.936387 pycti-6.0.8/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-03-24 13:40:27.000000 pycti-6.0.8/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-03-24 13:40:27.000000 pycti-6.0.8/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-24 13:40:27.000000 pycti-6.0.8/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-03-24 13:40:27.000000 pycti-6.0.8/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-03-24 13:40:27.000000 pycti-6.0.8/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-03-24 13:40:15.000000 pycti-6.0.8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-03-24 13:40:27.940387 pycti-6.0.8/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-04-03 11:20:58.000000 pycti-6.0.9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-04-03 11:21:10.684364 pycti-6.0.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-04-03 11:20:58.000000 pycti-6.0.9/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.672364 pycti-6.0.9/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4691 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.676365 pycti-6.0.9/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28980 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.676365 pycti-6.0.9/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55835 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18331 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27005 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17392 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20904 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33037 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    48728 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   103971 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    77998 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14610 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7915 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112190 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-03 11:20:58.000000 pycti-6.0.9/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-04-03 11:21:10.688365 pycti-6.0.9/setup.cfg
```

### Comparing `pycti-6.0.8/LICENSE` & `pycti-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/PKG-INFO` & `pycti-6.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.0.8
+Version: 6.0.9
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,20 +31,20 @@
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=69.2.0
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
 Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
 Requires-Dist: black~=24.3.0; extra == "dev"
-Requires-Dist: build~=1.1.1; extra == "dev"
+Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
-Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest_randomly~=3.15.0; extra == "dev"
 Requires-Dist: pytest~=8.1.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
```

### Comparing `pycti-6.0.8/README.md` & `pycti-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/__init__.py` & `pycti-6.0.9/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.0.8"
+__version__ = "6.0.9"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.0.8/pycti/api/opencti_api_client.py` & `pycti-6.0.9/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/api/opencti_api_connector.py` & `pycti-6.0.9/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/api/opencti_api_playbook.py` & `pycti-6.0.9/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/api/opencti_api_work.py` & `pycti-6.0.9/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/connector/opencti_connector.py` & `pycti-6.0.9/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/connector/opencti_connector_helper.py` & `pycti-6.0.9/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/connector/opencti_metric_handler.py` & `pycti-6.0.9/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_attack_pattern.py` & `pycti-6.0.9/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_campaign.py` & `pycti-6.0.9/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_case_incident.py` & `pycti-6.0.9/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_case_rfi.py` & `pycti-6.0.9/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_case_rft.py` & `pycti-6.0.9/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_channel.py` & `pycti-6.0.9/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_course_of_action.py` & `pycti-6.0.9/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_data_component.py` & `pycti-6.0.9/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_data_source.py` & `pycti-6.0.9/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_event.py` & `pycti-6.0.9/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_external_reference.py` & `pycti-6.0.9/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_feedback.py` & `pycti-6.0.9/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_grouping.py` & `pycti-6.0.9/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_identity.py` & `pycti-6.0.9/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_incident.py` & `pycti-6.0.9/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_indicator.py` & `pycti-6.0.9/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_infrastructure.py` & `pycti-6.0.9/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_intrusion_set.py` & `pycti-6.0.9/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.0.9/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_label.py` & `pycti-6.0.9/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_language.py` & `pycti-6.0.9/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_location.py` & `pycti-6.0.9/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_malware.py` & `pycti-6.0.9/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_malware_analysis.py` & `pycti-6.0.9/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_marking_definition.py` & `pycti-6.0.9/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_narrative.py` & `pycti-6.0.9/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_note.py` & `pycti-6.0.9/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_observed_data.py` & `pycti-6.0.9/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_opinion.py` & `pycti-6.0.9/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_report.py` & `pycti-6.0.9/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix.py` & `pycti-6.0.9/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_core_object.py` & `pycti-6.0.9/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.0.9/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.0.9/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.0.9/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.0.9/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.0.9/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.0.9/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_task.py` & `pycti-6.0.9/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_threat_actor.py` & `pycti-6.0.9/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.0.9/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.0.9/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_tool.py` & `pycti-6.0.9/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_vocabulary.py` & `pycti-6.0.9/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/entities/opencti_vulnerability.py` & `pycti-6.0.9/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/constants.py` & `pycti-6.0.9/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/opencti_logger.py` & `pycti-6.0.9/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/opencti_stix2.py` & `pycti-6.0.9/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.0.9/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/opencti_stix2_update.py` & `pycti-6.0.9/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti/utils/opencti_stix2_utils.py` & `pycti-6.0.9/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti.egg-info/PKG-INFO` & `pycti-6.0.9/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.0.8
+Version: 6.0.9
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,20 +31,20 @@
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=69.2.0
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
 Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
 Requires-Dist: black~=24.3.0; extra == "dev"
-Requires-Dist: build~=1.1.1; extra == "dev"
+Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
-Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest_randomly~=3.15.0; extra == "dev"
 Requires-Dist: pytest~=8.1.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
```

### Comparing `pycti-6.0.8/pycti.egg-info/SOURCES.txt` & `pycti-6.0.9/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/pycti.egg-info/requires.txt` & `pycti-6.0.9/pycti.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
 python-magic-bin~=0.4.14
 
 [dev]
 black~=24.3.0
-build~=1.1.1
+build~=1.2.1
 isort~=5.13.0
 types-pytz~=2024.1.0.20240203
-pre-commit~=3.6.0
+pre-commit~=3.7.0
 pytest-cases~=3.8.0
-pytest-cov~=4.1.0
+pytest-cov~=5.0.0
 pytest_randomly~=3.15.0
 pytest~=8.1.1
 types-python-dateutil~=2.9.0
 wheel~=0.43.0
 
 [doc]
 autoapi~=2.0.1
```

### Comparing `pycti-6.0.8/pyproject.toml` & `pycti-6.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.0.8/setup.cfg` & `pycti-6.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -44,20 +44,20 @@
 	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
 	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
 	black~=24.3.0
-	build~=1.1.1
+	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
-	pre-commit~=3.6.0
+	pre-commit~=3.7.0
 	pytest-cases~=3.8.0
-	pytest-cov~=4.1.0
+	pytest-cov~=5.0.0
 	pytest_randomly~=3.15.0
 	pytest~=8.1.1
 	types-python-dateutil~=2.9.0
 	wheel~=0.43.0
 doc = 
 	autoapi~=2.0.1
 	sphinx-autodoc-typehints~=2.0.0
```

