# Comparing `tmp/reptor-0.8.tar.gz` & `tmp/reptor-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reptor-0.8.tar", last modified: Fri Jan 12 07:45:32 2024, max compression
+gzip compressed data, was "reptor-0.9.tar", last modified: Thu Jan 25 18:17:36 2024, max compression
```

## Comparing `reptor-0.8.tar` & `reptor-0.9.tar`

### file list

```diff
@@ -1,235 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-12 07:45:23.000000 reptor-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55897 2024-01-12 07:45:23.000000 reptor-0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-01-12 07:45:32.354552 reptor-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-12 07:45:23.000000 reptor-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-01-12 07:45:23.000000 reptor-0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.326552 reptor-0.8/reptor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-12 07:45:23.000000 reptor-0.8/reptor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.330552 reptor-0.8/reptor/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/APIClient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/NotesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/ProjectDesignsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/ProjectsAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/TemplatesAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.330552 reptor-0.8/reptor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/tests/test_notes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-01-12 07:45:23.000000 reptor-0.8/reptor/api/tests/test_projects_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.330552 reptor-0.8/reptor/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/importers/BaseImporter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/importers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/importers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/importers/tests/test_baseimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/pluginmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/ConfBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/PluginMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/TestCaseToolPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/ToolBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/UploadBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.318552 reptor-0.8/reptor/lib/plugins/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/plugins/tests/data/findings/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/data/findings/idor.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/data/findings/invalid_finding.toml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/data/findings/sql.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.334552 reptor-0.8/reptor/lib/plugins/tests/data/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/data/templates/recommendation.md
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/plugins/tests/test_toolbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-01-12 07:45:23.000000 reptor-0.8/reptor/lib/reptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/Finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/FindingTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/Note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/Project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/ProjectDesign.py
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/Section.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/User.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-12 07:45:23.000000 reptor-0.8/reptor/models/tests/test_note_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/core/Conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Conf/Conf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/core/Conf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Conf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Conf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Conf/tests/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/core/Plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/Plugins/Plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.322552 reptor-0.8/reptor/plugins/importers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/importers/GhostWriter/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/importers/GhostWriter/GhostWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/importers/GhostWriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/importers/GhostWriter/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/importers/GhostWriter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/importers/GhostWriter/tests/test_ghostwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/importers/Importers/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/importers/Importers/Importers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.322552 reptor-0.8/reptor/plugins/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/projects/Project/
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Project/Project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.338552 reptor-0.8/reptor/plugins/projects/Project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Project/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Project/tests/test_integration_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Project/tests/test_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/Template/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Template/Template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/Template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Template/tests/test_integration_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/Translate/
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Translate/Translate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Translate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/Translate/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Translate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Translate/tests/test_integration_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/Translate/tests/test_translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/projectfindings/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/projectfindings/ProjectFindings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/projectfindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/projects/projectfindings/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/projectfindings/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/projects/projectfindings/tests/test_integration_projectfinding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.322552 reptor-0.8/reptor/plugins/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/tools/Nmap/
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/Nmap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/tools/Nmap/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/templates/nmap_table.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/tools/Nmap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/tests/test_integration_nmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Nmap/tests/test_nmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/tools/Sslyze/
--rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/Sslyze.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.342552 reptor-0.8/reptor/plugins/tools/Sslyze/findings/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/findings/weak_tls_setup.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/tools/Sslyze/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/certinfo.md
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_certinfo.md
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_misconfigurations.md
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_protocols.md
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_vulnerabilities.md
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/misconfigurations.md
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/protocols.md
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/summary.md
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/test.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/vulnerabilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/templates/weak_ciphers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/tools/Sslyze/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/tests/test_integration_sslyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    16113 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Sslyze/tests/test_sslyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/tools/Zap/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/Zap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/tools/Zap/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/templates/alert.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/templates/site.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/templates/zap-default.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/tools/Zap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/tests/test_integration_zap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/tools/Zap/tests/test_zap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.322552 reptor-0.8/reptor/plugins/uploads/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.346552 reptor-0.8/reptor/plugins/uploads/File/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/File/File.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/File/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/uploads/File/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/File/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/File/tests/test_integration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/uploads/Finding/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Finding/Finding.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Finding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/uploads/Finding/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Finding/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Finding/tests/test_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Finding/tests/test_integration_finding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/uploads/Note/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Note/Note.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Note/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/uploads/Note/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Note/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/uploads/Note/tests/test_integration_note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.326552 reptor-0.8/reptor/plugins/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/utils/packarchive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/packarchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/packarchive/packarchive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/utils/packarchive/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/packarchive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/packarchive/tests/test_packarchive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/plugins/utils/unpackarchive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/unpackarchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-01-12 07:45:23.000000 reptor-0.8/reptor/plugins/utils/unpackarchive/unpackarchive.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-01-12 07:45:23.000000 reptor-0.8/reptor/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-12 07:45:23.000000 reptor-0.8/reptor/subcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.326552 reptor-0.8/reptor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/templates/Toolbase/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/Toolbase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/templates/Toolbase/findings/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/findings/sample.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/templates/Toolbase/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/templates/default-template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.350552 reptor-0.8/reptor/templates/Toolbase/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-12 07:45:23.000000 reptor-0.8/reptor/templates/Toolbase/tests/test_me.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/reptor/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/reptor/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/data/text.md
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_docparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_finding_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_finding_template_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_project_design_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_project_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_section_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-12 07:45:23.000000 reptor-0.8/reptor/tests/test_user_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-12 07:45:23.000000 reptor-0.8/reptor/title.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/reptor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/django_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/string_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/reptor/utils/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-12 07:45:23.000000 reptor-0.8/reptor/utils/templatetags/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 07:45:32.354552 reptor-0.8/reptor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-12 07:45:32.000000 reptor-0.8/reptor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 07:45:32.354552 reptor-0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.018531 reptor-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-25 18:17:21.000000 reptor-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55897 2024-01-25 18:17:21.000000 reptor-0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-01-25 18:17:36.018531 reptor-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-01-25 18:17:21.000000 reptor-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-01-25 18:17:21.000000 reptor-0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.986531 reptor-0.9/reptor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-25 18:17:21.000000 reptor-0.9/reptor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.986531 reptor-0.9/reptor/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/APIClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/NotesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/ProjectDesignsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/ProjectsAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/TemplatesAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.990531 reptor-0.9/reptor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/tests/test_notes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-01-25 18:17:21.000000 reptor-0.9/reptor/api/tests/test_projects_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.990531 reptor-0.9/reptor/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.990531 reptor-0.9/reptor/lib/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/importers/BaseImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.990531 reptor-0.9/reptor/lib/importers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/importers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/importers/tests/test_baseimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/pluginmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/lib/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/ConfBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/PluginMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/TestCaseToolPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21079 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/ToolBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/UploadBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/lib/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.974531 reptor-0.9/reptor/lib/plugins/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/lib/plugins/tests/data/findings/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/data/findings/idor.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/data/findings/invalid_finding.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/data/findings/sql.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/lib/plugins/tests/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/data/templates/recommendation.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/plugins/tests/test_toolbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-01-25 18:17:21.000000 reptor-0.9/reptor/lib/reptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/Finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/FindingTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/Note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/ProjectDesign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/Section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-25 18:17:21.000000 reptor-0.9/reptor/models/tests/test_note_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/plugins/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.994531 reptor-0.9/reptor/plugins/core/Conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Conf/Conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/core/Conf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Conf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Conf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Conf/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/core/Plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/Plugins/Plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.978531 reptor-0.9/reptor/plugins/importers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/importers/GhostWriter/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/importers/GhostWriter/GhostWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/importers/GhostWriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/importers/GhostWriter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/importers/GhostWriter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/importers/GhostWriter/tests/test_ghostwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/importers/Importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/importers/Importers/Importers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.978531 reptor-0.9/reptor/plugins/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/CreateProject/
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/CreateProject/CreateProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/CreateProject/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/CreateProject/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/CreateProject/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/CreateProject/tests/test_createproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/Project/
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Project/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/Project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Project/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Project/tests/test_integration_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Project/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/Template/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Template/Template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/Template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Template/tests/test_integration_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.998531 reptor-0.9/reptor/plugins/projects/Translate/
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Translate/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Translate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/projects/Translate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Translate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Translate/tests/test_integration_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/Translate/tests/test_translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/projects/projectfindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/projectfindings/ProjectFindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/projectfindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/projects/projectfindings/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/projectfindings/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/projects/projectfindings/tests/test_integration_projectfinding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.978531 reptor-0.9/reptor/plugins/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/tools/Nmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/Nmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/tools/Nmap/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/templates/nmap_table.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/tools/Nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/tests/test_integration_nmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Nmap/tests/test_nmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/tools/Sslyze/
+-rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/Sslyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.002531 reptor-0.9/reptor/plugins/tools/Sslyze/findings/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/findings/weak_tls_setup.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/tools/Sslyze/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/certinfo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_certinfo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_misconfigurations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_protocols.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_vulnerabilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/misconfigurations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/protocols.md
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/summary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/test.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/vulnerabilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/templates/weak_ciphers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/tools/Sslyze/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/tests/test_integration_sslyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16113 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Sslyze/tests/test_sslyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/tools/Zap/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/Zap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/tools/Zap/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/templates/alert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/templates/site.md
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/templates/zap-default.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/tools/Zap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/tests/test_integration_zap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/tools/Zap/tests/test_zap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.982531 reptor-0.9/reptor/plugins/uploads/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/uploads/File/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/File/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/File/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/uploads/File/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/File/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/File/tests/test_integration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.006531 reptor-0.9/reptor/plugins/uploads/Finding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Finding/Finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Finding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/Finding/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Finding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Finding/tests/test_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Finding/tests/test_integration_finding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/Note/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Note/Note.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Note/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/Note/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Note/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/Note/tests/test_integration_note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/PushProject/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/PushProject/PushProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/PushProject/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/PushProject/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/PushProject/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/uploads/PushProject/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/PushProject/tests/data/input.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/uploads/PushProject/tests/test_push_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.982531 reptor-0.9/reptor/plugins/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/utils/packarchive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/packarchive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/utils/packarchive/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.982531 reptor-0.9/reptor/plugins/utils/packarchive/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/utils/packarchive/tests/data/unpacked/
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/tests/data/unpacked/project.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/tests/test_integration_un_pack_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/packarchive/tests/test_packarchive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.010531 reptor-0.9/reptor/plugins/utils/unpackarchive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/unpackarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-01-25 18:17:21.000000 reptor-0.9/reptor/plugins/utils/unpackarchive/unpackarchive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-01-25 18:17:21.000000 reptor-0.9/reptor/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-25 18:17:21.000000 reptor-0.9/reptor/subcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:35.982531 reptor-0.9/reptor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/templates/Toolbase/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/Toolbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/templates/Toolbase/findings/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/findings/sample.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/templates/Toolbase/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/templates/default-template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/templates/Toolbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-25 18:17:21.000000 reptor-0.9/reptor/templates/Toolbase/tests/test_me.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/data/text.md
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_docparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_finding_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_finding_template_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_project_design_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_project_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_section_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-25 18:17:21.000000 reptor-0.9/reptor/tests/test_user_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-25 18:17:21.000000 reptor-0.9/reptor/title.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/django_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/string_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor/utils/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-25 18:17:21.000000 reptor-0.9/reptor/utils/templatetags/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:17:36.014531 reptor-0.9/reptor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-25 18:17:35.000000 reptor-0.9/reptor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 18:17:36.018531 reptor-0.9/setup.cfg
```

### Comparing `reptor-0.8/LICENSE` & `reptor-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reptor-0.8/NOTICE` & `reptor-0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `reptor-0.8/PKG-INFO` & `reptor-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reptor
-Version: 0.8
+Version: 0.9
 Summary: reptor allows you automating pentest reporting with SysReptor.
 Author: Richard Schwabe
 Author-email: Aron Molnar <aron@syslifters.com>
 Maintainer-email: Syslifters <hello@syslifters.com>
 License: Copyright (c) 2023 SysReptor+reptor Developers
         See also the CREDITS.md who contributed to this project.
         
@@ -139,23 +139,25 @@
 subcommands:
   
   Core:
    conf                  Shows config and sets config
    plugins               Allows plugin management & development
   
   Projects & Templates:
+   createproject         Create a new pentest project
    project               Work with projects
    projectfindings       Export your project findings as a summary or checklist
    template              Queries Finding Templates from SysReptor
    translate             Translate Projects to other languages via Deepl
   
   Uploads:
    file                  Uploads a file
    finding               Uploads findings from JSON or TOML
    note                  Uploads and lists notes
+   pushproject           Push data to project from JSON or TOML
   
   Tools:
    nmap                  format nmap output
    sslyze                format sslyze JSON output
    zap                   Parses ZAP reports (JSON, XML)
   
   Importers:
```

