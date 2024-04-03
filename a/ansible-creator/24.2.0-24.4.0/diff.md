# Comparing `tmp/ansible-creator-24.2.0.tar.gz` & `tmp/ansible-creator-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-creator-24.2.0.tar", last modified: Wed Feb  7 15:30:16 2024, max compression
+gzip compressed data, was "ansible-creator-24.4.0.tar", last modified: Wed Apr  3 13:14:51 2024, max compression
```

## Comparing `ansible-creator-24.2.0.tar` & `ansible-creator-24.4.0.tar`

### file list

```diff
@@ -1,234 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.830023 ansible-creator-24.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.790024 ansible-creator-24.2.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.790024 ansible-creator-24.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.790024 ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.790024 ansible-creator-24.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.794024 ansible-creator-24.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.794024 ansible-creator-24.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/collection_creation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/installing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.806024 ansible-creator-24.2.0/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)  2113880 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/media/log-to-file.gif
--rw-r--r--   0 runner    (1001) docker     (127)  3211387 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/media/open-collection.gif
--rw-r--r--   0 runner    (1001) docker     (127)  2769642 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/media/open-folder.gif
--rw-r--r--   0 runner    (1001) docker     (127)  3250683 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/media/open-log-file.gif
--rw-r--r--   0 runner    (1001) docker     (127)   297010 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/docs/media/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 15:30:16.830023 ansible-creator-24.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.778024 ansible-creator-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.810024 ansible-creator-24.2.0/src/ansible_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.778024 ansible-creator-24.2.0/src/ansible_creator/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.778024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.github/workflows/release.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.github/workflows/test.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.isort.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.prettierignore.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/CONTRIBUTING
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/LICENSE.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/changelogs/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/changelogs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/docs/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/docs/docsite/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/docs/docsite/links.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/eda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/rulebook.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/molecule.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/converge.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/noop.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/vars.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/galaxy.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/action/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.814024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/cache/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/filter/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/filter/hello_world.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/inventory/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/module_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/module_utils/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/modules/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/plugin_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/plugin_utils/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/sub_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/sub_plugins/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/plugins/test/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/targets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/main.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/integration/test_integration.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tests/unit/.keep
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/tox-ansible.ini.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/src/ansible_creator/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/subcommands/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/templar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/src/ansible_creator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/src/ansible_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 15:30:16.000000 ansible-creator-24.2.0/src/ansible_creator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.818024 ansible-creator-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/tests/fixtures/collection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.prettierignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/CONTRIBUTING
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/changelogs/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/docs/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/docs/docsite/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.782024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/eda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/rulebook.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/noop.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/vars.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/action/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.822023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/filter/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/inventory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/module_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/module_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.786024 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tests/unit/.keep
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/integration/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 15:30:16.826023 ansible-creator-24.2.0/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/units/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tests/units/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-07 15:30:03.000000 ansible-creator-24.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.700425 ansible-creator-24.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/collection_creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/installing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.716425 ansible-creator-24.4.0/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)  2113880 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/media/log-to-file.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  3211387 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/media/open-collection.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  2769642 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/media/open-folder.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  3250683 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/media/open-log-file.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   297010 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/docs/media/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.684425 ansible-creator-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.720425 ansible-creator-24.4.0/src/ansible_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.684425 ansible-creator-24.4.0/src/ansible_creator/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.720425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.720425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.720425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/docker/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.devcontainer/podman/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.684425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.github/workflows/release.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.github/workflows/test.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.isort.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.prettierignore.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/CONTRIBUTING
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/LICENSE.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/changelogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/changelogs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/docs/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/docs/docsite/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/docs/docsite/links.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/eda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/rulebook.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/noop.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/vars.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/galaxy.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/action/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/cache/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/filter/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/filter/hello_world.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/inventory/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/module_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/module_utils/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/modules/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/plugin_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/plugin_utils/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/sub_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/sub_plugins/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.724425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/plugins/test/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/files/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/templates/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/tests/inventory
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/roles/run/vars/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/targets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.688425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/main.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/integration/test_integration.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tests/unit/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/tox-ansible.ini.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/src/ansible_creator/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/subcommands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/templar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/src/ansible_creator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/src/ansible_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 13:14:51.000000 ansible-creator-24.4.0/src/ansible_creator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.728425 ansible-creator-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.prettierignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/CONTRIBUTING
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/changelogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/docs/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/docs/docsite/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/eda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/rulebook.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.732425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/noop.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/vars.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/action/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/filter/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/inventory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/module_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/module_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.692425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/files/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/templates/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/tests/inventory
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/roles/run/vars/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.736425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.696425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.696425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tests/unit/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/integration/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:14:51.740425 ansible-creator-24.4.0/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/units/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tests/units/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-03 13:14:40.000000 ansible-creator-24.4.0/tox.ini
```

### Comparing `ansible-creator-24.2.0/.config/constraints.txt` & `ansible-creator-24.4.0/.config/constraints.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,78 +2,83 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --all-extras --no-annotate --output-file=.config/constraints.txt --strip-extras pyproject.toml
 #
 babel==2.14.0
 beautifulsoup4==4.12.3
