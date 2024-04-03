# Comparing `tmp/buildrunner-3.6.982.tar.gz` & `tmp/buildrunner-3.7.991.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-3.6.982.tar", last modified: Thu Mar 28 19:21:24 2024, max compression
+gzip compressed data, was "buildrunner-3.7.991.tar", last modified: Wed Apr  3 16:06:49 2024, max compression
```

## Comparing `buildrunner-3.6.982.tar` & `buildrunner-3.7.991.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.116207 buildrunner-3.6.982/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-28 19:21:18.000000 buildrunner-3.6.982/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 19:21:18.000000 buildrunner-3.6.982/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    46108 2024-03-28 19:21:24.116207 buildrunner-3.6.982/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    44108 2024-03-28 19:21:18.000000 buildrunner-3.6.982/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.104206 buildrunner-3.6.982/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-03-28 19:21:18.000000 buildrunner-3.6.982/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-03-28 19:21:18.000000 buildrunner-3.6.982/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.108206 buildrunner-3.6.982/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.108206 buildrunner-3.6.982/buildrunner/config/
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.108206 buildrunner-3.6.982/buildrunner/config/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/fetch/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/jinja_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/models_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23242 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/multiplatform_image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.112206 buildrunner-3.6.982/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-03-28 19:21:18.000000 buildrunner-3.6.982/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 19:21:23.000000 buildrunner-3.6.982/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.116207 buildrunner-3.6.982/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46108 2024-03-28 19:21:24.000000 buildrunner-3.6.982/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-28 19:21:24.000000 buildrunner-3.6.982/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:21:24.000000 buildrunner-3.6.982/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-28 19:21:24.000000 buildrunner-3.6.982/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 19:21:24.000000 buildrunner-3.6.982/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-03-28 19:21:18.000000 buildrunner-3.6.982/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:21:24.116207 buildrunner-3.6.982/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-03-28 19:21:18.000000 buildrunner-3.6.982/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-28 19:21:18.000000 buildrunner-3.6.982/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:21:24.116207 buildrunner-3.6.982/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_buildrunner_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_multiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_push_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_push_security_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_util_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_utils_flock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-28 19:21:18.000000 buildrunner-3.6.982/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 16:06:45.000000 buildrunner-3.7.991/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 16:06:45.000000 buildrunner-3.7.991/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-03 16:06:49.813845 buildrunner-3.7.991/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45194 2024-04-03 16:06:45.000000 buildrunner-3.7.991/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.801845 buildrunner-3.7.991/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-04-03 16:06:45.000000 buildrunner-3.7.991/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-03 16:06:45.000000 buildrunner-3.7.991/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.801845 buildrunner-3.7.991/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.805845 buildrunner-3.7.991/buildrunner/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.805845 buildrunner-3.7.991/buildrunner/config/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/fetch/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/jinja_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/models_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/multiplatform_image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.809846 buildrunner-3.7.991/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-03 16:06:45.000000 buildrunner-3.7.991/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 16:06:49.000000 buildrunner-3.7.991/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-03 16:06:45.000000 buildrunner-3.7.991/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:06:49.813845 buildrunner-3.7.991/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-03 16:06:45.000000 buildrunner-3.7.991/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 16:06:45.000000 buildrunner-3.7.991/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:06:49.813845 buildrunner-3.7.991/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_buildrunner_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_multiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_push_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_push_security_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_util_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_utils_flock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 16:06:45.000000 buildrunner-3.7.991/tests/test_version.py
```

### Comparing `buildrunner-3.6.982/LICENSE` & `buildrunner-3.7.991/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/PKG-INFO` & `buildrunner-3.7.991/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.6.982
+Version: 3.7.991
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -38,15 +38,15 @@
 Requires-Dist: paramiko==3.2.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.4.2
 Requires-Dist: pydantic-core==2.10.1
 Requires-Dist: pygments==2.15.1
 Requires-Dist: pynacl==1.5.0
-Requires-Dist: python-on-whales==0.65.0
+Requires-Dist: python-on-whales==0.70.1
 Requires-Dist: pyyaml==6.0
 Requires-Dist: readme-renderer==37.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: retry2==0.9.5
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.0
@@ -316,15 +316,15 @@
         no-cache: true/false (defaults to false)
 
         # Specify Docker images to consider as cache sources,
         # similar to the --cache-from option used by Docker.
         # Buildrunner will attempt to pull these images from the remote registry.
         # If the pull is unsuccessful, buildrunner will still pass in the image name
         # into --cache-from, allowing a cache check in the host machine cache
-        # NOTE: Does not work for multi-platform builds
+        # NOTE: Does not work for multiplatform builds
         cache_from:
           - my-images/image:PR-123
           - my-images/image:latest
 
         # Whether to do a docker pull of the "FROM" image prior to the build.
         # This is critical if you are building from images that are changing
         # with regularity.
@@ -340,19 +340,20 @@
         # This is useful if you are building an image for a different architecture than what
         # buildrunner is running on, such as using a linux/amd64 build node to produce an image
         # with a docker manifest compatible with an Apple M1 linux/arm64/v8 architecture
         platform: linux/amd64
         <or>
         platform: linux/arm64/v8 # an apple m1 architecture
 
-        # To build multi-platform images, add each platform to be built to this list and buildrunner
+        # To build multiplatform images, add each platform to be built to this list and buildrunner
         # will use docker buildx to build and provide a single tag containing all architectures specified.
-        # Note that buildx may be configured to build some platforms with emulation and therefore builds
-        # may take longer with this option specified. Also note that when using the platforms option, it is not
-        # valid to also specify the platform option.
+        # Notes:
+        #  * buildx may be configured to build some platforms with emulation and therefore builds may take longer with this option specified
+        #  * multiplatform builds cannot be used in the buildrunner docker image unless the 'build-registry' global config parameter is specified
+        #  * only one of platform or platforms may be specified
         platforms:
           - linux/amd64
           - linux/arm64/v8
 
         # Specify the build args that should be used when building your image,
         # similar to the --build-args option used by Docker
         buildargs:
