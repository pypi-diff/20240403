# Comparing `tmp/pwb_jupyterlab-0.2.4.tar.gz` & `tmp/pwb_jupyterlab-1.0.16.tar.gz`

## Comparing `pwb_jupyterlab-0.2.4.tar` & `pwb_jupyterlab-1.0.16.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/.yarnrc.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/babel.config.js
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/configure.mjs
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/conftest.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/install.json
--rw-r--r--   0        0        0   716933 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/package-lock.json
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/package.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/tsconfig.test.json
--rw-r--r--   0        0        0   501561 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/yarn.lock
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/images/posit-icon-fullcolor.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/images/posit-icon-unstyled.svg
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/jupyter-config/server-config/pwb_jupyterlab.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/jupyter-config/server-config/workbench_jupyterlab.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/.gitignore
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/_version.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/constants.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/handlers.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/network.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/process.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/proxiedServersProvider.py
--rw-r--r--   0        0        0    23012 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/build_log.json
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/package.json.orig
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/plugin.json
--rw-r--r--   0        0        0    34150 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js
--rw-r--r--   0        0        0    34975 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js.map
--rw-r--r--   0        0        0    29030 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/remoteEntry.ce8a05ff7585e16c9421.js
--rw-r--r--   0        0        0    27732 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/remoteEntry.ce8a05ff7585e16c9421.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0    22646 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js
--rw-r--r--   0        0        0    19029 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js.map
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/__init__.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/test_handlers.py
--rw-r--r--   0        0        0    21210 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/test_network.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/resources/.gitignore
--rwxr-xr-x   0        0        0    44075 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/resources/basics-jupyter.ipynb
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/resources/hello.qmd
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/schema/plugin.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/constants.ts
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/disconnectAlert.tsx
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/disconnectMonitor.ts
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/handler.ts
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/index.ts
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/proxiedServersComponent.tsx
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/svg.d.ts
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/src/widget.tsx
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/style/index.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/.gitignore
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/global-setup.ts
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/package.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/playwright.config.ts
--rw-r--r--   0        0        0   148176 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/yarn.lock
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/helpers/command-palette.ts
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/helpers/selectors.ts
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/helpers/terminal.ts
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/resources/.gitignore
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/resources/app.R
--rwxr-xr-x   0        0        0    44075 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/resources/basics-jupyter.ipynb
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/resources/hello.qmd
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/tests/posit-side-bar.spec.ts
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-quarto-notebook.spec.ts
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-quarto-server.spec.ts
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-shiny-server.spec.ts
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/ui-tests/tests/workbench-home.spec.ts
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/.gitignore
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/README.md
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pwb_jupyterlab-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/.yarnrc.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/babel.config.js
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/configure.mjs
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/conftest.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/install.json
+-rw-r--r--   0        0        0   716933 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/package-lock.json
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/package.json
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/tsconfig.test.json
+-rw-r--r--   0        0        0   501561 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/yarn.lock
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/images/posit-icon-fullcolor.svg
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/images/posit-icon-unstyled.svg
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/jupyter-config/server-config/pwb_jupyterlab.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/jupyter-config/server-config/workbench_jupyterlab.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/.gitignore
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/_version.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/constants.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/handlers.py
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/network.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/process.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/proxiedServersProvider.py
+-rw-r--r--   0        0        0    22783 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/build_log.json
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/package.json.orig
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/plugin.json
+-rw-r--r--   0        0        0    34150 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js
+-rw-r--r--   0        0        0    34975 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js.map
+-rw-r--r--   0        0        0    29031 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/remoteEntry.bfa8345edda3e3e864e0.js
+-rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/remoteEntry.bfa8345edda3e3e864e0.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0    22646 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js
+-rw-r--r--   0        0        0    19029 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js.map
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/__init__.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/test_handlers.py
+-rw-r--r--   0        0        0    21210 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/test_network.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/resources/.gitignore
+-rwxr-xr-x   0        0        0    44075 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/resources/basics-jupyter.ipynb
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/resources/hello.qmd
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/schema/plugin.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/constants.ts
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/disconnectAlert.tsx
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/disconnectMonitor.ts
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/handler.ts
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/index.ts
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/proxiedServersComponent.tsx
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/svg.d.ts
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/src/widget.tsx
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/style/index.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/.gitignore
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/global-setup.ts
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/package.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/playwright.config.ts
+-rw-r--r--   0        0        0   148176 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/helpers/command-palette.ts
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/helpers/selectors.ts
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/helpers/terminal.ts
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/resources/.gitignore
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/resources/app.R
+-rwxr-xr-x   0        0        0    44075 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/resources/basics-jupyter.ipynb
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/resources/hello.qmd
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/tests/posit-side-bar.spec.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-quarto-notebook.spec.ts
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-quarto-server.spec.ts
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-shiny-server.spec.ts
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/ui-tests/tests/workbench-home.spec.ts
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/.gitignore
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/README.md
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/pyproject.toml
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 pwb_jupyterlab-1.0.16/PKG-INFO
```

### Comparing `pwb_jupyterlab-0.2.4/configure.mjs` & `pwb_jupyterlab-1.0.16/configure.mjs`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/conftest.py` & `pwb_jupyterlab-1.0.16/conftest.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/package-lock.json` & `pwb_jupyterlab-1.0.16/package-lock.json`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/package.json` & `pwb_jupyterlab-1.0.16/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'1.0.16'"}*