-cachetools==5.3.2
+cachetools==5.3.3
 cairocffi==1.6.1
 cairosvg==2.7.1
 certifi==2024.2.2
 cffi==1.16.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.1
+coverage==7.4.4
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 distlib==0.3.8
-dnspython==2.5.0
+dnspython==2.6.1
 exceptiongroup==1.2.0
 execnet==2.0.2
-filelock==3.13.1
+filelock==3.13.3
 ghp-import==2.1.0
-griffe==0.40.0
+griffe==0.42.1
 htmlmin2==0.1.13
 idna==3.6
 iniconfig==2.0.0
 jinja2==3.1.3
 jsmin==3.0.1
 linkchecker==10.4.0
-markdown==3.5.2
+markdown==3.6
 markdown-exec==1.8.0
 markdown-include==0.8.1
 markupsafe==2.1.5
 mergedeep==1.3.4
 mkdocs==1.5.3
-mkdocs-ansible==24.2.1
-mkdocs-autorefs==0.5.0
+mkdocs-ansible==24.3.0
+mkdocs-autorefs==1.0.1
 mkdocs-gen-files==0.5.0
-mkdocs-htmlproofer-plugin==1.0.0
-mkdocs-material==9.5.8
+mkdocs-htmlproofer-plugin==1.2.0
+mkdocs-macros-plugin==1.0.5
+mkdocs-material==9.5.17
 mkdocs-material-extensions==1.3.1
 mkdocs-minify-plugin==0.8.0
 mkdocs-monorepo-plugin==1.1.0
-mkdocstrings==0.24.0
-mkdocstrings-python==1.8.0
-packaging==23.2
+mkdocstrings==0.24.2
+mkdocstrings-python==1.9.2
+packaging==24.0
 paginate==0.5.6
 pathspec==0.12.1
-pillow==10.2.0
-pipdeptree==2.13.2
+pillow==10.3.0
+pipdeptree==2.16.2
 platformdirs==4.2.0
 pluggy==1.4.0
-pycparser==2.21
+pycparser==2.22
 pygments==2.17.2
-pymdown-extensions==10.7
+pymdown-extensions==10.7.1
 pyproject-api==1.6.1
-pytest==8.0.0
+pytest==8.1.1
 pytest-xdist==3.5.0
-python-dateutil==2.8.2
-python-slugify==8.0.3
+python-dateutil==2.9.0.post0
+python-slugify==8.0.4
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
 regex==2023.12.25
 requests==2.31.0
 six==1.16.0
 soupsieve==2.5
+termcolor==2.4.0
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
-tox==4.12.1
-urllib3==2.2.0
-virtualenv==20.25.0
+tox==4.14.2
+urllib3==2.2.1
+virtualenv==20.25.1
 watchdog==4.0.0
 webencodings==0.5.1
+
+# The following packages are considered to be unsafe in a requirements file:
+# pip
```

### Comparing `ansible-creator-24.2.0/.config/dictionary.txt` & `ansible-creator-24.4.0/.config/dictionary.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 argparser
 argspec
 argvalues
 astimezone
 autorefs
 autosectionlabel
 basesystem
+boto
 BUILDDIR
 caplog
 capsys
 cliconf             # Ansible network cli abstraction plugin
 codeclimate
 colname
 COLORTERM
```

### Comparing `ansible-creator-24.2.0/.flake8` & `ansible-creator-24.4.0/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-creator-24.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/.github/workflows/release.yml` & `ansible-creator-24.4.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,10 @@
       - name: Install tox
         run: python3 -m pip install --user "tox>=4.0.0"
       - name: Check out src from Git
         uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
       - name: Build dists