@@ -432,15 +433,15 @@
       # Optional step dependency definition to specify which steps need to be processed before this step.
       # The `version` must be present and set to `2.0` or higher for buildrunner to utilize the step dependencies list.
       # An buildrunner error will occur if `depends` is present but `version` is missing or value is lower than `2.0`.
       depends:
         - test-step
         - validation-step
 
-      # This is not supported in the same step as a multi-platform build.
+      # This is not supported in the same step as a multiplatform build.
       run:
         # xfail indicates whether the run operation is expected to fail.  The
         # default is false - the operation is expected to succeed.  If xfail
         # is true and the operation succeeds then it will result in a failure.
         xfail: <boolean>
 
         # A map of additional containers that should be created and linked to
@@ -943,18 +944,31 @@
       build: .
       # To push the docker image to a registry
       push:
         repository: myimages/image1
         # Do not include default build tag
         add_build_tag: false
         tags: [ 'latest' ]
+        # Optional security scan configuration may be provided for each configured push
+        security-scan:
+          # See docs/global-configuration.rst for more information on these attributes.
+          #enabled: false
+          #scanner: "trivy"
+          #version: "latest"
+          # NOTE: Any configuration provided here will be merged with global/command line config
+          #config:
+          #  optional-param: val1
+          # Set to a float to fail the build if the maximum score
+          # is greater than or equal to this number
+          #max-score-threshold: 8.9
       # OR to just commit it locally to use in subsequent steps
       commit:
         repository: myimages/image1
         tags: [ 'latest' ]
+        # NOTE: Image security scans are disabled for images that are not pushed
 
 The configuration may also specify multiple repositories with their own tags
 (each list entry may be a string or specify additional tags):
 
 .. code:: yaml
 
   steps:
@@ -1047,17 +1061,24 @@
 
 This must never be used on a shared server such as a build server as it could
 cause port mapping conflicts.
 
 Image Security Scans
 ====================
 
-Pushed docker images may be automatically scanned for vulnerabilities using the ``security-scan``
-global configuration options or the ``--security-scan-*`` command line options that may override
-the global configuration.  Just set ``security-scan.enabled`` to true to enable automatic scans.
+Pushed docker images may be automatically scanned for vulnerabilities using (in priority order):
+
+* The ``security-scan`` configuration on ``push`` step attributes
+* The ``--security-scan-*`` command line options
+* The ``security-scan`` global configuration options
+
+Just set ``security-scan.enabled`` to true to enable automatic scans. The config specified on the
+command line options overrides the global config completely, but configuration on the push step
+attribute is merged with the command line/global config. Additionally note that the ``cache-dir``
+can only be configured on the global/command line level.
 
 The ``max-score-threshold`` may also be configured to fail the build if the max score of the
 detected vulnerabilities is greater than or equal to the ``max-score-threshold`` value. This
 score is the CVSS v3 score that ranges between 0 (none) to 10.0 (most critical).
 
 Any detected vulnerabilities are added to the ``artifacts.json`` file per Docker image platform,
 along with the detected maximum vulnerability score.
```

### Comparing `buildrunner-3.6.982/README.rst` & `buildrunner-3.7.991/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         no-cache: true/false (defaults to false)
 
         # Specify Docker images to consider as cache sources,
         # similar to the --cache-from option used by Docker.
         # Buildrunner will attempt to pull these images from the remote registry.
         # If the pull is unsuccessful, buildrunner will still pass in the image name
         # into --cache-from, allowing a cache check in the host machine cache
-        # NOTE: Does not work for multi-platform builds
+        # NOTE: Does not work for multiplatform builds
         cache_from:
           - my-images/image:PR-123
           - my-images/image:latest
 
         # Whether to do a docker pull of the "FROM" image prior to the build.
         # This is critical if you are building from images that are changing
         # with regularity.
@@ -275,19 +275,20 @@
         # This is useful if you are building an image for a different architecture than what
         # buildrunner is running on, such as using a linux/amd64 build node to produce an image
         # with a docker manifest compatible with an Apple M1 linux/arm64/v8 architecture
         platform: linux/amd64
         <or>
         platform: linux/arm64/v8 # an apple m1 architecture
 
-        # To build multi-platform images, add each platform to be built to this list and buildrunner
+        # To build multiplatform images, add each platform to be built to this list and buildrunner
         # will use docker buildx to build and provide a single tag containing all architectures specified.
-        # Note that buildx may be configured to build some platforms with emulation and therefore builds
-        # may take longer with this option specified. Also note that when using the platforms option, it is not
-        # valid to also specify the platform option.
+        # Notes:
+        #  * buildx may be configured to build some platforms with emulation and therefore builds may take longer with this option specified
+        #  * multiplatform builds cannot be used in the buildrunner docker image unless the 'build-registry' global config parameter is specified
+        #  * only one of platform or platforms may be specified
         platforms:
           - linux/amd64
           - linux/arm64/v8
 
         # Specify the build args that should be used when building your image,
         # similar to the --build-args option used by Docker
         buildargs:
@@ -367,15 +368,15 @@
       # Optional step dependency definition to specify which steps need to be processed before this step.
       # The `version` must be present and set to `2.0` or higher for buildrunner to utilize the step dependencies list.
       # An buildrunner error will occur if `depends` is present but `version` is missing or value is lower than `2.0`.
       depends:
         - test-step
         - validation-step
 
-      # This is not supported in the same step as a multi-platform build.
+      # This is not supported in the same step as a multiplatform build.
       run:
         # xfail indicates whether the run operation is expected to fail.  The
         # default is false - the operation is expected to succeed.  If xfail
         # is true and the operation succeeds then it will result in a failure.
         xfail: <boolean>
 
         # A map of additional containers that should be created and linked to
@@ -878,18 +879,31 @@
       build: .
       # To push the docker image to a registry
       push:
         repository: myimages/image1
         # Do not include default build tag
         add_build_tag: false
         tags: [ 'latest' ]