### Comparing `reptor-0.8/README.md` & `reptor-0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,23 +80,25 @@
 subcommands:
   
   Core:
    conf                  Shows config and sets config
    plugins               Allows plugin management & development
   
   Projects & Templates:
+   createproject         Create a new pentest project
    project               Work with projects
    projectfindings       Export your project findings as a summary or checklist
    template              Queries Finding Templates from SysReptor
    translate             Translate Projects to other languages via Deepl
   
   Uploads:
    file                  Uploads a file
    finding               Uploads findings from JSON or TOML
    note                  Uploads and lists notes
+   pushproject           Push data to project from JSON or TOML
   
   Tools:
    nmap                  format nmap output
    sslyze                format sslyze JSON output
    zap                   Parses ZAP reports (JSON, XML)
   
   Importers:
```

### Comparing `reptor-0.8/pyproject.toml` & `reptor-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reptor"
-version = "0.8"
+version = "0.9"
 authors = [
   { name="Richard Schwabe" },
   { name="Aron Molnar", email="aron@syslifters.com" }
 ]
 maintainers = [
   {name = 'Syslifters', email = 'hello@syslifters.com'}
 ]
```

### Comparing `reptor-0.8/reptor/api/APIClient.py` & `reptor-0.9/reptor/api/APIClient.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/NotesAPI.py` & `reptor-0.9/reptor/api/NotesAPI.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/ProjectDesignsAPI.py` & `reptor-0.9/reptor/api/ProjectDesignsAPI.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/ProjectsAPI.py` & `reptor-0.9/reptor/api/ProjectsAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typing
 from contextlib import contextmanager
 from functools import cached_property
 from posixpath import join as urljoin
