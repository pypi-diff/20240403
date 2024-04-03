# Comparing `tmp/sagemaker-jupyterlab-extension-0.2.0.tar.gz` & `tmp/sagemaker-jupyterlab-extension-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-jupyterlab-extension-0.2.0.tar", last modified: Tue Dec  5 00:42:02 2023, max compression
+gzip compressed data, was "sagemaker-jupyterlab-extension-0.3.0.tar", last modified: Tue Apr  2 23:22:26 2024, max compression
```

## Comparing `sagemaker-jupyterlab-extension-0.2.0.tar` & `sagemaker-jupyterlab-extension-0.3.0.tar`

### file list

```diff
@@ -1,141 +1,149 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/LICENSE
--rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/THIRD-PARTY-LICENSES
--rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/install.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.030437 sagemaker-jupyterlab-extension-0.2.0/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.034437 sagemaker-jupyterlab-extension-0.2.0/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3926 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.034437 sagemaker-jupyterlab-extension-0.2.0/public_dist/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  2339382 2023-12-05 00:40:19.000000 sagemaker-jupyterlab-extension-0.2.0/public_dist/sagemaker_jupyterlab_extension-0.2.0-py3-none-any.whl
--rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/pyproject.toml
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.038437 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/_version.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/handlers.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.038437 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4068 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.050436 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    25159 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   266480 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   139403 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12090 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2023-12-05 00:41:10.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2023-12-05 00:41:51.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.050436 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/helper.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.050436 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/metric_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2023-12-05 00:42:01.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5442 2023-12-05 00:42:02.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-12-05 00:42:01.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-12-05 00:39:15.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2023-12-05 00:42:01.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2023-12-05 00:42:02.000000 sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2952 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.050436 sagemaker-jupyterlab-extension-0.2.0/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.050436 sagemaker-jupyterlab-extension-0.2.0/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.054436 sagemaker-jupyterlab-extension-0.2.0/src/components/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/GitCloneComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/ResourceUsageComponent.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.054436 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/AutoComplete.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/CheckboxComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/GitCloneComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/InputField.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/ResourceUsageComponent.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.054436 sagemaker-jupyterlab-extension-0.2.0/src/components/common/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/common/AutoComplete.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/common/CheckboxComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/common/InputField.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/common/LinearProgressWithLabel.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.054436 sagemaker-jupyterlab-extension-0.2.0/src/components/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/styles/InputFieldStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/components/styles/autoCompleteStyles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.054436 sagemaker-jupyterlab-extension-0.2.0/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      924 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/errorMessages.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/gitCloneConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3136 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/il18Strings.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      136 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/resourceUsageConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/constants/sessionManagementConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      389 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/GitClonePlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/HideShutDownPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/utils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/ResourceUsagePlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/SessionManagementPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/GitClonePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/plugins/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/service/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/service/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/service/__tests__/index.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/service/__tests__/mock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      433 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/service/constants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/service/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/style/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/style/common.css
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/style/index.css
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/ReactWidgetWrapper.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/__tests__/gitCloneUtils.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/__tests__/sessionManagerUtils.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/gitCloneUtils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      476 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/utils/sessionManagerUtils.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.058436 sagemaker-jupyterlab-extension-0.2.0/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/GitCloneWidget.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/ResourceUsageWidget.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/src/widgets/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/__tests__/GitCloneWidget.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-12-05 00:42:02.062436 sagemaker-jupyterlab-extension-0.2.0/src/widgets/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/styles/gitCloneStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/src/widgets/styles/resourceUsageStyle.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2023-12-05 00:30:22.000000 sagemaker-jupyterlab-extension-0.2.0/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.279719 sagemaker-jupyterlab-extension-0.3.0/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/LICENSE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/THIRD-PARTY-LICENSES
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/install.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.223719 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.231719 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3949 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.231719 sagemaker-jupyterlab-extension-0.3.0/public_dist/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  2341780 2024-04-02 23:20:25.000000 sagemaker-jupyterlab-extension-0.3.0/public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/pyproject.toml
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.235719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/_version.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/handlers.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.235719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4091 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.251719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    28094 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   266482 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   139405 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12105 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2024-04-02 23:21:34.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.251719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/helper.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/metric_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5749 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-02 23:19:17.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-04-02 23:22:26.279719 sagemaker-jupyterlab-extension-0.3.0/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2953 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/components/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/GitCloneComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/ResourceUsageComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      970 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/SpaceMenu.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/AutoComplete.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/CheckboxComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/GitCloneComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/InputField.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/ResourceUsageComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2343 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/SpaceMenu.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/common/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/AutoComplete.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/CheckboxComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/InputField.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/LinearProgressWithLabel.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/InputFieldStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      469 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/SpaceMenuStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/autoCompleteStyles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.263719 sagemaker-jupyterlab-extension-0.3.0/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1201 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/errorMessages.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/gitCloneConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3228 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/il18Strings.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      174 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/resourceUsageConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/sessionManagementConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/spaceMenuConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      425 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.263719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/GitClonePlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/HideShutDownPlugin.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/utils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/ResourceUsagePlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/SessionManagementPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1167 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/SpaceMenuPlugin.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/GitClonePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1365 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SpaceMenuPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      226 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/service/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/index.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/mock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      526 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/constants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/style/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/style/common.css
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/style/index.css
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/ReactWidgetWrapper.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/gitCloneUtils.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/sessionManagerUtils.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/gitCloneUtils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      547 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/sessionManagerUtils.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/GitCloneWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/ResourceUsageWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      809 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/SpaceMenuWidget.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/GitCloneWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/SpaceMenuWidget.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/gitCloneStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/resourceUsageStyle.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/tsconfig.json
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/LICENSE` & `sagemaker-jupyterlab-extension-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/MANIFEST.in` & `sagemaker-jupyterlab-extension-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/PKG-INFO` & `sagemaker-jupyterlab-extension-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.2.0
+Version: 0.3.0
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/README.md` & `sagemaker-jupyterlab-extension-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/THIRD-PARTY-LICENSES` & `sagemaker-jupyterlab-extension-0.3.0/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/package.json` & `sagemaker-jupyterlab-extension-0.3.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9655172413793103%*

 * *Differences: {"'dependencies'": "{'cookie': '0.6.0'}", "'version'": "'0.3.0'"}*

```diff
@@ -20,14 +20,15 @@
         "@lumino/commands": "^2.0.0",
         "@lumino/polling": "^2.1.2",
         "@lumino/signaling": "^2.1.2",
         "@lumino/widgets": "^2.0.0",
         "@mui/icons-material": "5.14",
         "@mui/material": "^5.14.4",
         "@testing-library/react": "^13.0.0",
+        "cookie": "0.6.0",
         "isomorphic-fetch": "^3.0.0",
         "moment": "^2.29.4",
         "p-retry": "^5.1.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "SageMaker JupyterLab workspace primary extension module",
@@ -99,9 +100,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/public_dist/sagemaker_jupyterlab_extension-0.2.0-py3-none-any.whl` & `sagemaker-jupyterlab-extension-0.3.0/public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,78 +1,78 @@
-Zip file size: 2339382 bytes, number of entries: 76
+Zip file size: 2341780 bytes, number of entries: 76
 -rw-r--r--  2.0 unx     1133 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/__init__.py
 -rw-r--r--  2.0 unx      683 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/_version.py
 -rw-r--r--  2.0 unx    11587 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/handlers.py
--rw-r--r--  2.0 unx     4068 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/package.json
+-rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/package.json
 -rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
+-rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
 -rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 -rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 -rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 -rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--  2.0 unx    28094 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
 -rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 -rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 -rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 -rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 -rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 -rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 -rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 -rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--  2.0 unx    25159 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js
 -rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
--rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
--rw-r--r--  2.0 unx   266480 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js
+-rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
 -rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 -rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--  2.0 unx   139403 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
--rw-r--r--  2.0 unx    12090 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js
+-rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
+-rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
 -rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/style.js
 -rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/__init__.py
 -rw-r--r--  2.0 unx      405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/helper.py
 -rw-r--r--  2.0 unx     1647 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_error_util.py
 -rw-r--r--  2.0 unx     5332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 -rw-r--r--  2.0 unx     5041 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_handlers.py
 -rw-r--r--  2.0 unx     7701 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_request_logger.py
 -rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/__init__.py
 -rw-r--r--  2.0 unx      555 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/error_util.py
 -rw-r--r--  2.0 unx     2552 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/git_clone_util.py
 -rw-r--r--  2.0 unx      507 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/metric_util.py
 -rw-r--r--  2.0 unx     7250 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/request_logger.py
--rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/THIRD-PARTY-LICENSES
--rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
--rw-r--r--  2.0 unx     4068 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
--rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
--rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
--rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
--rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
--rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
--rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--  2.0 unx    25159 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/779.3a4f00c583226dabc471.js
--rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
--rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
--rw-r--r--  2.0 unx   266480 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.c3c95a37373ea011ffb4.js
--rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
--rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--  2.0 unx   139403 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
--rw-r--r--  2.0 unx    12090 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.e8f2ffedbb22ee676b66.js
--rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
--rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
--rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.2.0.dist-info/RECORD
-76 files, 11522050 bytes uncompressed, 2318824 bytes compressed:  79.9%
+-rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES
+-rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+-rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+-rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js
+-rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--  2.0 unx    28094 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js
+-rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+-rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+-rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js
+-rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+-rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
+-rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+-rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+-rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD
+76 files, 11528004 bytes uncompressed, 2321222 bytes compressed:  79.9%
```

#### zipnote «TEMP»/diffoscope_ddhmb_fn_/tmpb5467bc8_.zip

```diff
@@ -9,29 +9,32 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/package.json
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
+Filename: sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
+Comment: 
+
 Filename: sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
@@ -51,39 +54,36 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js
-Comment: 
-
 Filename: sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/style.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 Comment: 
@@ -117,113 +117,113 @@
 
 Filename: sagemaker_jupyterlab_extension/utils/metric_util.py
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/utils/request_logger.py
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/THIRD-PARTY-LICENSES
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/779.3a4f00c583226dabc471.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.c3c95a37373ea011ffb4.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.e8f2ffedbb22ee676b66.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.dist-info/LICENSE
+Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.dist-info/METADATA
+Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.dist-info/WHEEL
+Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.dist-info/top_level.txt
+Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.2.0.dist-info/RECORD
+Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### sagemaker_jupyterlab_extension/labextension/package.json

##### Pretty-printed

 * *Similarity: 0.9649616858237547%*

 * *Differences: {"'dependencies'": "{'cookie': '0.6.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.27a0e3dfb32431afe940.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -20,14 +20,15 @@
         "@lumino/commands": "^2.0.0",
         "@lumino/polling": "^2.1.2",
         "@lumino/signaling": "^2.1.2",
         "@lumino/widgets": "^2.0.0",
         "@mui/icons-material": "5.14",
         "@mui/material": "^5.14.4",
         "@testing-library/react": "^13.0.0",
+        "cookie": "0.6.0",
         "isomorphic-fetch": "^3.0.0",
         "moment": "^2.29.4",
         "p-retry": "^5.1.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "SageMaker JupyterLab workspace primary extension module",
@@ -59,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e8f2ffedbb22ee676b66.js",
+            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -104,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

#### sagemaker_jupyterlab_extension/tests/test_request_logger.py

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.2.0"
+    assert data["Context"]["ExtensionVersion"] == "0.3.0"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js` & `sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(8962),
+                f = o(7651),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        8962: (e, t, o) => {
+        7651: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js` & `sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js`

 * *Files 10% similar despite different names*

##### js-beautify {}

```diff
@@ -1,26 +1,27 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
-    [779], {
-        4779: (e, t, n) => {
-            n.r(t), n.d(t, {
-                default: () => Oe
+    [548], {
+        4548: (e, t, a) => {
+            a.r(t), a.d(t, {
+                default: () => Xe
             });
-            var a = n(5409);
+            var n = a(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
-                o = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
-                i = {
+                i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
+                o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
+                r = {
                     shutdown: "filemenu:shutdown"
                 },
-                r = "Sso",
-                l = 3e5,
-                c = 500,
-                d = 100,
-                u = 12e4,
-                p = {
+                l = "Sso",
+                c = 3e5,
+                d = 500,
+                u = 100,
+                p = 12e4,
+                m = {
                     SignInSession: {
                         closeButton: "Close",
                         signInButton: "Sign In",
                         saveButton: "Save",
                         saveAndRenewButton: "Save and renew session",
                         signinDialog: {
                             title: "Please sign in again",
@@ -71,898 +72,1001 @@
                             generalCloneErrorTitle: "Unable to clone repository to project.",
                             generalCloneErrorBody: "Something went wrong when trying to clone the repository to your project. Please try again later. ",
                             failedOptions: "Failed to handle additional options.",
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
+                    },
+                    Space: {
+                        privateSpaceHeader: "Personal Studio",
+                        unknownUser: "Unknown User"
                     }
                 },
                 g = "GitCloneDialogError",
-                m = "ValidRepoPathError",
-                h = {
+                h = "ValidRepoPathError",
+                y = "spaceMenuHeader",
+                v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [a.IMainMenu],
+                    requires: [n.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
-                        e.commands._commands.get(i.shutdown).isVisible = () => !1
+                        e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var y = n(9801),
-                v = n.n(y),
-                b = n(6029),
-                w = n.n(b),
-                E = n(3205),
-                f = n(7308);
-            class x {
+            var w = a(9801),
+                b = a.n(w),
+                E = a(6029),
+                f = a.n(E),
+                x = a(8368),
+                S = a(9510);
+            class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
                 getDismissTime() {
                     return this._dismissTime
                 }
             }
-            const S = () => {
-                    const e = C("authMode");
-                    return e && e[1] && e[1] === r
-                },
-                C = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
-                M = () => {
-                    const e = C("expiryTime"),
-                        t = C("ssoExpiryTimestamp");
-                    return S() && t ? Number(t[1]) : e ? Number(e[1]) : null
-                },
-                R = (e, t) => {
-                    var n, a;
-                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(E.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(E.ConnectionLost)
+            const M = () => {
+                    const e = R("authMode");
+                    return e && e[1] && e[1] === l
                 },
+                R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
-                    const e = C("redirectURL");
+                    const e = R("expiryTime"),
+                        t = R("ssoExpiryTimestamp");
+                    return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
+                },
+                j = (e, t) => {
+                    var a, n;
+                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                },
+                k = () => {
+                    const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
-                j = (e, t) => {
-                    const n = M(),
-                        a = window.open(e, "signin window", "width=800, height=600");
+                D = (e, t) => {
+                    const a = T(),
+                        n = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
-                    const o = window.setInterval((() => {
-                        if (a && a.closed && !s) return void window.clearInterval(o);
-                        const e = M();
-                        if (null !== e && null !== n && (e > n || isNaN(e))) {
-                            window.clearInterval(o), a && a.close(), s = !0;
+                    const i = window.setInterval((() => {
+                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        const e = T();
+                        if (null !== e && null !== a && (e > a || isNaN(e))) {
+                            window.clearInterval(i), n && n.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
-                            f.Dialog.tracker.forEach((e => e.reject()))
+                            S.Dialog.tracker.forEach((e => e.reject()))
                         }
-                    }), d)
+                    }), u)
                 },
-                k = async () => {
+                _ = async () => {
                     const {
                         SignInSession: e
-                    } = p, {
+                    } = m, {
                         signinDialog: t
-                    } = e, n = T(), a = n ? [f.Dialog.okButton({
+                    } = e, a = k(), n = a ? [S.Dialog.okButton({
                         label: e.signInButton
-                    })] : [f.Dialog.cancelButton({
+                    })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = n ? w().createElement("div", {
+                    })], s = a ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
-                    }, t.loggedOutBody) : w().createElement("div", {
+                    }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
-                    }, t.restartSessionBody), o = new f.Dialog({
+                    }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: a,
+                        buttons: n,
                         hasClose: !1
                     });
                     return {
-                        sigInDialogResult: await o.launch(),
-                        confirmDialog: o
+                        sigInDialogResult: await i.launch(),
+                        confirmDialog: i
                     }
                 };
-            var D = n(6797),
-                _ = n(6697),
-                B = n(7527),
-                N = n(125),
-                I = n(1165);
-            const A = (e, t, n, a, s, o, i) => {
-                    const r = M(),
-                        c = i(),
-                        d = c && c + l;
-                    if (null === r) R(e, !1);
+            var N = a(6797),
+                B = a(6697),
+                I = a(1638),
+                z = a(7217),
+                A = a(5326);
+            const U = (e, t, a, n, s, i, o) => {
+                    const r = T(),
+                        l = o(),
+                        d = l && l + c;
+                    if (null === r) j(e, !1);
                     else {
-                        const i = v().unix(r / 1e3).diff(v()()),
+                        const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(S(), r, i) ? (a(), (async (e, t, n) => {
+                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
                             const {
-                                SignInSession: a
-                            } = p, s = T();
-                            f.Dialog.tracker.forEach((e => e.reject())), R(e, !0);
+                                SignInSession: n
+                            } = m, s = k();
+                            S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
-                                sigInDialogResult: o,
-                                confirmDialog: i
-                            } = await k();
-                            if (o && o.button)
-                                if (n(), s) j(T(), t);
-                                else if (o && o.button.label === a.closeButton) {
-                                const e = M(),
+                                sigInDialogResult: i,
+                                confirmDialog: o
+                            } = await _();
+                            if (i && i.button)
+                                if (a(), s) D(k(), t);
+                                else if (i && i.button.label === n.closeButton) {
+                                const e = T(),
                                     t = e && e / 1e3,
-                                    n = t && v().unix(t).diff(v()());
-                                null !== n && n && n > l && (i.dispose(), setTimeout((async () => {
-                                    await k()
-                                }), l))
-                            } else i.dispose(), j(T(), t)
-                        })(e, t, s)) : i <= 9e5 && (void 0 === c || d && u > d) ? (a(), (async (e, t, n, a, s) => {
+                                    a = t && b().unix(t).diff(b()());
+                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    await _()
+                                }), c))
+                            } else o.dispose(), D(k(), t)
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
                             const {
-                                SignInSession: o
-                            } = p, {
-                                renewSessionDialog: i
-                            } = p.SignInSession, {
+                                SignInSession: i
+                            } = m, {
+                                renewSessionDialog: o
+                            } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
-                                } = p, {
+                                } = m, {
                                     renewSessionDialog: t
-                                } = p.SignInSession, n = T(), a = M(), s = a && v().unix(a / 1e3).fromNow(), o = `${t.contDownTimerMessage}${s}.`, i = `${S()?t.soonExpiringSessionBody:o}`, r = t.renewSessionBody, l = S() ? w().createElement(w().Fragment, null, w().createElement("div", {
+                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
-                                }, i, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), w().createElement("div", null, r)) : w().createElement("div", {
+                                }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
-                                }, w().createElement("p", null, i), w().createElement("p", null, t.renewSessionNow)), c = [f.Dialog.okButton({
+                                }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), n && f.Dialog.okButton({
+                                }), a && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
-                                })], d = new f.Dialog({
+                                })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
-                            if (r && r.button.label === i.remindText) {
-                                const e = new x;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
-                            } else r && r.button.label === o.saveAndRenewButton && (l.dispose(), n(), a(), S() || j(T(), t))
-                        })(0, t._sessions, n, s, o), R(e, !1)) : R(e, !1)
+                            if (r && r.button.label === o.remindText) {
+                                const e = new C;
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
+                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const n = e.serviceManager.sessions,
-                            a = () => {
+                        const a = e.serviceManager.sessions,
+                            n = () => {
                                 s.start()
                             },
-                            s = ((e, t, n, a, s, o, i) => new D.Poll({
+                            s = ((e, t, a, n, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => A(e, t, n, a, s, o, i),
+                                factory: async () => U(e, t, a, n, s, i, o),
                                 frequency: {
-                                    interval: c,
+                                    interval: d,
                                     backoff: !0,
-                                    max: u
+                                    max: p
                                 }
-                            }))(e, n, (() => {
-                                const t = new B.TextModelFactory,
-                                    n = new B.DocumentRegistry({
+                            }))(e, a, (() => {
+                                const t = new I.TextModelFactory,
+                                    a = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    a = new N.ServiceManager({}),
-                                    s = new I.DocumentManager({
-                                        registry: n,
-                                        manager: a,
+                                    n = new z.ServiceManager({}),
+                                    s = new A.DocumentManager({
+                                        registry: a,
+                                        manager: n,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
                                             }
                                         }
                                     });
-                                (0, _.each)(e.shell.widgets("main"), (e => {
+                                (0, B.each)(e.shell.widgets("main"), (e => {
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), a, (e => {
+                            }), n, (e => {
                                 t = e
                             }), (() => t));
-                        a()
+                        n()
                     }
                 };
-            var U = n(667);
+            var P = a(4613);
             const G = [200, 201];
-            var P, z = n(7749);
+            var $, O = a(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
-            }(P || (P = {}));
-            const $ = async (e, t) => {
-                const n = N.ServerConnection.makeSettings(),
-                    a = z.URLExt.join(n.baseUrl, e);
+            }($ || ($ = {}));
+            const F = async (e, t) => {
+                const a = z.ServerConnection.makeSettings(),
+                    n = O.URLExt.join(a.baseUrl, e);
                 try {
-                    const e = await N.ServerConnection.makeRequest(a, {
+                    const e = await z.ServerConnection.makeRequest(n, {
                         method: t
-                    }, n);
+                    }, a);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var F = n(5933);
-            const O = "8px",
-                V = "12px",
-                W = F.css`
+            var V = a(5933);
+            const Z = "8px",
+                W = "12px",
+                H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
-                Z = F.css`
+                q = V.css`
   background-color: var(--jp-layout-color2);
   border: solid 1px var(--jp-border-color2);
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   position: fixed;
   bottom: 25px;
 `,
-                q = F.css`
-  margin: 0 ${V} ${O};
+                J = V.css`
+  margin: 0 ${W} ${Z};
 `,