-        run: python -m tox -e pkg
+        run: python3 -m tox -e pkg
       - name: Publish to pypi.org
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `ansible-creator-24.2.0/.github/workflows/tox.yml` & `ansible-creator-24.4.0/.github/workflows/tox.yml`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
           path: ~/.cache/pip
           key: ${{ matrix.name }}-pip-${{ hashFiles('setup.cfg', 'tox.ini', 'pyproject.toml', '.pre-commit-config.yaml') }}
 
       - name: Install tox
         run: python3 -m pip install --upgrade 'tox>=4.0.3'
 
       - name: Initialize tox envs
-        run: python -m tox --notest --skip-missing-interpreters false -vv -e ${{ matrix.passed_name }}
+        run: python3 -m tox --notest --skip-missing-interpreters false -vv -e ${{ matrix.passed_name }}
 
       - name: "tox -e ${{ matrix.passed_name }}"
         continue-on-error: ${{ matrix.devel || false }}
         run: python3 -m tox -e ${{ matrix.passed_name }}
 
       - name: Archive logs
         uses: actions/upload-artifact@v4
@@ -87,15 +87,15 @@
       - name: Upload coverage data
         if: ${{ startsWith(matrix.passed_name, 'py') }}
         uses: codecov/codecov-action@v4
         with:
           name: ${{ matrix.name }}
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
-          fail_ci_if_error: true
+          fail_ci_if_error: false
 
   check: # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
       - build
     runs-on: ubuntu-22.04
```

### Comparing `ansible-creator-24.2.0/.pre-commit-config.yaml` & `ansible-creator-24.4.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     rev: v3.1.0
     hooks:
       - id: add-trailing-comma
         args:
           - --py36-plus
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
-    rev: v1.5.4
+    rev: v1.5.5
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
     rev: v4.0.0-alpha.8
     hooks:
@@ -40,78 +40,78 @@
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.1.1
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pappasam/toml-sort
     rev: v0.23.1
     hooks:
       - id: toml-sort-fix
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.0"
+    rev: "v0.3.4"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.3.0
+    rev: v8.6.1
     hooks:
       - id: cspell
         name: Spell check with cspell
 
   - repo: https://github.com/jsh9/pydoclint
-    rev: 0.3.9
+    rev: 0.4.1
     hooks:
       - id: pydoclint
         args:
           - "--config=pyproject.toml"
 
   - repo: https://github.com/pycqa/pylint.git
-    rev: v3.0.3
+    rev: v3.1.0
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
           - PyYAML
           - jinja2
           - jsonschema
           - black
           - pytest
           - tox
 
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
           - jinja2
           - black
           - types-jsonschema
           - types-pyyaml
           - pytest
         args:
           - src
           - --python-version=3.10
         pass_filenames: false
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.3.0
+    rev: 7.4.1
     hooks:
       - id: pip-compile
         name: deps
         alias: deps
         always_run: true
         entry: pip-compile -q --no-annotate --output-file=.config/constraints.txt pyproject.toml --all-extras --strip-extras
         files: ^.config\/.*(requirements|constraints).*$
```

### Comparing `ansible-creator-24.2.0/LICENSE` & `ansible-creator-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/PKG-INFO` & `ansible-creator-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-creator
-Version: 24.2.0
+Version: 24.4.0
 Summary: A CLI tool for scaffolding Ansible Content.
 Author-email: Nilashish Chakarborty <nchakrab@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: changelog, https://github.com/ansible-community/ansible-creator/releases
 Project-URL: documentation, https://ansible-creator.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/ansible-community/ansible-creator
```

### Comparing `ansible-creator-24.2.0/README.md` & `ansible-creator-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/cspell.config.yaml` & `ansible-creator-24.4.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/collection_creation.md` & `ansible-creator-24.4.0/docs/collection_creation.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/contributing.md` & `ansible-creator-24.4.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/index.md` & `ansible-creator-24.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/installing.md` & `ansible-creator-24.4.0/docs/installing.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 # Installation and Usage
 
 ansible-creator provides two main functionalities: `init` and `create`. The `init` command allows you to initialize an Ansible Collection, while `create` command allows you scaffold ansible plugins of your choice.
 
 ## Installation
 
