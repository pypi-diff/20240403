# Comparing `tmp/django_gem-1.5.1.tar.gz` & `tmp/django_gem-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.5.1.tar", max compression
+gzip compressed data, was "django_gem-1.5.2.tar", max compression
```

## Comparing `django_gem-1.5.1.tar` & `django_gem-1.5.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1067 2024-03-19 11:51:55.036803 django_gem-1.5.1/LICENSE
--rw-r--r--   0        0        0     2786 2024-03-19 11:51:55.040803 django_gem-1.5.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/apps.py
--rw-r--r--   0        0        0      535 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/constants.py
--rw-r--r--   0        0        0       71 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/context/__init__.py
--rw-r--r--   0        0        0      581 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/context/cutting_always_eager.py
--rw-r--r--   0        0        0      393 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/context/override_anvil.py
--rw-r--r--   0        0        0      458 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/context/override_cutting_mode.py
--rw-r--r--   0        0        0      298 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/context/override_gem_setting.py
--rw-r--r--   0        0        0      225 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/core.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      359 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/conditional_transaction.py
--rw-r--r--   0        0        0      537 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0      271 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/exceptions.py
--rw-r--r--   0        0        0     1536 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/entities/__init__.py
--rw-r--r--   0        0        0     1720 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/entities/models.py
--rw-r--r--   0        0        0     1706 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/entities/registry.py
--rw-r--r--   0        0        0      132 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/entities/source.py
--rw-r--r--   0        0        0     1385 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/logger.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/commands/__init__.py
--rw-r--r--   0        0        0      893 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/commands/cutmodel.py
--rw-r--r--   0        0        0      953 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/commands/cutqueryset.py
--rw-r--r--   0        0        0     3758 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/commands/gemmakemigrations.py
--rw-r--r--   0        0        0     2252 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/management/commands/gemmigrate.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/middlewares/__init__.py
--rw-r--r--   0        0        0      491 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/middlewares/gem_context_middleware.py
--rw-r--r--   0        0        0     2622 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/__init__.py
--rw-r--r--   0        0        0     2077 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2843 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1616 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1285 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     2393 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/overrides/save.py
--rw-r--r--   0        0        0      937 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      235 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      286 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      221 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      116 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      353 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      337 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2568 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     6067 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0        0 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/gem_migration/__init__.py
--rw-r--r--   0        0        0     1919 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/gem_migration/collector.py
--rw-r--r--   0        0        0      213 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/gem_migration/constants.py
--rw-r--r--   0        0        0      825 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/gem_migration/loader.py
--rw-r--r--   0        0        0     2698 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/gem_migration/recorder.py
--rw-r--r--   0        0        0     7833 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     6512 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0      940 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1824 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     5582 2024-03-19 11:51:55.040803 django_gem-1.5.1/django_gem/validators.py
--rw-r--r--   0        0        0      812 2024-03-19 11:51:55.044803 django_gem-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     3505 1970-01-01 00:00:00.000000 django_gem-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-03 11:32:19.891284 django_gem-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2786 2024-04-03 11:32:19.891284 django_gem-1.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/apps.py
+-rw-r--r--   0        0        0      535 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/constants.py
+-rw-r--r--   0        0        0       71 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/context/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/context/cutting_always_eager.py
+-rw-r--r--   0        0        0      393 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/context/override_anvil.py
+-rw-r--r--   0        0        0      458 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/context/override_cutting_mode.py
+-rw-r--r--   0        0        0      298 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/context/override_gem_setting.py
+-rw-r--r--   0        0        0      225 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/core.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.891284 django_gem-1.5.2/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      359 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/conditional_transaction.py
+-rw-r--r--   0        0        0      537 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0      271 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/exceptions.py
+-rw-r--r--   0        0        0     1536 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0     1720 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1706 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/entities/registry.py
+-rw-r--r--   0        0        0      132 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/entities/source.py
+-rw-r--r--   0        0        0     1385 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0      893 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0      953 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     3758 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/commands/gemmakemigrations.py
+-rw-r--r--   0        0        0     2252 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/management/commands/gemmigrate.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/middlewares/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/middlewares/gem_context_middleware.py
+-rw-r--r--   0        0        0     2622 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     2077 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2843 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1616 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1285 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     2393 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      937 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      286 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      221 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      353 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      337 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2568 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     6067 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/gem_migration/__init__.py
+-rw-r--r--   0        0        0     1919 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/gem_migration/collector.py
+-rw-r--r--   0        0        0      213 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/gem_migration/constants.py
+-rw-r--r--   0        0        0      825 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/gem_migration/loader.py
+-rw-r--r--   0        0        0     2698 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/gem_migration/recorder.py
+-rw-r--r--   0        0        0     7833 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     6506 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0      940 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1824 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     5582 2024-04-03 11:32:19.895285 django_gem-1.5.2/django_gem/validators.py
+-rw-r--r--   0        0        0      812 2024-04-03 11:32:19.899284 django_gem-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3505 1970-01-01 00:00:00.000000 django_gem-1.5.2/PKG-INFO
```

### Comparing `django_gem-1.5.1/LICENSE` & `django_gem-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/README.md` & `django_gem-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/constants.py` & `django_gem-1.5.2/django_gem/constants.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/context/cutting_always_eager.py` & `django_gem-1.5.2/django_gem/context/cutting_always_eager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/cutters/base.py` & `django_gem-1.5.2/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/decorators/context.py` & `django_gem-1.5.2/django_gem/decorators/context.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/decorators/cutters.py` & `django_gem-1.5.2/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/decorators/models.py` & `django_gem-1.5.2/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/entities/context.py` & `django_gem-1.5.2/django_gem/entities/context.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/entities/models.py` & `django_gem-1.5.2/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/entities/registry.py` & `django_gem-1.5.2/django_gem/entities/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/exceptions.py` & `django_gem-1.5.2/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/management/commands/cutmodel.py` & `django_gem-1.5.2/django_gem/management/commands/cutmodel.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/management/commands/cutqueryset.py` & `django_gem-1.5.2/django_gem/management/commands/cutqueryset.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/management/commands/gemmakemigrations.py` & `django_gem-1.5.2/django_gem/management/commands/gemmakemigrations.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/management/commands/gemmigrate.py` & `django_gem-1.5.2/django_gem/management/commands/gemmigrate.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/migrations/0001_initial.py` & `django_gem-1.5.2/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/models/base.py` & `django_gem-1.5.2/django_gem/models/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/models/gem_log_entry.py` & `django_gem-1.5.2/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.5.2/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/models/mixins.py` & `django_gem-1.5.2/django_gem/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/overrides/delete.py` & `django_gem-1.5.2/django_gem/overrides/delete.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/overrides/m2m_changed.py` & `django_gem-1.5.2/django_gem/overrides/m2m_changed.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/overrides/save.py` & `django_gem-1.5.2/django_gem/overrides/save.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/overrides/utils.py` & `django_gem-1.5.2/django_gem/overrides/utils.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/chest.py` & `django_gem-1.5.2/django_gem/toolkit/chest.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/forge.py` & `django_gem-1.5.2/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/gem_migration/collector.py` & `django_gem-1.5.2/django_gem/toolkit/gem_migration/collector.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/gem_migration/loader.py` & `django_gem-1.5.2/django_gem/toolkit/gem_migration/loader.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/gem_migration/recorder.py` & `django_gem-1.5.2/django_gem/toolkit/gem_migration/recorder.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/registry.py` & `django_gem-1.5.2/django_gem/toolkit/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/saw.py` & `django_gem-1.5.2/django_gem/toolkit/saw.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,11 +153,13 @@
                 natural_key = get_model_natural_key(reverse_cutter_trigger.model)
                 smith.add_item(
                     natural_key=natural_key,
                     object_ids=object_ids,
                     gem_fields=reverse_cutter_trigger.gem_fields,
                 )
                 cut_mapping[natural_key] += 1
-            with transaction.atomic():
-                smith.initiate_cutting(gem_cutting_context.anvil)
+
+        with transaction.atomic():
+            smith.initiate_cutting(gem_cutting_context.anvil)
+
         cut_mapping = dict(cut_mapping)
         return cut_mapping
```

### Comparing `django_gem-1.5.1/django_gem/toolkit/settings.py` & `django_gem-1.5.2/django_gem/toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/toolkit/smith.py` & `django_gem-1.5.2/django_gem/toolkit/smith.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/django_gem/validators.py` & `django_gem-1.5.2/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.5.1/pyproject.toml` & `django_gem-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.5.1"
+version = "1.5.2"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.5.1/PKG-INFO` & `django_gem-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.5.1
+Version: 1.5.2
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

