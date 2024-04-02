# Comparing `tmp/pipxu-1.4.tar.gz` & `tmp/pipxu-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipxu-1.4.tar", last modified: Tue Apr  2 01:19:18 2024, max compression
+gzip compressed data, was "pipxu-1.5.tar", last modified: Tue Apr  2 07:09:05 2024, max compression
```

## Comparing `pipxu-1.4.tar` & `pipxu-1.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pipxu-1.4/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-02-24 11:57:27.000000 pipxu-1.4/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      441 2024-03-29 00:15:14.000000 pipxu-1.4/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    14459 2024-04-02 01:19:18.885772 pipxu-1.4/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    13936 2024-04-02 01:08:56.000000 pipxu-1.4/README.md
--rwxr-xr-x   0 mark      (1000) mark      (1000)      258 2024-03-29 22:26:39.000000 pipxu-1.4/bootstrap.sh
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-03-29 00:15:14.000000 pipxu-1.4/pipxu/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-03-29 00:15:14.000000 pipxu-1.4/pipxu/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:11:43.000000 pipxu-1.4/pipxu/commands/inject.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4305 2024-04-02 01:08:36.000000 pipxu-1.4/pipxu/commands/install.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1369 2024-04-02 01:11:56.000000 pipxu-1.4/pipxu/commands/list.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1097 2024-04-02 01:12:02.000000 pipxu-1.4/pipxu/commands/reinstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2166 2024-04-02 01:12:09.000000 pipxu-1.4/pipxu/commands/reinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      957 2024-04-02 01:12:18.000000 pipxu-1.4/pipxu/commands/runpip.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:12:24.000000 pipxu-1.4/pipxu/commands/uninject.py
--rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-02 01:12:29.000000 pipxu-1.4/pipxu/commands/uninstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)      875 2024-04-02 01:12:35.000000 pipxu-1.4/pipxu/commands/uninstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-02 01:12:41.000000 pipxu-1.4/pipxu/commands/upgrade-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1368 2024-04-02 01:12:46.000000 pipxu-1.4/pipxu/commands/upgrade.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-02 01:12:52.000000 pipxu-1.4/pipxu/commands/version.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5646 2024-04-02 01:13:11.000000 pipxu-1.4/pipxu/pipxu.py
--rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-02 01:13:16.000000 pipxu-1.4/pipxu/run.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9670 2024-04-02 01:13:23.000000 pipxu-1.4/pipxu/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    14459 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      648 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1042 2024-03-29 05:04:28.000000 pipxu-1.4/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-02 01:19:18.885772 pipxu-1.4/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 07:09:05.577780 pipxu-1.5/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pipxu-1.5/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-02-24 11:57:27.000000 pipxu-1.5/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      441 2024-03-29 00:15:14.000000 pipxu-1.5/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    14488 2024-04-02 07:09:05.577780 pipxu-1.5/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    13965 2024-04-02 05:52:36.000000 pipxu-1.5/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 07:09:05.574447 pipxu-1.5/pipxu/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-03-29 00:15:14.000000 pipxu-1.5/pipxu/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-03-29 00:15:14.000000 pipxu-1.5/pipxu/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 07:09:05.577780 pipxu-1.5/pipxu/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:11:43.000000 pipxu-1.5/pipxu/commands/inject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4305 2024-04-02 01:08:36.000000 pipxu-1.5/pipxu/commands/install.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1369 2024-04-02 01:11:56.000000 pipxu-1.5/pipxu/commands/list.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1097 2024-04-02 01:12:02.000000 pipxu-1.5/pipxu/commands/reinstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2178 2024-04-02 03:40:36.000000 pipxu-1.5/pipxu/commands/reinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      957 2024-04-02 01:12:18.000000 pipxu-1.5/pipxu/commands/runpip.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:12:24.000000 pipxu-1.5/pipxu/commands/uninject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-02 01:12:29.000000 pipxu-1.5/pipxu/commands/uninstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      875 2024-04-02 01:12:35.000000 pipxu-1.5/pipxu/commands/uninstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-02 01:12:41.000000 pipxu-1.5/pipxu/commands/upgrade-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1357 2024-04-02 03:44:39.000000 pipxu-1.5/pipxu/commands/upgrade.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-02 01:12:52.000000 pipxu-1.5/pipxu/commands/version.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5786 2024-04-02 04:45:36.000000 pipxu-1.5/pipxu/pipxu.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-02 01:13:16.000000 pipxu-1.5/pipxu/run.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9979 2024-04-02 04:44:36.000000 pipxu-1.5/pipxu/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 07:09:05.577780 pipxu-1.5/pipxu.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    14488 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      675 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-02 07:09:05.000000 pipxu-1.5/pipxu.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1042 2024-04-02 03:15:29.000000 pipxu-1.5/pyproject.toml
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 07:09:05.577780 pipxu-1.5/scripts/
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      258 2024-04-02 03:17:38.000000 pipxu-1.5/scripts/bootstrap.sh
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      436 2024-04-02 03:36:35.000000 pipxu-1.5/scripts/pipxu-pudb
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-02 07:09:05.577780 pipxu-1.5/setup.cfg
```

### Comparing `pipxu-1.4/PKG-INFO` & `pipxu-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.4
+Version: 1.5
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -29,19 +29,19 @@
 the popular [`pipx`][pipx] tool but is **much faster** because it uses
 [`uv`][uv] to create and install application virtual environments
 instead of [`venv`][venv] and [`pip`][pip] as used by [`pipx`][pipx].
 The [`pipxu`][pipxu] code has been developed completely independently of
 [`pipx`][pipx] and is not a fork. For compatibility and ease of
 migration, the provided commands have the same names as [`pipx`][pipx].
 Most commands are implemented, at least for common use cases, although