+!!! Recommendation
+
+    The **recommended** approach to install `ansible-creator` is using the
+    `ansible-dev-tools` package.
+    [Ansible Development Tools (ADT)](https://ansible.readthedocs.io/projects/dev-tools/)
+    aims to streamline the setup and usage of several tools needed in order to
+    create [Ansible](https://www.ansible.com) content. ADT combines critical Ansible
+    development packages into a unified Python package.
+
+    ```bash
+    # This also installs ansible-core if it is not already installed
+    pip3 install ansible-dev-tools
+    ```
+
 To install ansible-creator, use the following pip command:
 
 ```console
 $ pip install ansible-creator
 ```
 
 ## CLI Usage
@@ -54,22 +68,22 @@
 
 #### Example
 
 ```console
 $ ansible-creator init testns.testname --init-path $HOME/collections/ansible_collections
 ```
 
-This command will scaffold the collection `testns.testname` at `/home/ansible-dev/collections/ansible_collections`
+This command will scaffold the collection `testns.testname` at `/home/ansible-dev/collections/ansible_collections/testns/testname`
 
 #### Generated Ansible Collection Structure
 
 Running the init command generates an Ansible Collection with a comprehensive directory structure. Explore it using:
 
 ```console
-$ tree -lla /home/ansible-dev/collections/ansible_collections
+$ tree -lla /home/ansible-dev/collections/ansible_collections/testns/testname
 .
 ├── CHANGELOG.rst
 ├── changelogs
 │   └── config.yaml
 ├── CODE_OF_CONDUCT.md
 ├── CONTRIBUTING
 ├── docs
@@ -88,14 +102,15 @@
 │           │   ├── converge.yml
 │           │   └── noop.yml
 │           └── vars
 │               └── vars.yml
 ├── galaxy.yml
 ├── .github
 │   └── workflows
+│       ├── release.yml
 │       └── test.yml
 ├── .isort.cfg
 ├── LICENSE
 ├── MAINTAINERS
 ├── meta
 │   └── runtime.yml
 ├── plugins
@@ -118,14 +133,33 @@
 │   │   └── __init__.py
 │   └── test
 │       └── __init__.py
 ├── .pre-commit-config.yaml
 ├── .prettierignore
 ├── pyproject.toml
 ├── README.md
+├── roles
+│   └── run
+│       ├── defaults
+│       │   └── main.yml
+│       ├── files
+│       │   └── .keep
+│       ├── handlers
+│       │   └── main.yaml
+│       ├── meta
+│       │   └── main.yml
+│       ├── README.md
+│       ├── tasks
+│       │   └── main.yml
+│       ├── templates
+│       │   └── .keep
+│       ├── tests
+│       │   └── inventory
+│       ├── vars
+│       │   └── main.yml
 ├── tests
 │   ├── .gitignore
 │   ├── integration
 │   │   ├── __init__.py
 │   │   ├── targets
 │   │   │   └── hello_world
 │   │   │       └── tasks
@@ -145,9 +179,11 @@
 
 - Git initialize the repository containing the scaffolded collection with `git init`.
 - `pip install ansible-core molecule pytest-xdist pytest-ansible`.
 - Invoke `pytest` from collection root.
 
 It also comes equipped with Github Action Workflows that use [ansible-content-actions](https://github.com/marketplace/actions/ansible-content-actions) for testing and publishing the collection. For details on how to use these, please refer to the following:
 
-- [Using the testing workflow](https://github.com/ansible/ansible-dev-tools/blob/main/docs/user-guide/ci-setup.md)
-- [Using the release workflow](https://github.com/ansible/ansible-dev-tools/blob/main/docs/user-guide/content-release.md)
+- [Using the testing workflow](https://ansible.readthedocs.io/projects/dev-tools/user-guide/ci-setup/)
+- [Using the release workflow](https://ansible.readthedocs.io/projects/dev-tools/user-guide/content-release/)
+
+Please ensure that you review any potential `TO-DO` items in the scaffolded content and make the necessary modifications according to your requirements.
```

### Comparing `ansible-creator-24.2.0/docs/media/log-to-file.gif` & `ansible-creator-24.4.0/docs/media/log-to-file.gif`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/media/open-collection.gif` & `ansible-creator-24.4.0/docs/media/open-collection.gif`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/media/open-folder.gif` & `ansible-creator-24.4.0/docs/media/open-folder.gif`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/media/open-log-file.gif` & `ansible-creator-24.4.0/docs/media/open-log-file.gif`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/docs/media/refresh.gif` & `ansible-creator-24.4.0/docs/media/refresh.gif`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/mkdocs.yml` & `ansible-creator-24.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/pyproject.toml` & `ansible-creator-24.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 documentation = "https://ansible-creator.readthedocs.io/en/latest/"
 homepage = "https://github.com/ansible-community/ansible-creator"
 repository = "https://github.com/ansible-community/ansible-creator"
 
 [tool.black]
 exclude = "tests/fixtures"
 
+[tool.coverage.report]
+exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
+omit = ["tests/*"]
+
 [tool.mypy]
 files = ["src"]
 
 [tool.pydoclint]
 allow-init-docstring = true
 
 [tool.pylint]
```

### Comparing `ansible-creator-24.2.0/src/ansible_creator/cli.py` & `ansible-creator-24.4.0/src/ansible_creator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/config.py` & `ansible-creator-24.4.0/src/ansible_creator/config.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/constants.py` & `ansible-creator-24.4.0/src/ansible_creator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/exceptions.py` & `ansible-creator-24.4.0/src/ansible_creator/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/output.py` & `ansible-creator-24.4.0/src/ansible_creator/output.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.github/workflows/test.yml.j2` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.github/workflows/test.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/LICENSE.j2` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/README.md.j2` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/changelogs/config.yaml` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/docs/docsite/links.yml` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/resources/new_collection/galaxy.yml.j2` & `ansible-creator-24.4.0/src/ansible_creator/resources/new_collection/galaxy.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/subcommands/init.py` & `ansible-creator-24.4.0/src/ansible_creator/subcommands/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 if TYPE_CHECKING:
     from ansible_creator.config import Config
     from ansible_creator.output import Output
 
 
 class Init:
-    """Class representing ansible-creator create subcommand."""
+    """Class representing ansible-creator init subcommand."""
 
     def __init__(
         self: Init,
         config: Config,
         output: Output,
     ) -> None:
         """Initialize the init action.
@@ -39,56 +39,61 @@
         self.output: Output = output
 
     def run(self: Init) -> None:
         """Start scaffolding collection skeleton.
 
         :raises CreatorError: if computed collection path is an existing directory or file.
         """
-        col_path = os.path.join(self._init_path, self._namespace, self._collection_name)
+        if self._init_path.endswith("collections/ansible_collections"):
+            self._init_path = os.path.join(
+                self._init_path,
+                self._namespace,
+                self._collection_name,
+            )
 
-        self.output.debug(msg=f"final collection path set to {col_path}")
+        self.output.debug(msg=f"final collection path set to {self._init_path}")
 
         # check if init_path already exists
-        if os.path.exists(col_path):
-            if os.path.isfile(col_path):
-                msg = f"the path {col_path} already exists, but is a file - aborting"
+        if os.path.exists(self._init_path):
+            if os.path.isfile(self._init_path):
+                msg = f"the path {self._init_path} already exists, but is a file - aborting"
                 raise CreatorError(
                     msg,
                 )
 
             if not self._force:
                 msg = (
-                    f"The directory {col_path} already exists.\n"
+                    f"The directory {self._init_path} already exists.\n"
                     f"You can use --force to re-initialize this directory."
                     f"\nHowever it will delete ALL existing contents in it."
                 )
                 raise CreatorError(msg)
 
             # user requested --force, re-initializing existing directory
-            self.output.warning(f"re-initializing existing directory {col_path}")
-            for root, dirs, files in os.walk(col_path, topdown=True):
+            self.output.warning(f"re-initializing existing directory {self._init_path}")
+            for root, dirs, files in os.walk(self._init_path, topdown=True):
                 for old_dir in dirs:
                     path = os.path.join(root, old_dir)
                     self.output.debug(f"removing tree {old_dir}")
                     shutil.rmtree(path)
                 for old_file in files:
                     path = os.path.join(root, old_file)
                     self.output.debug(f"removing file {old_file}")
                     os.unlink(path)
 
         # if init_path does not exist, create it
-        if not os.path.exists(col_path):
-            self.output.debug(msg=f"creating new directory at {col_path}")
-            os.makedirs(col_path)
+        if not os.path.exists(self._init_path):
+            self.output.debug(msg=f"creating new directory at {self._init_path}")
+            os.makedirs(self._init_path)
 
         # copy new_collection container to destination, templating files when found
         self.output.debug(msg="started copying collection skeleton to destination")
         copy_container(
             source="new_collection",
-            dest=col_path,
+            dest=self._init_path,
             templar=self._templar,
             template_data={
                 "namespace": self._namespace,
                 "collection_name": self._collection_name,
                 "creator_version": self._creator_version,
             },
             output=self.output,
```

### Comparing `ansible-creator-24.2.0/src/ansible_creator/templar.py` & `ansible-creator-24.4.0/src/ansible_creator/templar.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/src/ansible_creator/utils.py` & `ansible-creator-24.4.0/src/ansible_creator/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from importlib import resources
 from typing import TYPE_CHECKING
 
 from ansible_creator.exceptions import CreatorError
 
 
 if TYPE_CHECKING:
-    from importlib import abc
-
+    from ansible_creator.compat import Traversable
     from ansible_creator.output import Output
     from ansible_creator.templar import Templar
 
 PATH_REPLACERS = {
     "network_os": "collection_name",
     "resource": "resource",
 }
@@ -95,15 +94,15 @@
     :param allow_overwrite: A list of paths that should be overwritten at destination.
 
     :raises CreatorError: if allow_overwrite is not a list.
     """
     output.debug(msg=f"starting recursive copy with source container '{source}'")
     output.debug(msg=f"allow_overwrite set to {allow_overwrite}")
 
-    def _recursive_copy(root: abc.Traversable) -> None:
+    def _recursive_copy(root: Traversable) -> None:
         """Recursively traverses a resource container and copies content to destination.
 
         :param root: A traversable object representing root of the container to copy.
         """
         output.debug(msg=f"current root set to {root}")
 
         for obj in root.iterdir():
```

### Comparing `ansible-creator-24.2.0/src/ansible_creator.egg-info/PKG-INFO` & `ansible-creator-24.4.0/src/ansible_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-creator
-Version: 24.2.0
+Version: 24.4.0
 Summary: A CLI tool for scaffolding Ansible Content.
 Author-email: Nilashish Chakarborty <nchakrab@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: changelog, https://github.com/ansible-community/ansible-creator/releases
 Project-URL: documentation, https://ansible-creator.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/ansible-community/ansible-creator
```

### Comparing `ansible-creator-24.2.0/src/ansible_creator.egg-info/SOURCES.txt` & `ansible-creator-24.4.0/src/ansible_creator.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.prettierignore
 .readthedocs.yml
 .yamllint
 CHANGELOG.md
 LICENSE
 README.md
 codecov.yml
 cspell.config.yaml
@@ -26,14 +27,15 @@
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/security_bug_report.md
 .github/workflows/ack.yml
 .github/workflows/push.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
 .vscode/extensions.json
+.vscode/launch.json
 .vscode/settings.json
 docs/collection_creation.md
 docs/contributing.md
 docs/index.md
 docs/installing.md
 docs/media/log-to-file.gif
 docs/media/open-collection.gif
@@ -41,14 +43,15 @@
 docs/media/open-log-file.gif
 docs/media/refresh.gif
 src/ansible_creator/__init__.py
 src/ansible_creator/__main__.py
 src/ansible_creator/_version.py
 src/ansible_creator/_version.pyi
 src/ansible_creator/cli.py
+src/ansible_creator/compat.py
 src/ansible_creator/config.py
 src/ansible_creator/constants.py
 src/ansible_creator/exceptions.py
 src/ansible_creator/output.py
 src/ansible_creator/templar.py
 src/ansible_creator/utils.py
 src/ansible_creator.egg-info/PKG-INFO
@@ -65,14 +68,17 @@
 src/ansible_creator/resources/new_collection/CONTRIBUTING
 src/ansible_creator/resources/new_collection/LICENSE.j2
 src/ansible_creator/resources/new_collection/MAINTAINERS
 src/ansible_creator/resources/new_collection/README.md.j2
 src/ansible_creator/resources/new_collection/galaxy.yml.j2
 src/ansible_creator/resources/new_collection/pyproject.toml.j2
 src/ansible_creator/resources/new_collection/tox-ansible.ini.j2
+src/ansible_creator/resources/new_collection/.devcontainer/devcontainer.json
+src/ansible_creator/resources/new_collection/.devcontainer/docker/devcontainer.json
+src/ansible_creator/resources/new_collection/.devcontainer/podman/devcontainer.json
 src/ansible_creator/resources/new_collection/.github/workflows/release.yml.j2
 src/ansible_creator/resources/new_collection/.github/workflows/test.yml.j2
 src/ansible_creator/resources/new_collection/.vscode/extensions.json
 src/ansible_creator/resources/new_collection/changelogs/config.yaml
 src/ansible_creator/resources/new_collection/docs/.keep
 src/ansible_creator/resources/new_collection/docs/docsite/links.yml
 src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/rulebook.yml.j2
@@ -87,14 +93,23 @@
 src/ansible_creator/resources/new_collection/plugins/filter/hello_world.py.j2
 src/ansible_creator/resources/new_collection/plugins/inventory/__init__.py.j2
 src/ansible_creator/resources/new_collection/plugins/module_utils/__init__.py.j2
 src/ansible_creator/resources/new_collection/plugins/modules/__init__.py.j2
 src/ansible_creator/resources/new_collection/plugins/plugin_utils/__init__.py.j2
 src/ansible_creator/resources/new_collection/plugins/sub_plugins/__init__.py.j2
 src/ansible_creator/resources/new_collection/plugins/test/__init__.py.j2
+src/ansible_creator/resources/new_collection/roles/run/README.md.j2
+src/ansible_creator/resources/new_collection/roles/run/defaults/main.yml
+src/ansible_creator/resources/new_collection/roles/run/files/.keep
+src/ansible_creator/resources/new_collection/roles/run/handlers/main.yml
+src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2
+src/ansible_creator/resources/new_collection/roles/run/tasks/main.yml
+src/ansible_creator/resources/new_collection/roles/run/templates/.keep
+src/ansible_creator/resources/new_collection/roles/run/tests/inventory
+src/ansible_creator/resources/new_collection/roles/run/vars/main.yml
 src/ansible_creator/resources/new_collection/tests/.gitignore
 src/ansible_creator/resources/new_collection/tests/integration/__init__.py.j2
 src/ansible_creator/resources/new_collection/tests/integration/test_integration.py.j2
 src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/main.yml.j2
 src/ansible_creator/resources/new_collection/tests/unit/.keep
 src/ansible_creator/schemas/__init__.py
 src/ansible_creator/subcommands/__init__.py
@@ -110,14 +125,17 @@
 tests/fixtures/collection/testorg/testcol/CONTRIBUTING
 tests/fixtures/collection/testorg/testcol/LICENSE
 tests/fixtures/collection/testorg/testcol/MAINTAINERS
 tests/fixtures/collection/testorg/testcol/README.md
 tests/fixtures/collection/testorg/testcol/galaxy.yml
 tests/fixtures/collection/testorg/testcol/pyproject.toml
 tests/fixtures/collection/testorg/testcol/tox-ansible.ini
+tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json
+tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json
+tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json
 tests/fixtures/collection/testorg/testcol/.github/workflows/release.yml
 tests/fixtures/collection/testorg/testcol/.github/workflows/test.yml
 tests/fixtures/collection/testorg/testcol/.vscode/extensions.json
 tests/fixtures/collection/testorg/testcol/changelogs/config.yaml
 tests/fixtures/collection/testorg/testcol/docs/.keep
 tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml
 tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/rulebook.yml
@@ -132,14 +150,23 @@
 tests/fixtures/collection/testorg/testcol/plugins/filter/hello_world.py
 tests/fixtures/collection/testorg/testcol/plugins/inventory/__init__.py
 tests/fixtures/collection/testorg/testcol/plugins/module_utils/__init__.py
 tests/fixtures/collection/testorg/testcol/plugins/modules/__init__.py
 tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/__init__.py
 tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/__init__.py
 tests/fixtures/collection/testorg/testcol/plugins/test/__init__.py
+tests/fixtures/collection/testorg/testcol/roles/run/README.md
+tests/fixtures/collection/testorg/testcol/roles/run/defaults/main.yml
+tests/fixtures/collection/testorg/testcol/roles/run/files/.keep
+tests/fixtures/collection/testorg/testcol/roles/run/handlers/main.yml
+tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml
+tests/fixtures/collection/testorg/testcol/roles/run/tasks/main.yml
+tests/fixtures/collection/testorg/testcol/roles/run/templates/.keep
+tests/fixtures/collection/testorg/testcol/roles/run/tests/inventory
+tests/fixtures/collection/testorg/testcol/roles/run/vars/main.yml
 tests/fixtures/collection/testorg/testcol/tests/.gitignore
 tests/fixtures/collection/testorg/testcol/tests/integration/__init__.py
 tests/fixtures/collection/testorg/testcol/tests/integration/test_integration.py
 tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/main.yml
 tests/fixtures/collection/testorg/testcol/tests/unit/.keep
 tests/integration/__init__.py
 tests/integration/test_init.py
```

### Comparing `ansible-creator-24.2.0/tests/conftest.py` & `ansible-creator-24.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.github/workflows/test.yml` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/LICENSE` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/README.md` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/README.md`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/fixtures/collection/testorg/testcol/galaxy.yml` & `ansible-creator-24.4.0/tests/fixtures/collection/testorg/testcol/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/integration/test_init.py` & `ansible-creator-24.4.0/tests/integration/test_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,31 +72,41 @@
     assert (
         "ansible-creator init: error: the following arguments are required: collection"
         in result.stderr
     )
 
 
 def test_run_init_basic(cli, tmp_path):
-    result = cli(f"ansible-creator init testorg.testcol --init-path {tmp_path}")
+    final_dest = f"{tmp_path}/collections/ansible_collections"
+    cli(f"mkdir -p {final_dest}")
+
+    result = cli(
+        f"ansible-creator init testorg.testcol --init-path {final_dest}",
+    )
     assert result.returncode == 0
 
     # check stdout
     assert (
         re.search("Note: collection testorg.testcol created at", result.stdout)
         is not None
     )
 
     # fail to override existing collection with force=false (default)
-    result = cli(f"ansible-creator init testorg.testcol --init-path {tmp_path}")
+    result = cli(
+        f"ansible-creator init testorg.testcol --init-path {final_dest}",
+    )
+
     assert result.returncode != 0
+
+    # this is required to handle random line breaks in CI, especially with macos runners
+    mod_stderr = "".join([line.strip() for line in result.stderr.splitlines()])
     assert (
         re.search(
-            rf"Error: The directory\s+{tmp_path}/testorg/testcol\s+already exists.",
-            result.stderr,
-            flags=re.MULTILINE,
+            rf"Error:\s*The\s*directory\s*{final_dest}/testorg/testcol\s*already\s*exists",
+            mod_stderr,
         )
         is not None
     )
     assert "You can use --force to re-initialize this directory." in result.stderr
     assert "However it will delete ALL existing contents in it." in result.stderr
 
     # override existing collection with force=true
```

### Comparing `ansible-creator-24.2.0/tests/units/test_basic.py` & `ansible-creator-24.4.0/tests/units/test_basic.py`

 * *Files identical despite different names*

### Comparing `ansible-creator-24.2.0/tests/units/test_init.py` & `ansible-creator-24.4.0/tests/units/test_init.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "log_append": True,
         "log_file": tmp_path / "ansible-creator.log",
         "log_level": "debug",
         "no_ansi": False,
         "subcommand": "init",
         "verbose": 0,
         "collection": "testorg.testcol",
-        "init_path": tmp_path,
+        "init_path": tmp_path / "testorg" / "testcol",
     }
 
 
 @pytest.fixture()
 def output(tmp_path) -> Output:
     """Create an Output class object as fixture.
 
@@ -92,7 +92,36 @@
         output=output,
     )
     init.run()
     result = capsys.readouterr().out
     assert (
         re.search("Warning: re-initializing existing directory", result) is not None
     ), result
+
+
+def test_run_success_collections_alt_dir(
+    tmp_path,
+    capsys,
+    cli_args,
+    output,
+) -> None:
+    """Test Init.run() when init_path ends with "collections" / "ansible_collections"""
+    # successfully create new collection
+    cli_args["init_path"] = tmp_path / "collections" / "ansible_collections"
+    final_path = cli_args["init_path"] / "testorg" / "testcol"
+    init = Init(
+        Config(**cli_args),
+        output=output,
+    )
+    init.run()
+    result = capsys.readouterr().out
+
+    # this is required to handle random line breaks in CI, especially with macos runners
+    mod_result = "".join([line.strip() for line in result.splitlines()])
+
+    assert (
+        re.search(
+            rf"Note:\s*collection\s*testorg.testcol\s*created\s*at\s*{final_path}",
+            mod_result,
+        )
+        is not None
+    )
```

### Comparing `ansible-creator-24.2.0/tox.ini` & `ansible-creator-24.4.0/tox.ini`

 * *Files identical despite different names*