+        # Optional security scan configuration may be provided for each configured push
+        security-scan:
+          # See docs/global-configuration.rst for more information on these attributes.
+          #enabled: false
+          #scanner: "trivy"
+          #version: "latest"
+          # NOTE: Any configuration provided here will be merged with global/command line config
+          #config:
+          #  optional-param: val1
+          # Set to a float to fail the build if the maximum score
+          # is greater than or equal to this number
+          #max-score-threshold: 8.9
       # OR to just commit it locally to use in subsequent steps
       commit:
         repository: myimages/image1
         tags: [ 'latest' ]
+        # NOTE: Image security scans are disabled for images that are not pushed
 
 The configuration may also specify multiple repositories with their own tags
 (each list entry may be a string or specify additional tags):
 
 .. code:: yaml
 
   steps:
@@ -982,17 +996,24 @@
 
 This must never be used on a shared server such as a build server as it could
 cause port mapping conflicts.
 
 Image Security Scans
 ====================
 
-Pushed docker images may be automatically scanned for vulnerabilities using the ``security-scan``
-global configuration options or the ``--security-scan-*`` command line options that may override
-the global configuration.  Just set ``security-scan.enabled`` to true to enable automatic scans.
+Pushed docker images may be automatically scanned for vulnerabilities using (in priority order):
+
+* The ``security-scan`` configuration on ``push`` step attributes
+* The ``--security-scan-*`` command line options
+* The ``security-scan`` global configuration options
+
+Just set ``security-scan.enabled`` to true to enable automatic scans. The config specified on the
+command line options overrides the global config completely, but configuration on the push step
+attribute is merged with the command line/global config. Additionally note that the ``cache-dir``
+can only be configured on the global/command line level.
 
 The ``max-score-threshold`` may also be configured to fail the build if the max score of the
 detected vulnerabilities is greater than or equal to the ``max-score-threshold`` value. This
 score is the CVSS v3 score that ranges between 0 (none) to 10.0 (most critical).
 
 Any detected vulnerabilities are added to the ``artifacts.json`` file per Docker image platform,
 along with the detected maximum vulnerability score.
```

### Comparing `buildrunner-3.6.982/buildrunner/__init__.py` & `buildrunner-3.7.991/buildrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/cli.py` & `buildrunner-3.7.991/buildrunner/cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/__init__.py` & `buildrunner-3.7.991/buildrunner/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/fetch/__init__.py` & `buildrunner-3.7.991/buildrunner/config/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/fetch/file.py` & `buildrunner-3.7.991/buildrunner/config/fetch/file.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/fetch/github.py` & `buildrunner-3.7.991/buildrunner/config/fetch/github.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/jinja_context.py` & `buildrunner-3.7.991/buildrunner/config/jinja_context.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/loader.py` & `buildrunner-3.7.991/buildrunner/config/loader.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/config/models.py` & `buildrunner-3.7.991/buildrunner/config/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 NOTICE: Adobe permits you to use, modify, and distribute this file in accordance
 with the terms of the Adobe license agreement accompanying it.
 """
 
 import os
 import tempfile
+from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from pydantic import BaseModel, Field, field_validator, ValidationError
 
-from .models_step import Step
+from .models_step import Step, StepPushSecurityScanConfig
 from .validation import (
     get_validation_errors,
     validate_multiplatform_build,
     validate_multiplatform_are_not_retagged,
     validate_push,
 )
 
@@ -43,27 +44,56 @@
 
 class DockerBuildCacheConfig(BaseModel, extra="forbid"):
     builders: Optional[List[str]] = None
     from_config: Optional[Union[dict, str]] = Field(None, alias="from")
     to_config: Optional[Union[dict, str]] = Field(None, alias="to")
 
 
-class SecurityScanConfig(BaseModel, extra="forbid"):
+class GlobalSecurityScanConfig(BaseModel, extra="forbid"):
+    """
+    The global config version of security scan configuration has default values.
+    """
+
     enabled: bool = False
     scanner: str = "trivy"
     version: str = "latest"
     # The local cache directory for the scanner (used if supported by the scanner)
-    cache_dir: Optional[str] = None
+    cache_dir: Optional[str] = Field(None, alias="cache-dir")
     config: dict = {
         "timeout": "20m",
         # Do not error on vulnerabilities by default
         "exit-code": 0,
     }
     max_score_threshold: Optional[float] = Field(None, alias="max-score-threshold")
 
+    def merge_scan_config(
+        self, push_config: Optional[StepPushSecurityScanConfig]
+    ) -> "GlobalSecurityScanConfig":
+        """
+        Merges the push security scanning config with the global security config
+        and returns a merged config without modifying the global configuration.
+        :param push_config: the step push security scan config
+        :return: a merged scan config
+        """
+        if not push_config:
+            return self
+        new_model = {
+            field: getattr(push_config, field)
+            for field, value in self.model_fields.items()
+            if getattr(push_config, field, None) is not None
+        }
+        # model_copy does not handle actually copying the config dict, so copy this manually and update with
+        # the step config once the model copy is done
+        config_value = new_model.pop("config", None)
+        new_model["config"] = deepcopy(self.config)
+        cloned_config = self.model_copy(update=new_model)
+        if config_value:
+            cloned_config.config.update(config_value)
+        return cloned_config
+
 
 class GlobalConfig(BaseModel, extra="forbid"):
     """Top level global config model"""
 
     github: Optional[Dict[str, GithubModel]] = None
     env: Optional[Dict[str, Any]] = None
     build_servers: Optional[Dict[str, List[str]]] = Field(
@@ -92,16 +122,16 @@
     )
     build_registry: Optional[str] = Field(
         alias="build-registry", default=MP_LOCAL_REGISTRY
     )
     platform_builders: Optional[Dict[str, str]] = Field(
         alias="platform-builders", default=None
     )
-    security_scan: SecurityScanConfig = Field(
-        SecurityScanConfig(), alias="security-scan"
+    security_scan: GlobalSecurityScanConfig = Field(
+        GlobalSecurityScanConfig(), alias="security-scan"
     )
 
     @field_validator("ssh_keys", mode="before")
     @classmethod
     def transform_ssh_keys(cls, val) -> Optional[List[dict]]:
         if not isinstance(val, dict):
             return val
```

### Comparing `buildrunner-3.6.982/buildrunner/config/models_step.py` & `buildrunner-3.7.991/buildrunner/config/models_step.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,22 @@
         raise ValueError(f"Invalid artifact type: {value}")
     return value
 
 
 AnnotatedArtifact = Annotated[Any, BeforeValidator(_validate_artifact_type)]
 
 
+class StepPushSecurityScanConfig(BaseModel, extra="forbid"):
+    enabled: Optional[bool] = None
+    scanner: Optional[str] = None
+    version: Optional[str] = None
+    config: Optional[dict] = None
+    max_score_threshold: Optional[float] = Field(None, alias="max-score-threshold")
+
+
 class StepTask(BaseModel, extra="forbid"):
     """
     Used for type checking.
     """
 
 
 class StepPypiPush(StepTask):
@@ -169,14 +177,17 @@
     repository: str
     add_build_tag: bool = True
     tags: Optional[List[str]] = Field(
         None,
         min_length=1,
     )
     push: bool
+    security_scan: Optional[StepPushSecurityScanConfig] = Field(
+        None, alias="security-scan"
+    )
 
 
 class Step(BaseModel, extra="forbid"):
     """Step model"""
 
     # A build specified as a string is handled in the field validator
     build: Optional[StepBuild] = None
```

### Comparing `buildrunner-3.6.982/buildrunner/config/validation.py` & `buildrunner-3.7.991/buildrunner/config/validation.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/__init__.py` & `buildrunner-3.7.991/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/builder.py` & `buildrunner-3.7.991/buildrunner/docker/builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/daemon.py` & `buildrunner-3.7.991/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/image_info.py` & `buildrunner-3.7.991/buildrunner/docker/image_info.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/importer.py` & `buildrunner-3.7.991/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/docker/multiplatform_image_builder.py` & `buildrunner-3.7.991/buildrunner/docker/multiplatform_image_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Adobe
+Copyright 2024 Adobe
 All Rights Reserved.
 
 NOTICE: Adobe permits you to use, modify, and distribute this file in accordance
 with the terms of the Adobe license agreement accompanying it.
 """
 import logging
 import os