-from typing import Optional
 
 from requests import HTTPError
 
 from reptor.api.APIClient import APIClient
 from reptor.models.Finding import FindingRaw
 from reptor.models.Project import Project, ProjectOverview
+from reptor.models.ProjectDesign import ProjectDesign
 from reptor.models.Section import Section, SectionRaw
 
 
 class ProjectsAPI(APIClient):
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self._init_attrs()
@@ -26,14 +26,27 @@
         self.base_endpoint = f"{server}/api/v1/pentestprojects"
         self.debug(self.base_endpoint)
 
     @property
     def object_endpoint(self) -> str:
         return urljoin(self.base_endpoint, self.project_id)
 
+    def create_project(
+        self,
+        name: str,
+        project_design: str,
+        tags: typing.Optional[typing.List[str]] = None,
+    ) -> Project:
+        data = {
+            "name": name,
+            "project_type": project_design,
+            "tags": tags or list(),
+        }
+        return Project(self.post(self.base_endpoint, json=data).json(), ProjectDesign())
+
     def get_projects(self, readonly: bool = False) -> typing.List[ProjectOverview]:
         """Gets list of projects
 
         Args:
             readonly (bool, optional): Only archived projects. Defaults to False.
 
         Returns:
@@ -44,19 +57,21 @@
             url = f"{url}?readonly=true"
         response = self.get(url)
         return_data = list()
         for item in response.json()["results"]:
             return_data.append(ProjectOverview(item))
         return return_data
 
-    def search(self, search_term: Optional[str] = "") -> typing.List[ProjectOverview]:
+    def search(
+        self, search_term: typing.Optional[str] = ""
+    ) -> typing.List[ProjectOverview]:
         """Searches projects by search term and retrieves all projects that match
 
         Args:
