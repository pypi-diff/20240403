# Comparing `tmp/resilient_sdk-51.0.1.0.695.tar.gz` & `tmp/resilient_sdk-51.0.1.1.824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_sdk-51.0.1.0.695.tar", last modified: Wed Feb 14 14:46:45 2024, max compression
+gzip compressed data, was "resilient_sdk-51.0.1.1.824.tar", last modified: Wed Apr  3 15:17:18 2024, max compression
```

## Comparing `resilient_sdk-51.0.1.0.695.tar` & `resilient_sdk-51.0.1.1.824.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.727633 resilient_sdk-51.0.1.0.695/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12945 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-02-14 14:46:45.727633 resilient_sdk-51.0.1.0.695/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.507633 resilient_sdk-51.0.1.0.695/assets/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/assets/IBM_Security_lockup_pos_RGB.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.507633 resilient_sdk-51.0.1.0.695/resilient_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.507633 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      551 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8255 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36395 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37325 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11406 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38221 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/docgen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.507633 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8309 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/ext/ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7664 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13591 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8693 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47981 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/components/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3131 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/lib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     7935 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.511633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10817 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      962 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5425 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/docgen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/docgen/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16666 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/docgen/templates/README.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/run_init/
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/run_init/app.config.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/run_init/sdk_settings.json.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/.pylintrc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.515633 resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/templates/validate_report.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.519633 resilient_sdk-51.0.1.0.695/resilient_sdk/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9174 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/jinja2_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54989 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_genson_overwrites.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73816 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27552 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86804 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_issue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.507633 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    16016 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-02-14 14:46:45.000000 resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1399 2024-02-14 14:46:45.727633 resilient_sdk-51.0.1.0.695/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.519633 resilient_sdk-51.0.1.0.695/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20369 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3785 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.519633 resilient_sdk-51.0.1.0.695/tests/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/integration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/integration/test_installation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.523633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/.mock_sdk_settings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19566 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_app.log
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export.resz
--rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export_corrupt.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.523633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/customize_old.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.523633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   539206 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    46693 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.523633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.555633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5148 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.555633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.555633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.559633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.559633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.559633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.595633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.599633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.603633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.603633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.503633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.631633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.667633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.671633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.703633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.703633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup_py_lines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_reload_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_xml_test_report.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.715633 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/export.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/orgs.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/session.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_mock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3008 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/shared_mock_data/sdk_mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.715633 resilient_sdk-51.0.1.0.695/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.723633 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.723633 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6929 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/ext/test_ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20811 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34428 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19150 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_docgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1247 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8611 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9712 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23814 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:45.723633 resilient_sdk-51.0.1.0.695/tests/unit/test_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_jinja_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21936 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34738 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47084 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_issue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      994 2024-02-14 14:45:11.000000 resilient_sdk-51.0.1.0.695/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13053 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/assets/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/assets/IBM_Security_lockup_pos_RGB.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      551 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8255 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36395 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37325 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11406 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38221 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/docgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8309 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7664 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13591 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8693 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47981 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      608 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3131 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7935 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10817 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      962 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5425 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16666 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/README.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      146 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/app.config.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/sdk_settings.json.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/.pylintrc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/validate_report.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9174 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/jinja2_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54989 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_genson_overwrites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73816 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27552 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86804 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_issue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16016 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1399 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20369 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3785 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/tests/integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/integration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/integration/test_installation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/.mock_sdk_settings.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19566 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        3 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_app.log
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.resz
+-rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export_corrupt.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize_old.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   539206 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46693 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5148 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.334412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.362412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.398412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.434412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.438412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.438412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.470412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_py_lines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_reload_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_xml_test_report.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/orgs.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/session.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_mock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3008 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/sdk_mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6929 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/test_ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20811 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34428 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19150 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_docgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1247 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8611 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9712 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23814 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/tests/unit/test_util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_jinja_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21936 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      470 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34738 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47084 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_issue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tox.ini
```

### Comparing `resilient_sdk-51.0.1.0.695/CHANGES` & `resilient_sdk-51.0.1.1.824/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2024-04: version 51.0.1.1**
+
+* No major changes. Just bumping build number to coincide with other builds
+
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
 * The ``init`` command now includes an option to create an ``app.config`` file:
 
   .. code-block:: bash