@@ -20,14 +20,15 @@
 from python_on_whales import docker
 from retry import retry
 
 from buildrunner.config import BuildRunnerConfig
 from buildrunner.config.models import MP_LOCAL_REGISTRY
 from buildrunner.docker import get_dockerfile
 from buildrunner.docker.image_info import BuiltImageInfo, BuiltTaggedImage
+from buildrunner.errors import BuildRunnerConfigurationError
 
 
 LOGGER = logging.getLogger(__name__)
 OUTPUT_LINE = "-----------------------------------------------------------------"
 IMAGE_PREFIX = "buildrunner-mp"
 
 PUSH_TIMEOUT = 300
@@ -114,14 +115,20 @@
         """
         Starts a local docker registry container
 
         Returns:
             str: The name of the registry container
         """
         if not self._local_registry_is_running:
+            if os.getenv("BUILDRUNNER_CONTAINER"):
+                raise BuildRunnerConfigurationError(
+                    "Multiplatform builds cannot be used in the buildrunner Docker image without "
+                    "a 'build-registry' configured in the global buildrunner configuration."
+                )
+
             LOGGER.debug("Starting local docker registry")
             image = "registry"
             if self._docker_registry:
                 image = f"{self._docker_registry}/{image}"
             container = docker.run(image, detach=True, publish_all=True)
             ports = container.network_settings.ports
```

### Comparing `buildrunner-3.6.982/buildrunner/docker/runner.py` & `buildrunner-3.7.991/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/errors.py` & `buildrunner-3.7.991/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/loggers.py` & `buildrunner-3.7.991/buildrunner/loggers.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/provisioners/__init__.py` & `buildrunner-3.7.991/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/provisioners/salt.py` & `buildrunner-3.7.991/buildrunner/provisioners/salt.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/provisioners/shell.py` & `buildrunner-3.7.991/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.7.991/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/sshagent/__init__.py` & `buildrunner-3.7.991/buildrunner/sshagent/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/__init__.py` & `buildrunner-3.7.991/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import time
 from typing import Dict, List, Optional
 
 import yaml
 
 import buildrunner.docker
 from buildrunner.config import BuildRunnerConfig
-from buildrunner.config.models import SecurityScanConfig
-from buildrunner.config.models_step import StepPushCommit
+from buildrunner.config.models import GlobalSecurityScanConfig
+from buildrunner.config.models_step import StepPushCommit, StepPushSecurityScanConfig
 from buildrunner.docker.image_info import BuiltImageInfo
 from buildrunner.docker.multiplatform_image_builder import MultiplatformImageBuilder
 from buildrunner.docker.runner import DockerRunner
 from buildrunner.errors import (
     BuildRunnerProcessingError,
 )
 from buildrunner.steprunner.tasks import BuildStepRunnerTask
@@ -35,16 +35,18 @@
     """
     Contains the definition for a push repository.
     """
 
     def __init__(
         self,
         repository: str,
-        tags: Optional[List[str]] = None,
+        tags: Optional[List[str]],
+        security_scan: Optional[StepPushSecurityScanConfig],
     ):
+        self.security_scan = security_scan
         # Force a lower-case repo
         repo_lower = repository.lower()
         if repo_lower != repository:
             LOGGER.info(
                 f"Forcing repository to lowercase: {repository} => {repo_lower}"
             )
         self.repository = repo_lower
@@ -76,46 +78,60 @@
             timeout=step_runner.build_runner.docker_timeout,
         )
         self._commit_only = commit_only
         self._repos = [
             RepoDefinition(
                 push.repository,
                 push.tags,
+                push.security_scan,
             )
             for push in pushes
         ]
 
     def _security_scan_mp(
-        self, built_image: BuiltImageInfo, log_image_ref: str
+        self,
+        built_image: BuiltImageInfo,
+        log_image_ref: str,
+        push_security_scan: Optional[StepPushSecurityScanConfig],
     ) -> Dict[str, dict]:
         """
         Does a security scan for each built image in a multiplatform image.
         :param built_image: the multiplatform built image info
         :param log_image_ref: the image label to log
+        :param push_security_scan: the optional security scan overrides
         :return: a dictionary of platform names to security scan information (for each built platform image)
         """
         scan_results = {}
         for image in built_image.built_images:
             result = self._security_scan(
                 repository=image.repo,
                 tag=image.tag,
                 log_image_ref=f"{log_image_ref}:{image.platform}",
                 pull=True,
+                push_security_scan=push_security_scan,
             )
             if result:
                 scan_results[image.platform] = result
         if not scan_results:
             return {}
         return {ARTIFACT_SECURITY_SCAN_KEY: scan_results}
 