-                J = F.css`
+                Y = V.css`
   font-weight: bold;
-  margin: ${O} 0 0 ${O};
+  margin: ${Z} 0 0 ${Z};
 `,
-                H = (F.css`
-  margin: 0 ${V} 0 ${"16px"};
-`, F.css`
+                Q = (V.css`
+  margin: 0 ${W} 0 ${"16px"};
+`, V.css`
   border-radius: 10px;
   height: 100%;
   width: 30px;
 `),
-                Y = F.css`
+                K = V.css`
   line-height: 24px;
   padding: 0 5px;
 
   &:hover {
     background-color: var(--jp-layout-color2);
   }
 `,
-                Q = (F.css`
+                X = (V.css`
   padding-left: 4px;
-`, F.css`
+`, V.css`
   display: flex;
   justify-content: flex-start;
   align-items: center;
   margin: 6px 12px;
 `),
-                K = F.css`
+                ee = V.css`
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   padding-right: 5px;
 `,
-                X = F.css`
+                te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ee = (F.css`
+                ae = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
-`, F.css`
+`, V.css`
   display: flex;
   align-items: center;
 `);
-            var te = n(8441);
-            const ne = ({
+            var ne = a(8441);
+            const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: n,
-                    label: a,
+                    displayValue: a,
+                    label: n,
                     labelClassName: s,
-                    conatinerClassName: o
-                }) => w().createElement("div", {
+                    conatinerClassName: i
+                }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
-                }, w().createElement("div", {
-                    className: o
-                }, a && w().createElement("span", {
+                }, f().createElement("div", {
+                    className: i
+                }, n && f().createElement("span", {
                     className: s
-                }, a, " ", n, "%"), w().createElement(te.Z, {
+                }, n, " ", a, "%"), f().createElement(ne.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
-                ae = "jlStudio-",
-                se = `${ae}ResourceUsageWidgetContainer`,
-                oe = `${ae}MetricsWidgetContainer`,
-                ie = ({
+                ie = "jlStudio-",
+                oe = `${ie}ResourceUsageWidgetContainer`,
+                re = `${ie}MetricsWidgetContainer`,
+                le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: n
+                    instanceMetricsDisplayValue: a
                 }) => {
-                    const [a, s] = (0, b.useState)(!1), [o, i] = (0, b.useState)(0), [r, l] = (0, b.useState)(0), [c, d] = (0, b.useState)(0), [u, g] = (0, b.useState)(!1), m = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
-                    (0, b.useEffect)((() => {
+                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, o = e.storage.total_space_in_bytes, r = s && o && s / o * 100;
-                            i(n), l(a), d(r)
+                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(a), l(n), d(r)
                         }
-                    }), [t]), (0, b.useEffect)((() => {
+                    }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
-                            } = p.ResourceUsage;
-                            f.Notification.info(e.title), g(!0)
+                            } = m.ResourceUsage;
+                            S.Notification.info(e.title), p(!0)
                         }
                     }), [u, c]);
                     const {
                         instanceMemoryProgressBarTitle: y,
                         instanceMetricsTitle: v,
-                        cpuMetricTitle: E,
-                        memoryMetricTitle: x,
-                        storageMetricTitle: S
-                    } = p.ResourceUsage;
-                    return w().createElement("div", {
+                        cpuMetricTitle: w,
+                        memoryMetricTitle: b,
+                        storageMetricTitle: x
+                    } = m.ResourceUsage;
+                    return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
-                        className: `${se} ${Y}`
-                    }, w().createElement("div", {
-                        className: ee,
+                        className: `${oe} ${K}`
+                    }, f().createElement("div", {
+                        className: ae,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(a),
+                        })(n),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === n ? w().createElement(te.Z, {
+                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
-                        className: X
-                    }) : w().createElement("div", {
-                        className: ee,
+                        className: te
+                    }) : f().createElement("div", {
+                        className: ae,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, w().createElement(te.Z, {
-                        className: X,
+                    }, f().createElement(ne.Z, {
+                        className: te,
                         variant: "determinate",
-                        value: 0 | n
-                    }), n ? Math.round(n) : 0, "%")), a && w().createElement("div", {
-                        className: `${oe} ${Z}`,
+                        value: 0 | a
+                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
-                    }, w().createElement("div", {
-                        className: W
-                    }, w().createElement("div", {
+                    }, f().createElement("div", {
+                        className: H
+                    }, f().createElement("div", {
+                        className: Y
+                    }, v), f().createElement("div", {
                         className: J
-                    }, v), w().createElement("div", {
-                        className: q
-                    }, w().createElement("div", null, w().createElement(ne, {
-                        value: m(o),
-                        displayValue: h(o),
-                        label: E,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                    }, f().createElement("div", null, f().createElement(se, {
+                        value: g(i),
+                        displayValue: h(i),
+                        label: w,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-cpu"
-                    }), w().createElement(ne, {
-                        value: m(r),
+                    }), f().createElement(se, {
+                        value: g(r),
                         displayValue: h(r),
-                        label: x,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: b,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-memory"
-                    }), w().createElement(ne, {
-                        value: m(c),
+                    }), f().createElement(se, {
+                        value: g(c),
                         displayValue: h(c),
-                        label: S,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: x,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-storage"
                     }))))))
                 };
-            class re extends f.ReactWidget {
+            class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
-                        await $("aws/sagemaker/api/instance/metrics", P.GET).then((e => {
+                        await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, n;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, a;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
-                    return w().createElement(ie, {
+                    return f().createElement(le, {
                         onClickHandler: this.clickHandler,
                         instanceMetricsResponse: this._instanceMetricsResponse,
                         instanceMetricsDisplayValue: this._instanceMetricsDisplayValue
                     })
                 }
             }
-            const le = {
+            const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
-                requires: [U.IStatusBar],
+                requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const n = new re;
+                    const a = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: n,
+                        item: a,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ce = n(2419),
-                de = n(2715);
-            const ue = F.css`
+            var ue = a(8031),
+                pe = a(2715);
+            const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
-                pe = ({
+                ge = ({
                     label: e,
                     id: t,
-                    helperText: n,
-                    error: a,
+                    helperText: a,
+                    error: n,
                     handleChange: s,
-                    regEx: o,
-                    ...i
+                    regEx: i,
+                    ...o
                 }) => {
-                    const [r, l] = (0, b.useState)(""), [c, d] = (0, b.useState)(!0);
-                    return w().createElement(de.Z, {
+                    const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
+                    return f().createElement(pe.Z, {
                         variant: "standard",
-                        className: ue,
+                        className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: n,
+                        helperText: a,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
-                            const t = new RegExp(o);
+                            const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
-                        ...i
+                        ...o
                     })
                 },
-                ge = F.css`
+                he = V.css`
   z-index: 2;
 `,
-                me = F.css`
+                ye = V.css`
   width: 460px;
   input {
     width: 460px;
   }
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
-            F.css`
+            V.css`
   margin-bottom: 20px;
 `;
-            var he = n(3776);
-            const ye = (e = !1) => F.css`
+            var ve = a(3776);
+            const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
-                ve = F.css`
+                be = V.css`
   margin-top: 20px;
 `,
-                be = ({
+                Ee = ({
                     options: e,
                     handleChange: t,
-                    label: n,
-                    freeSolo: a
+                    label: a,
+                    freeSolo: n
                 }) => {
-                    const s = (e, n) => {
-                        t(n)
+                    const s = (e, a) => {
+                        t(a)
                     };
-                    return b.createElement("div", {
-                        className: ve
-                    }, b.createElement("label", {
-                        className: ye(!0)
-                    }, n), b.createElement(he.Z, {
+                    return E.createElement("div", {
+                        className: be
+                    }, E.createElement("label", {
+                        className: we(!0)
+                    }, a), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: a,
+                        freeSolo: n,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
-                        renderInput: e => b.createElement(de.Z, {
+                        renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var we = n(2671),
-                Ee = n(847);
-            const fe = ({
+            var fe = a(2671),
+                xe = a(847);
+            const Se = ({
                     label: e,
                     id: t,
-                    handleChange: n,
-                    ...a
+                    handleChange: a,
+                    ...n
                 }) => {
-                    const [s, o] = (0, b.useState)(!0);
-                    return w().createElement(w().Fragment, null, w().createElement(Ee.Z, {
-                        control: w().createElement(we.Z, {
+                    const [s, i] = (0, E.useState)(!0);
+                    return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
+                        control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                o(e.target.checked), n(e.target.checked)
+                                i(e.target.checked), a(e.target.checked)
                             },
                             id: t,
-                            ...a
+                            ...n
                         }),
                         label: e
                     }))
                 },
-                xe = ({
+                Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: n,
-                    setOpenREADME: a
+                    setPath: a,
+                    setOpenREADME: n
                 }) => {
-                    const [s, o] = (0, b.useState)(""), [i, r] = (0, b.useState)(""), [l, c] = (0, b.useState)(!0), [d, u] = (0, b.useState)([]), {
-                        repoTitle: g,
-                        pathTitle: m,
+                    const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
+                        repoTitle: p,
+                        pathTitle: g,
                         openReadMeFilesLabel: h
-                    } = p.GitClone;
-                    return (0, b.useEffect)((() => {
+                    } = m.GitClone;
+                    return (0, E.useEffect)((() => {
                         if (e && e.GitCodeRepositories.length >= 0) {
                             const t = [];
                             e.GitCodeRepositories.length > 0 && e.GitCodeRepositories.forEach((e => t.push({
                                 value: e,
                                 label: e
                             }))), u(t)
                         }
-                    }), [e]), w().createElement("div", {
-                        className: me,
+                    }), [e]), f().createElement("div", {
+                        className: ye,
                         "data-testid": "git-clone-container",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab"
-                    }, w().createElement(be, {
+                    }, f().createElement(Ee, {
                         "data-testid": "autocomplete-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Repo-AutoComplete",
-                        label: g,
+                        label: p,
                         options: d,
-                        value: i,
+                        value: o,
                         handleChange: e => {
                             r(e), t(e)
                         },
                         freeSolo: !0
-                    }), w().createElement(pe, {
+                    }), f().createElement(ge, {
                         "data-testid": "text-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
-                        label: m,
+                        label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            o(e), n(e)
+                            i(e), a(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
-                    }), w().createElement(fe, {
+                    }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), a(e)
+                            c(e), n(e)
                         },
                         checked: l
                     }))
                 };
-            class Se extends f.ReactWidget {
+            class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
                         this.URL = e
                     }, this.setPath = e => {
                         this.path = e
                     }, this.setOpenREADME = e => {
                         this.openREADME = e
                     }, this.getGitRepositories = async () => {
-                        await $("aws/sagemaker/api/git/list-repositories", P.GET).then((e => {
+                        await F("aws/sagemaker/api/git/list-repositories", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this._gitCloneRepositories = e || null, this.update()
                             }))
                         }))
                     }, this.URL = "", this.path = "", this.openREADME = !0, this._gitCloneRepositories = null, this.getGitRepositories()
                 }
                 getValue() {
                     return {
                         URL: this.URL,
                         path: this.path,
                         openREADME: this.openREADME
                     }
                 }
                 render() {
-                    return w().createElement(xe, {
+                    return f().createElement(Ce, {
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Ce = n(9053),
-                Me = n(2190);
+            var Re = a(5962),
+                Te = a(2190);
             const {
-                name: Re,
-                version: Te
-            } = n(4147), je = (e, t, n) => e.child({
-                ExtensionName: Re,
-                ExtensionVersion: Te,
+                name: je,
+                version: ke
+            } = a(4147), De = (e, t, a) => e.child({
+                ExtensionName: je,
+                ExtensionVersion: ke,
                 PluginId: t
-            }, n);
-            var ke;
+            }, a);
+            var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
-            }(ke || (ke = {}));
-            const De = [{
+            }(_e || (_e = {}));
+            const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                _e = async (e, t, n) => {
+                Be = async (e, t, a) => {
                     const {
-                        repoPath: a,
+                        repoPath: n,
                         openREADME: s
-                    } = n;
+                    } = a;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: a
+                            path: n
                         }), !0 === s) try {
-                        await (async (e, t, n) => {
-                            const a = await t.get(e);
-                            if ("directory" === a.type) {
-                                const t = De.find((e => a.content.some((t => t.name === e.name))));
-                                t && await n.execute("docmanager:open", {
-                                    path: z.PathExt.join(e, t.name),
+                        await (async (e, t, a) => {
+                            const n = await t.get(e);
+                            if ("directory" === n.type) {
+                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
+                                t && await a.execute("docmanager:open", {
+                                    path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(a, t, e)
+                        })(n, t, e)
                     } catch (e) {}
-                }, Be = async (e, t) => {
-                    let n;
+                }, Ie = async (e, t) => {
+                    let a;
                     try {
-                        n = await t.get(e)
+                        a = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === n.type
+                    return "directory" === a.type
                 };
-            var Ne = n(1775),
-                Ie = n(248),
-                Ae = n(4337),
-                Le = n(9510);
+            var ze = a(1775),
+                Ae = a(248),
+                Ue = a(4337),
+                Le = a(8625);
             const {
-                dialogTitle: Ue,
+                dialogTitle: Pe,
                 cancelButton: Ge,
-                cloneButton: Pe,
-                errors: ze
-            } = p.GitClone, $e = {
+                cloneButton: $e,
+                errors: Oe
+            } = m.GitClone, Fe = {
                 id: s,
-                requires: [ce.IFileBrowserFactory, ce.IDefaultFileBrowser, Me.IGitExtension, f.IToolbarWidgetRegistry, Ie.ILogger, Ce.ITranslator],
+                requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, n, a, o, i, r) => {
+                activate: async (e, t, a, n, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
-                    } = e, d = c.contents, u = je(i, s), h = (r = r || Ce.nullTranslator).load("sagemaker_studio");
-                    l.addCommand(Ae.TQ.gitClone, {
+                    } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
+                    l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, n, a, s) => {
-                            var o, i;
+                        execute: () => (async (e, t, a, n, s) => {
+                            var i, o;
                             const r = t.model;
                             let l = "";
-                            const c = null === (i = null === (o = null == e ? void 0 : e.tracker) || void 0 === o ? void 0 : o.currentWidget) || void 0 === i ? void 0 : i.model.path;
+                            const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
-                                h = !0,
+                                p = !0,
                                 y = !0;
-                            const v = new f.Dialog({
-                                title: Ue,
-                                body: new Se,
+                            const v = new S.Dialog({
+                                title: Pe,
+                                body: new Me,
                                 focusNodeSelector: "input",
-                                buttons: [f.Dialog.cancelButton({
+                                buttons: [S.Dialog.cancelButton({
                                     label: Ge
-                                }), f.Dialog.okButton({
-                                    label: Pe
+                                }), S.Dialog.okButton({
+                                    label: $e
                                 })],
                                 hasClose: !1
                             });
-                            v.addClass(ge);
+                            v.addClass(he);
                             try {
                                 d = await v.launch()
                             } catch (e) {
                                 return void s.error({
                                     Message: g,
                                     Error: e
                                 })
                             }
                             if (!d.button.accept || !d.value) return;
-                            var b;
+                            var w;
                             if (({
                                     URL: l,
                                     path: u,
-                                    openREADME: h,
+                                    openREADME: p,
                                     findEnvironment: y
-                                } = d.value), "string" == typeof(b = u) && b.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, f.showErrorMessage)(ze.invalidCloneUrlTitle, {
-                                message: ze.invalidCloneUrlBody
+                                } = d.value), "string" == typeof(w = u) && w.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, S.showErrorMessage)(Oe.invalidCloneUrlTitle, {
+                                message: Oe.invalidCloneUrlBody
                             });
-                            const w = (e => {
-                                    const t = z.URLExt.parse(e);
-                                    return z.PathExt.basename(t.pathname, ".git")
+                            const b = (e => {
+                                    const t = O.URLExt.parse(e);
+                                    return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
-                                E = z.PathExt.join(u, w);
-                            let x;
+                                E = O.PathExt.join(u, b);
+                            let f;
                             try {
-                                x = await (async (e, t, n, a) => {
+                                f = await (async (e, t, a, n) => {
                                     const {
                                         errors: s
-                                    } = p.GitClone;
-                                    return await Be(t, e) ? await Be(a, e) ? (await (0, f.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + n
-                                    }), ke.AlreadyCloned) : ke.CanClone : (await (0, f.showErrorMessage)(s.directoryNotExistTitle, {
+                                    } = m.GitClone;
+                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + a
+                                    }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
-                                    }), ke.NotExist)
-                                })(n, u, l, E)
+                                    }), _e.NotExist)
+                                })(a, u, l, E)
                             } catch (e) {
                                 s.error({
-                                    Message: m,
+                                    Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
-                            const S = {
+                            const x = {
                                 repoPath: E,
-                                openREADME: h,
+                                openREADME: p,
                                 findEnvironment: y
                             };
-                            x === ke.CanClone ? (async (e, t, n, a, s, o) => {
+                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
                                 const {
-                                    errors: i
-                                } = p.GitClone, r = await e.execute("terminal:create-new");
+                                    errors: o
+                                } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
-                                s && (l += `cd ${s} && `), l += `git clone ${o} && exit\r`;
+                                s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async a => {
-                                        if ("disconnected" === a.connectionStatus) try {
-                                            await _e(e, t, n)
+                                    }), s.session.connectionStatusChanged.connect((async n => {
+                                        if ("disconnected" === n.connectionStatus) try {
+                                            await Be(e, t, a)
                                         } catch (e) {
-                                            await (0, f.showErrorMessage)(i.failedOptions, i.failedOptionsBody, [f.Dialog.warnButton({
+                                            await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await a.refresh()
+                                    })), await n.refresh()
                                 } catch (e) {
-                                    r.dispose(), await (0, f.showErrorMessage)(i.generalCloneErrorTitle, {
-                                        message: i.generalCloneErrorBody + e
+                                    r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
+                                        message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(a, n, S, r, u, l) : x === ke.AlreadyCloned && _e(a, n, S)
-                        })(t, n, d, l, u),
+                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
+                        })(t, a, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
-                    }), o.addFactory("FileBrowser", "gitClone", (() => f.ReactWidget.create(w().createElement(f.UseSignal, {
-                        signal: a.repositoryChanged,
+                    }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
+                        signal: n.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: a.pathRepository
+                            newValue: n.pathRepository
                         }
-                    }, ((t, n) => w().createElement(f.ToolbarButtonComponent, {
-                        enabled: null === (null == n ? void 0 : n.newValue),
+                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == a ? void 0 : a.newValue),
                         icon: Le.W6,
                         onClick: () => {
-                            e.commands.execute(Ae.TQ.gitClone)
+                            e.commands.execute(Ue.TQ.gitClone)
                         },
-                        tooltip: h.__("Git Clone")
-                    })))))), (0, Ne.ZM)(a, n, e.serviceManager.contents, e.contextMenu, h), u.info({
+                        tooltip: p.__("Git Clone")
+                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
-            }, Fe = e => {
-                var t, n;
-                const a = `${e}.AWSSageMakerUI`;
-                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
-            }, Oe = [h, L, le, $e, {
-                id: o,
-                requires: [Ie.ILogger],
+            }, Ve = e => {
+                var t, a;
+                const n = `${e}.AWSSageMakerUI`;
+                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+            }, Ze = {
+                id: i,
+                requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let a = {};
-                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
+                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let n = {};
+                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: n,
+                                requestStart: a,
                                 responseStart: s,
-                                startTime: o
+                                startTime: i
                             } = e;
-                            n && t && (a = {
-                                ...a,
-                                TimeToFirstByteMS: Math.round(s - o)
+                            a && t && (n = {
+                                ...n,
+                                TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
-                            o = null,
                             i = null,
+                            o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
-                        if (c) s = c.redirectCount, o = c.redirectEnd - c.redirectStart, i = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
+                        if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
-                            s = performance.navigation.redirectCount, o = e.redirectEnd - e.redirectStart, i = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
+                            s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        a = {
-                            ...a,
+                        n = {
+                            ...n,
                             RedirectCount: s,
-                            RedirectTimeMS: o,
-                            TimeToDOMContentLoadedMS: i,
+                            RedirectTimeMS: i,
+                            TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(a), t.started.then((() => {
+                        }, e.info(n), t.started.then((() => {
                             e.info({
-                                TimeToAppStartedMS: Math.round(Fe("timeToAppStarted"))
+                                TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (n = Math.round(Fe("timeToAppRestored"))) > 0 ? n : null;
-                            var n;
+                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
+                            var a;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
-                    })(je(t, o, Ie.logSchemas.performance), e)
+                    })(De(t, i, Ae.logSchemas.performance), e)
+                }
+            };
+            var We = a(87),
+                He = a(8201);
+            const qe = {
+                    SpaceMenuHeader: V.css`
+  margin: -6px 0;
+  padding: 0 var(--jp-size-2);
+  height: 10;
+  border-radius: var(--jp-radius-small);
+  font-size: var(--jp-size-3);
+  display: flex;
+  justify-content: center;
+  align-items: center;
+
+  & > p {
+    display: inline-block;
+    user-select: none;
+    color: var(--jp-color-root-light-800);
+  }
+
+  & > svg {
+    padding: 0 var(--jp-size-2);
+  }
+`
+                },
+                {
+                    privateSpaceHeader: Je,
+                    unknownUser: Ye
+                } = m.Space,
+                Qe = ({
+                    spaceName: e
+                }) => {
+                    const t = !!e,
+                        a = R("studioUserProfileName");
+                    return f().createElement("div", {
+                        className: qe.SpaceMenuHeader,
+                        "data-testid": y
+                    }, t ? f().createElement(We.Z, {
+                        fontSize: "small"
+                    }) : f().createElement(He.Z, {
+                        fontSize: "small"
+                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                };
+            class Ke extends S.ReactWidget {
+                constructor() {
+                    super(), this.getSpaceName = async () => {
+                        await F("aws/sagemaker/api/context", $.GET).then((e => {
+                            e && e.json().then((e => {
+                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                            }))
+                        }))
+                    }, this.spaceName = "", this.getSpaceName()
+                }
+                render() {
+                    return f().createElement(Qe, {
+                        spaceName: this.spaceName
+                    })
+                }
+            }
+            const Xe = [v, L, de, Fe, Ze, {
+                id: o,
+                requires: [Ae.ILogger],
+                autoStart: !0,
+                activate: async (e, t) => {
+                    const a = new Ke;
+                    a.id = S.DOMUtils.createDomID();
+                    const n = De(t, o);
+                    e.shell.add(a, "top", {
+                        rank: 1e3
+                    }), window && window.panorama && window.panorama("trackCustomEvent", {
+                        eventType: "render",
+                        eventDetail: "Space-Plugin",
+                        eventContext: "JupyterLab",
+                        timestamp: Date.now()
+                    }), n.info({
+                        Message: "Successfully loaded Space plugin"
+                    })
                 }
             }]
         },
+        8201: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
+                }), "AccountCircle");
+            t.Z = o
+        },
+        87: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
+                }), "Language");
+            t.Z = o
+        },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.2.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js` & `sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(8962),
+                Ds = o(7651),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js` & `sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -14,35 +14,35 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(7308),
-                s = i(7807),
-                r = i(7749),
-                o = i(4085),
+            var n = i(9510),
+                s = i(3471),
+                r = i(6311),
+                o = i(3452),
                 a = i(6697),
                 l = i(7930),
-                c = i(8778),
+                c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
                     super(...e), this.name = "CancelledError"
                 }
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(9510),
+                v = i(8625),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1757,15 +1757,15 @@
                     width: "100%"
                 }),
                 m = (0, s.oB)({
                     display: "flex",
                     marginLeft: "auto",
                     overflow: "hidden"
                 });
-            var _, y = i(2688),
+            var _, y = i(4387),
                 v = i(7320);
             class b extends n.PureComponent {
                 constructor() {
                     super(...arguments), this._onDoubleClick = e => {
                         e.stopPropagation()
                     }
                 }
@@ -1854,16 +1854,16 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(7308),
-                s = i(8778),
+            var n = i(9510),
+                s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
             const h = a.clearTimeout,
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(9510),
+            var v = i(8625),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(4085),
+                C = i(3452),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,17 +2703,17 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(4085),
+            var n = i(3452),
                 s = i(6029),
-                r = i(2688),
+                r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
                     l = (null === (t = e.filetype) || void 0 === t ? void 0 : t.icon) || n.fileIcon;
                 return s.createElement(s.Fragment, null, s.createElement(l.react, {
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(7308),
+            var n = i(9510),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,19 +3180,19 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(7807),
-                s = i(7454),
-                r = i(9053),
+            var n = i(3471),
+                s = i(7777),
+                r = i(5962),
                 o = i(7930),
-                a = i(8778),
+                a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
                 editorFactory: e,
                 languageRegistry: t,
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(7749),
-                s = i(125),
+            var n = i(6311),
+                s = i(7217),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(7749),
-                r = i(7527),
+            var n, s = i(6311),
+                r = i(1638),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4499,15 +4499,15 @@
                         },
                         t = `&:hover .${r}`;
                     return e.$nest[t] = {
                         display: "block"
                     }, e
                 })()
         },
-        2688: (e, t, i) => {
+        4387: (e, t, i) => {
             "use strict";
             i.d(t, {
                 cf: () => s,
                 gW: () => o,
                 ge: () => r
             });
             var n = i(9946);
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        9510: (e, t, i) => {
+        8625: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(4085);
+            var n = i(3452);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(125);
+            var n = i(7217);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(7749),
+            var n = i(6311),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(9053),
-                o = i(8778),
+                r = i(5962),
+                o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(7807),
-                f = i(7454);
+                u = i(3471),
+                f = i(7777);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js` & `sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,36 +1,36 @@
-/*! For license information please see 891.ada29ec8d5578292aa74.js.LICENSE.txt */
+/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(3205),
-                r = s(7308),
-                a = s(7807),
-                o = s(1165),
-                n = s(2419),
-                l = s(5409),
-                d = s(9499),
-                c = s(8190),
-                h = s(667),
-                p = s(9053),
+            var i = s(8368),
+                r = s(9510),
+                a = s(3471),
+                o = s(5326),
+                n = s(8031),
+                l = s(9557),
+                d = s(8048),
+                c = s(4008),
+                h = s(4613),
+                p = s(5962),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(9510),
+                f = s(8625),
                 _ = s(4337),
-                b = s(8778);
+                b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
                 }
                 getValue() {
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(7932),
+                it = s(6963),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(5390);
+            var _t = s(1778);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(7749),
-                us = s(125);
+                ms = s(6311),
+                us = s(7217);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(4085),
+            var Ss = s(3452),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7454),
+            var Rr = s(7777),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js` & `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js`

 * *Files 8% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, d, u, f, c, s, p, m, b, h, v, g, y, j, w, P, k = {
-            9110: (e, r, t) => {
+    var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
+            1514: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -48,61 +48,61 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.2.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(445), S.e(779)]).then((() => () => S(4779))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(445), S.e(875)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -234,98 +234,98 @@
                 } else {
                     if (i <= a || f < c != n) return !1;
                     d = !1
                 } else "s" != c && "n" != c && (d = !1, i--)
             }
         }
         var s = [],
-            p = s.pop.bind(s);
+            b = s.pop.bind(s);
         for (l = 1; l < e.length; l++) {
-            var m = e[l];
-            s.push(1 == m ? p() | p() : 2 == m ? p() & p() : m ? o(m, r) : !p())
+            var p = e[l];
+            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
         }
-        return !!p()
+        return !!b()
     }, l = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = d(e, t);
-        return o(a, n) || p(u(e, t, n, a)), b(e[t][n])
+        return o(a, n) || b(u(e, t, n, a)), m(e[t][n])
     }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, p = e => {
+    }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, m = (e, r, t, a) => {
-        p(s(e, r, t, a))
-    }, b = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
+    }, p = (e, r, t, a) => {
+        b(s(e, r, t, a))
+    }, m = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => (l(e, t), b(c(r, t, a) || m(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
+    })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
-        return o ? b(o) : n()
+        return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
-        125: () => g("default", "@jupyterlab/services", [1, 7, 0, 9]),
-        667: () => g("default", "@jupyterlab/statusbar", [1, 4, 0, 9]),
-        1165: () => g("default", "@jupyterlab/docmanager", [1, 4, 0, 9]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        2419: () => g("default", "@jupyterlab/filebrowser", [1, 4, 0, 9]),
-        3205: () => g("default", "@jupyterlab/application", [1, 4, 0, 9]),
-        4085: () => g("default", "@jupyterlab/ui-components", [1, 4, 0, 9]),
+        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
+        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
+        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5409: () => g("default", "@jupyterlab/mainmenu", [1, 4, 0, 9]),
+        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
+        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
+        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        7308: () => g("default", "@jupyterlab/apputils", [1, 4, 1, 9]),
-        7454: () => g("default", "@jupyterlab/codemirror", [1, 4, 0, 9]),
-        7527: () => v("default", "@jupyterlab/docregistry", [1, 4, 0, 9]),
-        7749: () => g("default", "@jupyterlab/coreutils", [1, 6, 0, 9]),
-        7807: () => g("default", "@jupyterlab/codeeditor", [1, 4, 0, 9]),
+        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
+        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
+        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        7932: () => v("default", "@jupyterlab/nbformat", [1, 4, 0, 9]),
+        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8778: () => g("default", "@lumino/widgets", [1, 2, 0, 1]),
-        9053: () => g("default", "@jupyterlab/translation", [1, 4, 0, 9]),
+        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
+        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(875)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
+        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
+        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
-        5390: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 9]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8190: () => g("default", "@jupyterlab/settingregistry", [1, 4, 0, 9]),
-        9499: () => g("default", "@jupyterlab/rendermime", [1, 4, 0, 9]),
+        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
-        445: [125, 667, 1165, 1373, 2419, 3205, 4085, 4901, 5409, 6211, 6697, 6797, 7308, 7454, 7527, 7749, 7807, 7930, 7932, 8093, 8204, 8778, 9053],
+        548: [248, 2190, 5933, 9801],
+        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
-        779: [248, 2190, 5933, 9801],
         798: [851, 7138],
         800: [8800],
-        875: [5359, 5390, 5633, 7350, 7489, 7858, 8190, 9499]
+        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|445|704|798|800|875)$/.test(r)) e[r] = 0;
+                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(9110);
+    var E = S(1514);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/THIRD-PARTY-LICENSES` & `sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json`

 * *Files 2% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.9649616858237547%*

 * *Differences: {"'dependencies'": "{'cookie': '0.6.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.27a0e3dfb32431afe940.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -20,14 +20,15 @@
         "@lumino/commands": "^2.0.0",
         "@lumino/polling": "^2.1.2",
         "@lumino/signaling": "^2.1.2",
         "@lumino/widgets": "^2.0.0",
         "@mui/icons-material": "5.14",
         "@mui/material": "^5.14.4",
         "@testing-library/react": "^13.0.0",
+        "cookie": "0.6.0",
         "isomorphic-fetch": "^3.0.0",
         "moment": "^2.29.4",
         "p-retry": "^5.1.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "SageMaker JupyterLab workspace primary extension module",
@@ -59,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e8f2ffedbb22ee676b66.js",
+            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -104,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(8962),
+                f = o(7651),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        8962: (e, t, o) => {
+        7651: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/779.3a4f00c583226dabc471.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js`

 * *Files 10% similar despite different names*

##### js-beautify {}

```diff
@@ -1,26 +1,27 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
-    [779], {
-        4779: (e, t, n) => {
-            n.r(t), n.d(t, {
-                default: () => Oe
+    [548], {
+        4548: (e, t, a) => {
+            a.r(t), a.d(t, {
+                default: () => Xe
             });
-            var a = n(5409);
+            var n = a(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
-                o = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
-                i = {
+                i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
+                o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
+                r = {
                     shutdown: "filemenu:shutdown"
                 },
-                r = "Sso",
-                l = 3e5,
-                c = 500,
-                d = 100,
-                u = 12e4,
-                p = {
+                l = "Sso",
+                c = 3e5,
+                d = 500,
+                u = 100,
+                p = 12e4,
+                m = {
                     SignInSession: {
                         closeButton: "Close",
                         signInButton: "Sign In",
                         saveButton: "Save",
                         saveAndRenewButton: "Save and renew session",
                         signinDialog: {
                             title: "Please sign in again",
@@ -71,898 +72,1001 @@
                             generalCloneErrorTitle: "Unable to clone repository to project.",
                             generalCloneErrorBody: "Something went wrong when trying to clone the repository to your project. Please try again later. ",
                             failedOptions: "Failed to handle additional options.",
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
+                    },
+                    Space: {
+                        privateSpaceHeader: "Personal Studio",
+                        unknownUser: "Unknown User"
                     }
                 },
                 g = "GitCloneDialogError",
-                m = "ValidRepoPathError",
-                h = {
+                h = "ValidRepoPathError",
+                y = "spaceMenuHeader",
+                v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [a.IMainMenu],
+                    requires: [n.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
-                        e.commands._commands.get(i.shutdown).isVisible = () => !1
+                        e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var y = n(9801),
-                v = n.n(y),
-                b = n(6029),
-                w = n.n(b),
-                E = n(3205),
-                f = n(7308);
-            class x {
+            var w = a(9801),
+                b = a.n(w),
+                E = a(6029),
+                f = a.n(E),
+                x = a(8368),
+                S = a(9510);
+            class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
                 getDismissTime() {
                     return this._dismissTime
                 }
             }
-            const S = () => {
-                    const e = C("authMode");
-                    return e && e[1] && e[1] === r
-                },
-                C = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
-                M = () => {
-                    const e = C("expiryTime"),
-                        t = C("ssoExpiryTimestamp");
-                    return S() && t ? Number(t[1]) : e ? Number(e[1]) : null
-                },
-                R = (e, t) => {
-                    var n, a;
-                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(E.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(E.ConnectionLost)
+            const M = () => {
+                    const e = R("authMode");
+                    return e && e[1] && e[1] === l
                 },
+                R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
-                    const e = C("redirectURL");
+                    const e = R("expiryTime"),
+                        t = R("ssoExpiryTimestamp");
+                    return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
+                },
+                j = (e, t) => {
+                    var a, n;
+                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                },
+                k = () => {
+                    const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
-                j = (e, t) => {
-                    const n = M(),
-                        a = window.open(e, "signin window", "width=800, height=600");
+                D = (e, t) => {
+                    const a = T(),
+                        n = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
-                    const o = window.setInterval((() => {
-                        if (a && a.closed && !s) return void window.clearInterval(o);
-                        const e = M();
-                        if (null !== e && null !== n && (e > n || isNaN(e))) {
-                            window.clearInterval(o), a && a.close(), s = !0;
+                    const i = window.setInterval((() => {
+                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        const e = T();
+                        if (null !== e && null !== a && (e > a || isNaN(e))) {
+                            window.clearInterval(i), n && n.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
-                            f.Dialog.tracker.forEach((e => e.reject()))
+                            S.Dialog.tracker.forEach((e => e.reject()))
                         }
-                    }), d)
+                    }), u)
                 },
-                k = async () => {
+                _ = async () => {
                     const {
                         SignInSession: e
-                    } = p, {
+                    } = m, {
                         signinDialog: t
-                    } = e, n = T(), a = n ? [f.Dialog.okButton({
+                    } = e, a = k(), n = a ? [S.Dialog.okButton({
                         label: e.signInButton
-                    })] : [f.Dialog.cancelButton({
+                    })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = n ? w().createElement("div", {
+                    })], s = a ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
-                    }, t.loggedOutBody) : w().createElement("div", {
+                    }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
-                    }, t.restartSessionBody), o = new f.Dialog({
+                    }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: a,
+                        buttons: n,
                         hasClose: !1
                     });
                     return {
-                        sigInDialogResult: await o.launch(),
-                        confirmDialog: o
+                        sigInDialogResult: await i.launch(),
+                        confirmDialog: i
                     }
                 };
-            var D = n(6797),
-                _ = n(6697),
-                B = n(7527),
-                N = n(125),
-                I = n(1165);
-            const A = (e, t, n, a, s, o, i) => {
-                    const r = M(),
-                        c = i(),
-                        d = c && c + l;
-                    if (null === r) R(e, !1);
+            var N = a(6797),
+                B = a(6697),
+                I = a(1638),
+                z = a(7217),
+                A = a(5326);
+            const U = (e, t, a, n, s, i, o) => {
+                    const r = T(),
+                        l = o(),
+                        d = l && l + c;
+                    if (null === r) j(e, !1);
                     else {
-                        const i = v().unix(r / 1e3).diff(v()()),
+                        const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(S(), r, i) ? (a(), (async (e, t, n) => {
+                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
                             const {
-                                SignInSession: a
-                            } = p, s = T();
-                            f.Dialog.tracker.forEach((e => e.reject())), R(e, !0);
+                                SignInSession: n
+                            } = m, s = k();
+                            S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
-                                sigInDialogResult: o,
-                                confirmDialog: i
-                            } = await k();
-                            if (o && o.button)
-                                if (n(), s) j(T(), t);
-                                else if (o && o.button.label === a.closeButton) {
-                                const e = M(),
+                                sigInDialogResult: i,
+                                confirmDialog: o
+                            } = await _();
+                            if (i && i.button)
+                                if (a(), s) D(k(), t);
+                                else if (i && i.button.label === n.closeButton) {
+                                const e = T(),
                                     t = e && e / 1e3,
-                                    n = t && v().unix(t).diff(v()());
-                                null !== n && n && n > l && (i.dispose(), setTimeout((async () => {
-                                    await k()
-                                }), l))
-                            } else i.dispose(), j(T(), t)
-                        })(e, t, s)) : i <= 9e5 && (void 0 === c || d && u > d) ? (a(), (async (e, t, n, a, s) => {
+                                    a = t && b().unix(t).diff(b()());
+                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    await _()
+                                }), c))
+                            } else o.dispose(), D(k(), t)
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
                             const {
-                                SignInSession: o
-                            } = p, {
-                                renewSessionDialog: i
-                            } = p.SignInSession, {
+                                SignInSession: i
+                            } = m, {
+                                renewSessionDialog: o
+                            } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
-                                } = p, {
+                                } = m, {
                                     renewSessionDialog: t
-                                } = p.SignInSession, n = T(), a = M(), s = a && v().unix(a / 1e3).fromNow(), o = `${t.contDownTimerMessage}${s}.`, i = `${S()?t.soonExpiringSessionBody:o}`, r = t.renewSessionBody, l = S() ? w().createElement(w().Fragment, null, w().createElement("div", {
+                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
-                                }, i, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), w().createElement("div", null, r)) : w().createElement("div", {
+                                }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
-                                }, w().createElement("p", null, i), w().createElement("p", null, t.renewSessionNow)), c = [f.Dialog.okButton({
+                                }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), n && f.Dialog.okButton({
+                                }), a && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
-                                })], d = new f.Dialog({
+                                })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
-                            if (r && r.button.label === i.remindText) {
-                                const e = new x;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
-                            } else r && r.button.label === o.saveAndRenewButton && (l.dispose(), n(), a(), S() || j(T(), t))
-                        })(0, t._sessions, n, s, o), R(e, !1)) : R(e, !1)
+                            if (r && r.button.label === o.remindText) {
+                                const e = new C;
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
+                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const n = e.serviceManager.sessions,
-                            a = () => {
+                        const a = e.serviceManager.sessions,
+                            n = () => {
                                 s.start()
                             },
-                            s = ((e, t, n, a, s, o, i) => new D.Poll({
+                            s = ((e, t, a, n, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => A(e, t, n, a, s, o, i),
+                                factory: async () => U(e, t, a, n, s, i, o),
                                 frequency: {
-                                    interval: c,
+                                    interval: d,
                                     backoff: !0,
-                                    max: u
+                                    max: p
                                 }
-                            }))(e, n, (() => {
-                                const t = new B.TextModelFactory,
-                                    n = new B.DocumentRegistry({
+                            }))(e, a, (() => {
+                                const t = new I.TextModelFactory,
+                                    a = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    a = new N.ServiceManager({}),
-                                    s = new I.DocumentManager({
-                                        registry: n,
-                                        manager: a,
+                                    n = new z.ServiceManager({}),
+                                    s = new A.DocumentManager({
+                                        registry: a,
+                                        manager: n,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
                                             }
                                         }
                                     });
-                                (0, _.each)(e.shell.widgets("main"), (e => {
+                                (0, B.each)(e.shell.widgets("main"), (e => {
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), a, (e => {
+                            }), n, (e => {
                                 t = e
                             }), (() => t));
-                        a()
+                        n()
                     }
                 };
-            var U = n(667);
+            var P = a(4613);
             const G = [200, 201];
-            var P, z = n(7749);
+            var $, O = a(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
-            }(P || (P = {}));
-            const $ = async (e, t) => {
-                const n = N.ServerConnection.makeSettings(),
-                    a = z.URLExt.join(n.baseUrl, e);
+            }($ || ($ = {}));
+            const F = async (e, t) => {
+                const a = z.ServerConnection.makeSettings(),
+                    n = O.URLExt.join(a.baseUrl, e);
                 try {
-                    const e = await N.ServerConnection.makeRequest(a, {
+                    const e = await z.ServerConnection.makeRequest(n, {
                         method: t
-                    }, n);
+                    }, a);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var F = n(5933);
-            const O = "8px",
-                V = "12px",
-                W = F.css`
+            var V = a(5933);
+            const Z = "8px",
+                W = "12px",
+                H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
-                Z = F.css`
+                q = V.css`
   background-color: var(--jp-layout-color2);
   border: solid 1px var(--jp-border-color2);
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   position: fixed;
   bottom: 25px;
 `,
-                q = F.css`
-  margin: 0 ${V} ${O};
+                J = V.css`
+  margin: 0 ${W} ${Z};
 `,
-                J = F.css`
+                Y = V.css`
   font-weight: bold;
-  margin: ${O} 0 0 ${O};
+  margin: ${Z} 0 0 ${Z};
 `,
-                H = (F.css`
-  margin: 0 ${V} 0 ${"16px"};
-`, F.css`
+                Q = (V.css`
+  margin: 0 ${W} 0 ${"16px"};
+`, V.css`
   border-radius: 10px;
   height: 100%;
   width: 30px;
 `),
-                Y = F.css`
+                K = V.css`
   line-height: 24px;
   padding: 0 5px;
 
   &:hover {
     background-color: var(--jp-layout-color2);
   }
 `,
-                Q = (F.css`
+                X = (V.css`
   padding-left: 4px;
-`, F.css`
+`, V.css`
   display: flex;
   justify-content: flex-start;
   align-items: center;
   margin: 6px 12px;
 `),
-                K = F.css`
+                ee = V.css`
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   padding-right: 5px;
 `,
-                X = F.css`
+                te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ee = (F.css`
+                ae = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
-`, F.css`
+`, V.css`
   display: flex;
   align-items: center;
 `);
-            var te = n(8441);
-            const ne = ({
+            var ne = a(8441);
+            const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: n,
-                    label: a,
+                    displayValue: a,
+                    label: n,
                     labelClassName: s,
-                    conatinerClassName: o
-                }) => w().createElement("div", {
+                    conatinerClassName: i
+                }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
-                }, w().createElement("div", {
-                    className: o
-                }, a && w().createElement("span", {
+                }, f().createElement("div", {
+                    className: i
+                }, n && f().createElement("span", {
                     className: s
-                }, a, " ", n, "%"), w().createElement(te.Z, {
+                }, n, " ", a, "%"), f().createElement(ne.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
-                ae = "jlStudio-",
-                se = `${ae}ResourceUsageWidgetContainer`,
-                oe = `${ae}MetricsWidgetContainer`,
-                ie = ({
+                ie = "jlStudio-",
+                oe = `${ie}ResourceUsageWidgetContainer`,
+                re = `${ie}MetricsWidgetContainer`,
+                le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: n
+                    instanceMetricsDisplayValue: a
                 }) => {
-                    const [a, s] = (0, b.useState)(!1), [o, i] = (0, b.useState)(0), [r, l] = (0, b.useState)(0), [c, d] = (0, b.useState)(0), [u, g] = (0, b.useState)(!1), m = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
-                    (0, b.useEffect)((() => {
+                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, o = e.storage.total_space_in_bytes, r = s && o && s / o * 100;
-                            i(n), l(a), d(r)
+                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(a), l(n), d(r)
                         }
-                    }), [t]), (0, b.useEffect)((() => {
+                    }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
-                            } = p.ResourceUsage;
-                            f.Notification.info(e.title), g(!0)
+                            } = m.ResourceUsage;
+                            S.Notification.info(e.title), p(!0)
                         }
                     }), [u, c]);
                     const {
                         instanceMemoryProgressBarTitle: y,
                         instanceMetricsTitle: v,
-                        cpuMetricTitle: E,
-                        memoryMetricTitle: x,
-                        storageMetricTitle: S
-                    } = p.ResourceUsage;
-                    return w().createElement("div", {
+                        cpuMetricTitle: w,
+                        memoryMetricTitle: b,
+                        storageMetricTitle: x
+                    } = m.ResourceUsage;
+                    return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
-                        className: `${se} ${Y}`
-                    }, w().createElement("div", {
-                        className: ee,
+                        className: `${oe} ${K}`
+                    }, f().createElement("div", {
+                        className: ae,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(a),
+                        })(n),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === n ? w().createElement(te.Z, {
+                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
-                        className: X
-                    }) : w().createElement("div", {
-                        className: ee,
+                        className: te
+                    }) : f().createElement("div", {
+                        className: ae,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, w().createElement(te.Z, {
-                        className: X,
+                    }, f().createElement(ne.Z, {
+                        className: te,
                         variant: "determinate",
-                        value: 0 | n
-                    }), n ? Math.round(n) : 0, "%")), a && w().createElement("div", {
-                        className: `${oe} ${Z}`,
+                        value: 0 | a
+                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
-                    }, w().createElement("div", {
-                        className: W
-                    }, w().createElement("div", {
+                    }, f().createElement("div", {
+                        className: H
+                    }, f().createElement("div", {
+                        className: Y
+                    }, v), f().createElement("div", {
                         className: J
-                    }, v), w().createElement("div", {
-                        className: q
-                    }, w().createElement("div", null, w().createElement(ne, {
-                        value: m(o),
-                        displayValue: h(o),
-                        label: E,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                    }, f().createElement("div", null, f().createElement(se, {
+                        value: g(i),
+                        displayValue: h(i),
+                        label: w,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-cpu"
-                    }), w().createElement(ne, {
-                        value: m(r),
+                    }), f().createElement(se, {
+                        value: g(r),
                         displayValue: h(r),
-                        label: x,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: b,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-memory"
-                    }), w().createElement(ne, {
-                        value: m(c),
+                    }), f().createElement(se, {
+                        value: g(c),
                         displayValue: h(c),
-                        label: S,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: x,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-storage"
                     }))))))
                 };
-            class re extends f.ReactWidget {
+            class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
-                        await $("aws/sagemaker/api/instance/metrics", P.GET).then((e => {
+                        await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, n;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, a;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
-                    return w().createElement(ie, {
+                    return f().createElement(le, {
                         onClickHandler: this.clickHandler,
                         instanceMetricsResponse: this._instanceMetricsResponse,
                         instanceMetricsDisplayValue: this._instanceMetricsDisplayValue
                     })
                 }
             }
-            const le = {
+            const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
-                requires: [U.IStatusBar],
+                requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const n = new re;
+                    const a = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: n,
+                        item: a,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ce = n(2419),
-                de = n(2715);
-            const ue = F.css`
+            var ue = a(8031),
+                pe = a(2715);
+            const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
-                pe = ({
+                ge = ({
                     label: e,
                     id: t,
-                    helperText: n,
-                    error: a,
+                    helperText: a,
+                    error: n,
                     handleChange: s,
-                    regEx: o,
-                    ...i
+                    regEx: i,
+                    ...o
                 }) => {
-                    const [r, l] = (0, b.useState)(""), [c, d] = (0, b.useState)(!0);
-                    return w().createElement(de.Z, {
+                    const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
+                    return f().createElement(pe.Z, {
                         variant: "standard",
-                        className: ue,
+                        className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: n,
+                        helperText: a,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
-                            const t = new RegExp(o);
+                            const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
-                        ...i
+                        ...o
                     })
                 },
-                ge = F.css`
+                he = V.css`
   z-index: 2;
 `,
-                me = F.css`
+                ye = V.css`
   width: 460px;
   input {
     width: 460px;
   }
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
-            F.css`
+            V.css`
   margin-bottom: 20px;
 `;
-            var he = n(3776);
-            const ye = (e = !1) => F.css`
+            var ve = a(3776);
+            const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
-                ve = F.css`
+                be = V.css`
   margin-top: 20px;
 `,
-                be = ({
+                Ee = ({
                     options: e,
                     handleChange: t,
-                    label: n,
-                    freeSolo: a
+                    label: a,
+                    freeSolo: n
                 }) => {
-                    const s = (e, n) => {
-                        t(n)
+                    const s = (e, a) => {
+                        t(a)
                     };
-                    return b.createElement("div", {
-                        className: ve
-                    }, b.createElement("label", {
-                        className: ye(!0)
-                    }, n), b.createElement(he.Z, {
+                    return E.createElement("div", {
+                        className: be
+                    }, E.createElement("label", {
+                        className: we(!0)
+                    }, a), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: a,
+                        freeSolo: n,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
-                        renderInput: e => b.createElement(de.Z, {
+                        renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var we = n(2671),
-                Ee = n(847);
-            const fe = ({
+            var fe = a(2671),
+                xe = a(847);
+            const Se = ({
                     label: e,
                     id: t,
-                    handleChange: n,
-                    ...a
+                    handleChange: a,
+                    ...n
                 }) => {
-                    const [s, o] = (0, b.useState)(!0);
-                    return w().createElement(w().Fragment, null, w().createElement(Ee.Z, {
-                        control: w().createElement(we.Z, {
+                    const [s, i] = (0, E.useState)(!0);
+                    return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
+                        control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                o(e.target.checked), n(e.target.checked)
+                                i(e.target.checked), a(e.target.checked)
                             },
                             id: t,
-                            ...a
+                            ...n
                         }),
                         label: e
                     }))
                 },
-                xe = ({
+                Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: n,
-                    setOpenREADME: a
+                    setPath: a,
+                    setOpenREADME: n
                 }) => {
-                    const [s, o] = (0, b.useState)(""), [i, r] = (0, b.useState)(""), [l, c] = (0, b.useState)(!0), [d, u] = (0, b.useState)([]), {
-                        repoTitle: g,
-                        pathTitle: m,
+                    const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
+                        repoTitle: p,
+                        pathTitle: g,
                         openReadMeFilesLabel: h
-                    } = p.GitClone;
-                    return (0, b.useEffect)((() => {
+                    } = m.GitClone;
+                    return (0, E.useEffect)((() => {
                         if (e && e.GitCodeRepositories.length >= 0) {
                             const t = [];
                             e.GitCodeRepositories.length > 0 && e.GitCodeRepositories.forEach((e => t.push({
                                 value: e,
                                 label: e
                             }))), u(t)
                         }
-                    }), [e]), w().createElement("div", {
-                        className: me,
+                    }), [e]), f().createElement("div", {
+                        className: ye,
                         "data-testid": "git-clone-container",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab"
-                    }, w().createElement(be, {
+                    }, f().createElement(Ee, {
                         "data-testid": "autocomplete-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Repo-AutoComplete",
-                        label: g,
+                        label: p,
                         options: d,
-                        value: i,
+                        value: o,
                         handleChange: e => {
                             r(e), t(e)
                         },
                         freeSolo: !0
-                    }), w().createElement(pe, {
+                    }), f().createElement(ge, {
                         "data-testid": "text-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
-                        label: m,
+                        label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            o(e), n(e)
+                            i(e), a(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
-                    }), w().createElement(fe, {
+                    }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), a(e)
+                            c(e), n(e)
                         },
                         checked: l
                     }))
                 };
-            class Se extends f.ReactWidget {
+            class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
                         this.URL = e
                     }, this.setPath = e => {
                         this.path = e
                     }, this.setOpenREADME = e => {
                         this.openREADME = e
                     }, this.getGitRepositories = async () => {
-                        await $("aws/sagemaker/api/git/list-repositories", P.GET).then((e => {
+                        await F("aws/sagemaker/api/git/list-repositories", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this._gitCloneRepositories = e || null, this.update()
                             }))
                         }))
                     }, this.URL = "", this.path = "", this.openREADME = !0, this._gitCloneRepositories = null, this.getGitRepositories()
                 }
                 getValue() {
                     return {
                         URL: this.URL,
                         path: this.path,
                         openREADME: this.openREADME
                     }
                 }
                 render() {
-                    return w().createElement(xe, {
+                    return f().createElement(Ce, {
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Ce = n(9053),
-                Me = n(2190);
+            var Re = a(5962),
+                Te = a(2190);
             const {
-                name: Re,
-                version: Te
-            } = n(4147), je = (e, t, n) => e.child({
-                ExtensionName: Re,
-                ExtensionVersion: Te,
+                name: je,
+                version: ke
+            } = a(4147), De = (e, t, a) => e.child({
+                ExtensionName: je,
+                ExtensionVersion: ke,
                 PluginId: t
-            }, n);
-            var ke;
+            }, a);
+            var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
-            }(ke || (ke = {}));
-            const De = [{
+            }(_e || (_e = {}));
+            const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                _e = async (e, t, n) => {
+                Be = async (e, t, a) => {
                     const {
-                        repoPath: a,
+                        repoPath: n,
                         openREADME: s
-                    } = n;
+                    } = a;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: a
+                            path: n
                         }), !0 === s) try {
-                        await (async (e, t, n) => {
-                            const a = await t.get(e);
-                            if ("directory" === a.type) {
-                                const t = De.find((e => a.content.some((t => t.name === e.name))));
-                                t && await n.execute("docmanager:open", {
-                                    path: z.PathExt.join(e, t.name),
+                        await (async (e, t, a) => {
+                            const n = await t.get(e);
+                            if ("directory" === n.type) {
+                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
+                                t && await a.execute("docmanager:open", {
+                                    path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(a, t, e)
+                        })(n, t, e)
                     } catch (e) {}
-                }, Be = async (e, t) => {
-                    let n;
+                }, Ie = async (e, t) => {
+                    let a;
                     try {
-                        n = await t.get(e)
+                        a = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === n.type
+                    return "directory" === a.type
                 };
-            var Ne = n(1775),
-                Ie = n(248),
-                Ae = n(4337),
-                Le = n(9510);
+            var ze = a(1775),
+                Ae = a(248),
+                Ue = a(4337),
+                Le = a(8625);
             const {
-                dialogTitle: Ue,
+                dialogTitle: Pe,
                 cancelButton: Ge,
-                cloneButton: Pe,
-                errors: ze
-            } = p.GitClone, $e = {
+                cloneButton: $e,
+                errors: Oe
+            } = m.GitClone, Fe = {
                 id: s,
-                requires: [ce.IFileBrowserFactory, ce.IDefaultFileBrowser, Me.IGitExtension, f.IToolbarWidgetRegistry, Ie.ILogger, Ce.ITranslator],
+                requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, n, a, o, i, r) => {
+                activate: async (e, t, a, n, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
-                    } = e, d = c.contents, u = je(i, s), h = (r = r || Ce.nullTranslator).load("sagemaker_studio");
-                    l.addCommand(Ae.TQ.gitClone, {
+                    } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
+                    l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, n, a, s) => {
-                            var o, i;
+                        execute: () => (async (e, t, a, n, s) => {
+                            var i, o;
                             const r = t.model;
                             let l = "";
-                            const c = null === (i = null === (o = null == e ? void 0 : e.tracker) || void 0 === o ? void 0 : o.currentWidget) || void 0 === i ? void 0 : i.model.path;
+                            const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
-                                h = !0,
+                                p = !0,
                                 y = !0;
-                            const v = new f.Dialog({
-                                title: Ue,
-                                body: new Se,
+                            const v = new S.Dialog({
+                                title: Pe,
+                                body: new Me,
                                 focusNodeSelector: "input",
-                                buttons: [f.Dialog.cancelButton({
+                                buttons: [S.Dialog.cancelButton({
                                     label: Ge
-                                }), f.Dialog.okButton({
-                                    label: Pe
+                                }), S.Dialog.okButton({
+                                    label: $e
                                 })],
                                 hasClose: !1
                             });
-                            v.addClass(ge);
+                            v.addClass(he);
                             try {
                                 d = await v.launch()
                             } catch (e) {
                                 return void s.error({
                                     Message: g,
                                     Error: e
                                 })
                             }
                             if (!d.button.accept || !d.value) return;
-                            var b;
+                            var w;
                             if (({
                                     URL: l,
                                     path: u,
-                                    openREADME: h,
+                                    openREADME: p,
                                     findEnvironment: y
-                                } = d.value), "string" == typeof(b = u) && b.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, f.showErrorMessage)(ze.invalidCloneUrlTitle, {
-                                message: ze.invalidCloneUrlBody
+                                } = d.value), "string" == typeof(w = u) && w.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, S.showErrorMessage)(Oe.invalidCloneUrlTitle, {
+                                message: Oe.invalidCloneUrlBody
                             });
-                            const w = (e => {
-                                    const t = z.URLExt.parse(e);
-                                    return z.PathExt.basename(t.pathname, ".git")
+                            const b = (e => {
+                                    const t = O.URLExt.parse(e);
+                                    return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
-                                E = z.PathExt.join(u, w);
-                            let x;
+                                E = O.PathExt.join(u, b);
+                            let f;
                             try {
-                                x = await (async (e, t, n, a) => {
+                                f = await (async (e, t, a, n) => {
                                     const {
                                         errors: s
-                                    } = p.GitClone;
-                                    return await Be(t, e) ? await Be(a, e) ? (await (0, f.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + n
-                                    }), ke.AlreadyCloned) : ke.CanClone : (await (0, f.showErrorMessage)(s.directoryNotExistTitle, {
+                                    } = m.GitClone;
+                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + a
+                                    }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
-                                    }), ke.NotExist)
-                                })(n, u, l, E)
+                                    }), _e.NotExist)
+                                })(a, u, l, E)
                             } catch (e) {
                                 s.error({
-                                    Message: m,
+                                    Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
-                            const S = {
+                            const x = {
                                 repoPath: E,
-                                openREADME: h,
+                                openREADME: p,
                                 findEnvironment: y
                             };
-                            x === ke.CanClone ? (async (e, t, n, a, s, o) => {
+                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
                                 const {
-                                    errors: i
-                                } = p.GitClone, r = await e.execute("terminal:create-new");
+                                    errors: o
+                                } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
-                                s && (l += `cd ${s} && `), l += `git clone ${o} && exit\r`;
+                                s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async a => {
-                                        if ("disconnected" === a.connectionStatus) try {
-                                            await _e(e, t, n)
+                                    }), s.session.connectionStatusChanged.connect((async n => {
+                                        if ("disconnected" === n.connectionStatus) try {
+                                            await Be(e, t, a)
                                         } catch (e) {
-                                            await (0, f.showErrorMessage)(i.failedOptions, i.failedOptionsBody, [f.Dialog.warnButton({
+                                            await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await a.refresh()
+                                    })), await n.refresh()
                                 } catch (e) {
-                                    r.dispose(), await (0, f.showErrorMessage)(i.generalCloneErrorTitle, {
-                                        message: i.generalCloneErrorBody + e
+                                    r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
+                                        message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(a, n, S, r, u, l) : x === ke.AlreadyCloned && _e(a, n, S)
-                        })(t, n, d, l, u),
+                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
+                        })(t, a, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
-                    }), o.addFactory("FileBrowser", "gitClone", (() => f.ReactWidget.create(w().createElement(f.UseSignal, {
-                        signal: a.repositoryChanged,
+                    }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
+                        signal: n.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: a.pathRepository
+                            newValue: n.pathRepository
                         }
-                    }, ((t, n) => w().createElement(f.ToolbarButtonComponent, {
-                        enabled: null === (null == n ? void 0 : n.newValue),
+                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == a ? void 0 : a.newValue),
                         icon: Le.W6,
                         onClick: () => {
-                            e.commands.execute(Ae.TQ.gitClone)
+                            e.commands.execute(Ue.TQ.gitClone)
                         },
-                        tooltip: h.__("Git Clone")
-                    })))))), (0, Ne.ZM)(a, n, e.serviceManager.contents, e.contextMenu, h), u.info({
+                        tooltip: p.__("Git Clone")
+                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
-            }, Fe = e => {
-                var t, n;
-                const a = `${e}.AWSSageMakerUI`;
-                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
-            }, Oe = [h, L, le, $e, {
-                id: o,
-                requires: [Ie.ILogger],
+            }, Ve = e => {
+                var t, a;
+                const n = `${e}.AWSSageMakerUI`;
+                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+            }, Ze = {
+                id: i,
+                requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let a = {};
-                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
+                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let n = {};
+                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: n,
+                                requestStart: a,
                                 responseStart: s,
-                                startTime: o
+                                startTime: i
                             } = e;
-                            n && t && (a = {
-                                ...a,
-                                TimeToFirstByteMS: Math.round(s - o)
+                            a && t && (n = {
+                                ...n,
+                                TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
-                            o = null,
                             i = null,
+                            o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
-                        if (c) s = c.redirectCount, o = c.redirectEnd - c.redirectStart, i = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
+                        if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
-                            s = performance.navigation.redirectCount, o = e.redirectEnd - e.redirectStart, i = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
+                            s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        a = {
-                            ...a,
+                        n = {
+                            ...n,
                             RedirectCount: s,
-                            RedirectTimeMS: o,
-                            TimeToDOMContentLoadedMS: i,
+                            RedirectTimeMS: i,
+                            TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(a), t.started.then((() => {
+                        }, e.info(n), t.started.then((() => {
                             e.info({
-                                TimeToAppStartedMS: Math.round(Fe("timeToAppStarted"))
+                                TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (n = Math.round(Fe("timeToAppRestored"))) > 0 ? n : null;
-                            var n;
+                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
+                            var a;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
-                    })(je(t, o, Ie.logSchemas.performance), e)
+                    })(De(t, i, Ae.logSchemas.performance), e)
+                }
+            };
+            var We = a(87),
+                He = a(8201);
+            const qe = {
+                    SpaceMenuHeader: V.css`
+  margin: -6px 0;
+  padding: 0 var(--jp-size-2);
+  height: 10;
+  border-radius: var(--jp-radius-small);
+  font-size: var(--jp-size-3);
+  display: flex;
+  justify-content: center;
+  align-items: center;
+
+  & > p {
+    display: inline-block;
+    user-select: none;
+    color: var(--jp-color-root-light-800);
+  }
+
+  & > svg {
+    padding: 0 var(--jp-size-2);
+  }
+`
+                },
+                {
+                    privateSpaceHeader: Je,
+                    unknownUser: Ye
+                } = m.Space,
+                Qe = ({
+                    spaceName: e
+                }) => {
+                    const t = !!e,
+                        a = R("studioUserProfileName");
+                    return f().createElement("div", {
+                        className: qe.SpaceMenuHeader,
+                        "data-testid": y
+                    }, t ? f().createElement(We.Z, {
+                        fontSize: "small"
+                    }) : f().createElement(He.Z, {
+                        fontSize: "small"
+                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                };
+            class Ke extends S.ReactWidget {
+                constructor() {
+                    super(), this.getSpaceName = async () => {
+                        await F("aws/sagemaker/api/context", $.GET).then((e => {
+                            e && e.json().then((e => {
+                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                            }))
+                        }))
+                    }, this.spaceName = "", this.getSpaceName()
+                }
+                render() {
+                    return f().createElement(Qe, {
+                        spaceName: this.spaceName
+                    })
+                }
+            }
+            const Xe = [v, L, de, Fe, Ze, {
+                id: o,
+                requires: [Ae.ILogger],
+                autoStart: !0,
+                activate: async (e, t) => {
+                    const a = new Ke;
+                    a.id = S.DOMUtils.createDomID();
+                    const n = De(t, o);
+                    e.shell.add(a, "top", {
+                        rank: 1e3
+                    }), window && window.panorama && window.panorama("trackCustomEvent", {
+                        eventType: "render",
+                        eventDetail: "Space-Plugin",
+                        eventContext: "JupyterLab",
+                        timestamp: Date.now()
+                    }), n.info({
+                        Message: "Successfully loaded Space plugin"
+                    })
                 }
             }]
         },
+        8201: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
+                }), "AccountCircle");
+            t.Z = o
+        },
+        87: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
+                }), "Language");
+            t.Z = o
+        },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.2.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(8962),
+                Ds = o(7651),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.c3c95a37373ea011ffb4.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -14,35 +14,35 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(7308),
-                s = i(7807),
-                r = i(7749),
-                o = i(4085),
+            var n = i(9510),
+                s = i(3471),
+                r = i(6311),
+                o = i(3452),
                 a = i(6697),
                 l = i(7930),
-                c = i(8778),
+                c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
                     super(...e), this.name = "CancelledError"
                 }
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(9510),
+                v = i(8625),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1757,15 +1757,15 @@
                     width: "100%"
                 }),
                 m = (0, s.oB)({
                     display: "flex",
                     marginLeft: "auto",
                     overflow: "hidden"
                 });
-            var _, y = i(2688),
+            var _, y = i(4387),
                 v = i(7320);
             class b extends n.PureComponent {
                 constructor() {
                     super(...arguments), this._onDoubleClick = e => {
                         e.stopPropagation()
                     }
                 }
@@ -1854,16 +1854,16 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(7308),
-                s = i(8778),
+            var n = i(9510),
+                s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
             const h = a.clearTimeout,
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(9510),
+            var v = i(8625),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(4085),
+                C = i(3452),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,17 +2703,17 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(4085),
+            var n = i(3452),
                 s = i(6029),
-                r = i(2688),
+                r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
                     l = (null === (t = e.filetype) || void 0 === t ? void 0 : t.icon) || n.fileIcon;
                 return s.createElement(s.Fragment, null, s.createElement(l.react, {
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(7308),
+            var n = i(9510),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,19 +3180,19 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(7807),
-                s = i(7454),
-                r = i(9053),
+            var n = i(3471),
+                s = i(7777),
+                r = i(5962),
                 o = i(7930),
-                a = i(8778),
+                a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
                 editorFactory: e,
                 languageRegistry: t,
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(7749),
-                s = i(125),
+            var n = i(6311),
+                s = i(7217),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(7749),
-                r = i(7527),
+            var n, s = i(6311),
+                r = i(1638),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4499,15 +4499,15 @@
                         },
                         t = `&:hover .${r}`;
                     return e.$nest[t] = {
                         display: "block"
                     }, e
                 })()
         },
-        2688: (e, t, i) => {
+        4387: (e, t, i) => {
             "use strict";
             i.d(t, {
                 cf: () => s,
                 gW: () => o,
                 ge: () => r
             });
             var n = i(9946);
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        9510: (e, t, i) => {
+        8625: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(4085);
+            var n = i(3452);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(125);
+            var n = i(7217);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(7749),
+            var n = i(6311),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(9053),
-                o = i(8778),
+                r = i(5962),
+                o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(7807),
-                f = i(7454);
+                u = i(3471),
+                f = i(7777);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,36 +1,36 @@
-/*! For license information please see 891.ada29ec8d5578292aa74.js.LICENSE.txt */
+/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(3205),
-                r = s(7308),
-                a = s(7807),
-                o = s(1165),
-                n = s(2419),
-                l = s(5409),
-                d = s(9499),
-                c = s(8190),
-                h = s(667),
-                p = s(9053),
+            var i = s(8368),
+                r = s(9510),
+                a = s(3471),
+                o = s(5326),
+                n = s(8031),
+                l = s(9557),
+                d = s(8048),
+                c = s(4008),
+                h = s(4613),
+                p = s(5962),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(9510),
+                f = s(8625),
                 _ = s(4337),
-                b = s(8778);
+                b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
                 }
                 getValue() {
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(7932),
+                it = s(6963),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(5390);
+            var _t = s(1778);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(7749),
-                us = s(125);
+                ms = s(6311),
+                us = s(7217);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(4085),
+            var Ss = s(3452),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7454),
+            var Rr = s(7777),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.e8f2ffedbb22ee676b66.js` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js`

 * *Files 8% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, d, u, f, c, s, p, m, b, h, v, g, y, j, w, P, k = {
-            9110: (e, r, t) => {
+    var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
+            1514: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -48,61 +48,61 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.2.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(445), S.e(779)]).then((() => () => S(4779))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(445), S.e(875)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -234,98 +234,98 @@
                 } else {
                     if (i <= a || f < c != n) return !1;
                     d = !1
                 } else "s" != c && "n" != c && (d = !1, i--)
             }
         }
         var s = [],
-            p = s.pop.bind(s);
+            b = s.pop.bind(s);
         for (l = 1; l < e.length; l++) {
-            var m = e[l];
-            s.push(1 == m ? p() | p() : 2 == m ? p() & p() : m ? o(m, r) : !p())
+            var p = e[l];
+            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
         }
-        return !!p()
+        return !!b()
     }, l = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = d(e, t);
-        return o(a, n) || p(u(e, t, n, a)), b(e[t][n])
+        return o(a, n) || b(u(e, t, n, a)), m(e[t][n])
     }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, p = e => {
+    }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, m = (e, r, t, a) => {
-        p(s(e, r, t, a))
-    }, b = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
+    }, p = (e, r, t, a) => {
+        b(s(e, r, t, a))
+    }, m = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => (l(e, t), b(c(r, t, a) || m(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
+    })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
-        return o ? b(o) : n()
+        return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
-        125: () => g("default", "@jupyterlab/services", [1, 7, 0, 9]),
-        667: () => g("default", "@jupyterlab/statusbar", [1, 4, 0, 9]),
-        1165: () => g("default", "@jupyterlab/docmanager", [1, 4, 0, 9]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        2419: () => g("default", "@jupyterlab/filebrowser", [1, 4, 0, 9]),
-        3205: () => g("default", "@jupyterlab/application", [1, 4, 0, 9]),
-        4085: () => g("default", "@jupyterlab/ui-components", [1, 4, 0, 9]),
+        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
+        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
+        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5409: () => g("default", "@jupyterlab/mainmenu", [1, 4, 0, 9]),
+        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
+        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
+        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        7308: () => g("default", "@jupyterlab/apputils", [1, 4, 1, 9]),
-        7454: () => g("default", "@jupyterlab/codemirror", [1, 4, 0, 9]),
-        7527: () => v("default", "@jupyterlab/docregistry", [1, 4, 0, 9]),
-        7749: () => g("default", "@jupyterlab/coreutils", [1, 6, 0, 9]),
-        7807: () => g("default", "@jupyterlab/codeeditor", [1, 4, 0, 9]),
+        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
+        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
+        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        7932: () => v("default", "@jupyterlab/nbformat", [1, 4, 0, 9]),
+        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8778: () => g("default", "@lumino/widgets", [1, 2, 0, 1]),
-        9053: () => g("default", "@jupyterlab/translation", [1, 4, 0, 9]),
+        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
+        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(875)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
+        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
+        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
-        5390: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 9]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8190: () => g("default", "@jupyterlab/settingregistry", [1, 4, 0, 9]),
-        9499: () => g("default", "@jupyterlab/rendermime", [1, 4, 0, 9]),
+        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
-        445: [125, 667, 1165, 1373, 2419, 3205, 4085, 4901, 5409, 6211, 6697, 6797, 7308, 7454, 7527, 7749, 7807, 7930, 7932, 8093, 8204, 8778, 9053],
+        548: [248, 2190, 5933, 9801],
+        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
-        779: [248, 2190, 5933, 9801],
         798: [851, 7138],
         800: [8800],
-        875: [5359, 5390, 5633, 7350, 7489, 7858, 8190, 9499]
+        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|445|704|798|800|875)$/.test(r)) e[r] = 0;
+                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(9110);
+    var E = S(1514);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json` & `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.dist-info/LICENSE` & `sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.dist-info/METADATA` & `sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.2.0
+Version: 0.3.0
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

#### Comparing `sagemaker_jupyterlab_extension-0.2.0.dist-info/RECORD` & `sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 sagemaker_jupyterlab_extension/__init__.py,sha256=hxDcPQ4HLDyOST0TL-Lu5fvzhEwrIgSkZLybVPPEkgk,1133
 sagemaker_jupyterlab_extension/_version.py,sha256=H8LOQyA3X6Xj3pixozSSsatne-Jd9sIhfgCIwlM6AGg,683
 sagemaker_jupyterlab_extension/handlers.py,sha256=j2uNNvU6Vu2guPRev4OEuyKtc_YkOJfAql3exvdn1nw,11587
-sagemaker_jupyterlab_extension/labextension/package.json,sha256=moRR4TE_HZ8nXRKpHXZudCohWf-9v6IH6zPxS3zUVKk,4068
+sagemaker_jupyterlab_extension/labextension/package.json,sha256=vNBJJjg0D1EZFYUpr5nhKC-qF876ZBk3JTiFLal9Q2Q,4091
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
-sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
+sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js,sha256=ITWmKXaTsJZi2RNSG_PhVswJsCWBUWbBG0NIspc16uY,92715
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
+sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js,sha256=U1C3Q_miNdniZQpaU-SBDzhd4-P6ZkDu9G0foZd9rbU,28094
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
-sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js,sha256=Ok8AxYMibavEcUS-EFziQqjANWhU9snSiVydXFyqvpk,25159
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
-sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
-sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js,sha256=w8laNzc-oBH_tKep2Abs4tbHNSPCIXUbBgFWAODegLw,266480
+sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js,sha256=xQj-q53990lCFADTVbj3XegiS7kmYg8nAZtBnh79AG4,237708
+sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js,sha256=fwYWONRwdax2vgvW-p1L_6Sxs96H0fuY5f-tv22OsFs,266482
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
-sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js,sha256=dgt7EUDDDaLCJz6c2CyRFM8-VZoxX36p5rVOgVxNYDo,139403
-sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js,sha256=6PL_7bsi7mdrZuBN9b8Mcg7cpWC3_Me3agE3hhxzULM,12090
+sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
+sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js,sha256=J6Dj37MkMa_pQGmyuP4D6AwYwfeTQf73i5AJieQzCl4,12105
 sagemaker_jupyterlab_extension/labextension/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
 sagemaker_jupyterlab_extension/tests/__init__.py,sha256=LJe9lg48SCXTjTOe_oc0_Zj9blApYphXi-12E_3fh2s,60
 sagemaker_jupyterlab_extension/tests/helper.py,sha256=bH3LEHznHOzkfOfBmRn-S8hh5sUuRHj_EmjvjUdQ4uc,405
 sagemaker_jupyterlab_extension/tests/test_error_util.py,sha256=QBhspnhVQzw_a8yUVlfhxalT8ywS3sntb_diFK4nvDw,1647
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py,sha256=O-QWKCetqSPCpzhBlFqS4zO1dp9_nJdGGpE_mqor2BU,5332
 sagemaker_jupyterlab_extension/tests/test_handlers.py,sha256=6BOEKL3v87psZtcqVbqlHjfRzyiBFZfFcUbig-ELCB8,5041
-sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=475L1399lYR2yb2Udt-9cT1ZkKFZh89xr2WTEmoz2ew,7701
+sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=y9sHb49HgUQDBLLQLwmSa-Cz1CwXnW2mu7qHvZUR4qE,7701
 sagemaker_jupyterlab_extension/utils/__init__.py,sha256=r4W_GQMVXe3D90bLPU9hZUehj0U1AhbN1qDE9M5vI6Y,64
 sagemaker_jupyterlab_extension/utils/error_util.py,sha256=fT6BDMGeHK9J70A8vyGkl_ygL662XQ5incmoq8X_R1Y,555
 sagemaker_jupyterlab_extension/utils/git_clone_util.py,sha256=pHExYjlSniCLZ-Q78OjrfIvsPPz2Cd13jB7F9Jiiu-s,2552
 sagemaker_jupyterlab_extension/utils/metric_util.py,sha256=h2w-vEFVpJkSSOA97gr5hpG6ROe6xgfYbK_VaaBItvg,507
 sagemaker_jupyterlab_extension/utils/request_logger.py,sha256=SNq6_gng-ElaUDl_akXmcFRYy9gFlydcRwWRZphNFs4,7250
-sagemaker_jupyterlab_extension-0.2.0.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
-sagemaker_jupyterlab_extension-0.2.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=moRR4TE_HZ8nXRKpHXZudCohWf-9v6IH6zPxS3zUVKk,4068
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/779.3a4f00c583226dabc471.js,sha256=Ok8AxYMibavEcUS-EFziQqjANWhU9snSiVydXFyqvpk,25159
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.c3c95a37373ea011ffb4.js,sha256=w8laNzc-oBH_tKep2Abs4tbHNSPCIXUbBgFWAODegLw,266480
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js,sha256=dgt7EUDDDaLCJz6c2CyRFM8-VZoxX36p5rVOgVxNYDo,139403
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.ada29ec8d5578292aa74.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.e8f2ffedbb22ee676b66.js,sha256=6PL_7bsi7mdrZuBN9b8Mcg7cpWC3_Me3agE3hhxzULM,12090
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
-sagemaker_jupyterlab_extension-0.2.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
-sagemaker_jupyterlab_extension-0.2.0.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
-sagemaker_jupyterlab_extension-0.2.0.dist-info/METADATA,sha256=ar4zGHxMn32UgbnSSTBBBhSxr-YAfGoeiaZbkGqy1Pw,2281
-sagemaker_jupyterlab_extension-0.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-sagemaker_jupyterlab_extension-0.2.0.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
-sagemaker_jupyterlab_extension-0.2.0.dist-info/RECORD,,
+sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
+sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=vNBJJjg0D1EZFYUpr5nhKC-qF876ZBk3JTiFLal9Q2Q,4091
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js,sha256=ITWmKXaTsJZi2RNSG_PhVswJsCWBUWbBG0NIspc16uY,92715
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js,sha256=U1C3Q_miNdniZQpaU-SBDzhd4-P6ZkDu9G0foZd9rbU,28094
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js,sha256=xQj-q53990lCFADTVbj3XegiS7kmYg8nAZtBnh79AG4,237708
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js,sha256=fwYWONRwdax2vgvW-p1L_6Sxs96H0fuY5f-tv22OsFs,266482
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js,sha256=J6Dj37MkMa_pQGmyuP4D6AwYwfeTQf73i5AJieQzCl4,12105
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
+sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
+sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
+sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA,sha256=bhG-_zyCuCnM3Bevz3uvAefQ3kyqYXCiyZLjLZE-jZc,2281
+sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
+sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD,,
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/__init__.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/_version.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/_version.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/handlers.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/package.json` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649616858237547%*

 * *Differences: {"'dependencies'": "{'cookie': '0.6.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.27a0e3dfb32431afe940.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -20,14 +20,15 @@
         "@lumino/commands": "^2.0.0",
         "@lumino/polling": "^2.1.2",
         "@lumino/signaling": "^2.1.2",
         "@lumino/widgets": "^2.0.0",
         "@mui/icons-material": "5.14",
         "@mui/material": "^5.14.4",
         "@testing-library/react": "^13.0.0",
+        "cookie": "0.6.0",
         "isomorphic-fetch": "^3.0.0",
         "moment": "^2.29.4",
         "p-retry": "^5.1.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "SageMaker JupyterLab workspace primary extension module",
@@ -59,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e8f2ffedbb22ee676b66.js",
+            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -104,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(8962),
+                f = o(7651),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        8962: (e, t, o) => {
+        7651: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,27 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
-    [779], {
-        4779: (e, t, n) => {
-            n.r(t), n.d(t, {
-                default: () => Oe
+    [548], {
+        4548: (e, t, a) => {
+            a.r(t), a.d(t, {
+                default: () => Xe
             });
-            var a = n(5409);
+            var n = a(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
-                o = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
-                i = {
+                i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
+                o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
+                r = {
                     shutdown: "filemenu:shutdown"
                 },
-                r = "Sso",
-                l = 3e5,
-                c = 500,
-                d = 100,
-                u = 12e4,
-                p = {
+                l = "Sso",
+                c = 3e5,
+                d = 500,
+                u = 100,
+                p = 12e4,
+                m = {
                     SignInSession: {
                         closeButton: "Close",
                         signInButton: "Sign In",
                         saveButton: "Save",
                         saveAndRenewButton: "Save and renew session",
                         signinDialog: {
                             title: "Please sign in again",
@@ -71,898 +72,1001 @@
                             generalCloneErrorTitle: "Unable to clone repository to project.",
                             generalCloneErrorBody: "Something went wrong when trying to clone the repository to your project. Please try again later. ",
                             failedOptions: "Failed to handle additional options.",
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
+                    },
+                    Space: {
+                        privateSpaceHeader: "Personal Studio",
+                        unknownUser: "Unknown User"
                     }
                 },
                 g = "GitCloneDialogError",
-                m = "ValidRepoPathError",
-                h = {
+                h = "ValidRepoPathError",
+                y = "spaceMenuHeader",
+                v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [a.IMainMenu],
+                    requires: [n.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
-                        e.commands._commands.get(i.shutdown).isVisible = () => !1
+                        e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var y = n(9801),
-                v = n.n(y),
-                b = n(6029),
-                w = n.n(b),
-                E = n(3205),
-                f = n(7308);
-            class x {
+            var w = a(9801),
+                b = a.n(w),
+                E = a(6029),
+                f = a.n(E),
+                x = a(8368),
+                S = a(9510);
+            class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
                 getDismissTime() {
                     return this._dismissTime
                 }
             }
-            const S = () => {
-                    const e = C("authMode");
-                    return e && e[1] && e[1] === r
-                },
-                C = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
-                M = () => {
-                    const e = C("expiryTime"),
-                        t = C("ssoExpiryTimestamp");
-                    return S() && t ? Number(t[1]) : e ? Number(e[1]) : null
-                },
-                R = (e, t) => {
-                    var n, a;
-                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(E.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(E.ConnectionLost)
+            const M = () => {
+                    const e = R("authMode");
+                    return e && e[1] && e[1] === l
                 },
+                R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
-                    const e = C("redirectURL");
+                    const e = R("expiryTime"),
+                        t = R("ssoExpiryTimestamp");
+                    return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
+                },
+                j = (e, t) => {
+                    var a, n;
+                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                },
+                k = () => {
+                    const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
-                j = (e, t) => {
-                    const n = M(),
-                        a = window.open(e, "signin window", "width=800, height=600");
+                D = (e, t) => {
+                    const a = T(),
+                        n = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
-                    const o = window.setInterval((() => {
-                        if (a && a.closed && !s) return void window.clearInterval(o);
-                        const e = M();
-                        if (null !== e && null !== n && (e > n || isNaN(e))) {
-                            window.clearInterval(o), a && a.close(), s = !0;
+                    const i = window.setInterval((() => {
+                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        const e = T();
+                        if (null !== e && null !== a && (e > a || isNaN(e))) {
+                            window.clearInterval(i), n && n.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
-                            f.Dialog.tracker.forEach((e => e.reject()))
+                            S.Dialog.tracker.forEach((e => e.reject()))
                         }
-                    }), d)
+                    }), u)
                 },
-                k = async () => {
+                _ = async () => {
                     const {
                         SignInSession: e
-                    } = p, {
+                    } = m, {
                         signinDialog: t
-                    } = e, n = T(), a = n ? [f.Dialog.okButton({
+                    } = e, a = k(), n = a ? [S.Dialog.okButton({
                         label: e.signInButton
-                    })] : [f.Dialog.cancelButton({
+                    })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = n ? w().createElement("div", {
+                    })], s = a ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
-                    }, t.loggedOutBody) : w().createElement("div", {
+                    }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
-                    }, t.restartSessionBody), o = new f.Dialog({
+                    }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: a,
+                        buttons: n,
                         hasClose: !1
                     });
                     return {
-                        sigInDialogResult: await o.launch(),
-                        confirmDialog: o
+                        sigInDialogResult: await i.launch(),
+                        confirmDialog: i
                     }
                 };
-            var D = n(6797),
-                _ = n(6697),
-                B = n(7527),
-                N = n(125),
-                I = n(1165);
-            const A = (e, t, n, a, s, o, i) => {
-                    const r = M(),
-                        c = i(),
-                        d = c && c + l;
-                    if (null === r) R(e, !1);
+            var N = a(6797),
+                B = a(6697),
+                I = a(1638),
+                z = a(7217),
+                A = a(5326);
+            const U = (e, t, a, n, s, i, o) => {
+                    const r = T(),
+                        l = o(),
+                        d = l && l + c;
+                    if (null === r) j(e, !1);
                     else {
-                        const i = v().unix(r / 1e3).diff(v()()),
+                        const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(S(), r, i) ? (a(), (async (e, t, n) => {
+                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
                             const {
-                                SignInSession: a
-                            } = p, s = T();
-                            f.Dialog.tracker.forEach((e => e.reject())), R(e, !0);
+                                SignInSession: n
+                            } = m, s = k();
+                            S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
-                                sigInDialogResult: o,
-                                confirmDialog: i
-                            } = await k();
-                            if (o && o.button)
-                                if (n(), s) j(T(), t);
-                                else if (o && o.button.label === a.closeButton) {
-                                const e = M(),
+                                sigInDialogResult: i,
+                                confirmDialog: o
+                            } = await _();
+                            if (i && i.button)
+                                if (a(), s) D(k(), t);
+                                else if (i && i.button.label === n.closeButton) {
+                                const e = T(),
                                     t = e && e / 1e3,
-                                    n = t && v().unix(t).diff(v()());
-                                null !== n && n && n > l && (i.dispose(), setTimeout((async () => {
-                                    await k()
-                                }), l))
-                            } else i.dispose(), j(T(), t)
-                        })(e, t, s)) : i <= 9e5 && (void 0 === c || d && u > d) ? (a(), (async (e, t, n, a, s) => {
+                                    a = t && b().unix(t).diff(b()());
+                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    await _()
+                                }), c))
+                            } else o.dispose(), D(k(), t)
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
                             const {
-                                SignInSession: o
-                            } = p, {
-                                renewSessionDialog: i
-                            } = p.SignInSession, {
+                                SignInSession: i
+                            } = m, {
+                                renewSessionDialog: o
+                            } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
-                                } = p, {
+                                } = m, {
                                     renewSessionDialog: t
-                                } = p.SignInSession, n = T(), a = M(), s = a && v().unix(a / 1e3).fromNow(), o = `${t.contDownTimerMessage}${s}.`, i = `${S()?t.soonExpiringSessionBody:o}`, r = t.renewSessionBody, l = S() ? w().createElement(w().Fragment, null, w().createElement("div", {
+                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
-                                }, i, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), w().createElement("div", null, r)) : w().createElement("div", {
+                                }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
-                                }, w().createElement("p", null, i), w().createElement("p", null, t.renewSessionNow)), c = [f.Dialog.okButton({
+                                }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), n && f.Dialog.okButton({
+                                }), a && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
-                                })], d = new f.Dialog({
+                                })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
-                            if (r && r.button.label === i.remindText) {
-                                const e = new x;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
-                            } else r && r.button.label === o.saveAndRenewButton && (l.dispose(), n(), a(), S() || j(T(), t))
-                        })(0, t._sessions, n, s, o), R(e, !1)) : R(e, !1)
+                            if (r && r.button.label === o.remindText) {
+                                const e = new C;
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
+                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const n = e.serviceManager.sessions,
-                            a = () => {
+                        const a = e.serviceManager.sessions,
+                            n = () => {
                                 s.start()
                             },
-                            s = ((e, t, n, a, s, o, i) => new D.Poll({
+                            s = ((e, t, a, n, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => A(e, t, n, a, s, o, i),
+                                factory: async () => U(e, t, a, n, s, i, o),
                                 frequency: {
-                                    interval: c,
+                                    interval: d,
                                     backoff: !0,
-                                    max: u
+                                    max: p
                                 }
-                            }))(e, n, (() => {
-                                const t = new B.TextModelFactory,
-                                    n = new B.DocumentRegistry({
+                            }))(e, a, (() => {
+                                const t = new I.TextModelFactory,
+                                    a = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    a = new N.ServiceManager({}),
-                                    s = new I.DocumentManager({
-                                        registry: n,
-                                        manager: a,
+                                    n = new z.ServiceManager({}),
+                                    s = new A.DocumentManager({
+                                        registry: a,
+                                        manager: n,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
                                             }
                                         }
                                     });
-                                (0, _.each)(e.shell.widgets("main"), (e => {
+                                (0, B.each)(e.shell.widgets("main"), (e => {
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), a, (e => {
+                            }), n, (e => {
                                 t = e
                             }), (() => t));
-                        a()
+                        n()
                     }
                 };
-            var U = n(667);
+            var P = a(4613);
             const G = [200, 201];
-            var P, z = n(7749);
+            var $, O = a(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
-            }(P || (P = {}));
-            const $ = async (e, t) => {
-                const n = N.ServerConnection.makeSettings(),
-                    a = z.URLExt.join(n.baseUrl, e);
+            }($ || ($ = {}));
+            const F = async (e, t) => {
+                const a = z.ServerConnection.makeSettings(),
+                    n = O.URLExt.join(a.baseUrl, e);
                 try {
-                    const e = await N.ServerConnection.makeRequest(a, {
+                    const e = await z.ServerConnection.makeRequest(n, {
                         method: t
-                    }, n);
+                    }, a);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var F = n(5933);
-            const O = "8px",
-                V = "12px",
-                W = F.css`
+            var V = a(5933);
+            const Z = "8px",
+                W = "12px",
+                H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
-                Z = F.css`
+                q = V.css`
   background-color: var(--jp-layout-color2);
   border: solid 1px var(--jp-border-color2);
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   position: fixed;
   bottom: 25px;
 `,
-                q = F.css`
-  margin: 0 ${V} ${O};
+                J = V.css`
+  margin: 0 ${W} ${Z};
 `,
-                J = F.css`
+                Y = V.css`
   font-weight: bold;
-  margin: ${O} 0 0 ${O};
+  margin: ${Z} 0 0 ${Z};
 `,
-                H = (F.css`
-  margin: 0 ${V} 0 ${"16px"};
-`, F.css`
+                Q = (V.css`
+  margin: 0 ${W} 0 ${"16px"};
+`, V.css`
   border-radius: 10px;
   height: 100%;
   width: 30px;
 `),
-                Y = F.css`
+                K = V.css`
   line-height: 24px;
   padding: 0 5px;
 
   &:hover {
     background-color: var(--jp-layout-color2);
   }
 `,
-                Q = (F.css`
+                X = (V.css`
   padding-left: 4px;
-`, F.css`
+`, V.css`
   display: flex;
   justify-content: flex-start;
   align-items: center;
   margin: 6px 12px;
 `),
-                K = F.css`
+                ee = V.css`
   color: var(--jp-ui-font-color1);
   font-size: var(--jp-ui-font-size1);
   padding-right: 5px;
 `,
-                X = F.css`
+                te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ee = (F.css`
+                ae = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
-`, F.css`
+`, V.css`
   display: flex;
   align-items: center;
 `);
-            var te = n(8441);
-            const ne = ({
+            var ne = a(8441);
+            const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: n,
-                    label: a,
+                    displayValue: a,
+                    label: n,
                     labelClassName: s,
-                    conatinerClassName: o
-                }) => w().createElement("div", {
+                    conatinerClassName: i
+                }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
-                }, w().createElement("div", {
-                    className: o
-                }, a && w().createElement("span", {
+                }, f().createElement("div", {
+                    className: i
+                }, n && f().createElement("span", {
                     className: s
-                }, a, " ", n, "%"), w().createElement(te.Z, {
+                }, n, " ", a, "%"), f().createElement(ne.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
-                ae = "jlStudio-",
-                se = `${ae}ResourceUsageWidgetContainer`,
-                oe = `${ae}MetricsWidgetContainer`,
-                ie = ({
+                ie = "jlStudio-",
+                oe = `${ie}ResourceUsageWidgetContainer`,
+                re = `${ie}MetricsWidgetContainer`,
+                le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: n
+                    instanceMetricsDisplayValue: a
                 }) => {
-                    const [a, s] = (0, b.useState)(!1), [o, i] = (0, b.useState)(0), [r, l] = (0, b.useState)(0), [c, d] = (0, b.useState)(0), [u, g] = (0, b.useState)(!1), m = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
-                    (0, b.useEffect)((() => {
+                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, o = e.storage.total_space_in_bytes, r = s && o && s / o * 100;
-                            i(n), l(a), d(r)
+                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(a), l(n), d(r)
                         }
-                    }), [t]), (0, b.useEffect)((() => {
+                    }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
-                            } = p.ResourceUsage;
-                            f.Notification.info(e.title), g(!0)
+                            } = m.ResourceUsage;
+                            S.Notification.info(e.title), p(!0)
                         }
                     }), [u, c]);
                     const {
                         instanceMemoryProgressBarTitle: y,
                         instanceMetricsTitle: v,
-                        cpuMetricTitle: E,
-                        memoryMetricTitle: x,
-                        storageMetricTitle: S
-                    } = p.ResourceUsage;
-                    return w().createElement("div", {
+                        cpuMetricTitle: w,
+                        memoryMetricTitle: b,
+                        storageMetricTitle: x
+                    } = m.ResourceUsage;
+                    return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
-                        className: `${se} ${Y}`
-                    }, w().createElement("div", {
-                        className: ee,
+                        className: `${oe} ${K}`
+                    }, f().createElement("div", {
+                        className: ae,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(a),
+                        })(n),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === n ? w().createElement(te.Z, {
+                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
-                        className: X
-                    }) : w().createElement("div", {
-                        className: ee,
+                        className: te
+                    }) : f().createElement("div", {
+                        className: ae,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, w().createElement(te.Z, {
-                        className: X,
+                    }, f().createElement(ne.Z, {
+                        className: te,
                         variant: "determinate",
-                        value: 0 | n
-                    }), n ? Math.round(n) : 0, "%")), a && w().createElement("div", {
-                        className: `${oe} ${Z}`,
+                        value: 0 | a
+                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
-                    }, w().createElement("div", {
-                        className: W
-                    }, w().createElement("div", {
+                    }, f().createElement("div", {
+                        className: H
+                    }, f().createElement("div", {
+                        className: Y
+                    }, v), f().createElement("div", {
                         className: J
-                    }, v), w().createElement("div", {
-                        className: q
-                    }, w().createElement("div", null, w().createElement(ne, {
-                        value: m(o),
-                        displayValue: h(o),
-                        label: E,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                    }, f().createElement("div", null, f().createElement(se, {
+                        value: g(i),
+                        displayValue: h(i),
+                        label: w,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-cpu"
-                    }), w().createElement(ne, {
-                        value: m(r),
+                    }), f().createElement(se, {
+                        value: g(r),
                         displayValue: h(r),
-                        label: x,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: b,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-memory"
-                    }), w().createElement(ne, {
-                        value: m(c),
+                    }), f().createElement(se, {
+                        value: g(c),
                         displayValue: h(c),
-                        label: S,
-                        labelClassName: K,
-                        singleProgressBarStyle: H,
-                        conatinerClassName: Q,
+                        label: x,
+                        labelClassName: ee,
+                        singleProgressBarStyle: Q,
+                        conatinerClassName: X,
                         "data-testid": "resource-usage-data-container-storage"
                     }))))))
                 };
-            class re extends f.ReactWidget {
+            class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
-                        await $("aws/sagemaker/api/instance/metrics", P.GET).then((e => {
+                        await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, n;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, a;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
-                    return w().createElement(ie, {
+                    return f().createElement(le, {
                         onClickHandler: this.clickHandler,
                         instanceMetricsResponse: this._instanceMetricsResponse,
                         instanceMetricsDisplayValue: this._instanceMetricsDisplayValue
                     })
                 }
             }
-            const le = {
+            const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
-                requires: [U.IStatusBar],
+                requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const n = new re;
+                    const a = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: n,
+                        item: a,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ce = n(2419),
-                de = n(2715);
-            const ue = F.css`
+            var ue = a(8031),
+                pe = a(2715);
+            const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
-                pe = ({
+                ge = ({
                     label: e,
                     id: t,
-                    helperText: n,
-                    error: a,
+                    helperText: a,
+                    error: n,
                     handleChange: s,
-                    regEx: o,
-                    ...i
+                    regEx: i,
+                    ...o
                 }) => {
-                    const [r, l] = (0, b.useState)(""), [c, d] = (0, b.useState)(!0);
-                    return w().createElement(de.Z, {
+                    const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
+                    return f().createElement(pe.Z, {
                         variant: "standard",
-                        className: ue,
+                        className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: n,
+                        helperText: a,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
-                            const t = new RegExp(o);
+                            const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
-                        ...i
+                        ...o
                     })
                 },
-                ge = F.css`
+                he = V.css`
   z-index: 2;
 `,
-                me = F.css`
+                ye = V.css`
   width: 460px;
   input {
     width: 460px;
   }
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
-            F.css`
+            V.css`
   margin-bottom: 20px;
 `;
-            var he = n(3776);
-            const ye = (e = !1) => F.css`
+            var ve = a(3776);
+            const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
-                ve = F.css`
+                be = V.css`
   margin-top: 20px;
 `,
-                be = ({
+                Ee = ({
                     options: e,
                     handleChange: t,
-                    label: n,
-                    freeSolo: a
+                    label: a,
+                    freeSolo: n
                 }) => {
-                    const s = (e, n) => {
-                        t(n)
+                    const s = (e, a) => {
+                        t(a)
                     };
-                    return b.createElement("div", {
-                        className: ve
-                    }, b.createElement("label", {
-                        className: ye(!0)
-                    }, n), b.createElement(he.Z, {
+                    return E.createElement("div", {
+                        className: be
+                    }, E.createElement("label", {
+                        className: we(!0)
+                    }, a), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: a,
+                        freeSolo: n,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
-                        renderInput: e => b.createElement(de.Z, {
+                        renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var we = n(2671),
-                Ee = n(847);
-            const fe = ({
+            var fe = a(2671),
+                xe = a(847);
+            const Se = ({
                     label: e,
                     id: t,
-                    handleChange: n,
-                    ...a
+                    handleChange: a,
+                    ...n
                 }) => {
-                    const [s, o] = (0, b.useState)(!0);
-                    return w().createElement(w().Fragment, null, w().createElement(Ee.Z, {
-                        control: w().createElement(we.Z, {
+                    const [s, i] = (0, E.useState)(!0);
+                    return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
+                        control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                o(e.target.checked), n(e.target.checked)
+                                i(e.target.checked), a(e.target.checked)
                             },
                             id: t,
-                            ...a
+                            ...n
                         }),
                         label: e
                     }))
                 },
-                xe = ({
+                Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: n,
-                    setOpenREADME: a
+                    setPath: a,
+                    setOpenREADME: n
                 }) => {
-                    const [s, o] = (0, b.useState)(""), [i, r] = (0, b.useState)(""), [l, c] = (0, b.useState)(!0), [d, u] = (0, b.useState)([]), {
-                        repoTitle: g,
-                        pathTitle: m,
+                    const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
+                        repoTitle: p,
+                        pathTitle: g,
                         openReadMeFilesLabel: h
-                    } = p.GitClone;
-                    return (0, b.useEffect)((() => {
+                    } = m.GitClone;
+                    return (0, E.useEffect)((() => {
                         if (e && e.GitCodeRepositories.length >= 0) {
                             const t = [];
                             e.GitCodeRepositories.length > 0 && e.GitCodeRepositories.forEach((e => t.push({
                                 value: e,
                                 label: e
                             }))), u(t)
                         }
-                    }), [e]), w().createElement("div", {
-                        className: me,
+                    }), [e]), f().createElement("div", {
+                        className: ye,
                         "data-testid": "git-clone-container",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab"
-                    }, w().createElement(be, {
+                    }, f().createElement(Ee, {
                         "data-testid": "autocomplete-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Repo-AutoComplete",
-                        label: g,
+                        label: p,
                         options: d,
-                        value: i,
+                        value: o,
                         handleChange: e => {
                             r(e), t(e)
                         },
                         freeSolo: !0
-                    }), w().createElement(pe, {
+                    }), f().createElement(ge, {
                         "data-testid": "text-field-container",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
-                        label: m,
+                        label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            o(e), n(e)
+                            i(e), a(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
-                    }), w().createElement(fe, {
+                    }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), a(e)
+                            c(e), n(e)
                         },
                         checked: l
                     }))
                 };
-            class Se extends f.ReactWidget {
+            class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
                         this.URL = e
                     }, this.setPath = e => {
                         this.path = e
                     }, this.setOpenREADME = e => {
                         this.openREADME = e
                     }, this.getGitRepositories = async () => {
-                        await $("aws/sagemaker/api/git/list-repositories", P.GET).then((e => {
+                        await F("aws/sagemaker/api/git/list-repositories", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this._gitCloneRepositories = e || null, this.update()
                             }))
                         }))
                     }, this.URL = "", this.path = "", this.openREADME = !0, this._gitCloneRepositories = null, this.getGitRepositories()
                 }
                 getValue() {
                     return {
                         URL: this.URL,
                         path: this.path,
                         openREADME: this.openREADME
                     }
                 }
                 render() {
-                    return w().createElement(xe, {
+                    return f().createElement(Ce, {
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Ce = n(9053),
-                Me = n(2190);
+            var Re = a(5962),
+                Te = a(2190);
             const {
-                name: Re,
-                version: Te
-            } = n(4147), je = (e, t, n) => e.child({
-                ExtensionName: Re,
-                ExtensionVersion: Te,
+                name: je,
+                version: ke
+            } = a(4147), De = (e, t, a) => e.child({
+                ExtensionName: je,
+                ExtensionVersion: ke,
                 PluginId: t
-            }, n);
-            var ke;
+            }, a);
+            var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
-            }(ke || (ke = {}));
-            const De = [{
+            }(_e || (_e = {}));
+            const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                _e = async (e, t, n) => {
+                Be = async (e, t, a) => {
                     const {
-                        repoPath: a,
+                        repoPath: n,
                         openREADME: s
-                    } = n;
+                    } = a;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: a
+                            path: n
                         }), !0 === s) try {
-                        await (async (e, t, n) => {
-                            const a = await t.get(e);
-                            if ("directory" === a.type) {
-                                const t = De.find((e => a.content.some((t => t.name === e.name))));
-                                t && await n.execute("docmanager:open", {
-                                    path: z.PathExt.join(e, t.name),
+                        await (async (e, t, a) => {
+                            const n = await t.get(e);
+                            if ("directory" === n.type) {
+                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
+                                t && await a.execute("docmanager:open", {
+                                    path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(a, t, e)
+                        })(n, t, e)
                     } catch (e) {}
-                }, Be = async (e, t) => {
-                    let n;
+                }, Ie = async (e, t) => {
+                    let a;
                     try {
-                        n = await t.get(e)
+                        a = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === n.type
+                    return "directory" === a.type
                 };
-            var Ne = n(1775),
-                Ie = n(248),
-                Ae = n(4337),
-                Le = n(9510);
+            var ze = a(1775),
+                Ae = a(248),
+                Ue = a(4337),
+                Le = a(8625);
             const {
-                dialogTitle: Ue,
+                dialogTitle: Pe,
                 cancelButton: Ge,
-                cloneButton: Pe,
-                errors: ze
-            } = p.GitClone, $e = {
+                cloneButton: $e,
+                errors: Oe
+            } = m.GitClone, Fe = {
                 id: s,
-                requires: [ce.IFileBrowserFactory, ce.IDefaultFileBrowser, Me.IGitExtension, f.IToolbarWidgetRegistry, Ie.ILogger, Ce.ITranslator],
+                requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, n, a, o, i, r) => {
+                activate: async (e, t, a, n, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
-                    } = e, d = c.contents, u = je(i, s), h = (r = r || Ce.nullTranslator).load("sagemaker_studio");
-                    l.addCommand(Ae.TQ.gitClone, {
+                    } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
+                    l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, n, a, s) => {
-                            var o, i;
+                        execute: () => (async (e, t, a, n, s) => {
+                            var i, o;
                             const r = t.model;
                             let l = "";
-                            const c = null === (i = null === (o = null == e ? void 0 : e.tracker) || void 0 === o ? void 0 : o.currentWidget) || void 0 === i ? void 0 : i.model.path;
+                            const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
-                                h = !0,
+                                p = !0,
                                 y = !0;
-                            const v = new f.Dialog({
-                                title: Ue,
-                                body: new Se,
+                            const v = new S.Dialog({
+                                title: Pe,
+                                body: new Me,
                                 focusNodeSelector: "input",
-                                buttons: [f.Dialog.cancelButton({
+                                buttons: [S.Dialog.cancelButton({
                                     label: Ge
-                                }), f.Dialog.okButton({
-                                    label: Pe
+                                }), S.Dialog.okButton({
+                                    label: $e
                                 })],
                                 hasClose: !1
                             });
-                            v.addClass(ge);
+                            v.addClass(he);
                             try {
                                 d = await v.launch()
                             } catch (e) {
                                 return void s.error({
                                     Message: g,
                                     Error: e
                                 })
                             }
                             if (!d.button.accept || !d.value) return;
-                            var b;
+                            var w;
                             if (({
                                     URL: l,
                                     path: u,
-                                    openREADME: h,
+                                    openREADME: p,
                                     findEnvironment: y
-                                } = d.value), "string" == typeof(b = u) && b.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, f.showErrorMessage)(ze.invalidCloneUrlTitle, {
-                                message: ze.invalidCloneUrlBody
+                                } = d.value), "string" == typeof(w = u) && w.length > 0 || (u = "./"), !(e => /^(https:\/\/|git)([:/@.~\-_a-zA-Z0-9])+$/.test(e))(l)) return void await (0, S.showErrorMessage)(Oe.invalidCloneUrlTitle, {
+                                message: Oe.invalidCloneUrlBody
                             });
-                            const w = (e => {
-                                    const t = z.URLExt.parse(e);
-                                    return z.PathExt.basename(t.pathname, ".git")
+                            const b = (e => {
+                                    const t = O.URLExt.parse(e);
+                                    return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
-                                E = z.PathExt.join(u, w);
-                            let x;
+                                E = O.PathExt.join(u, b);
+                            let f;
                             try {
-                                x = await (async (e, t, n, a) => {
+                                f = await (async (e, t, a, n) => {
                                     const {
                                         errors: s
-                                    } = p.GitClone;
-                                    return await Be(t, e) ? await Be(a, e) ? (await (0, f.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + n
-                                    }), ke.AlreadyCloned) : ke.CanClone : (await (0, f.showErrorMessage)(s.directoryNotExistTitle, {
+                                    } = m.GitClone;
+                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + a
+                                    }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
-                                    }), ke.NotExist)
-                                })(n, u, l, E)
+                                    }), _e.NotExist)
+                                })(a, u, l, E)
                             } catch (e) {
                                 s.error({
-                                    Message: m,
+                                    Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
-                            const S = {
+                            const x = {
                                 repoPath: E,
-                                openREADME: h,
+                                openREADME: p,
                                 findEnvironment: y
                             };
-                            x === ke.CanClone ? (async (e, t, n, a, s, o) => {
+                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
                                 const {
-                                    errors: i
-                                } = p.GitClone, r = await e.execute("terminal:create-new");
+                                    errors: o
+                                } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
-                                s && (l += `cd ${s} && `), l += `git clone ${o} && exit\r`;
+                                s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async a => {
-                                        if ("disconnected" === a.connectionStatus) try {
-                                            await _e(e, t, n)
+                                    }), s.session.connectionStatusChanged.connect((async n => {
+                                        if ("disconnected" === n.connectionStatus) try {
+                                            await Be(e, t, a)
                                         } catch (e) {
-                                            await (0, f.showErrorMessage)(i.failedOptions, i.failedOptionsBody, [f.Dialog.warnButton({
+                                            await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await a.refresh()
+                                    })), await n.refresh()
                                 } catch (e) {
-                                    r.dispose(), await (0, f.showErrorMessage)(i.generalCloneErrorTitle, {
-                                        message: i.generalCloneErrorBody + e
+                                    r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
+                                        message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(a, n, S, r, u, l) : x === ke.AlreadyCloned && _e(a, n, S)
-                        })(t, n, d, l, u),
+                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
+                        })(t, a, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
-                    }), o.addFactory("FileBrowser", "gitClone", (() => f.ReactWidget.create(w().createElement(f.UseSignal, {
-                        signal: a.repositoryChanged,
+                    }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
+                        signal: n.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: a.pathRepository
+                            newValue: n.pathRepository
                         }
-                    }, ((t, n) => w().createElement(f.ToolbarButtonComponent, {
-                        enabled: null === (null == n ? void 0 : n.newValue),
+                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == a ? void 0 : a.newValue),
                         icon: Le.W6,
                         onClick: () => {
-                            e.commands.execute(Ae.TQ.gitClone)
+                            e.commands.execute(Ue.TQ.gitClone)
                         },
-                        tooltip: h.__("Git Clone")
-                    })))))), (0, Ne.ZM)(a, n, e.serviceManager.contents, e.contextMenu, h), u.info({
+                        tooltip: p.__("Git Clone")
+                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
-            }, Fe = e => {
-                var t, n;
-                const a = `${e}.AWSSageMakerUI`;
-                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
-            }, Oe = [h, L, le, $e, {
-                id: o,
-                requires: [Ie.ILogger],
+            }, Ve = e => {
+                var t, a;
+                const n = `${e}.AWSSageMakerUI`;
+                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+            }, Ze = {
+                id: i,
+                requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let a = {};
-                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
+                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let n = {};
+                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: n,
+                                requestStart: a,
                                 responseStart: s,
-                                startTime: o
+                                startTime: i
                             } = e;
-                            n && t && (a = {
-                                ...a,
-                                TimeToFirstByteMS: Math.round(s - o)
+                            a && t && (n = {
+                                ...n,
+                                TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
-                            o = null,
                             i = null,
+                            o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
-                        if (c) s = c.redirectCount, o = c.redirectEnd - c.redirectStart, i = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
+                        if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
-                            s = performance.navigation.redirectCount, o = e.redirectEnd - e.redirectStart, i = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
+                            s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        a = {
-                            ...a,
+                        n = {
+                            ...n,
                             RedirectCount: s,
-                            RedirectTimeMS: o,
-                            TimeToDOMContentLoadedMS: i,
+                            RedirectTimeMS: i,
+                            TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(a), t.started.then((() => {
+                        }, e.info(n), t.started.then((() => {
                             e.info({
-                                TimeToAppStartedMS: Math.round(Fe("timeToAppStarted"))
+                                TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (n = Math.round(Fe("timeToAppRestored"))) > 0 ? n : null;
-                            var n;
+                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
+                            var a;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
-                    })(je(t, o, Ie.logSchemas.performance), e)
+                    })(De(t, i, Ae.logSchemas.performance), e)
+                }
+            };
+            var We = a(87),
+                He = a(8201);
+            const qe = {
+                    SpaceMenuHeader: V.css`
+  margin: -6px 0;
+  padding: 0 var(--jp-size-2);
+  height: 10;
+  border-radius: var(--jp-radius-small);
+  font-size: var(--jp-size-3);
+  display: flex;
+  justify-content: center;
+  align-items: center;
+
+  & > p {
+    display: inline-block;
+    user-select: none;
+    color: var(--jp-color-root-light-800);
+  }
+
+  & > svg {
+    padding: 0 var(--jp-size-2);
+  }
+`
+                },
+                {
+                    privateSpaceHeader: Je,
+                    unknownUser: Ye
+                } = m.Space,
+                Qe = ({
+                    spaceName: e
+                }) => {
+                    const t = !!e,
+                        a = R("studioUserProfileName");
+                    return f().createElement("div", {
+                        className: qe.SpaceMenuHeader,
+                        "data-testid": y
+                    }, t ? f().createElement(We.Z, {
+                        fontSize: "small"
+                    }) : f().createElement(He.Z, {
+                        fontSize: "small"
+                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                };
+            class Ke extends S.ReactWidget {
+                constructor() {
+                    super(), this.getSpaceName = async () => {
+                        await F("aws/sagemaker/api/context", $.GET).then((e => {
+                            e && e.json().then((e => {
+                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                            }))
+                        }))
+                    }, this.spaceName = "", this.getSpaceName()
+                }
+                render() {
+                    return f().createElement(Qe, {
+                        spaceName: this.spaceName
+                    })
+                }
+            }
+            const Xe = [v, L, de, Fe, Ze, {
+                id: o,
+                requires: [Ae.ILogger],
+                autoStart: !0,
+                activate: async (e, t) => {
+                    const a = new Ke;
+                    a.id = S.DOMUtils.createDomID();
+                    const n = De(t, o);
+                    e.shell.add(a, "top", {
+                        rank: 1e3
+                    }), window && window.panorama && window.panorama("trackCustomEvent", {
+                        eventType: "render",
+                        eventDetail: "Space-Plugin",
+                        eventContext: "JupyterLab",
+                        timestamp: Date.now()
+                    }), n.info({
+                        Message: "Successfully loaded Space plugin"
+                    })
                 }
             }]
         },
+        8201: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
+                }), "AccountCircle");
+            t.Z = o
+        },
+        87: (e, t, a) => {
+            var n = a(5318);
+            t.Z = void 0;
+            var s = n(a(4938)),
+                i = a(5893),
+                o = (0, s.default)((0, i.jsx)("path", {
+                    d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
+                }), "Language");
+            t.Z = o
+        },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.2.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(8962),
+                Ds = o(7651),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -14,35 +14,35 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(7308),
-                s = i(7807),
-                r = i(7749),
-                o = i(4085),
+            var n = i(9510),
+                s = i(3471),
+                r = i(6311),
+                o = i(3452),
                 a = i(6697),
                 l = i(7930),
-                c = i(8778),
+                c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
                     super(...e), this.name = "CancelledError"
                 }
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(9510),
+                v = i(8625),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1757,15 +1757,15 @@
                     width: "100%"
                 }),
                 m = (0, s.oB)({
                     display: "flex",
                     marginLeft: "auto",
                     overflow: "hidden"
                 });
-            var _, y = i(2688),
+            var _, y = i(4387),
                 v = i(7320);
             class b extends n.PureComponent {
                 constructor() {
                     super(...arguments), this._onDoubleClick = e => {
                         e.stopPropagation()
                     }
                 }
@@ -1854,16 +1854,16 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(7308),
-                s = i(8778),
+            var n = i(9510),
+                s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
             const h = a.clearTimeout,
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(9510),
+            var v = i(8625),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(4085),
+                C = i(3452),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,17 +2703,17 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(4085),
+            var n = i(3452),
                 s = i(6029),
-                r = i(2688),
+                r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
                     l = (null === (t = e.filetype) || void 0 === t ? void 0 : t.icon) || n.fileIcon;
                 return s.createElement(s.Fragment, null, s.createElement(l.react, {
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(7308),
+            var n = i(9510),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,19 +3180,19 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(7807),
-                s = i(7454),
-                r = i(9053),
+            var n = i(3471),
+                s = i(7777),
+                r = i(5962),
                 o = i(7930),
-                a = i(8778),
+                a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
                 editorFactory: e,
                 languageRegistry: t,
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(7749),
-                s = i(125),
+            var n = i(6311),
+                s = i(7217),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(7749),
-                r = i(7527),
+            var n, s = i(6311),
+                r = i(1638),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4499,15 +4499,15 @@
                         },
                         t = `&:hover .${r}`;
                     return e.$nest[t] = {
                         display: "block"
                     }, e
                 })()
         },
-        2688: (e, t, i) => {
+        4387: (e, t, i) => {
             "use strict";
             i.d(t, {
                 cf: () => s,
                 gW: () => o,
                 ge: () => r
             });
             var n = i(9946);
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        9510: (e, t, i) => {
+        8625: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(4085);
+            var n = i(3452);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(125);
+            var n = i(7217);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(7749),
+            var n = i(6311),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(7308);
+            var n = i(9510);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(9053),
-                o = i(8778),
+                r = i(5962),
+                o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(7807),
-                f = i(7454);
+                u = i(3471),
+                f = i(7777);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(7932),
+            var n = i(6963),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,36 @@
-/*! For license information please see 891.ada29ec8d5578292aa74.js.LICENSE.txt */
+/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(3205),
-                r = s(7308),
-                a = s(7807),
-                o = s(1165),
-                n = s(2419),
-                l = s(5409),
-                d = s(9499),
-                c = s(8190),
-                h = s(667),
-                p = s(9053),
+            var i = s(8368),
+                r = s(9510),
+                a = s(3471),
+                o = s(5326),
+                n = s(8031),
+                l = s(9557),
+                d = s(8048),
+                c = s(4008),
+                h = s(4613),
+                p = s(5962),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(9510),
+                f = s(8625),
                 _ = s(4337),
-                b = s(8778);
+                b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
                 }
                 getValue() {
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(7932),
+                it = s(6963),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(5390);
+            var _t = s(1778);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(7749),
-                us = s(125);
+                ms = s(6311),
+                us = s(7217);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(4085),
+            var Ss = s(3452),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7454),
+            var Rr = s(7777),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, d, u, f, c, s, p, m, b, h, v, g, y, j, w, P, k = {
-            9110: (e, r, t) => {
+    var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
+            1514: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(445), t.e(779)]).then((() => () => t(4779))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -48,61 +48,61 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "9a0cdfa414e5cba3947c",
+        181: "2135a6297693b09662d9",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
-        445: "541fc908d081ce33a2a9",
         505: "36ee543eaffaebaab59c",
+        548: "5350b743f9a235d9e265",
+        571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
-        779: "3a4f00c583226dabc471",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "e93d309a2347b726b4c9",
+        799: "c508feab9dfdf7494214",
         800: "61e818e75a1cec06f3f1",
-        823: "c3c95a37373ea011ffb4",
+        823: "7f061638d47075ac76be",
+        853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
-        875: "78afc4b132e6a8796ce9",
-        891: "ada29ec8d5578292aa74"
+        891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.2.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(445), S.e(779)]).then((() => () => S(4779))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(445), S.e(875)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -234,98 +234,98 @@
                 } else {
                     if (i <= a || f < c != n) return !1;
                     d = !1
                 } else "s" != c && "n" != c && (d = !1, i--)
             }
         }
         var s = [],
-            p = s.pop.bind(s);
+            b = s.pop.bind(s);
         for (l = 1; l < e.length; l++) {
-            var m = e[l];
-            s.push(1 == m ? p() | p() : 2 == m ? p() & p() : m ? o(m, r) : !p())
+            var p = e[l];
+            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
         }
-        return !!p()
+        return !!b()
     }, l = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = d(e, t);
-        return o(a, n) || p(u(e, t, n, a)), b(e[t][n])
+        return o(a, n) || b(u(e, t, n, a)), m(e[t][n])
     }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, p = e => {
+    }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, m = (e, r, t, a) => {
-        p(s(e, r, t, a))
-    }, b = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
+    }, p = (e, r, t, a) => {
+        b(s(e, r, t, a))
+    }, m = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => (l(e, t), b(c(r, t, a) || m(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
+    })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
-        return o ? b(o) : n()
+        return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
-        125: () => g("default", "@jupyterlab/services", [1, 7, 0, 9]),
-        667: () => g("default", "@jupyterlab/statusbar", [1, 4, 0, 9]),
-        1165: () => g("default", "@jupyterlab/docmanager", [1, 4, 0, 9]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        2419: () => g("default", "@jupyterlab/filebrowser", [1, 4, 0, 9]),
-        3205: () => g("default", "@jupyterlab/application", [1, 4, 0, 9]),
-        4085: () => g("default", "@jupyterlab/ui-components", [1, 4, 0, 9]),
+        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
+        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
+        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5409: () => g("default", "@jupyterlab/mainmenu", [1, 4, 0, 9]),
+        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
+        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
+        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        7308: () => g("default", "@jupyterlab/apputils", [1, 4, 1, 9]),
-        7454: () => g("default", "@jupyterlab/codemirror", [1, 4, 0, 9]),
-        7527: () => v("default", "@jupyterlab/docregistry", [1, 4, 0, 9]),
-        7749: () => g("default", "@jupyterlab/coreutils", [1, 6, 0, 9]),
-        7807: () => g("default", "@jupyterlab/codeeditor", [1, 4, 0, 9]),
+        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
+        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
+        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        7932: () => v("default", "@jupyterlab/nbformat", [1, 4, 0, 9]),
+        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8778: () => g("default", "@lumino/widgets", [1, 2, 0, 1]),
-        9053: () => g("default", "@jupyterlab/translation", [1, 4, 0, 9]),
+        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
+        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(875)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
+        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
+        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
-        5390: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 9]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8190: () => g("default", "@jupyterlab/settingregistry", [1, 4, 0, 9]),
-        9499: () => g("default", "@jupyterlab/rendermime", [1, 4, 0, 9]),
+        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
-        445: [125, 667, 1165, 1373, 2419, 3205, 4085, 4901, 5409, 6211, 6697, 6797, 7308, 7454, 7527, 7749, 7807, 7930, 7932, 8093, 8204, 8778, 9053],
+        548: [248, 2190, 5933, 9801],
+        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
-        779: [248, 2190, 5933, 9801],
         798: [851, 7138],
         800: [8800],
-        875: [5359, 5390, 5633, 7350, 7489, 7858, 8190, 9499]
+        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|445|704|798|800|875)$/.test(r)) e[r] = 0;
+                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(9110);
+    var E = S(1514);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_error_util.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_handlers.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.2.0"
+    assert data["Context"]["ExtensionVersion"] == "0.3.0"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/error_util.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension/utils/request_logger.py` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/request_logger.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.2.0
+Version: 0.3.0
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt` & `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 THIRD-PARTY-LICENSES
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
-public_dist/sagemaker_jupyterlab_extension-0.2.0-py3-none-any.whl
+public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl
 sagemaker_jupyterlab_extension/__init__.py
 sagemaker_jupyterlab_extension/_version.py
 sagemaker_jupyterlab_extension/handlers.py
 sagemaker_jupyterlab_extension.egg-info/PKG-INFO
 sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
 sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
 sagemaker_jupyterlab_extension.egg-info/not-zip-safe
 sagemaker_jupyterlab_extension.egg-info/requires.txt
 sagemaker_jupyterlab_extension.egg-info/top_level.txt
 sagemaker_jupyterlab_extension/labextension/package.json
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
-sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
+sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
+sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
-sagemaker_jupyterlab_extension/labextension/static/779.3a4f00c583226dabc471.js
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
-sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
-sagemaker_jupyterlab_extension/labextension/static/823.c3c95a37373ea011ffb4.js
+sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
+sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
-sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js
-sagemaker_jupyterlab_extension/labextension/static/891.ada29ec8d5578292aa74.js.LICENSE.txt
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.e8f2ffedbb22ee676b66.js
+sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
+sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
 sagemaker_jupyterlab_extension/labextension/static/style.js
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 sagemaker_jupyterlab_extension/tests/__init__.py
 sagemaker_jupyterlab_extension/tests/helper.py
 sagemaker_jupyterlab_extension/tests/test_error_util.py
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 sagemaker_jupyterlab_extension/tests/test_handlers.py
@@ -56,56 +56,64 @@
 sagemaker_jupyterlab_extension/utils/git_clone_util.py
 sagemaker_jupyterlab_extension/utils/metric_util.py
 sagemaker_jupyterlab_extension/utils/request_logger.py
 src/index.ts
 src/__mocks__/fileMock.ts
 src/components/GitCloneComponent.tsx
 src/components/ResourceUsageComponent.tsx
+src/components/SpaceMenu.tsx
 src/components/__tests__/AutoComplete.spec.tsx
 src/components/__tests__/CheckboxComponent.spec.tsx
 src/components/__tests__/GitCloneComponent.spec.tsx
 src/components/__tests__/InputField.spec.tsx
 src/components/__tests__/LinearProgressWithLabel.spec.tsx
 src/components/__tests__/ResourceUsageComponent.spec.tsx
+src/components/__tests__/SpaceMenu.spec.tsx
 src/components/common/AutoComplete.tsx
 src/components/common/CheckboxComponent.tsx
 src/components/common/InputField.tsx
 src/components/common/LinearProgressWithLabel.tsx
 src/components/styles/InputFieldStyles.ts
+src/components/styles/SpaceMenuStyles.ts
 src/components/styles/autoCompleteStyles.ts
 src/constants/common.ts
 src/constants/errorMessages.ts
 src/constants/gitCloneConstants.ts
 src/constants/il18Strings.ts
 src/constants/index.ts
 src/constants/resourceUsageConstants.ts
 src/constants/sessionManagementConstants.ts
+src/constants/spaceMenuConstants.ts
 src/plugins/GitClonePlugin.tsx
 src/plugins/HideShutDownPlugin.ts
 src/plugins/ResourceUsagePlugin.ts
 src/plugins/SessionManagementPlugin.ts
+src/plugins/SpaceMenuPlugin.tsx
 src/plugins/index.ts
 src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
 src/plugins/PerformancePlugin/index.ts
 src/plugins/PerformancePlugin/utils.ts
 src/plugins/__tests__/GitClonePlugin.spec.ts
 src/plugins/__tests__/HideShutDownPlugin.spec.ts
 src/plugins/__tests__/ResourceUsagePlugin.spec.ts
 src/plugins/__tests__/SessionManagementPlugin.spec.ts
+src/plugins/__tests__/SpaceMenuPlugin.spec.ts
 src/service/constants.ts
 src/service/index.ts
 src/service/__tests__/index.spec.ts
 src/service/__tests__/mock.ts
 src/style/common.css
 src/style/index.css
 src/utils/ReactWidgetWrapper.tsx
 src/utils/gitCloneUtils.ts
 src/utils/logger.ts
 src/utils/sessionManagerUtils.tsx
 src/utils/__tests__/gitCloneUtils.spec.ts
 src/utils/__tests__/sessionManagerUtils.spec.tsx
 src/widgets/GitCloneWidget.tsx
 src/widgets/ResourceUsageWidget.tsx
+src/widgets/SpaceMenuWidget.tsx
 src/widgets/__tests__/GitCloneWidget.spec.tsx
 src/widgets/__tests__/ResourceUsageWidget.spec.tsx
+src/widgets/__tests__/SpaceMenuWidget.spec.tsx
 src/widgets/styles/gitCloneStyles.ts
 src/widgets/styles/resourceUsageStyle.ts
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/setup.py` & `sagemaker-jupyterlab-extension-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 sagemaker_jupyterlab_extension setup
 """
+
 import os
 import json
 import setuptools
 from pathlib import Path
 
 from jupyter_packaging import (
     create_cmdclass,
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/GitCloneComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/GitCloneComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/ResourceUsageComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/ResourceUsageComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/AutoComplete.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/AutoComplete.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/CheckboxComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/CheckboxComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/GitCloneComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/GitCloneComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/InputField.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/InputField.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/__tests__/ResourceUsageComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/ResourceUsageComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/common/AutoComplete.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/common/AutoComplete.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/common/CheckboxComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/common/CheckboxComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/common/InputField.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/common/InputField.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/common/LinearProgressWithLabel.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/components/common/LinearProgressWithLabel.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/components/styles/InputFieldStyles.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/components/styles/InputFieldStyles.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/constants/common.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/constants/common.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 const pluginIds = {
   ExamplePlugin: '@amzn/sagemaker-jupyterlab-extensions:example',
   HideShutDownPlugin: '@amzn/sagemaker-jupyterlab-extensions:hideshutdown',
   SessionManagementPlugin: '@amzn/sagemaker-jupyterlab-extensions:sessionmanagement',
   ResourceUsagePlugin: '@amzn/sagemaker-jupyterlab-extensions:resourceusage',
   GitClonePlugin: '@amzn/sagemaker-jupyterlab-extensions:gitclone',
   PerformanceMeteringPlugin: '@amzn/sagemaker-jupyterlab-extensions:performance-metering',
+  SpaceMenuPlugin: '@amzn/sagemaker-jupyterlab-extensions:spacemenu',
 };
 
 const JUPYTER_COMMAND_IDS = {
   mainMenu: {
     fileMenu: {
       shutdown: 'filemenu:shutdown',
     },
   },
   createTerminal: 'terminal:create-new',
   openDocManager: 'docmanager:open',
   goToPath: 'filebrowser:go-to-path',
 };
 
 const RESOURCE_PLUGIN_ID = '@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget';
+const SPACE_MENU_PLUGIN_ID = '@amzn/sagemaker-jupyterlab-extensions:spacemenu:space-menu-widget';
 
 const i18nStrings = {};
 
-export { pluginIds, i18nStrings, JUPYTER_COMMAND_IDS, RESOURCE_PLUGIN_ID };
+const COOKIE_NAMES = {
+  USER_PROFILE_NAME: 'studioUserProfileName',
+};
+
+export { pluginIds, i18nStrings, JUPYTER_COMMAND_IDS, RESOURCE_PLUGIN_ID, COOKIE_NAMES, SPACE_MENU_PLUGIN_ID };
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/constants/il18Strings.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/constants/il18Strings.ts`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,12 @@
         'Something went wrong when trying to clone the repository to your project. Please try again later. ',
       failedOptions: 'Failed to handle additional options.',
       failedOptionsBody: 'Something went wrong when trying to open README file within the repo.',
       invalidCloneUrlTitle: 'Invalid URL provided',
       invalidCloneUrlBody: 'The URL provided is not valid. Please input a valid URL to clone.',
     },
   },
+  Space: {
+    privateSpaceHeader: 'Personal Studio',
+    unknownUser: 'Unknown User',
+  },
 };
```

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/constants/resourceUsageConstants.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/constants/resourceUsageConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/constants/sessionManagementConstants.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/constants/sessionManagementConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/GitClonePlugin.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/GitClonePlugin.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/HideShutDownPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/HideShutDownPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/PerformancePlugin/utils.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/utils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/ResourceUsagePlugin.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/ResourceUsagePlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/SessionManagementPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/SessionManagementPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/GitClonePlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/GitClonePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/service/__tests__/index.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/service/__tests__/mock.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/mock.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/service/index.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/service/index.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/utils/ReactWidgetWrapper.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/utils/ReactWidgetWrapper.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/utils/__tests__/gitCloneUtils.spec.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/gitCloneUtils.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/utils/__tests__/sessionManagerUtils.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/sessionManagerUtils.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/utils/gitCloneUtils.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/utils/gitCloneUtils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/utils/sessionManagerUtils.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/utils/sessionManagerUtils.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/widgets/GitCloneWidget.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/widgets/GitCloneWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/widgets/ResourceUsageWidget.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/widgets/ResourceUsageWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/widgets/__tests__/GitCloneWidget.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/GitCloneWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/src/widgets/styles/resourceUsageStyle.ts` & `sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/resourceUsageStyle.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.2.0/tsconfig.json` & `sagemaker-jupyterlab-extension-0.3.0/tsconfig.json`

 * *Files identical despite different names*