```diff
@@ -223,9 +223,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "1.0.16"
 }
```

### Comparing `pwb_jupyterlab-0.2.4/tsconfig.json` & `pwb_jupyterlab-1.0.16/tsconfig.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'compilerOptions'": "{delete: ['skipLibCheck']}"}*

```diff
@@ -11,15 +11,14 @@
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
-        "skipLibCheck": true,
         "strict": false,
         "strictNullChecks": true,
         "target": "ES2018",
         "types": [
             "node"
         ]
     },
```

### Comparing `pwb_jupyterlab-0.2.4/yarn.lock` & `pwb_jupyterlab-1.0.16/yarn.lock`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/images/posit-icon-fullcolor.svg` & `pwb_jupyterlab-1.0.16/images/posit-icon-fullcolor.svg`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/images/posit-icon-unstyled.svg` & `pwb_jupyterlab-1.0.16/images/posit-icon-unstyled.svg`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/__init__.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/constants.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/constants.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/handlers.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/handlers.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/network.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/network.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/process.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/process.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/proxiedServersProvider.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/proxiedServersProvider.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/build_log.json` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/build_log.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9862799600009148%*

 * *Differences: {'0': "{'module': {'rules': {1: {'use': "*

 * *      "['/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/style-loader/dist/cjs.js', "*

 * *      "'/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/css-loader/dist/cjs.js']}, "*

 * *      "16: {'use': "*

 * *      "['/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/@jupyterlab/bu […]*

```diff
@@ -9,16 +9,16 @@
                 {
                     "test": "/\\.raw\\.css$/",
                     "type": "asset/source"
                 },
                 {
                     "test": "/(?<!\\.raw)\\.css$/",
                     "use": [
-                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/style-loader/dist/cjs.js",
-                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/css-loader/dist/cjs.js"
+                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/style-loader/dist/cjs.js",
+                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/css-loader/dist/cjs.js"
                     ]
                 },
                 {
                     "test": "/\\.txt$/",
                     "type": "asset/source"
                 },
                 {
@@ -80,37 +80,37 @@
                     "test": "/\\.html$/",
                     "type": "asset/resource"
                 },
                 {
                     "enforce": "pre",
                     "test": "/\\.js$/",
                     "use": [
-                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/@jupyterlab/builder/node_modules/source-map-loader/dist/cjs.js"
+                        "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/@jupyterlab/builder/node_modules/source-map-loader/dist/cjs.js"
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/pwb_jupyterlab/labextension/static",
+            "path": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/pwb_jupyterlab/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
-                        "./index": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
-                        "./style": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/style/index.js"
+                        "./extension": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
+                        "./index": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
+                        "./style": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "pwb_jupyterlab"
                         ],
@@ -146,430 +146,430 @@
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^1.1.1",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.2.4",
+                            "requiredVersion": "^4.2.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/buildutils": {},
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.1.4",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mermaid": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mermaid-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.1.4"
+                            "requiredVersion": "^5.1.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pluginmanager": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/pluginmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.9.4",
+                            "requiredVersion": "^3.9.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.1.4",
+                            "requiredVersion": "^7.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.1.4",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.1.4"
+                            "requiredVersion": "^6.1.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.1.4",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.1.4"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -661,17 +661,17 @@
                             "import": false,
                             "requiredVersion": "^2.49.2",
                             "singleton": true
                         },
                         "ip": {},
                         "npm": {},
                         "pwb_jupyterlab": {
-                            "import": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
+                            "import": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/lib/index.js",
                             "singleton": true,
-                            "version": "0.2.4"
+                            "version": "1.0.16"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
@@ -689,16 +689,16 @@
             },
             {}
         ],
         "resolve": {
             "fallback": {
                 "buffer": false,
                 "crypto": false,
-                "path": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/path-browserify/index.js",
-                "process": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab-test/feature%2Fpwb-jlab-gha/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/process/browser.js",
+                "path": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/path-browserify/index.js",
+                "process": "/var/lib/jenkins/workspace/IDE/pwb-jupyterlab/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/package.json` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.980448717948718%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.bfa8345edda3e3e864e0.js'}}",*

 * * "'version'": "'1.0.16'"}*

```diff
@@ -126,15 +126,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ce8a05ff7585e16c9421.js",
+            "load": "static/remoteEntry.bfa8345edda3e3e864e0.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "pwb_jupyterlab"
                 },
@@ -228,9 +228,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "1.0.16"
 }
```

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/package.json.orig` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/schemas/pwb_jupyterlab/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'1.0.16'"}*

```diff
@@ -223,9 +223,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "1.0.16"
 }