-            search_term (Optional[str], optional): Search Term to look for. Defaults to None.
+            search_term (typing.Optional[str], optional): Search Term to look for. Defaults to None.
 
         Returns:
             typing.List[Project]: List of project overviews (without sections, findings) that match search
         """
 
         response = self.get(f"{self.base_endpoint}?search={search_term}")
```

### Comparing `reptor-0.8/reptor/api/TemplatesAPI.py` & `reptor-0.9/reptor/api/TemplatesAPI.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/enums.py` & `reptor-0.9/reptor/api/enums.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/manager.py` & `reptor-0.9/reptor/api/manager.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/tests/test_notes_api.py` & `reptor-0.9/reptor/api/tests/test_notes_api.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/api/tests/test_projects_api.py` & `reptor-0.9/reptor/api/tests/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/conf.py` & `reptor-0.9/reptor/lib/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,24 +68,28 @@
         if plugin:
             plugin_settings = self._raw_config.get(plugin, {})
             plugin_settings.update({key: value})
             self._raw_config.update({plugin: plugin_settings})
         else:
             self._raw_config.update({key: value})
 
-    def load_config(self):
+    def load_config(self, return_only: bool = False) -> dict:
         """Loads config file from user home directory"""
         if not settings.PERSONAL_SYSREPTOR_HOME.exists():
             # exist_ok=True because logger might be faster, when creating log file and parents=True
             settings.PERSONAL_SYSREPTOR_HOME.mkdir(exist_ok=True)
+        config = dict()
         try:
             with open(settings.PERSONAL_CONFIG_FILE, "r") as f:
-                self._raw_config = yaml.safe_load(f.read())
+                config = yaml.safe_load(f.read())
+                if not return_only:
+                    self._raw_config = config
         except FileNotFoundError:
             self._no_config_file = True
+        return config
 
     def get_config_from_user(self):
         """Asks the user for the individiual settings and offers to
         write them into a config file
         """
         default_server = self._raw_config.get("server")
         self._raw_config["server"] = (
@@ -119,22 +123,24 @@
             store = input(
                 f"Store to config to {settings.PERSONAL_CONFIG_FILE}? [y/n]: "
             )[:1].lower()
         if store == "y":
             self._write_to_file()
         self.instance._raw_config = self._raw_config
 
-    def _write_to_file(self):
+    def _write_to_file(self, config: typing.Optional[dict] = None):
         """Writes config file as yaml file"""
-        if self._raw_config:
+        if not config:
+            config = self._raw_config
+        if config:
             settings.PERSONAL_SYSREPTOR_HOME.mkdir(exist_ok=True)
             with open(settings.PERSONAL_CONFIG_FILE, "w") as f:
                 filtered_config = {
                     k: v
-                    for k, v in self._raw_config.items()
+                    for k, v in config.items()
                     if k not in self._ignored_keys_in_config
                 }
                 yaml.dump(filtered_config, f, encoding="utf-8")
         else:
             raise ValueError("No config is currently set")
 
     def get_server(self) -> str:
```

### Comparing `reptor-0.8/reptor/lib/importers/BaseImporter.py` & `reptor-0.9/reptor/lib/importers/BaseImporter.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/importers/tests/test_baseimporter.py` & `reptor-0.9/reptor/lib/importers/tests/test_baseimporter.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/logger.py` & `reptor-0.9/reptor/lib/logger.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/pluginmanager.py` & `reptor-0.9/reptor/lib/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/plugins/Base.py` & `reptor-0.9/reptor/lib/plugins/Base.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/plugins/PluginMeta.py` & `reptor-0.9/reptor/lib/plugins/PluginMeta.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/plugins/TestCaseToolPlugin.py` & `reptor-0.9/reptor/lib/plugins/TestCaseToolPlugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         except KeyError:
             pass
 
     @classmethod
     def patch_apis(cls):
         cls.reptor._api = APIManager(reptor=cls.reptor)
         cls.reptor._config = Config()
-        # cls.reptor._config.load_config()
         cls.reptor._config._raw_config = {
             "project_id": "db837c68-ff58-4f63-9161-d2310d71999b",
             "server": "https://demo.sysre.pt",
             "token": "sysreptor_ABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890",
         }
         APIClient.get = APIClient.post = APIClient.put = APIClient.patch = Mock(
             side_effect=RuntimeError(
```

### Comparing `reptor-0.8/reptor/lib/plugins/ToolBase.py` & `reptor-0.9/reptor/lib/plugins/ToolBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import tomli
 import xmltodict
 from django.template import Context, Template
 from django.template.loader import render_to_string
 
 import reptor.settings as settings
-from reptor.lib.exceptions import IncompatibleDesignException
 from reptor.models.Finding import Finding
 from reptor.models.Note import NoteTemplate
 from reptor.models.ProjectDesign import ProjectDesign
 
 from .Base import Base
 
 log = logging.getLogger("reptor")
@@ -473,15 +472,15 @@
 
                 try:
                     finding = Finding(
                         finding_dict,
                         project_design=ProjectDesign(),
                         raise_on_unknown_fields=True,
                     )
-                except IncompatibleDesignException:
+                except ValueError:
                     self.log.info(
                         "Finding data not compatible with project design. Fetching project design from project."
                     )
                     project_design = self.reptor.api.project_designs.project_design
                     finding = Finding(
                         finding_dict,
                         project_design,
```

### Comparing `reptor-0.8/reptor/lib/plugins/tests/data/findings/idor.toml` & `reptor-0.9/reptor/lib/plugins/tests/data/findings/idor.toml`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/plugins/tests/test_toolbase.py` & `reptor-0.9/reptor/lib/plugins/tests/test_toolbase.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/lib/reptor.py` & `reptor-0.9/reptor/lib/reptor.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/Base.py` & `reptor-0.9/reptor/models/Base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
 import enum
+import logging
 import typing
 from copy import deepcopy
 from dataclasses import dataclass
 
 
 @dataclass
 class BaseModel:
     """
     Base Model
     """
 
     id: str = ""
     created: datetime.datetime = datetime.datetime.now()
     updated: datetime.datetime = datetime.datetime.now()
+    _log = logging.getLogger("reptor")
 
     def __init__(self, data: typing.Optional[typing.Dict] = None):
         if data:
             self._fill_from_api(data)
 
     def _get_combined_class_type_hints(self) -> dict:
         type_hints = list()
@@ -37,21 +39,20 @@
         """Fills Model from reptor.api return JSON data
 
         Args:
             data (str): API Return Data
         """
         # Import here to prevent circular imports
         from reptor.models.Finding import FindingDataRaw
-        from reptor.models.FindingTemplate import (
-            FindingTemplate,
-            FindingTemplateTranslation,
-        )
+        from reptor.models.FindingTemplate import (FindingTemplate,
+                                                   FindingTemplateTranslation)
         from reptor.models.Note import Note
         from reptor.models.Project import Project
-        from reptor.models.ProjectDesign import ProjectDesign, ProjectDesignField
+        from reptor.models.ProjectDesign import (ProjectDesign,
+                                                 ProjectDesignField)
         from reptor.models.Section import SectionDataRaw
         from reptor.models.User import User
 
         combined_class_type_hints = self._get_combined_class_type_hints()
 
         for attr in combined_class_type_hints.items():
             if attr[0] in data:
```

### Comparing `reptor-0.8/reptor/models/Finding.py` & `reptor-0.9/reptor/models/Finding.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/FindingTemplate.py` & `reptor-0.9/reptor/models/FindingTemplate.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/Note.py` & `reptor-0.9/reptor/models/Note.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/Project.py` & `reptor-0.9/reptor/models/Project.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/ProjectDesign.py` & `reptor-0.9/reptor/models/ProjectDesign.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/Section.py` & `reptor-0.9/reptor/models/Section.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 import typing
 from copy import deepcopy
 from typing import Any
 from uuid import UUID
 
-from reptor.lib.exceptions import IncompatibleDesignException
 from reptor.models.Base import BaseModel, ProjectFieldTypes
 from reptor.models.ProjectDesign import ProjectDesign, ProjectDesignField
 
 
 class SectionDataRaw(BaseModel):
     def _fill_from_api(self, data: typing.Dict):
         """Fills Model from reptor.api return JSON data