-some command functionality, options, and output are different.
+some command functionality, options, and output are slightly different.
 
-This utility was developed and tested on Linux. It may work on other
-platforms, such as Windows and macOS, but has not been tried there.
-The latest documentation and code is available at
+This utility has been developed and tested on Linux. It may work on
+other platforms, such as Windows and macOS, but has not been tried
+there. The latest documentation and code is available at
 https://github.com/bulletmark/pipxu.
 
 ## Usage
 
 Type `pipxu` or `pipxu -h` to view the usage summary:
 
 ```
@@ -300,20 +300,20 @@
 
 ```sh
 curl -LsSf https://astral.sh/uv/install.sh | sh
 ```
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
-script](https://github.com/bulletmark/pipxu/blob/main/bootstrap.sh)
+script](https://github.com/bulletmark/pipxu/blob/main/scripts/bootstrap.sh)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
 ```
-$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/bootstrap.sh | sh
+$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/scripts/bootstrap.sh | sh
 ```
 
 To upgrade:
 
 ```
 $ pipxu upgrade pipxu
 ```
@@ -406,15 +406,15 @@
 `~/.config/pipxu-flags.conf`. If that file exists then each line of
 options will be concatenated and automatically prepended to your `pipxu`
 command line arguments. Comments in the file (i.e. `#` and anything
 after on a line) are ignored. Type `pipxu` to see all supported options.
 
 The global options: `--uv`, `--no-man-pages`, `--home`, `--bin-dir`,
 `--man-dir`, `--default-python`, are the only sensible candidates to
-consider setting as a default.
+consider setting as defaults.
 
 ## License
 
 Copyright (C) 2024 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
 General Public License as published by the Free Software Foundation,
```

### Comparing `pipxu-1.4/README.md` & `pipxu-1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 the popular [`pipx`][pipx] tool but is **much faster** because it uses
 [`uv`][uv] to create and install application virtual environments
 instead of [`venv`][venv] and [`pip`][pip] as used by [`pipx`][pipx].
 The [`pipxu`][pipxu] code has been developed completely independently of
 [`pipx`][pipx] and is not a fork. For compatibility and ease of
 migration, the provided commands have the same names as [`pipx`][pipx].
 Most commands are implemented, at least for common use cases, although
-some command functionality, options, and output are different.
+some command functionality, options, and output are slightly different.
 
-This utility was developed and tested on Linux. It may work on other
-platforms, such as Windows and macOS, but has not been tried there.
-The latest documentation and code is available at
+This utility has been developed and tested on Linux. It may work on
+other platforms, such as Windows and macOS, but has not been tried
+there. The latest documentation and code is available at
 https://github.com/bulletmark/pipxu.
 
 ## Usage
 
 Type `pipxu` or `pipxu -h` to view the usage summary:
 
 ```
@@ -285,20 +285,20 @@
 
 ```sh
 curl -LsSf https://astral.sh/uv/install.sh | sh
 ```
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
-script](https://github.com/bulletmark/pipxu/blob/main/bootstrap.sh)
+script](https://github.com/bulletmark/pipxu/blob/main/scripts/bootstrap.sh)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
 ```
-$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/bootstrap.sh | sh
+$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/scripts/bootstrap.sh | sh
 ```
 
 To upgrade:
 
 ```
 $ pipxu upgrade pipxu
 ```
@@ -391,15 +391,15 @@
 `~/.config/pipxu-flags.conf`. If that file exists then each line of
 options will be concatenated and automatically prepended to your `pipxu`
 command line arguments. Comments in the file (i.e. `#` and anything
 after on a line) are ignored. Type `pipxu` to see all supported options.
 
 The global options: `--uv`, `--no-man-pages`, `--home`, `--bin-dir`,
 `--man-dir`, `--default-python`, are the only sensible candidates to