-    def _security_scan_single(self, repo: str) -> Dict[str, dict]:
-        tag = BuildRunnerConfig.get_instance().default_tag
+    def _security_scan_single(
+        self,
+        repo: str,
+        tag: str,
+        push_security_scan: Optional[StepPushSecurityScanConfig],
+    ) -> Dict[str, dict]:
         log_image_ref = f"{repo}:{tag}"
         result = self._security_scan(
-            repository=repo, tag=tag, log_image_ref=log_image_ref, pull=False
+            repository=repo,
+            tag=tag,
+            log_image_ref=log_image_ref,
+            pull=False,
+            push_security_scan=push_security_scan,
         )
         if not result:
             return {}
         return {
             ARTIFACT_SECURITY_SCAN_KEY: {
                 MultiplatformImageBuilder.get_native_platform(): result
             }
@@ -124,18 +140,19 @@
     def _security_scan(
         self,
         *,
         repository: str,
         tag: str,
         log_image_ref: str,
         pull: bool,
+        push_security_scan: Optional[StepPushSecurityScanConfig],
     ) -> Optional[dict]:
         # If the security scan is not enabled, do nothing
-        security_scan_config = (
-            BuildRunnerConfig.get_instance().global_config.security_scan
+        security_scan_config = BuildRunnerConfig.get_instance().global_config.security_scan.merge_scan_config(
+            push_security_scan
         )
         if log_image_ref != f"{repository}:{tag}":
             log_image_ref = f"{log_image_ref} ({repository}:{tag})"
         if not security_scan_config.enabled:
             LOGGER.debug(
                 f"Image scanning is disabled, skipping scan of {log_image_ref}"
             )
@@ -153,15 +170,15 @@
                 log_image_ref=log_image_ref,
                 pull=pull,
             )
         raise Exception(f"Unsupported scanner {security_scan_config.scanner}")
 
     @staticmethod
     def _security_scan_trivy_parse_results(
-        security_scan_config: SecurityScanConfig, results: dict
+        security_scan_config: GlobalSecurityScanConfig, results: dict
     ) -> dict:
         max_score = 0
         vulnerabilities = []
         for result in results.get("Results", []):
             if not result.get("Vulnerabilities"):
                 continue
             for cur_vuln in result.get("Vulnerabilities"):
@@ -197,15 +214,15 @@
             "max_score": max_score,
             "vulnerabilities": vulnerabilities,
         }
 
     def _security_scan_trivy(
         self,
         *,
-        security_scan_config: SecurityScanConfig,
+        security_scan_config: GlobalSecurityScanConfig,
         repository: str,
         tag: str,
         log_image_ref: str,
         pull: bool,
     ) -> dict:
         # Pull image for scanning (if not already pulled) so that it can be scanned locally
         if pull:
@@ -336,14 +353,15 @@
                             "docker:image": built_image_ids_str,
                             "docker:repository": repo.repository,
                             "docker:tags": repo.tags,
                             "docker:platforms": built_image_id_with_platforms,
                             **self._security_scan_mp(
                                 built_image,
                                 f"{repo.repository}:{repo.tags[0]}",
+                                repo.security_scan,
                             ),
                         },
                     )
 
             # Tag all images locally for the native platform
             self.step_runner.multi_platform.tag_native_platform(built_image)
 