```

### Comparing `resilient_sdk-51.0.1.0.695/PKG-INFO` & `resilient_sdk-51.0.1.1.824/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_sdk
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-51.0.1.0.695/README.md` & `resilient_sdk-51.0.1.1.824/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/assets/IBM_Security_lockup_pos_RGB.png` & `resilient_sdk-51.0.1.1.824/assets/IBM_Security_lockup_pos_RGB.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/LICENSE` & `resilient_sdk-51.0.1.1.824/resilient_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/app.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/__init__.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/base_cmd.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/clone.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/codegen.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/dev.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/docgen.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/ext/ext_package.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/extract.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/list.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/list.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/run_init.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/cmds/validate.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,10 @@
 ARG BASE_IMAGE_TAG=latest
 
 FROM ${BASE_IMAGE_REPO}/ibmresilient/soarapps-base-docker-image:${BASE_IMAGE_TAG}
 
 ARG APPLICATION={{package_name}}
 
 COPY ./dist /tmp/packages
+USER 0
 RUN pip install /tmp/packages/${APPLICATION}-*.tar.gz
+USER 1001
```

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/docgen/templates/README.md.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/icons/app_logo.png` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/ext/icons/company_logo.png` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/run_init/sdk_settings.json.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/sdk_settings.json.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/.pylintrc` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/.pylintrc`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/data/validate/templates/validate_report.md.jinja2` & `resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/validate_report.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/constants.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 LOGGER_NAME = "resilient_sdk_log"
 LOG_DIVIDER = "\n------------------------\n"
 ENV_VAR_DEV = "RES_SDK_DEV"
 ENV_VAR_APP_CONFIG_FILE = "APP_CONFIG_FILE"
 
 # UPDATE BEFORE RELEASING NEW VERSION
-RESILIENT_LIBRARIES_VERSION = "51.0.1.0.0"
-RESILIENT_LIBRARIES_VERSION_DEV = "51.0.1.0.0"
+RESILIENT_LIBRARIES_VERSION = "51.0.1.1.0"
+RESILIENT_LIBRARIES_VERSION_DEV = "51.0.1.1.0"
 
 RESILIENT_VERSION_WITH_PROXY_SUPPORT = (42, 0, 0)
 CURRENT_SOAR_SERVER_VERSION = None
 MIN_SOAR_SERVER_VERSION_PLAYBOOKS = parse_version("44.0")
 # new SOAR versioning schema introduced in v51.0.0.x
 # use "51.0.0" rather than "51.0.0.0" so that sonarqube
 # won't flag as an IP address...
```

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/jinja2_filters.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/package_file_helpers.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/resilient_objects.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_argparse.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_argparse.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_exception.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_genson_overwrites.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_genson_overwrites.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_helpers.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_configs.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_helpers.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk/util/sdk_validate_issue.py` & `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/PKG-INFO` & `resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-sdk
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-51.0.1.0.695/resilient_sdk.egg-info/SOURCES.txt` & `resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/setup.cfg` & `resilient_sdk-51.0.1.1.824/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient >= 51.0.1.0
+	resilient >= 51.0.1.1
 	
 	genson    ~= 1.2
 	
 	packaging ~= 23.2; python_version > "3.6"
 	jinja2    ~= 3.1;  python_version > "3.6"
 	
 	packaging ~= 21.3; python_version == "3.6"
```

### Comparing `resilient_sdk-51.0.1.0.695/tests/conftest.py` & `resilient_sdk-51.0.1.1.824/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/helpers.py` & `resilient_sdk-51.0.1.1.824/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/integration/test_installation.py` & `resilient_sdk-51.0.1.1.824/tests/integration/test_installation.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/.mock_sdk_settings.json` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/.mock_sdk_settings.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/README.md` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_app.log` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_app.log`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export.resz` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.resz`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_export_corrupt.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export_corrupt.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/config.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/customize.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/customize_old.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize_old.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup_callable_data.txt` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_callable_data.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_package_files/setup_py_lines.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_py_lines.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_reload_export.res` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_reload_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/mock_xml_test_report.xml` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_xml_test_report.xml`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/export.JSON` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/orgs.JSON` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/orgs.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_data/session.JSON` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/resilient_api_mock.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_mock.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/shared_mock_data/sdk_mock_paths.py` & `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/sdk_mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_app.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/ext/test_ext_package.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/test_ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_base_cmd.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_clone.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_codegen.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_dev.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_docgen.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_extract.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_list.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_list.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_run_init.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_cmds/test_validate.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_jinja_filters.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_package_file_helpers.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_resilient_objects.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_exception.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_helpers.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_configs.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_helpers.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tests/unit/test_util/test_sdk_validate_issue.py` & `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.0.695/tox.ini` & `resilient_sdk-51.0.1.1.824/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 [testenv:UNIT]
 deps =
     pytest
     pylint
     mock
     requests
-    requests-mock ~= 1.9
+    requests-mock     ~= 1.12; python_version>="3.6"
+    requests-mock      < 1.12; python_version=="2.7"
     pytest-cov
     pathlib ; python_version=="2.7"
 
 setenv =
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
 
 commands =
```