-consider setting as a default.
+consider setting as defaults.
 
 ## License
 
 Copyright (C) 2024 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
 General Public License as published by the Free Software Foundation,
```

### Comparing `pipxu-1.4/pipxu/commands/inject.py` & `pipxu-1.5/pipxu/commands/inject.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/install.py` & `pipxu-1.5/pipxu/commands/install.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/list.py` & `pipxu-1.5/pipxu/commands/list.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/reinstall-all.py` & `pipxu-1.5/pipxu/commands/reinstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/reinstall.py` & `pipxu-1.5/pipxu/commands/reinstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             shutil.copyfile(vdir / args._freeze_file, tfile)
 
             # Recreate the vdir
             if not run(f'uv venv{venv_args} {vdir}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to recreate {vdir} for {pkgname}.'
 
-            if not utils.piprun(vdir, f'sync{pip_args} {tfile}'):
+            if not utils.piprun(vdir, f'sync{pip_args} --reinstall {tfile}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to resync {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
```

### Comparing `pipxu-1.4/pipxu/commands/runpip.py` & `pipxu-1.5/pipxu/commands/runpip.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/uninject.py` & `pipxu-1.5/pipxu/commands/uninject.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/uninstall-all.py` & `pipxu-1.5/pipxu/commands/uninstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/uninstall.py` & `pipxu-1.5/pipxu/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/upgrade-all.py` & `pipxu-1.5/pipxu/commands/upgrade-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/commands/upgrade.py` & `pipxu-1.5/pipxu/commands/upgrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to upgrade')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
-    pip_args = utils.make_args((args.verbose, '-v'), (True, '-U'))
+    pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
         data = utils.get_json(vdir, args) or {}
         editpath = data.get('editpath')
         pkg = f'-e {editpath}' if editpath else pkgname
         extras = ' '.join(data.get('injected', []))
-        if not utils.piprun(vdir, f'install --reinstall'
+        if not utils.piprun(vdir, f'install --reinstall -U'
                             f'{pip_args} {pkg} {extras}'):
             return f'Error: failed to {args.name} {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
```

### Comparing `pipxu-1.4/pipxu/commands/version.py` & `pipxu-1.5/pipxu/commands/version.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/pipxu.py` & `pipxu-1.5/pipxu/pipxu.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,23 +139,26 @@
     # Keep some useful info in the namespace passed to the command
     args._uv = uv
     args._packages_dir = home_dir / 'packages'
     args._packages_dir.mkdir(parents=True, exist_ok=True)
     args._venvs_dir = home_dir / 'venvs'
     args._venvs_dir.mkdir(parents=True, exist_ok=True)
     args._bin_dir = bin_dir
+    args._bin_dir.mkdir(parents=True, exist_ok=True)
     args._man_dir = man_dir
+    if not args.no_man_pages:
+        args._man_dir.mkdir(parents=True, exist_ok=True)
     args._pyexe = pyexe
     args._prog = PROG
     args._meta_file = f'{PROG}_metadata.json'
     args._freeze_file = f'{PROG}_freeze.txt'
     if not hasattr(args, 'verbose'):
         args.verbose = False
 
-    # Purge any old venvs left lying around
-    utils.purge_old_venvs(args)
+    # Purge any old files left lying around
+    utils.purge_old_files(args)
 
     # Run the command that the user specified
     return args.func(args)
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `pipxu-1.4/pipxu/run.py` & `pipxu-1.5/pipxu/run.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.4/pipxu/utils.py` & `pipxu-1.5/pipxu/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,18 @@
             print(f'Linking {srcfile} -> {tgtfile}')
 
         tgtfile.parent.mkdir(parents=True, exist_ok=True)
         tgtfile.symlink_to(srcfile)
 
 def _unlink_all_files(vdir: Path, args: Namespace) -> None:
     'Unlink all link files'
-    for srcdir, pat in ((args._bin_dir, '*'), (args._man_dir, '*/*')):
+    dirlist = [(args._bin_dir, '*')]
+    if args._man_dir.is_dir():
+        dirlist.append((args._man_dir, '*/*'))
+    for srcdir, pat in dirlist:
         if srcdir.is_dir():
             for file in srcdir.glob(pat):
                 if file.is_symlink() and vdir in file.resolve().parents:
                     if args.verbose:
                         print(f'Removing link {file}')
                     file.unlink()
 
@@ -228,16 +231,16 @@
     'Remove the given path'
     print(f'Purging stray {path}', file=sys.stderr)
     if path.is_dir():
         shutil.rmtree(path)
     else:
         path.unlink()
 
-def purge_old_venvs(args: Namespace) -> None:
-    'Clean out any old virtual environments and package names'
+def purge_old_files(args: Namespace) -> None:
+    'Clean out any old virtual environments, packages, and executables'
     # Remove any packages that do not point to a dir in the venvs directory
     valids_venvs = set()
     for pkg in args._packages_dir.iterdir():
         vdir = pkg.resolve()
         if vdir.parent != args._venvs_dir or not vdir.is_dir() \
                 or not vdir.name.isdigit():
             rm_path(pkg)
@@ -245,14 +248,20 @@
             valids_venvs.add(vdir.name)
 
     # Remove any venvs that are not in the packages directory
     for vdir in args._venvs_dir.iterdir():
         if vdir.name not in valids_venvs:
             rm_path(vdir)
 
+    # Remove any executables that point to a non-existent path
+    for exe in args._bin_dir.iterdir():
+        rexe = exe.resolve()
+        if args._venvs_dir in rexe.parents and not rexe.exists():
+            rm_path(exe)
+
 def get_all_package_names(args: Namespace) -> list[str]:
     'Return a sorted list of all package names'
     return sorted(set(f.name for f in args._packages_dir.iterdir())
                   - set(args.skip or []))
 
 def get_python(args: Namespace) -> str:
     'Return the python executable based on command line args'
```

### Comparing `pipxu-1.4/pipxu.egg-info/PKG-INFO` & `pipxu-1.5/pipxu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.4
+Version: 1.5
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -29,19 +29,19 @@
 the popular [`pipx`][pipx] tool but is **much faster** because it uses
 [`uv`][uv] to create and install application virtual environments
 instead of [`venv`][venv] and [`pip`][pip] as used by [`pipx`][pipx].
 The [`pipxu`][pipxu] code has been developed completely independently of
 [`pipx`][pipx] and is not a fork. For compatibility and ease of
 migration, the provided commands have the same names as [`pipx`][pipx].
 Most commands are implemented, at least for common use cases, although
-some command functionality, options, and output are different.
+some command functionality, options, and output are slightly different.
 
-This utility was developed and tested on Linux. It may work on other
-platforms, such as Windows and macOS, but has not been tried there.
-The latest documentation and code is available at
+This utility has been developed and tested on Linux. It may work on
+other platforms, such as Windows and macOS, but has not been tried
+there. The latest documentation and code is available at
 https://github.com/bulletmark/pipxu.
 
 ## Usage
 
 Type `pipxu` or `pipxu -h` to view the usage summary:
 
 ```
@@ -300,20 +300,20 @@
 
 ```sh
 curl -LsSf https://astral.sh/uv/install.sh | sh
 ```
 
 Note [`pipxu` is on PyPI](https://pypi.org/project/pipxu/). Run the tiny
 [bootstrap shell
-script](https://github.com/bulletmark/pipxu/blob/main/bootstrap.sh)
+script](https://github.com/bulletmark/pipxu/blob/main/scripts/bootstrap.sh)
 which installs `pipxu` to a temporary directory then runs `pipxu` from
 there to install itself normally.
 
 ```
-$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/bootstrap.sh | sh
+$ curl -LsSf https://raw.githubusercontent.com/bulletmark/pipxu/main/scripts/bootstrap.sh | sh
 ```
 
 To upgrade:
 
 ```
 $ pipxu upgrade pipxu
 ```
@@ -406,15 +406,15 @@
 `~/.config/pipxu-flags.conf`. If that file exists then each line of
 options will be concatenated and automatically prepended to your `pipxu`
 command line arguments. Comments in the file (i.e. `#` and anything
 after on a line) are ignored. Type `pipxu` to see all supported options.
 
 The global options: `--uv`, `--no-man-pages`, `--home`, `--bin-dir`,
 `--man-dir`, `--default-python`, are the only sensible candidates to
-consider setting as a default.
+consider setting as defaults.
 
 ## License
 
 Copyright (C) 2024 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
 General Public License as published by the Free Software Foundation,
```

### Comparing `pipxu-1.4/pipxu.egg-info/SOURCES.txt` & `pipxu-1.5/pipxu.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .flake8
 .gitignore
 Makefile
 README.md
-bootstrap.sh
 pyproject.toml
 pipxu/__init__.py
 pipxu/__main__.py
 pipxu/pipxu.py
 pipxu/run.py
 pipxu/utils.py
 pipxu.egg-info/PKG-INFO
@@ -22,8 +21,10 @@
 pipxu/commands/reinstall.py
 pipxu/commands/runpip.py
 pipxu/commands/uninject.py
 pipxu/commands/uninstall-all.py
 pipxu/commands/uninstall.py
 pipxu/commands/upgrade-all.py
 pipxu/commands/upgrade.py
-pipxu/commands/version.py
+pipxu/commands/version.py
+scripts/bootstrap.sh
+scripts/pipxu-pudb
```

### Comparing `pipxu-1.4/pyproject.toml` & `pipxu-1.5/pyproject.toml`

 * *Files identical despite different names*