@@ -406,15 +424,17 @@
                     self.step_runner.build_runner.add_artifact(
                         os.path.join(self.step_runner.name, image_to_use),
                         {
                             "type": "docker-image",
                             "docker:image": image_to_use,
                             "docker:repository": repo.repository,
                             "docker:tags": repo.tags,
-                            **self._security_scan_single(repo.repository),
+                            **self._security_scan_single(
+                                repo.repository, repo.tags[-1], repo.security_scan
+                            ),
                         },
                     )
 
 
 class CommitBuildStepRunnerTask(PushBuildStepRunnerTask):
     """
     Class used to commit the resulting image (either from the build task, or if
```

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.7.991/buildrunner/steprunner/tasks/run.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner/utils.py` & `buildrunner-3.7.991/buildrunner/utils.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner.egg-info/PKG-INFO` & `buildrunner-3.7.991/buildrunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.6.982
+Version: 3.7.991
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -38,15 +38,15 @@
 Requires-Dist: paramiko==3.2.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.4.2
 Requires-Dist: pydantic-core==2.10.1
 Requires-Dist: pygments==2.15.1
 Requires-Dist: pynacl==1.5.0
-Requires-Dist: python-on-whales==0.65.0
+Requires-Dist: python-on-whales==0.70.1
 Requires-Dist: pyyaml==6.0
 Requires-Dist: readme-renderer==37.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: retry2==0.9.5
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.0
@@ -316,15 +316,15 @@
         no-cache: true/false (defaults to false)
 
         # Specify Docker images to consider as cache sources,
         # similar to the --cache-from option used by Docker.
         # Buildrunner will attempt to pull these images from the remote registry.
         # If the pull is unsuccessful, buildrunner will still pass in the image name
         # into --cache-from, allowing a cache check in the host machine cache
-        # NOTE: Does not work for multi-platform builds
+        # NOTE: Does not work for multiplatform builds
         cache_from:
           - my-images/image:PR-123
           - my-images/image:latest
 
         # Whether to do a docker pull of the "FROM" image prior to the build.
         # This is critical if you are building from images that are changing
         # with regularity.
@@ -340,19 +340,20 @@
         # This is useful if you are building an image for a different architecture than what
         # buildrunner is running on, such as using a linux/amd64 build node to produce an image
         # with a docker manifest compatible with an Apple M1 linux/arm64/v8 architecture
         platform: linux/amd64
         <or>
         platform: linux/arm64/v8 # an apple m1 architecture
 
-        # To build multi-platform images, add each platform to be built to this list and buildrunner
+        # To build multiplatform images, add each platform to be built to this list and buildrunner
         # will use docker buildx to build and provide a single tag containing all architectures specified.
-        # Note that buildx may be configured to build some platforms with emulation and therefore builds
-        # may take longer with this option specified. Also note that when using the platforms option, it is not
-        # valid to also specify the platform option.
+        # Notes:
+        #  * buildx may be configured to build some platforms with emulation and therefore builds may take longer with this option specified
+        #  * multiplatform builds cannot be used in the buildrunner docker image unless the 'build-registry' global config parameter is specified
+        #  * only one of platform or platforms may be specified
         platforms:
           - linux/amd64
           - linux/arm64/v8
 
         # Specify the build args that should be used when building your image,
         # similar to the --build-args option used by Docker
         buildargs:
@@ -432,15 +433,15 @@
       # Optional step dependency definition to specify which steps need to be processed before this step.
       # The `version` must be present and set to `2.0` or higher for buildrunner to utilize the step dependencies list.
       # An buildrunner error will occur if `depends` is present but `version` is missing or value is lower than `2.0`.
       depends:
         - test-step
         - validation-step
 
-      # This is not supported in the same step as a multi-platform build.
+      # This is not supported in the same step as a multiplatform build.
       run:
         # xfail indicates whether the run operation is expected to fail.  The
         # default is false - the operation is expected to succeed.  If xfail
         # is true and the operation succeeds then it will result in a failure.
         xfail: <boolean>
 
         # A map of additional containers that should be created and linked to
@@ -943,18 +944,31 @@
       build: .
       # To push the docker image to a registry
       push:
         repository: myimages/image1
         # Do not include default build tag
         add_build_tag: false
         tags: [ 'latest' ]
+        # Optional security scan configuration may be provided for each configured push
+        security-scan:
+          # See docs/global-configuration.rst for more information on these attributes.
+          #enabled: false
+          #scanner: "trivy"
+          #version: "latest"
+          # NOTE: Any configuration provided here will be merged with global/command line config
+          #config:
+          #  optional-param: val1
+          # Set to a float to fail the build if the maximum score
+          # is greater than or equal to this number
+          #max-score-threshold: 8.9
       # OR to just commit it locally to use in subsequent steps
       commit:
         repository: myimages/image1
         tags: [ 'latest' ]
+        # NOTE: Image security scans are disabled for images that are not pushed
 
 The configuration may also specify multiple repositories with their own tags
 (each list entry may be a string or specify additional tags):
 
 .. code:: yaml
 
   steps:
@@ -1047,17 +1061,24 @@
 
 This must never be used on a shared server such as a build server as it could
 cause port mapping conflicts.
 
 Image Security Scans
 ====================
 
-Pushed docker images may be automatically scanned for vulnerabilities using the ``security-scan``
-global configuration options or the ``--security-scan-*`` command line options that may override
-the global configuration.  Just set ``security-scan.enabled`` to true to enable automatic scans.
+Pushed docker images may be automatically scanned for vulnerabilities using (in priority order):
+
+* The ``security-scan`` configuration on ``push`` step attributes
+* The ``--security-scan-*`` command line options
+* The ``security-scan`` global configuration options
+
+Just set ``security-scan.enabled`` to true to enable automatic scans. The config specified on the
+command line options overrides the global config completely, but configuration on the push step
+attribute is merged with the command line/global config. Additionally note that the ``cache-dir``
+can only be configured on the global/command line level.
 
 The ``max-score-threshold`` may also be configured to fail the build if the max score of the
 detected vulnerabilities is greater than or equal to the ``max-score-threshold`` value. This
 score is the CVSS v3 score that ranges between 0 (none) to 10.0 (most critical).
 
 Any detected vulnerabilities are added to the ``artifacts.json`` file per Docker image platform,
 along with the detected maximum vulnerability score.
```

### Comparing `buildrunner-3.6.982/buildrunner.egg-info/SOURCES.txt` & `buildrunner-3.7.991/buildrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/buildrunner.egg-info/requires.txt` & `buildrunner-3.7.991/buildrunner.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 paramiko==3.2.0
 pkginfo==1.9.6
 pycparser==2.21
 pydantic==2.4.2
 pydantic-core==2.10.1
 pygments==2.15.1
 pynacl==1.5.0
-python-on-whales==0.65.0
+python-on-whales==0.70.1
 pyyaml==6.0
 readme-renderer==37.3
 requests==2.31.0
 requests-toolbelt==1.0.0
 retry2==0.9.5
 rfc3986==2.0.0
 rich==13.7.0
```

### Comparing `buildrunner-3.6.982/requirements.txt` & `buildrunner-3.7.991/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     # via pydantic
 pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pynacl==1.5.0
     # via paramiko
-python-on-whales==0.65.0
+python-on-whales==0.70.1
     # via -r requirements.in
 pyyaml==6.0
     # via -r requirements.in
 readme-renderer==37.3
     # via twine
 requests==2.31.0
     # via
```

### Comparing `buildrunner-3.6.982/setup.py` & `buildrunner-3.7.991/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import subprocess
 import sys
 import types
 
 from setuptools import setup, find_packages
 
 
-BASE_VERSION = "3.6"
+BASE_VERSION = "3.7"
 
 SOURCE_DIR = os.path.dirname(os.path.abspath(__file__))
 BUILDRUNNER_DIR = os.path.join(SOURCE_DIR, "buildrunner")
 VERSION_FILE = os.path.join(BUILDRUNNER_DIR, "version.py")
 
 THIS_DIR = os.path.dirname(__file__)
```

### Comparing `buildrunner-3.6.982/test_requirements.txt` & `buildrunner-3.7.991/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_buildrunner_files.py` & `buildrunner-3.7.991/tests/test_buildrunner_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,26 @@
         # Override platform to amd
         return ["--platform", "linux/amd64"]
 
     if file_name == "test-local-images-and-platform.yaml":
         # Override platform to amd and use local images
         return ["--local-images", "--platform", "linux/amd64"]
 
+    if file_name == "test-security-scan.yaml":
+        # Override to enable security scanning
+        return ["--security-scan-enabled", "true"]
+
     # No additional args for this test file
     return None
 
 
 def _get_exit_code(file_name: str) -> int:
+    if file_name.startswith("test-xfail-security-scan"):
+        return 1
+
     if file_name.startswith("test-xfail"):
         return os.EX_CONFIG
 
     if file_name.startswith("test-inject-nonexistent-dir"):
         return os.EX_CONFIG
 
     if file_name.startswith("test-docker-pull-failure"):
```

### Comparing `buildrunner-3.6.982/tests/test_caching.py` & `buildrunner-3.7.991/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_cli.py` & `buildrunner-3.7.991/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_dependencies.py` & `buildrunner-3.7.991/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_image_info.py` & `buildrunner-3.7.991/tests/test_image_info.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_loggers.py` & `buildrunner-3.7.991/tests/test_loggers.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_multiplatform.py` & `buildrunner-3.7.991/tests/test_multiplatform.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_push_artifact.py` & `buildrunner-3.7.991/tests/test_push_artifact.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_push_security_scan.py` & `buildrunner-3.7.991/tests/test_push_security_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from unittest import mock
 
 import pytest
 import yaml
 
-from buildrunner.config.models import SecurityScanConfig
+from buildrunner.config.models import GlobalSecurityScanConfig
 from buildrunner.errors import BuildRunnerProcessingError
 from buildrunner.steprunner.tasks import push
 
 
 @pytest.fixture(name="config_mock")
 def fixture_config_mock():
     with mock.patch(
@@ -33,132 +33,160 @@
 
     self_mock = mock.MagicMock()
     self_mock._security_scan.side_effect = (
         lambda **kwargs: None
         if kwargs["repository"] == "repo2"
         else {"image": kwargs["repository"]}
     )
+    push_security_scan = mock.MagicMock()
 
     assert push.PushBuildStepRunnerTask._security_scan_mp(
-        self_mock, image_info, "image_ref1"
+        self_mock,
+        image_info,
+        "image_ref1",
+        push_security_scan,
     ) == {
         "docker:security-scan": {
             "platform1": {"image": "repo1"},
             "platform3": {"image": "repo3"},
         }
     }
     assert self_mock._security_scan.call_args_list == [
         mock.call(
             repository="repo1",
             tag="tag1",
             log_image_ref="image_ref1:platform1",
             pull=True,
+            push_security_scan=push_security_scan,
         ),
         mock.call(
             repository="repo2",
             tag="tag2",
             log_image_ref="image_ref1:platform2",
             pull=True,
+            push_security_scan=push_security_scan,
         ),
         mock.call(
             repository="repo3",
             tag="tag3",
             log_image_ref="image_ref1:platform3",
             pull=True,
+            push_security_scan=push_security_scan,
         ),
     ]
 
 
 def test__security_scan_mp_empty():
     image_info = mock.MagicMock()
     image_info.built_images = [_generate_built_image(num) for num in range(1, 4)]
 
     self_mock = mock.MagicMock()
     self_mock._security_scan.return_value = None
 
     assert not push.PushBuildStepRunnerTask._security_scan_mp(
-        self_mock, image_info, "image_ref1"
+        self_mock,
+        image_info,
+        "image_ref1",
+        None,
     )
 
 
 @mock.patch(
     "buildrunner.steprunner.tasks.push.MultiplatformImageBuilder.get_native_platform"
 )
-def test__security_scan_single(get_native_platform_mock, config_mock):
+def test__security_scan_single(get_native_platform_mock):
     get_native_platform_mock.return_value = "platform1"
-    config_mock.default_tag = "abc123"
     self_mock = mock.MagicMock()
     self_mock._security_scan.return_value = {"result": True}
-    assert push.PushBuildStepRunnerTask._security_scan_single(self_mock, "repo1") == {
-        "docker:security-scan": {"platform1": {"result": True}}
-    }
+    push_security_scan = mock.MagicMock()
+
+    assert push.PushBuildStepRunnerTask._security_scan_single(
+        self_mock, "repo1", "abc123", push_security_scan
+    ) == {"docker:security-scan": {"platform1": {"result": True}}}
     self_mock._security_scan.assert_called_once_with(
-        repository="repo1", tag="abc123", log_image_ref="repo1:abc123", pull=False
+        repository="repo1",
+        tag="abc123",
+        log_image_ref="repo1:abc123",
+        pull=False,
+        push_security_scan=push_security_scan,
     )
 
 
 @mock.patch(
     "buildrunner.steprunner.tasks.push.MultiplatformImageBuilder.get_native_platform"
 )
-def test__security_scan_single_empty(get_native_platform_mock, config_mock):
+def test__security_scan_single_empty(get_native_platform_mock):
     get_native_platform_mock.return_value = "platform1"
-    config_mock.default_tag = "abc123"
     self_mock = mock.MagicMock()
     self_mock._security_scan.return_value = None
-    assert push.PushBuildStepRunnerTask._security_scan_single(self_mock, "repo1") == {}
+    assert (
+        push.PushBuildStepRunnerTask._security_scan_single(
+            self_mock, "repo1", "abc123", None
+        )
+        == {}
+    )
     self_mock._security_scan.assert_called_once()
 
 
 def test__security_scan_scanner_disabled(config_mock):
-    config_mock.global_config.security_scan = SecurityScanConfig(enabled=False)
+    config_mock.global_config.security_scan = GlobalSecurityScanConfig(enabled=False)
     self_mock = mock.MagicMock()
     assert not push.PushBuildStepRunnerTask._security_scan(
         self_mock,
         repository="repo1",
         tag="tag1",
         log_image_ref="image1",
         pull=False,
+        push_security_scan=None,
     )
     self_mock._security_scan_trivy.assert_not_called()
 
 
 def test__security_scan_scanner_trivy(config_mock):
-    config_mock.global_config.security_scan = SecurityScanConfig(
-        enabled=True, scanner="trivy"
-    )
+    security_scan_mock = mock.MagicMock()
+    merged_config_mock = mock.MagicMock()
+    config_mock.global_config.security_scan = security_scan_mock
+    security_scan_mock.merge_scan_config.return_value = merged_config_mock
+    merged_config_mock.enabled = True
+    merged_config_mock.scanner = "trivy"
+    push_security_scan = mock.MagicMock()
+
     self_mock = mock.MagicMock()
     self_mock._security_scan_trivy.return_value = {"result": True}
     assert push.PushBuildStepRunnerTask._security_scan(
         self_mock,
         repository="repo1",
         tag="tag1",
         log_image_ref="image1",
         pull=False,
+        push_security_scan=push_security_scan,
     ) == {"result": True}
     self_mock._security_scan_trivy.assert_called_once_with(
-        security_scan_config=config_mock.global_config.security_scan,
+        security_scan_config=merged_config_mock,
         repository="repo1",
         tag="tag1",
         log_image_ref="image1 (repo1:tag1)",
         pull=False,
     )
+    security_scan_mock.merge_scan_config.assert_called_once_with(push_security_scan)
 
 
 def test__security_scan_scanner_unsupported(config_mock):
-    config_mock.global_config.security_scan = SecurityScanConfig(
+    config_mock.global_config.security_scan = GlobalSecurityScanConfig(
         enabled=True, scanner="bogus"
     )
     self_mock = mock.MagicMock()
     with pytest.raises(Exception) as exc_info:
         assert push.PushBuildStepRunnerTask._security_scan(
             self_mock,
             repository="repo1",
             tag="tag1",
             log_image_ref="image1",
             pull=False,
+            push_security_scan=None,
         ) == {"result": True}
     assert "Unsupported scanner" in str(exc_info.value)
     self_mock._security_scan_trivy.assert_not_called()
 
 
 @pytest.mark.parametrize(
     "input_results, parsed_results",
@@ -211,15 +239,15 @@
                     }
                 ],
             },
         ),
     ],
 )
 def test__security_scan_trivy_parse_results(input_results, parsed_results):
-    security_scan_config = SecurityScanConfig()
+    security_scan_config = GlobalSecurityScanConfig()
     assert (
         push.PushBuildStepRunnerTask._security_scan_trivy_parse_results(
             security_scan_config, input_results
         )
         == parsed_results
     )
 
@@ -231,15 +259,15 @@
         (2.11, False),
         (2.1, True),
     ],
 )
 def test__security_scan_trivy_parse_results_max_score_threshold(
     max_score_threshold, exception_raised
 ):
-    security_scan_config = SecurityScanConfig(
+    security_scan_config = GlobalSecurityScanConfig(
         **{"max-score-threshold": max_score_threshold}
     )
     input_results = {
         "Results": [
             {
                 "Vulnerabilities": [
                     {
@@ -291,15 +319,15 @@
     os_mock.getgid.return_value = "234"
 
     run_path = tmp_path / "run"
     run_path.mkdir()
     tempfile_mock.TemporaryDirectory.return_value.__enter__.return_value = str(run_path)
 
     config_mock.global_config.docker_registry = "registry1"
-    security_scan_config = SecurityScanConfig()
+    security_scan_config = GlobalSecurityScanConfig()
     self_mock = mock.MagicMock()
     self_mock._security_scan_trivy_parse_results.return_value = {"parsed_results": True}
     config_mock.global_config.temp_dir = str(tmp_path)
 
     def _call_run(command, **kwargs):
         _ = kwargs
         if command.startswith("trivy --config"):
@@ -366,15 +394,15 @@
         security_scan_config, {"results": True}
     )
 
 
 @mock.patch("buildrunner.steprunner.tasks.push.DockerRunner")
 def test__security_scan_trivy_failure(docker_runner_mock, config_mock, tmp_path):
     config_mock.global_config.docker_registry = "registry1"
-    security_scan_config = SecurityScanConfig()
+    security_scan_config = GlobalSecurityScanConfig()
     self_mock = mock.MagicMock()
     config_mock.global_config.temp_dir = str(tmp_path)
     docker_runner_mock.return_value.run.return_value = 1
 
     with pytest.raises(BuildRunnerProcessingError, match="Could not scan"):
         push.PushBuildStepRunnerTask._security_scan_trivy(
             self_mock,
@@ -394,15 +422,15 @@
 
 
 @mock.patch("buildrunner.steprunner.tasks.push.DockerRunner")
 def test__security_scan_trivy_file_not_created(
     docker_runner_mock, config_mock, tmp_path
 ):
     config_mock.global_config.docker_registry = "registry1"
-    security_scan_config = SecurityScanConfig()
+    security_scan_config = GlobalSecurityScanConfig()
     self_mock = mock.MagicMock()
     config_mock.global_config.temp_dir = str(tmp_path)
     docker_runner_mock.return_value.run.return_value = 0
 
     with pytest.raises(BuildRunnerProcessingError, match="does not exist"):
         push.PushBuildStepRunnerTask._security_scan_trivy(
             self_mock,
@@ -420,15 +448,15 @@
     tempfile_mock, docker_runner_mock, config_mock, tmp_path
 ):
     run_path = tmp_path / "run"
     run_path.mkdir()
     tempfile_mock.TemporaryDirectory.return_value.__enter__.return_value = str(run_path)
 
     config_mock.global_config.docker_registry = "registry1"
-    security_scan_config = SecurityScanConfig()
+    security_scan_config = GlobalSecurityScanConfig()
     self_mock = mock.MagicMock()
     config_mock.global_config.temp_dir = str(tmp_path)
 
     def _call_run(command, **kwargs):
         _ = kwargs
         if command.startswith("trivy --config"):
             (run_path / "results.json").write_text("{}")
```

### Comparing `buildrunner-3.6.982/tests/test_runner.py` & `buildrunner-3.7.991/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_util_checksum.py` & `buildrunner-3.7.991/tests/test_util_checksum.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_utils_flock.py` & `buildrunner-3.7.991/tests/test_utils_flock.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.6.982/tests/test_version.py` & `buildrunner-3.7.991/tests/test_version.py`

 * *Files identical despite different names*