@@ -45,14 +44,15 @@
         value: typing.Union[
             str,
             typing.List,
             bool,
             float,
             Any,
         ],
+        raise_on_unknown_fields: bool = True,
     ):
         # Set attributes from ProjectDesignField
         project_design_type_hints = typing.get_type_hints(ProjectDesignField)
         for attr in project_design_type_hints.items():
             self.__setattr__(attr[0], design_field.__getattribute__(attr[0]))
 
         if self.type == ProjectFieldTypes.object.value:
@@ -61,18 +61,19 @@
                 # property is of type ProjectDesignField
                 try:
                     property_value[property.name] = self.__class__(
                         property, value[property.name]
                     )
 
                 except KeyError:
-                    raise KeyError(
-                        f"Object name '{property.name}' not found. Did you mix"
-                        f"mismatched project design with project data?"
-                    )
+                    if raise_on_unknown_fields:
+                        raise KeyError(
+                            f"Object name '{property.name}' not found. Did you use "
+                            f"wrong project design for your data?"
+                        )
             self.value = property_value
         elif self.type == ProjectFieldTypes.list.value:
             self.value = list()
             if not isinstance(value, list):
                 raise ValueError(f"Value of '{self.name}' must be list.")
             for v in value:  # type: ignore
                 self.value.append(self.__class__(self.items, v))  # type: ignore
@@ -214,29 +215,45 @@
 
     def __init__(
         self,
         data_raw: SectionDataRaw,
         design_fields: typing.List[ProjectDesignField],
         raise_on_unknown_fields: bool = False,
     ):
+        error = False
         for design_field in design_fields:
             try:
                 value = data_raw.__getattribute__(design_field.name)
             except AttributeError:
                 continue
-            self.__setattr__(
-                design_field.name,
-                self.field_class(design_field, value),
-            )
+            try:
+                self.__setattr__(
+                    design_field.name,
+                    self.field_class(
+                        design_field,
+                        value,
+                        raise_on_unknown_fields=raise_on_unknown_fields,
+                    ),
+                )
+            except ValueError as e:
+                self._log.error(e)
+                error = True
+            except KeyError:
+                pass
+
         if raise_on_unknown_fields:
             unknown_fields = [f for f in data_raw.__dict__ if not hasattr(self, f)]
             if len(unknown_fields) > 0:
-                raise IncompatibleDesignException(
+                if raise_on_unknown_fields:
+                    error = True
+                self._log.error(
                     f"Incompatible data and designs: Fields in data but not in design: {','.join(unknown_fields)}"
                 )
+        if error:
+            raise ValueError("Invalid data format")
 
     def __iter__(self):
         """Recursive iteration through cls attributes
         returns FindingDataField"""
         for _, finding_field in vars(self).items():
             for nested_field in finding_field:
                 yield nested_field
@@ -269,14 +286,15 @@
         data:
     """
 
     project: str = ""
     project_type: str = ""
     language: str = ""
     lock_info: bool = False
+    fields: typing.List[str] = []
     template: str = ""
     assignee: str = ""
     status: str = "in-progress"
     data: SectionDataRaw
 
     def __init__(self, data, *args, **kwargs):
         if "data" not in data:
@@ -287,17 +305,23 @@
 class Section(SectionRaw):
     data: SectionData
 
     def __init__(
         self,
         raw: typing.Union[SectionRaw, typing.Dict],
         project_design: typing.Optional[ProjectDesign] = None,
+        raise_on_unknown_fields: bool = False,
     ):
         if project_design is None:
             project_design = ProjectDesign()
         if isinstance(raw, dict):
             raw = SectionRaw(raw)
 
         # Set attributes from SectionRaw
         for attr in typing.get_type_hints(SectionRaw).items():
             self.__setattr__(attr[0], raw.__getattribute__(attr[0]))
-        self.data = SectionData(raw.data, project_design.report_fields)
+
+        self.data = SectionData(
+            raw.data,
+            project_design.report_fields,
+            raise_on_unknown_fields=raise_on_unknown_fields,
+        )
```

### Comparing `reptor-0.8/reptor/models/User.py` & `reptor-0.9/reptor/models/User.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/models/tests/test_note_model.py` & `reptor-0.9/reptor/models/tests/test_note_model.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/core/Conf/Conf.py` & `reptor-0.9/reptor/plugins/core/Conf/Conf.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/core/Plugins/Plugins.py` & `reptor-0.9/reptor/plugins/core/Plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/importers/GhostWriter/GhostWriter.py` & `reptor-0.9/reptor/plugins/importers/GhostWriter/GhostWriter.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/importers/GhostWriter/tests/test_ghostwriter.py` & `reptor-0.9/reptor/plugins/importers/GhostWriter/tests/test_ghostwriter.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/importers/Importers/Importers.py` & `reptor-0.9/reptor/plugins/importers/Importers/Importers.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Project/Project.py` & `reptor-0.9/reptor/plugins/projects/Project/Project.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Project/tests/test_integration_project.py` & `reptor-0.9/reptor/plugins/projects/Project/tests/test_integration_project.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Project/tests/test_project.py` & `reptor-0.9/reptor/plugins/projects/Project/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Template/Template.py` & `reptor-0.9/reptor/plugins/projects/Template/Template.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Template/tests/test_integration_template.py` & `reptor-0.9/reptor/plugins/projects/Template/tests/test_integration_template.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Translate/Translate.py` & `reptor-0.9/reptor/plugins/projects/Translate/Translate.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Translate/tests/test_integration_translate.py` & `reptor-0.9/reptor/plugins/projects/Translate/tests/test_integration_translate.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/Translate/tests/test_translate.py` & `reptor-0.9/reptor/plugins/projects/Translate/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/projectfindings/ProjectFindings.py` & `reptor-0.9/reptor/plugins/projects/projectfindings/ProjectFindings.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/projects/projectfindings/tests/test_integration_projectfinding.py` & `reptor-0.9/reptor/plugins/projects/projectfindings/tests/test_integration_projectfinding.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Nmap/Nmap.py` & `reptor-0.9/reptor/plugins/tools/Nmap/Nmap.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Nmap/templates/nmap_table.md` & `reptor-0.9/reptor/plugins/tools/Nmap/templates/nmap_table.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Nmap/tests/test_integration_nmap.py` & `reptor-0.9/reptor/plugins/tools/Nmap/tests/test_integration_nmap.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Nmap/tests/test_nmap.py` & `reptor-0.9/reptor/plugins/tools/Nmap/tests/test_nmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from pathlib import Path
 
 import pytest
 
 from reptor.lib.plugins.TestCaseToolPlugin import TestCaseToolPlugin
-from reptor.models.Note import NoteTemplate
 
 from ..Nmap import Nmap
 
 
 class TestNmap(TestCaseToolPlugin):
     templates_path = os.path.normpath(Path(os.path.dirname(__file__)) / "../templates")
 
@@ -160,15 +159,15 @@
                 "service": "abyss",
                 "version": None,
             },
         ]
         self._load_xml_data("nmap_with_mac.xml")
         self.nmap.parse()
         for entry in entries:
-           assert entry in self.nmap.parsed_input
+            assert entry in self.nmap.parsed_input
 
     def test_xml_parse_single_target(self):
         entries = [
             {
                 "ip": "63.35.51.142",
                 "hostname": "www.syslifters.com",
                 "port": "80",
```

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/Sslyze.py` & `reptor-0.9/reptor/plugins/tools/Sslyze/Sslyze.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/findings/weak_tls_setup.toml` & `reptor-0.9/reptor/plugins/tools/Sslyze/findings/weak_tls_setup.toml`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/certinfo.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/certinfo.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_certinfo.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_certinfo.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_misconfigurations.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_misconfigurations.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_protocols.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_protocols.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/finding_vulnerabilities.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/finding_vulnerabilities.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/misconfigurations.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/misconfigurations.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/protocols.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/protocols.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/test.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/test.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/vulnerabilities.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/vulnerabilities.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/templates/weak_ciphers.md` & `reptor-0.9/reptor/plugins/tools/Sslyze/templates/weak_ciphers.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/tests/test_integration_sslyze.py` & `reptor-0.9/reptor/plugins/tools/Sslyze/tests/test_integration_sslyze.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Sslyze/tests/test_sslyze.py` & `reptor-0.9/reptor/plugins/tools/Sslyze/tests/test_sslyze.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/README.md` & `reptor-0.9/reptor/plugins/tools/Zap/README.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/Zap.py` & `reptor-0.9/reptor/plugins/tools/Zap/Zap.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/models.py` & `reptor-0.9/reptor/plugins/tools/Zap/models.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/templates/alert.md` & `reptor-0.9/reptor/plugins/tools/Zap/templates/alert.md`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/tests/test_integration_zap.py` & `reptor-0.9/reptor/plugins/tools/Zap/tests/test_integration_zap.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/tools/Zap/tests/test_zap.py` & `reptor-0.9/reptor/plugins/tools/Zap/tests/test_zap.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/File/File.py` & `reptor-0.9/reptor/plugins/uploads/File/File.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/File/tests/test_integration_file.py` & `reptor-0.9/reptor/plugins/uploads/File/tests/test_integration_file.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/Finding/Finding.py` & `reptor-0.9/reptor/plugins/uploads/Finding/Finding.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/Finding/tests/test_finding.py` & `reptor-0.9/reptor/plugins/uploads/Finding/tests/test_finding.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/Finding/tests/test_integration_finding.py` & `reptor-0.9/reptor/plugins/uploads/Finding/tests/test_integration_finding.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/Note/Note.py` & `reptor-0.9/reptor/plugins/uploads/Note/Note.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/uploads/Note/tests/test_integration_note.py` & `reptor-0.9/reptor/plugins/uploads/Note/tests/test_integration_note.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/utils/packarchive/packarchive.py` & `reptor-0.9/reptor/plugins/utils/packarchive/packarchive.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             "-o",
             "--output",
             type=argparse.FileType("wb"),
             default="packed_archive.tar.gz",
         )
 
     def run(self):
+        if not self.directories:
+            return
         with tarfile.open(fileobj=self.output, mode="w:gz") as tar:
             for path_dir in self.directories:
                 # Add NOTICE files at top level
                 notice_path = path_dir / "NOTICE"
                 if notice_path.is_file():
                     notice_filename = "NOTICE"
                     if notice_filename in tar.getnames():
```

### Comparing `reptor-0.8/reptor/plugins/utils/packarchive/tests/test_packarchive.py` & `reptor-0.9/reptor/plugins/utils/packarchive/tests/test_packarchive.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/plugins/utils/unpackarchive/unpackarchive.py` & `reptor-0.9/reptor/plugins/utils/unpackarchive/unpackarchive.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import tarfile
 import tempfile
 from pathlib import Path
 from shutil import copytree
 from typing import Any
+from io import FileIO
 
 import tomlkit
 import tomlkit.items
 
 from reptor.lib.plugins.Base import Base
 
 
@@ -53,43 +54,42 @@
         for v in data:
             if v is not None:
                 array.append(to_toml(v))
         return array
     elif isinstance(data, bool):
         return tomlkit.items.Bool(data, trivia=tomlkit.items.Trivia())
     elif isinstance(data, int):
-        return tomlkit.items.Integer(data, trivia=tomlkit.items.Trivia())
+        return tomlkit.items.Integer(data, trivia=tomlkit.items.Trivia(), raw=str(data))
     elif isinstance(data, float):
-        return tomlkit.items.Float(data, trivia=tomlkit.items.Trivia())
+        return tomlkit.items.Float(data, trivia=tomlkit.items.Trivia(), raw=str(data))
     elif isinstance(data, str):
         if "\n" in data:
-            str_encoded = tomlkit.string(data, multiline=True).as_string()
-            str_formatted = "\\\n" + str_encoded[3:-3] + "\\\n"
-
-            return tomlkit.string(
-                str_formatted, literal=True, multiline=True, escape=False
-            )
+            if data[0] != "\n":
+                data = "\n" + data
+            if data[-1] != "\n":
+                data += "\n"
+            return tomlkit.string(data, multiline=True)
         else:
             return tomlkit.string(data)
     # elif data is None:
-    #     # TOML does not support null values
-    #     return None
+    #    # TOML does not support null values
+    #    return None
     else:
         raise Exception(f"Unhandled type: {type(data)}")
 
 
 class UnpackArchive(Base):
     meta = {
         "name": "UnpackArchive",
         "summary": "Unpack .tar.gz exported archives",
     }
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.files: list[Path] = kwargs.get("files", [])
+        self.files: list[FileIO] = kwargs.get("files", [])
         self.output = kwargs.get("output") or "./unpacked_archive"
         self.format = kwargs.get("format") or "toml"
 
     @classmethod
     def add_arguments(cls, parser, plugin_filepath=None):
         super().add_arguments(parser, plugin_filepath)
```

### Comparing `reptor-0.8/reptor/settings.py` & `reptor-0.9/reptor/settings.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/templates/Toolbase/Toolbase.py` & `reptor-0.9/reptor/templates/Toolbase/Toolbase.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/templates/Toolbase/tests/test_me.py` & `reptor-0.9/reptor/templates/Toolbase/tests/test_me.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_docparser.py` & `reptor-0.9/reptor/tests/test_docparser.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_finding_model.py` & `reptor-0.9/reptor/tests/test_finding_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from copy import deepcopy
 
 import pytest
 
-from reptor.lib.exceptions import IncompatibleDesignException
 from reptor.models.Finding import (
     Finding,
     FindingData,
     FindingDataField,
     FindingDataRaw,
     FindingRaw,
 )
@@ -122,17 +121,17 @@
         }
     }
 """
 
     def test_incompatible_finding_without_design(self):
         finding_raw = FindingRaw(json.loads(self.incompatible_finding))
         Finding(finding_raw, ProjectDesign(), raise_on_unknown_fields=False)
-        with pytest.raises(IncompatibleDesignException):
+        with pytest.raises(ValueError):
             Finding(finding_raw, ProjectDesign(), raise_on_unknown_fields=True)
-        with pytest.raises(IncompatibleDesignException):
+        with pytest.raises(ValueError):
             Finding(finding_raw, ProjectDesign(), raise_on_unknown_fields=True)
 
     def test_finding_unwanted_casting(self):
         finding = Finding(
             json.loads(self.finding_with_predefined_fields),
             ProjectDesign(),
             raise_on_unknown_fields=True,
```

### Comparing `reptor-0.8/reptor/tests/test_finding_template_model.py` & `reptor-0.9/reptor/tests/test_finding_template_model.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_project_design_models.py` & `reptor-0.9/reptor/tests/test_project_design_models.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_project_models.py` & `reptor-0.9/reptor/tests/test_project_models.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_section_model.py` & `reptor-0.9/reptor/tests/test_section_model.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/tests/test_user_models.py` & `reptor-0.9/reptor/tests/test_user_models.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/utils/django_tags.py` & `reptor-0.9/reptor/utils/django_tags.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/utils/table.py` & `reptor-0.9/reptor/utils/table.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor/utils/templatetags/md.py` & `reptor-0.9/reptor/utils/templatetags/md.py`

 * *Files identical despite different names*

### Comparing `reptor-0.8/reptor.egg-info/PKG-INFO` & `reptor-0.9/reptor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reptor
-Version: 0.8
+Version: 0.9
 Summary: reptor allows you automating pentest reporting with SysReptor.
 Author: Richard Schwabe
 Author-email: Aron Molnar <aron@syslifters.com>
 Maintainer-email: Syslifters <hello@syslifters.com>
 License: Copyright (c) 2023 SysReptor+reptor Developers
         See also the CREDITS.md who contributed to this project.
         
@@ -139,23 +139,25 @@
 subcommands:
   
   Core:
    conf                  Shows config and sets config
    plugins               Allows plugin management & development
   
   Projects & Templates:
+   createproject         Create a new pentest project
    project               Work with projects
    projectfindings       Export your project findings as a summary or checklist
    template              Queries Finding Templates from SysReptor
    translate             Translate Projects to other languages via Deepl
   
   Uploads:
    file                  Uploads a file
    finding               Uploads findings from JSON or TOML
    note                  Uploads and lists notes
+   pushproject           Push data to project from JSON or TOML
   
   Tools:
    nmap                  format nmap output
    sslyze                format sslyze JSON output
    zap                   Parses ZAP reports (JSON, XML)
   
   Importers:
```

### Comparing `reptor-0.8/reptor.egg-info/SOURCES.txt` & `reptor-0.9/reptor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 reptor/plugins/core/Conf/tests/test_dummy.py
 reptor/plugins/core/Plugins/Plugins.py
 reptor/plugins/importers/GhostWriter/GhostWriter.py
 reptor/plugins/importers/GhostWriter/__init__.py
 reptor/plugins/importers/GhostWriter/tests/__init__.py
 reptor/plugins/importers/GhostWriter/tests/test_ghostwriter.py
 reptor/plugins/importers/Importers/Importers.py
+reptor/plugins/projects/CreateProject/CreateProject.py
+reptor/plugins/projects/CreateProject/__init__.py
+reptor/plugins/projects/CreateProject/tests/__init__.py
+reptor/plugins/projects/CreateProject/tests/test_createproject.py
 reptor/plugins/projects/Project/Project.py
 reptor/plugins/projects/Project/__init__.py
 reptor/plugins/projects/Project/tests/__init__.py
 reptor/plugins/projects/Project/tests/test_integration_project.py
 reptor/plugins/projects/Project/tests/test_project.py
 reptor/plugins/projects/Template/Template.py
 reptor/plugins/projects/Template/__init__.py
@@ -135,18 +139,25 @@
 reptor/plugins/uploads/Finding/tests/__init__.py
 reptor/plugins/uploads/Finding/tests/test_finding.py
 reptor/plugins/uploads/Finding/tests/test_integration_finding.py
 reptor/plugins/uploads/Note/Note.py
 reptor/plugins/uploads/Note/__init__.py
 reptor/plugins/uploads/Note/tests/__init__.py
 reptor/plugins/uploads/Note/tests/test_integration_note.py
+reptor/plugins/uploads/PushProject/PushProject.py
+reptor/plugins/uploads/PushProject/__init__.py
+reptor/plugins/uploads/PushProject/tests/__init__.py
+reptor/plugins/uploads/PushProject/tests/test_push_project.py
+reptor/plugins/uploads/PushProject/tests/data/input.toml
 reptor/plugins/utils/packarchive/__init__.py
 reptor/plugins/utils/packarchive/packarchive.py
 reptor/plugins/utils/packarchive/tests/__init__.py
+reptor/plugins/utils/packarchive/tests/test_integration_un_pack_archive.py
 reptor/plugins/utils/packarchive/tests/test_packarchive.py
+reptor/plugins/utils/packarchive/tests/data/unpacked/project.toml
 reptor/plugins/utils/unpackarchive/__init__.py
 reptor/plugins/utils/unpackarchive/unpackarchive.py
 reptor/templates/Toolbase/README.md
 reptor/templates/Toolbase/Toolbase.py
 reptor/templates/Toolbase/__init__.py
 reptor/templates/Toolbase/findings/sample.toml
 reptor/templates/Toolbase/templates/default-template.md
```