```

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js.map` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/lib_index_js.9a18123aec885513160b.js.map`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/remoteEntry.ce8a05ff7585e16c9421.js` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/remoteEntry.bfa8345edda3e3e864e0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -427,15 +427,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("pwb_jupyterlab", "0.2.4", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("pwb_jupyterlab", "1.0.16", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -828,23 +828,23 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 1, 4])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 1, 4])),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 1, 5])),
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 18, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 4])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 4])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 5])),
             /******/
             "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 2, 0, 0])),
             /******/
             "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])),
             /******/
             "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 18, 2, 0]))
             /******/
@@ -1108,8 +1108,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/pwb_jupyterlab");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).pwb_jupyterlab = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.ce8a05ff7585e16c9421.js.map
+//# sourceMappingURL=remoteEntry.bfa8345edda3e3e864e0.js.map
```

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/remoteEntry.ce8a05ff7585e16c9421.js.map` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/remoteEntry.bfa8345edda3e3e864e0.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.bfa8345edda3e3e864e0.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.ce8a05ff7585e16c9421.js",
+    "file": "remoteEntry.bfa8345edda3e3e864e0.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WC5LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://pwb_jupyterlab/webpack/container-entry",
         "webpack://pwb_jupyterlab/webpack/bootstrap",
         "webpack://pwb_jupyterlab/webpack/runtime/compat get default export",
@@ -30,17 +30,17 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"9a18123aec885513160b\",\"style_index_js\":\"6ff6ba1bc54f497e4f17\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"pwb_jupyterlab:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"pwb_jupyterlab\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"pwb_jupyterlab\", \"0.2.4\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"pwb_jupyterlab\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"pwb_jupyterlab\", \"1.0.16\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,4])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,4])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,4])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,18,2,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,5])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,5])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,18,2,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"pwb_jupyterlab\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkpwb_jupyterlab\"] = self[\"webpackChunkpwb_jupyterlab\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/pwb_jupyterlab\");\n",
         ""
     ],
     "version": 3
```

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js.map` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/labextension/static/style_index_js.6ff6ba1bc54f497e4f17.js.map`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/test_handlers.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/test_network.py` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pwb_jupyterlab/tests/resources/basics-jupyter.ipynb` & `pwb_jupyterlab-1.0.16/pwb_jupyterlab/tests/resources/basics-jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/disconnectAlert.tsx` & `pwb_jupyterlab-1.0.16/src/disconnectAlert.tsx`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/disconnectMonitor.ts` & `pwb_jupyterlab-1.0.16/src/disconnectMonitor.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/handler.ts` & `pwb_jupyterlab-1.0.16/src/handler.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/index.ts` & `pwb_jupyterlab-1.0.16/src/index.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/proxiedServersComponent.tsx` & `pwb_jupyterlab-1.0.16/src/proxiedServersComponent.tsx`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/src/widget.tsx` & `pwb_jupyterlab-1.0.16/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/style/base.css` & `pwb_jupyterlab-1.0.16/style/base.css`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/global-setup.ts` & `pwb_jupyterlab-1.0.16/ui-tests/global-setup.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/yarn.lock` & `pwb_jupyterlab-1.0.16/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/helpers/command-palette.ts` & `pwb_jupyterlab-1.0.16/ui-tests/helpers/command-palette.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/helpers/selectors.ts` & `pwb_jupyterlab-1.0.16/ui-tests/helpers/selectors.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/resources/app.R` & `pwb_jupyterlab-1.0.16/ui-tests/resources/app.R`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/resources/basics-jupyter.ipynb` & `pwb_jupyterlab-1.0.16/ui-tests/resources/basics-jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/tests/posit-side-bar.spec.ts` & `pwb_jupyterlab-1.0.16/ui-tests/tests/posit-side-bar.spec.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-quarto-notebook.spec.ts` & `pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-quarto-notebook.spec.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-quarto-server.spec.ts` & `pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-quarto-server.spec.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/tests/proxy-shiny-server.spec.ts` & `pwb_jupyterlab-1.0.16/ui-tests/tests/proxy-shiny-server.spec.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/ui-tests/tests/workbench-home.spec.ts` & `pwb_jupyterlab-1.0.16/ui-tests/tests/workbench-home.spec.ts`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/.gitignore` & `pwb_jupyterlab-1.0.16/.gitignore`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/README.md` & `pwb_jupyterlab-1.0.16/README.md`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/pyproject.toml` & `pwb_jupyterlab-1.0.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pwb_jupyterlab-0.2.4/PKG-INFO` & `pwb_jupyterlab-1.0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pwb_jupyterlab
-Version: 0.2.4
+Version: 1.0.16
+Dynamic: Keywords
 Summary: Enhance experience of running JupyterLab 4 in Posit Workbench.
 Project-URL: Homepage, https://docs.posit.co/ide/server-pro/user/jupyter-lab/guide/posit-workbench-extension.html
 Project-URL: Repository, https://github.com/rstudio/rstudio-pro/tree/main/src/cpp/session/workspaces/pwb-jupyterlab/extensions
 Author: Posit Software, PBC
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
```

