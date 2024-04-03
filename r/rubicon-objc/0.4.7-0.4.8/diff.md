# Comparing `tmp/rubicon-objc-0.4.7.tar.gz` & `tmp/rubicon-objc-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-objc-0.4.7.tar", last modified: Thu Oct 19 03:27:44 2023, max compression
+gzip compressed data, was "rubicon-objc-0.4.8.tar", last modified: Wed Apr  3 05:07:38 2024, max compression
```

## Comparing `rubicon-objc-0.4.7.tar` & `rubicon-objc-0.4.8.tar`

### file list

```diff
@@ -1,113 +1,112 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.767685 rubicon-objc-0.4.7/
--rw-r--r--   0 runner     (501) staff       (20)       71 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.git-blame-ignore-revs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.724080 rubicon-objc-0.4.7/.github/
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.726569 rubicon-objc-0.4.7/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     2035 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/workflows/ci.yml
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/workflows/dependabot-changenote.yml
--rw-r--r--   0 runner     (501) staff       (20)      257 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/workflows/pre-commit-update.yml
--rw-r--r--   0 runner     (501) staff       (20)      740 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/workflows/publish.yml
--rw-r--r--   0 runner     (501) staff       (20)     1891 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      158 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      837 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)      707 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.readthedocs.yml
--rw-r--r--   0 runner     (501) staff       (20)      842 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/.travis.yml
--rw-r--r--   0 runner     (501) staff       (20)      140 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/CHANGELOG.rst
--rw-r--r--   0 runner     (501) staff       (20)      181 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner     (501) staff       (20)     3278 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      656 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5363 2023-10-19 03:27:44.767467 rubicon-objc-0.4.7/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3411 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.727595 rubicon-objc-0.4.7/changes/
--rw-r--r--   0 runner     (501) staff       (20)       12 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/changes/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      792 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/changes/template.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.730012 rubicon-objc-0.4.7/docs/
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.714365 rubicon-objc-0.4.7/docs/_mocked_modules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.731048 rubicon-objc-0.4.7/docs/_mocked_modules/ctypes/
--rw-r--r--   0 runner     (501) staff       (20)    10469 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/_mocked_modules/ctypes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/_mocked_modules/ctypes/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.714775 rubicon-objc-0.4.7/docs/_static/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.731680 rubicon-objc-0.4.7/docs/_static/images/
--rw-r--r--   0 runner     (501) staff       (20)    22360 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/_static/images/rubicon.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.734871 rubicon-objc-0.4.7/docs/background/
--rw-r--r--   0 runner     (501) staff       (20)     1045 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/community.rst
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/faq.rst
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    27741 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/releases.rst
--rw-r--r--   0 runner     (501) staff       (20)       18 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/roadmap.rst
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/background/success.rst
--rw-r--r--   0 runner     (501) staff       (20)    10851 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/conf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.739573 rubicon-objc-0.4.7/docs/how-to/
--rw-r--r--   0 runner     (501) staff       (20)     3667 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/async.rst
--rw-r--r--   0 runner     (501) staff       (20)    21084 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/c-functions.rst
--rw-r--r--   0 runner     (501) staff       (20)     4934 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/contribute-code.rst
--rw-r--r--   0 runner     (501) staff       (20)     2656 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/contribute-docs.rst
--rw-r--r--   0 runner     (501) staff       (20)      511 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/get-started.rst
--rw-r--r--   0 runner     (501) staff       (20)      490 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/index.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.740568 rubicon-objc-0.4.7/docs/how-to/internal/
--rw-r--r--   0 runner     (501) staff       (20)      229 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/internal/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4264 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/internal/release.rst
--rw-r--r--   0 runner     (501) staff       (20)     4699 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/memory-management.rst
--rw-r--r--   0 runner     (501) staff       (20)     3802 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/protocols.rst
--rw-r--r--   0 runner     (501) staff       (20)    15036 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/how-to/type-mapping.rst
--rw-r--r--   0 runner     (501) staff       (20)     1504 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/index.rst
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/make.bat
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.743671 rubicon-objc-0.4.7/docs/reference/
--rw-r--r--   0 runner     (501) staff       (20)      448 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    20168 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/rubicon-objc-api.rst
--rw-r--r--   0 runner     (501) staff       (20)      791 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/rubicon-objc-eventloop.rst
--rw-r--r--   0 runner     (501) staff       (20)     5641 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/rubicon-objc-runtime.rst
--rw-r--r--   0 runner     (501) staff       (20)    15405 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/rubicon-objc-types.rst
--rw-r--r--   0 runner     (501) staff       (20)     3418 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/reference/rubicon-objc.rst
--rw-r--r--   0 runner     (501) staff       (20)      476 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/spelling_wordlist
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.745159 rubicon-objc-0.4.7/docs/tutorial/
--rw-r--r--   0 runner     (501) staff       (20)      506 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/tutorial/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4624 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/tutorial/tutorial-1.rst
--rw-r--r--   0 runner     (501) staff       (20)     4891 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/docs/tutorial/tutorial-2.rst
--rw-r--r--   0 runner     (501) staff       (20)     1019 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1709 2023-10-19 03:27:44.768597 rubicon-objc-0.4.7/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.716856 rubicon-objc-0.4.7/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.716623 rubicon-objc-0.4.7/src/rubicon/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.749155 rubicon-objc-0.4.7/src/rubicon/objc/
--rw-r--r--   0 runner     (501) staff       (20)     3540 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    97912 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/api.py
--rw-r--r--   0 runner     (501) staff       (20)    13945 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/collections.py
--rw-r--r--   0 runner     (501) staff       (20)    10066 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)    24377 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/eventloop.py
--rw-r--r--   0 runner     (501) staff       (20)    42297 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/runtime.py
--rw-r--r--   0 runner     (501) staff       (20)    31846 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/src/rubicon/objc/types.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.751673 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5363 2023-10-19 03:27:44.000000 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2367 2023-10-19 03:27:44.000000 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-10-19 03:27:44.000000 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      332 2023-10-19 03:27:44.000000 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2023-10-19 03:27:44.000000 rubicon-objc-0.4.7/src/rubicon_objc.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.755849 rubicon-objc-0.4.7/tests/
--rw-r--r--   0 runner     (501) staff       (20)      492 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-19 03:27:44.764326 rubicon-objc-0.4.7/tests/objc/
--rw-r--r--   0 runner     (501) staff       (20)      104 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Altered_Example.h
--rw-r--r--   0 runner     (501) staff       (20)       85 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Altered_Example.m
--rw-r--r--   0 runner     (501) staff       (20)      567 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/BaseExample.h
--rw-r--r--   0 runner     (501) staff       (20)     1331 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/BaseExample.m
--rw-r--r--   0 runner     (501) staff       (20)      929 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Blocks.h
--rw-r--r--   0 runner     (501) staff       (20)     1239 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Blocks.m
--rw-r--r--   0 runner     (501) staff       (20)      264 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Callback.h
--rw-r--r--   0 runner     (501) staff       (20)      392 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/DescriptionTester.h
--rw-r--r--   0 runner     (501) staff       (20)      641 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/DescriptionTester.m
--rw-r--r--   0 runner     (501) staff       (20)     2558 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Example.h
--rw-r--r--   0 runner     (501) staff       (20)     4767 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Example.m
--rw-r--r--   0 runner     (501) staff       (20)      593 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Makefile
--rw-r--r--   0 runner     (501) staff       (20)      197 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Protocols.h
--rw-r--r--   0 runner     (501) staff       (20)      104 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/SpecificExample.h
--rw-r--r--   0 runner     (501) staff       (20)      394 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/SpecificExample.m
--rw-r--r--   0 runner     (501) staff       (20)      328 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Thing.h
--rw-r--r--   0 runner     (501) staff       (20)      711 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/objc/Thing.m
--rw-r--r--   0 runner     (501) staff       (20)    11932 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_NSArray.py
--rw-r--r--   0 runner     (501) staff       (20)    13268 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_NSDictionary.py
--rw-r--r--   0 runner     (501) staff       (20)    16420 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_NSString.py
--rw-r--r--   0 runner     (501) staff       (20)     5871 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_async.py
--rw-r--r--   0 runner     (501) staff       (20)     8086 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_blocks.py
--rw-r--r--   0 runner     (501) staff       (20)    69806 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_core.py
--rw-r--r--   0 runner     (501) staff       (20)     4369 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tests/test_ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)     1988 2023-10-19 03:26:38.000000 rubicon-objc-0.4.7/tox.ini
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.894561 rubicon-objc-0.4.8/
+-rw-r--r--   0 runner     (501) staff       (20)       71 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.git-blame-ignore-revs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.844670 rubicon-objc-0.4.8/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      377 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.848033 rubicon-objc-0.4.8/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     2386 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner     (501) staff       (20)      281 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/config-file-deps-bump.yml
+-rw-r--r--   0 runner     (501) staff       (20)      230 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/dependabot-changenote.yml
+-rw-r--r--   0 runner     (501) staff       (20)      257 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/pre-commit-update.yml
+-rw-r--r--   0 runner     (501) staff       (20)      740 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      158 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      855 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      707 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/.readthedocs.yml
+-rw-r--r--   0 runner     (501) staff       (20)      140 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/CHANGELOG.rst
+-rw-r--r--   0 runner     (501) staff       (20)      182 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0 runner     (501) staff       (20)     3278 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     5714 2024-04-03 05:07:38.893824 rubicon-objc-0.4.8/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3411 2024-04-03 05:06:50.000000 rubicon-objc-0.4.8/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.849081 rubicon-objc-0.4.8/changes/
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/changes/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      792 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/changes/template.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.851839 rubicon-objc-0.4.8/docs/
+-rw-r--r--   0 runner     (501) staff       (20)      728 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/Makefile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.835752 rubicon-objc-0.4.8/docs/_mocked_modules/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.852902 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/
+-rw-r--r--   0 runner     (501) staff       (20)    10469 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.836190 rubicon-objc-0.4.8/docs/_static/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.853464 rubicon-objc-0.4.8/docs/_static/images/
+-rw-r--r--   0 runner     (501) staff       (20)    22360 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/_static/images/rubicon.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.856880 rubicon-objc-0.4.8/docs/background/
+-rw-r--r--   0 runner     (501) staff       (20)     1045 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/community.rst
+-rw-r--r--   0 runner     (501) staff       (20)      826 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/faq.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    28855 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/releases.rst
+-rw-r--r--   0 runner     (501) staff       (20)       18 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/roadmap.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/background/success.rst
+-rw-r--r--   0 runner     (501) staff       (20)    10989 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/conf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.861678 rubicon-objc-0.4.8/docs/how-to/
+-rw-r--r--   0 runner     (501) staff       (20)     3667 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/async.rst
+-rw-r--r--   0 runner     (501) staff       (20)    21047 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/c-functions.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4934 2024-04-03 05:06:51.000000 rubicon-objc-0.4.8/docs/how-to/contribute-code.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4159 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/contribute-docs.rst
+-rw-r--r--   0 runner     (501) staff       (20)      508 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/get-started.rst
+-rw-r--r--   0 runner     (501) staff       (20)      490 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/index.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.862809 rubicon-objc-0.4.8/docs/how-to/internal/
+-rw-r--r--   0 runner     (501) staff       (20)      229 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/internal/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4264 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/internal/release.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4699 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/memory-management.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3709 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/protocols.rst
+-rw-r--r--   0 runner     (501) staff       (20)    14675 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/how-to/type-mapping.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)      933 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/make.bat
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.866447 rubicon-objc-0.4.8/docs/reference/
+-rw-r--r--   0 runner     (501) staff       (20)      448 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    20276 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-api.rst
+-rw-r--r--   0 runner     (501) staff       (20)      791 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-eventloop.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5641 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-runtime.rst
+-rw-r--r--   0 runner     (501) staff       (20)    15405 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc-types.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3418 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/reference/rubicon-objc.rst
+-rw-r--r--   0 runner     (501) staff       (20)      493 2024-04-03 05:06:52.000000 rubicon-objc-0.4.8/docs/spelling_wordlist
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.867983 rubicon-objc-0.4.8/docs/tutorial/
+-rw-r--r--   0 runner     (501) staff       (20)      506 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4506 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/tutorial-1.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5518 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/docs/tutorial/tutorial-2.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3126 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-03 05:07:38.894728 rubicon-objc-0.4.8/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.838425 rubicon-objc-0.4.8/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.838160 rubicon-objc-0.4.8/src/rubicon/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.872398 rubicon-objc-0.4.8/src/rubicon/objc/
+-rw-r--r--   0 runner     (501) staff       (20)     3656 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)   100198 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/api.py
+-rw-r--r--   0 runner     (501) staff       (20)    13945 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/collections.py
+-rw-r--r--   0 runner     (501) staff       (20)    10066 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)    24378 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/eventloop.py
+-rw-r--r--   0 runner     (501) staff       (20)    42343 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/runtime.py
+-rw-r--r--   0 runner     (501) staff       (20)    31846 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/src/rubicon/objc/types.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.889200 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5714 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2377 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      432 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2024-04-03 05:07:38.000000 rubicon-objc-0.4.8/src/rubicon_objc.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.879645 rubicon-objc-0.4.8/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      492 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 05:07:38.888573 rubicon-objc-0.4.8/tests/objc/
+-rw-r--r--   0 runner     (501) staff       (20)      104 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/Altered_Example.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/Altered_Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      567 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/BaseExample.h
+-rw-r--r--   0 runner     (501) staff       (20)     1331 2024-04-03 05:06:53.000000 rubicon-objc-0.4.8/tests/objc/BaseExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      929 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Blocks.h
+-rw-r--r--   0 runner     (501) staff       (20)     1239 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Blocks.m
+-rw-r--r--   0 runner     (501) staff       (20)      264 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Callback.h
+-rw-r--r--   0 runner     (501) staff       (20)      392 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/DescriptionTester.h
+-rw-r--r--   0 runner     (501) staff       (20)      641 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/DescriptionTester.m
+-rw-r--r--   0 runner     (501) staff       (20)     2558 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Example.h
+-rw-r--r--   0 runner     (501) staff       (20)     4767 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      593 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)      197 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Protocols.h
+-rw-r--r--   0 runner     (501) staff       (20)      104 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/SpecificExample.h
+-rw-r--r--   0 runner     (501) staff       (20)      394 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/SpecificExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      328 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Thing.h
+-rw-r--r--   0 runner     (501) staff       (20)      711 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/objc/Thing.m
+-rw-r--r--   0 runner     (501) staff       (20)    11932 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSArray.py
+-rw-r--r--   0 runner     (501) staff       (20)    13268 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSDictionary.py
+-rw-r--r--   0 runner     (501) staff       (20)    16420 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_NSString.py
+-rw-r--r--   0 runner     (501) staff       (20)     5843 2024-04-03 05:06:54.000000 rubicon-objc-0.4.8/tests/test_async.py
+-rw-r--r--   0 runner     (501) staff       (20)     8086 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_blocks.py
+-rw-r--r--   0 runner     (501) staff       (20)    74860 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_core.py
+-rw-r--r--   0 runner     (501) staff       (20)     4369 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tests/test_ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)     2508 2024-04-03 05:06:55.000000 rubicon-objc-0.4.8/tox.ini
```

### Comparing `rubicon-objc-0.4.7/.github/workflows/ci.yml` & `rubicon-objc-0.4.8/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -36,34 +36,49 @@
 
   unit-tests:
     name: Unit tests
     needs: [pre-commit, towncrier, package]
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
+      fail-fast: false
       matrix:
-        platform: [ "macOS-11", "macOS-12", "macOS-13" ]
-        python-version: [ "3.8", "3.9", "3.10", "3.11", "3.12-dev" ]
+        platform: [
+          # X86-64 runners
+          "macos-11", "macos-12", "macos-13",
+          # M1 runners
+          "macos-14"
+        ]
+        python-version: [ "3.8", "3.9", "3.10", "3.11", "3.12", "3.13-dev" ]
         include:
           - experimental: false
-          - python-version: "3.12-dev"
+          - python-version: "3.13-dev"
             experimental: true
+
+        exclude:
+          # actions/setup-python doesn't provide Python3.8 or 3.9 for M1.
+          - platform: "macos-14"
+            python-version : "3.8"
+
+          - platform: "macos-14"
+            python-version : "3.9"
+
     steps:
     - name: Checkout
-      uses: actions/checkout@v4.1.0
+      uses: actions/checkout@v4.1.2
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.7.1
+      uses: actions/setup-python@v5.1.0
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Get packages
-      uses: actions/download-artifact@v3.0.2
+      uses: actions/download-artifact@v4.1.4
       with:
         name: ${{ needs.package.outputs.artifact-name }}
         path: dist
 
     - name: Install dev dependencies
       run: |
         # We don't actually want to install rubicon;
```

### Comparing `rubicon-objc-0.4.7/.github/workflows/publish.yml` & `rubicon-objc-0.4.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/.github/workflows/release.yml` & `rubicon-objc-0.4.8/.github/workflows/release.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,33 +5,41 @@
     tags:
       - "v*"
 
 jobs:
   ci:
     uses: ./.github/workflows/ci.yml
 
+  docs:
+    name: Verify Docs Build
+    uses: beeware/.github/.github/workflows/docs-build-verify.yml@main
+    secrets: inherit
+    with:
+      project-name: "rubicon-objc"
+      project-version: ${{ github.ref_name }}
+
   release:
     name: Create Release
     needs: ci
     # This has to be run on macOS, because rubicon tries to load the Foundation library
     runs-on: macOS-latest
     permissions:
       contents: write
     steps:
       - name: Set build variables
         run: |
           echo "VERSION=${GITHUB_REF_NAME#v}" >> $GITHUB_ENV
 
       - name: Set up Python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: "3.X"
 
       - name: Get packages
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.4
         with:
           name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
 
       - name: Install packages
         run: pip install dist/rubicon_objc-*.whl
 
@@ -39,32 +47,32 @@
         # Check that the setuptools_scm-generated version number is still the same when
         # installed from a wheel with setuptools_scm not present.
         run: |
           set -x
           test $(python -c "from rubicon.objc import __version__; print(__version__)") = $VERSION
 
       - name: Create Release
-        uses: ncipollo/release-action@v1.13.0
+        uses: ncipollo/release-action@v1.14.0
         with:
           name: ${{ env.VERSION }}
           draft: true
           artifacts: dist/*
           artifactErrorsFailBuild: true
 
   test-publish:
     name: Publish test package
-    needs: [ci, release]
+    needs: [ci, docs, release]
     runs-on: ubuntu-latest
     permissions:
       contents: write
       # This permission is required for trusted publishing.
       id-token: write
     steps:
       - name: Get packages
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.4
         with:
           name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
 
       - name: Publish release to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `rubicon-objc-0.4.7/.pre-commit-config.yaml` & `rubicon-objc-0.4.8/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
       - id: check-toml
       - id: check-yaml
       - id: check-case-conflict
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         additional_dependencies: [toml]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
-  - repo: https://github.com/psf/black
-    rev: 23.9.1
+  - repo: https://github.com/psf/black-pre-commit-mirror
+    rev: 24.3.0
     hooks:
     - id: black
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
     - id: codespell
       additional_dependencies:
```

### Comparing `rubicon-objc-0.4.7/.readthedocs.yml` & `rubicon-objc-0.4.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/LICENSE` & `rubicon-objc-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/PKG-INFO` & `rubicon-objc-0.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.7
+Version: 0.4.8
 Summary: A bridge between an Objective C runtime environment and Python.
-Home-page: https://beeware.org/rubicon
-Author: Russell Keith-Magee
-Author-email: russell@keith-magee.com
+Author-email: Russell Keith-Magee <russell@keith-magee.com>
+Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
+Project-URL: Homepage, https://beeware.org/rubicon
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/beeware/rubicon-objc/issues
 Project-URL: Source, https://github.com/beeware/rubicon-objc
+Keywords: macOS,iOS,Objective C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Objective C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: pre-commit==3.5.0; extra == "dev"
-Requires-Dist: pytest==7.4.2; extra == "dev"
+Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-tldr==0.2.5; extra == "dev"
-Requires-Dist: setuptools_scm[toml]==8.0.4; extra == "dev"
-Requires-Dist: tox==4.11.3; extra == "dev"
+Requires-Dist: setuptools_scm==8.0.4; extra == "dev"
+Requires-Dist: tox==4.14.2; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2023.9.10; extra == "docs"
+Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
 Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
-Requires-Dist: sphinx_tabs==3.4.1; extra == "docs"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
+Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
+Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
 .. image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
     :width: 72px
     :target: https://beeware.org/rubicon
```

### Comparing `rubicon-objc-0.4.7/README.rst` & `rubicon-objc-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/changes/template.rst` & `rubicon-objc-0.4.8/changes/template.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/Makefile` & `rubicon-objc-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/_mocked_modules/ctypes/__init__.py` & `rubicon-objc-0.4.8/docs/_mocked_modules/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/_static/images/rubicon.png` & `rubicon-objc-0.4.8/docs/_static/images/rubicon.png`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/background/community.rst` & `rubicon-objc-0.4.8/docs/background/community.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/background/faq.rst` & `rubicon-objc-0.4.8/docs/background/faq.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/background/releases.rst` & `rubicon-objc-0.4.8/docs/background/releases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,39 @@
 Release History
 ===============
 
 .. towncrier release notes start
 
+0.4.8 (2024-04-03)
+==================
+
+Features
+--------
+
+* Name clashes caused by re-registering Objective C classes and protocols can now be automatically avoided by marking the class with ``auto_rename``. (#181)
+* Apple Silicon is now formally tested by Rubicon's continuous integration configuration. (#374)
+* Support for Python 3.13 was added. (#374)
+* The ``__repr__`` output for  ``ObjCBoundMethod``, ``ObjCClass``, ``ObjCInstance``, ``ObjCMethod``, ``ObjCPartialMethod``, and ``ObjCProtocol`` were simplified. (#432)
+
+Bugfixes
+--------
+
+* The ``__all__`` definition for ``rubicon.objc`` was corrected to use strings, rather than symbols. (#401)
+
+Documentation
+-------------
+
+* The documentation contribution guide was updated to use a more authoritative reStructuredText reference. (#427)
+
+Misc
+----
+
+* #381, #382, #383, #384, #385, #386, #387, #388, #389, #390, #391, #392, #393, #395, #396, #397, #398, #399, #400, #402, #403, #404, #405, #407, #408, #409, #410, #411, #412, #413, #414, #415, #416, #417, #418, #420, #421, #422, #423, #424, #425, #426, #429, #430, #431, #433, #434, #435, #437, #438
+
+
 0.4.7 (2023-10-19)
 ==================
 
 Features
 --------
 
 * The ``__repr__`` and ``__str__`` implementations for ``NSPoint``, ``CGPoint``, ``NSRect``, ``CGRect``, ``NSSize``, ``CGSize``, ``NSRange``, ``CFRange``, ``NSEdgeInsets`` and ``UIEdgeInsets`` have been improved. (`#222 <https://github.com/beeware/rubicon-objc/pulls/222>`_)
@@ -26,15 +53,15 @@
 
 * Support for Python 3.7 was dropped. (`#334 <https://github.com/beeware/rubicon-objc/pulls/334>`_)
 
 
 Documentation
 -------------
 
-* All code blocks were updated to add a button to copy the relevant contents on to the user's clipboard. (`#300 https://github.com/beeware/rubicon-objc/pull/300`_)
+* All code blocks were updated to add a button to copy the relevant contents on to the user's clipboard. (`#300 <https://github.com/beeware/rubicon-objc/pull/300>`_)
 
 
 Misc
 ----
 
 * #295, #296, #297, #298, #299, #301, #302, #303, #305, #306, #307, #310, #311, #312, #314, #315, #319, #320, #321, #326, #327, #328, #329, #330, #331, #332, #335, #336, #337, #338, #341, #342, #343, #344, #345, #346, #348, #349, #350, #351, #353, #354, #355, #356, #358, #359, #360, #361, #362, #363, #364, #365, #366, #367, #368, #369, #370, #371, #372, #373, #375, #376, #377, #378, #379, #380
```

### Comparing `rubicon-objc-0.4.7/docs/conf.py` & `rubicon-objc-0.4.8/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Rubicon"
-copyright = "2014, Russell Keith-Magee"
+copyright = "Russell Keith-Magee"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
 release = metadata_version("rubicon-objc")
@@ -108,14 +108,19 @@
 ]
 
 # 2023-07-10: Github Line number anchors fail link checks when retrieved by robots. This
 # drops the line number anchor from any link checks, but still validates the base URL is
 # valid.
 linkcheck_anchors_ignore = [r"L\d+"]
 
+linkcheck_ignore = [
+    r"^https://github.com/beeware/rubicon-objc/issues/\d+$",
+    r"^https://github.com/beeware/rubicon-objc/pull/\d+$",
+]
+
 # -- Options for copy button ---------------------------------------------------
 
 # virtual env prefix: (venv), (beeware-venv), (testenv)
 venv = r"\((?:(?:beeware-)?venv|testvenv)\)"
 # macOS and Linux shell prompt: $
 shell = r"\$"
 # win CMD prompt: C:\>, C:\...>
```

### Comparing `rubicon-objc-0.4.7/docs/how-to/async.rst` & `rubicon-objc-0.4.8/docs/how-to/async.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/how-to/c-functions.rst` & `rubicon-objc-0.4.8/docs/how-to/c-functions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
 .. code-block:: python
 
     >>> from rubicon.objc import objc_const
     >>> from rubicon.objc.runtime import Foundation
     >>> NSMetadataItemFSNameKey = objc_const(Foundation, "NSMetadataItemFSNameKey")
     >>> NSMetadataItemFSNameKey
-    <rubicon.objc.collections.ObjCStrInstance 0x10eecf350: __NSCFConstantString at 0x1072a67e8: kMDItemFSName>
+    <ObjCStrInstance: __NSCFConstantString at 0x10eecf350: kMDItemFSName>
 
 .. note::
 
     Sometimes it's not obvious that a constant is an Objective-C object,
     because its actual type is hidden behind a ``typedef``. This is common with
     the "extensible string enum" pattern, where a set of related string
     constants are defined together. An example can be found in
```

### Comparing `rubicon-objc-0.4.7/docs/how-to/contribute-code.rst` & `rubicon-objc-0.4.8/docs/how-to/contribute-code.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/how-to/contribute-docs.rst` & `rubicon-objc-0.4.8/docs/how-to/contribute-docs.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Contributing to the documentation
 =================================
 
 Here are some tips for working on this documentation. You're welcome to add
 more and help us out!
 
-First of all, you should check the `Restructured Text (reST) and Sphinx
-CheatSheet <http://thomas-cokelaer.info/tutorials/sphinx/rest_syntax.html>`_ to
+First of all, you should check the `reStructuredText (reST) Primer
+<https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_ to
 learn how to write your ``.rst`` file.
 
 Create a ``.rst`` file
 ----------------------
 
 Look at the structure and choose the best category to put your ``.rst`` file.
 Make sure that it is referenced in the index of the corresponding category,
@@ -104,7 +104,66 @@
 
     .. code-block:: doscon
 
       C:\...>tox -e docs-all
 
 The documentation should be fully rebuilt in the ``docs/_build/html`` folder.
 If there are any markup problems, they'll raise an error.
+
+Live documentation preview
+--------------------------
+
+To support rapid editing of documentation, Rubicon also has a "live preview" mode:
+
+.. tabs::
+
+  .. group-tab:: macOS
+
+    .. code-block:: console
+
+      (venv) $ tox -e docs-live
+
+  .. group-tab:: Linux
+
+    .. code-block:: console
+
+      (venv) $ tox -e docs-live
+
+  .. group-tab:: Windows
+
+    .. code-block:: doscon
+
+      (venv) C:\...>tox -e docs-live
+
+This will build the documentation, start a web server to serve the build documentation,
+and watch the file system for any changes to the documentation source. If a change is
+detected, the documentation will be rebuilt, and any browser viewing the modified page
+will be automatically refreshed.
+
+Live preview mode will only monitor the ``docs`` directory for changes. If you're
+updating the inline documentation associated with Toga source code, you'll need to use
+the ``docs-live-src`` target to build docs:
+
+.. tabs::
+
+  .. group-tab:: macOS
+
+    .. code-block:: console
+
+      (venv) $ tox -e docs-live-src
+
+  .. group-tab:: Linux
+
+    .. code-block:: console
+
+      (venv) $ tox -e docs-live-src
+
+  .. group-tab:: Windows
+
+    .. code-block:: doscon
+
+      (venv) C:\...>tox -e docs-live-src
+
+This behaves the same as ``docs-live``, but will also monitor any changes to the
+``src/rubicon/objc`` folder, reflecting any changes to inline documentation.
+However, the rebuild process takes much longer, so you may not want to use this
+target unless you're actively editing inline documentation.
```

### Comparing `rubicon-objc-0.4.7/docs/how-to/internal/release.rst` & `rubicon-objc-0.4.8/docs/how-to/internal/release.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/how-to/memory-management.rst` & `rubicon-objc-0.4.8/docs/how-to/memory-management.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/how-to/protocols.rst` & `rubicon-objc-0.4.8/docs/how-to/protocols.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Protocol objects can be looked up using the ``ObjCProtocol`` constructor,
 similar to how classes can be looked up using ``ObjCClass``:
 
 .. code-block:: python
 
     >>> NSCopying = ObjCProtocol('NSCopying')
     >>> NSCopying
-    <rubicon.objc.api.ObjCProtocol: NSCopying at 0x7fff76543210>
+    <ObjCProtocol: NSCopying>
 
 The ``isinstance`` function can be used to check whether an object conforms to
 a protocol:
 
 .. code-block:: python
 
     >>> isinstance(NSObject.new(), NSCopying)
@@ -63,17 +63,17 @@
 We can now use our class. The ``copy`` method (which uses our implemented
 ``copyWithZone:`` method) can also be used:
 
 .. code-block:: python
 
     >>> ua = UserAccount.alloc().initWithUsername_emailAddress_(at('person'), at('person@example.com'))
     >>> ua
-    <rubicon.objc.api.ObjCInstance 0x106543210: UserAccount at 0x106543220: <UserAccount: 0x106543220>>
+    <ObjCInstance: UserAccount at 0x106543210: <UserAccount: 0x106543220>>
     >>> ua.copy()
-    <rubicon.objc.api.ObjCInstance 0x106543210: UserAccount at 0x106543220: <UserAccount: 0x106543220>>
+    <ObjCInstance: UserAccount at 0x106543210: <UserAccount: 0x106543220>>
 
 And we can check that the class conforms to the protocol:
 
 .. code-block:: python
 
     >>> isinstance(ua, NSCopying)
     True
```

### Comparing `rubicon-objc-0.4.7/docs/how-to/type-mapping.rst` & `rubicon-objc-0.4.8/docs/how-to/type-mapping.rst`

 * *Files 4% similar despite different names*

```diff
@@ -129,19 +129,19 @@
 other Objective-C and Python strings.
 
 .. code-block:: python
 
     # Call an Objective-C method that returns a string.
     # We're using NSBundle to give us a string version of a path
     >>> NSBundle.mainBundle.bundlePath
-    <rubicon.objc.collections.ObjCStrInstance 0x114a94d68: __NSCFString at 0x7fec8ba7fbd0: /Users/brutus/path/to/somewhere>
+    <ObjCStrInstance: __NSCFString at 0x114a94d68: /Users/brutus/path/to/somewhere>
 
     # Slice the Objective-C string
     >>> NSBundle.mainBundle.bundlePath[:14]
-    <rubicon.objc.collections.ObjCStrInstance 0x114aa80f0: __NSCFString at 0x7fec8ba7fbd0: /Users/brutus/>
+    <ObjCStrInstance: __NSCFString at 0x114aa80f0: /Users/brutus/>
 
 .. note::
 
     :class:`~rubicon.objc.api.ObjCInstance` objects wrapping a
     :class:`~rubicon.objc.api.NSString` internally have the class
     ``ObjCStrInstance``, and you will see this name in the :func:`repr` of
     :class:`~rubicon.objc.api.NSString` objects. This is an implementation
@@ -167,15 +167,15 @@
 .. code-block:: python
 
     >>> from rubicon.objc import at
     # Create a Python string
     >>> py_str = 'hello world'
     # Convert to an Objective-C string
     >>> at(py_str)
-    <rubicon.objc.collections.ObjCStrInstance 0x114a94e48: __NSCFString at 0x7fec8ba7fc10: hello world>
+    <ObjCStrInstance: __NSCFString at 0x114a94e48: hello world>
 
 :class:`~rubicon.objc.api.NSString` also supports all the utility methods that
 are available on :class:`str`, such as ``replace`` and ``split``. When these
 methods return a string, the implementation may return Python :class:`str` or
 Objective-C :class:`~rubicon.objc.api.NSString` instances. If you need to use
 the return value from these methods, you should always use :class:`str` or
 :func:`~rubicon.objc.api.at` to ensure that you have the right kind of string
@@ -212,15 +212,15 @@
 .. code-block:: python
 
     >>> from rubicon.objc import NSArray
     >>> array = NSArray.arrayWithArray(list(range(4)))
     >>> array[0]
     0
     >>> array[1:3]
-    <rubicon.objc.collections.ObjCListInstance 0x10b855208: __NSArrayI at 0x7f86f8e61950: <__NSArrayI 0x7f86f8e61950>(
+    <ObjCListInstance: _NSArrayI at 0x10b855208: <__NSArrayI 0x7f86f8e61950>(
     1,
     2
     )
     >
     >>> len(array)
     4
     >>> 2 in array
@@ -243,24 +243,24 @@
 
 .. code-block:: python
 
     >>> from rubicon.objc import NSMutableArray
     >>> mutarray = NSMutableArray.arrayWithArray(list(range(4)))
     >>> mutarray[0] = 42
     >>> mutarray
-    <rubicon.objc.collections.ObjCMutableListInstance 0x10b8558d0: __NSArrayM at 0x7f86fb04d9f0: <__NSArrayM 0x7f86fb04d9f0>(
+    <ObjCMutableListInstance: __NSArrayM at 0x10b8558d0: <__NSArrayM 0x7f86fb04d9f0>(
     42,
     1,
     2,
     3
     )
     >
     >>> mutarray[1:3] = [9, 8, 7]
     >>> mutarray
-    <rubicon.objc.collections.ObjCMutableListInstance 0x10b8558d0: __NSArrayM at 0x7f86fb04d9f0: <__NSArrayM 0x7f86fb04d9f0>(
+    <ObjCMutableListInstance: __NSArrayM at 0x10b8558d0: <__NSArrayM 0x7f86fb04d9f0>(
     42,
     9,
     8,
     7,
     3
     )
     >
@@ -314,32 +314,32 @@
 mutating operations, like item assignment:
 
 .. code-block:: python
 
     >>> md = objc.NSMutableDictionary.dictionaryWithDictionary({"one": 1, "two": 2})
     >>> md["three"] = 3
     >>> md
-    <rubicon.objc.collections.ObjCMutableDictInstance 0x10b8a7860: __NSDictionaryM at 0x7f86fb164b60: {
+    <ObjCMutableDictInstance: __NSDictionaryM at 0x10b8a7860: {
         one = 1;
         three = 3;
         two = 2;
     }>
 
 Mapping methods like ``keys`` and ``values`` are also supported:
 
 .. code-block:: python
 
     >>> d.keys()
-    <rubicon.objc.collections.ObjCListInstance 0x10b898a90: __NSArrayI at 0x7f86f8db6b70: <__NSArrayI 0x7f86f8db6b70>(
+    <ObjCListInstance: __NSArrayI at 0x10b898a90: <__NSArrayI 0x7f86f8db6b70>(
     one,
     two
     )
     >
     >>> d.values()
-    <rubicon.objc.collections.ObjCListInstance 0x10b8a7b38: __NSArrayI at 0x7f86f8c00370: <__NSArrayI 0x7f86f8c00370>(
+    <ObjCListInstance: __NSArrayI at 0x10b8a7b38: <__NSArrayI 0x7f86f8c00370>(
     1,
     2
     )
     >
 
 .. note::
```

### Comparing `rubicon-objc-0.4.7/docs/index.rst` & `rubicon-objc-0.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/make.bat` & `rubicon-objc-0.4.8/docs/make.bat`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
+	echo.https://sphinx-doc.org/
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :help
```

### Comparing `rubicon-objc-0.4.7/docs/reference/rubicon-objc-api.rst` & `rubicon-objc-0.4.8/docs/reference/rubicon-objc-api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,23 @@
     .. automethod:: __setattr__
 
 .. autofunction:: objc_const
 
 Objective-C classes
 -------------------
 
-.. autoclass:: ObjCClass(name_or_ptr, [bases, attrs, [protocols=()]])
+.. autoclass:: ObjCClass(name_or_ptr, [bases, attrs, [protocols=(), auto_rename=None]])
 
     .. attribute:: name
 
         The name of this class, as a :class:`str`.
 
     .. autoattribute:: superclass
     .. autoattribute:: protocols
+    .. autoattribute:: auto_rename
     .. automethod:: declare_property
     .. automethod:: declare_class_property
     .. automethod:: __instancecheck__
     .. automethod:: __subclasscheck__
 
 .. autoclass:: ObjCMetaClass(name_or_ptr)
 
@@ -316,18 +317,19 @@
         update([other], **kwargs)
 
         Python-style mutable mapping interface.
 
 Objective-C protocols
 ---------------------
 
-.. autoclass:: ObjCProtocol(name_or_ptr, [bases, attrs])
+.. autoclass:: ObjCProtocol(name_or_ptr, [bases, attrs, [auto_rename=None]])
 
     .. autoattribute:: name
     .. autoattribute:: protocols
+    .. autoattribute:: auto_rename
     .. automethod:: __instancecheck__
     .. automethod:: __subclasscheck__
 
 Standard Objective-C and Foundation protocols
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following protocols from the `Objective-C runtime
```

### Comparing `rubicon-objc-0.4.7/docs/reference/rubicon-objc-eventloop.rst` & `rubicon-objc-0.4.8/docs/reference/rubicon-objc-eventloop.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/reference/rubicon-objc-runtime.rst` & `rubicon-objc-0.4.8/docs/reference/rubicon-objc-runtime.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/reference/rubicon-objc-types.rst` & `rubicon-objc-0.4.8/docs/reference/rubicon-objc-types.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/reference/rubicon-objc.rst` & `rubicon-objc-0.4.8/docs/reference/rubicon-objc.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/docs/tutorial/tutorial-1.rst` & `rubicon-objc-0.4.8/docs/tutorial/tutorial-1.rst`

 * *Files 9% similar despite different names*

```diff
@@ -94,29 +94,29 @@
 
 .. code-block:: pycon
 
     >>> longer.description
     'https://beeware.org/contributing/how/first-time/'
 
     >>> longer.debugDescription
-    'https://beeware.org/contributing/how/first-time/>'
+    'https://beeware.org/contributing/how/first-time/'
 
 Internally, ``description`` and ``debugDescription`` are hooked up to their
 Python equivalents, ``__str__()`` and ``__repr__()``, respectively:
 
 .. code-block:: pycon
 
     >>> str(absolute)
-    'https://beeware.org/contributing/how/first-time/'
+    'https://beeware.org/contributing/'
 
     >>> repr(absolute)
-    '<rubicon.objc.api.ObjCInstance 0x1114a3cf8: NSURL at 0x7fb2abdd0b20: https://beeware.org/contributing/>'
+    '<ObjCInstance: NSURL at 0x1114a3cf8: https://beeware.org/contributing/>'
 
     >>> print(absolute)
-    <rubicon.objc.api.ObjCInstance 0x1114a3cf8: NSURL at 0x7fb2abdd0b20: https://beeware.org/contributing/>
+    https://beeware.org/contributing/
 
 Time to take over the world!
 ============================
 
 You now have access to *any* method, on *any* class, in any library, in the
 entire macOS or iOS ecosystem! If you can invoke something in Objective-C, you
 can invoke it in Python - all you need to do is:
```

### Comparing `rubicon-objc-0.4.7/docs/tutorial/tutorial-2.rst` & `rubicon-objc-0.4.8/docs/tutorial/tutorial-2.rst`

 * *Files 10% similar despite different names*

```diff
@@ -106,19 +106,37 @@
 
 .. code-block:: pycon
 
     >>> class Handler(NSObject):
     ...     pass
     Traceback (most recent call last)
     ...
-    RuntimeError: ObjC runtime already contains a registered class named 'Handler'.
+    RuntimeError: An Objective-C class named b'Handler' already exists
 
 You'll need to be careful (and sometimes, painfully verbose) when choosing class
 names.
 
+To allow a class name to be re-used, you can set the class variable
+:attr:`~rubicon.objc.api.ObjCClass.auto_rename` to ``True``. This option enables
+automatic renaming of the Objective C class if a naming collision is detected:
+
+.. code-block:: pycon
+
+    >>> ObjCClass.auto_rename = True
+
+This option can also be enabled on a per-class basis by using the
+``auto_rename`` argument in the class declaration:
+
+.. code-block:: pycon
+
+    >>> class Handler(NSObject, auto_rename=True):
+    ...     pass
+
+If this option is used, the Objective C class name will have a numeric suffix
+(e.g., `Handler_2`). The Python class name will be unchanged.
 What, no ``__init__()``?
 ========================
 
 You'll also notice that our example code *doesn't* have an ``__init__()``
 method like you'd normally expect of Python code. As we're defining an
 Objective-C class, we need to follow the Objective-C object life cycle - which
 means defining initializer methods that are visible to the Objective-C runtime,
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/__init__.py` & `rubicon-objc-0.4.8/src/rubicon/objc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,66 +84,66 @@
     UIEdgeInsetsZero,
     UniChar,
     unichar,
 )
 
 __all__ = [
     "__version__",
-    CFIndex,
-    CFRange,
-    CGFloat,
-    CGGlyph,
-    CGPoint,
-    CGPointMake,
-    CGRect,
-    CGRectMake,
-    CGSize,
-    CGSizeMake,
-    NSEdgeInsets,
-    NSEdgeInsetsMake,
-    NSInteger,
-    NSMakePoint,
-    NSMakeRect,
-    NSMakeSize,
-    NSPoint,
-    NSRange,
-    NSRect,
-    NSSize,
-    NSTimeInterval,
-    NSUInteger,
-    NSZeroPoint,
-    UIEdgeInsets,
-    UIEdgeInsetsMake,
-    UIEdgeInsetsZero,
-    UniChar,
-    unichar,
-    SEL,
-    send_message,
-    send_super,
-    Block,
-    NSArray,
-    NSDictionary,
-    NSMutableArray,
-    NSMutableDictionary,
-    NSObject,
-    NSObjectProtocol,
-    ObjCBlock,
-    ObjCClass,
-    ObjCInstance,
-    ObjCMetaClass,
-    ObjCProtocol,
-    at,
-    ns_from_py,
-    objc_block,
-    objc_classmethod,
-    objc_const,
-    objc_id,
-    objc_ivar,
-    objc_method,
-    objc_property,
-    objc_rawmethod,
-    py_from_ns,
-    api,
-    collections,
-    runtime,
-    types,
+    "CFIndex",
+    "CFRange",
+    "CGFloat",
+    "CGGlyph",
+    "CGPoint",
+    "CGPointMake",
+    "CGRect",
+    "CGRectMake",
+    "CGSize",
+    "CGSizeMake",
+    "NSEdgeInsets",
+    "NSEdgeInsetsMake",
+    "NSInteger",
+    "NSMakePoint",
+    "NSMakeRect",
+    "NSMakeSize",
+    "NSPoint",
+    "NSRange",
+    "NSRect",
+    "NSSize",
+    "NSTimeInterval",
+    "NSUInteger",
+    "NSZeroPoint",
+    "UIEdgeInsets",
+    "UIEdgeInsetsMake",
+    "UIEdgeInsetsZero",
+    "UniChar",
+    "unichar",
+    "SEL",
+    "send_message",
+    "send_super",
+    "Block",
+    "NSArray",
+    "NSDictionary",
+    "NSMutableArray",
+    "NSMutableDictionary",
+    "NSObject",
+    "NSObjectProtocol",
+    "ObjCBlock",
+    "ObjCClass",
+    "ObjCInstance",
+    "ObjCMetaClass",
+    "ObjCProtocol",
+    "at",
+    "ns_from_py",
+    "objc_block",
+    "objc_classmethod",
+    "objc_const",
+    "objc_id",
+    "objc_ivar",
+    "objc_method",
+    "objc_property",
+    "objc_rawmethod",
+    "py_from_ns",
+    "api",
+    "collections",
+    "runtime",
+    "types",
 ]
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/api.py` & `rubicon-objc-0.4.8/src/rubicon/objc/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         self.name = self.selector.name
         self.encoding = libobjc.method_getTypeEncoding(method)
         self.restype, *self.imp_argtypes = ctypes_for_method_encoding(self.encoding)
         assert self.imp_argtypes[:2] == [objc_id, SEL]
         self.method_argtypes = self.imp_argtypes[2:]
 
     def __repr__(self):
-        return f"<ObjCMethod: {self.name} {self.encoding}>"
+        return f"<{type(self).__qualname__}: {self.name.decode()} {self.encoding.decode()}>"
 
     def __call__(self, receiver, *args, convert_args=True, convert_result=True):
         """Call the method on an object with the given arguments.
 
         The passed arguments are automatically converted to the expected
         argument types as needed:
 
@@ -239,15 +239,15 @@
     def __init__(self, name_start):
         super().__init__()
 
         self.name_start = name_start
         self.methods = {}  # Initialized in ObjCClass._load_methods
 
     def __repr__(self):
-        return f"{type(self).__module__}.{type(self).__qualname__}({self.name_start!r})"
+        return f"{type(self).__qualname__}({self.name_start!r})"
 
     def __call__(self, receiver, first_arg=_sentinel, **kwargs):
         if first_arg is ObjCPartialMethod._sentinel:
             if kwargs:
                 raise TypeError("Missing first (positional) argument")
 
             args = []
@@ -281,15 +281,15 @@
         self.method = method
         if type(receiver) is Class:
             self.receiver = cast(receiver, objc_id)
         else:
             self.receiver = receiver
 
     def __repr__(self):
-        return f"{type(self).__module__}.{type(self).__qualname__}({self.method}, {self.receiver})"
+        return f"{type(self).__qualname__}({self.method}, {self.receiver})"
 
     def __call__(self, *args, **kwargs):
         """Call the method with the given arguments."""
         return self.method(self.receiver, *args, **kwargs)
 
 
 def convert_method_arguments(encoding, args):
@@ -991,18 +991,18 @@
         if desc is not None:
             return str(desc)
 
         return repr(self)
 
     def __repr__(self):
         """Get a debugging representation of ``self``, which includes the
-        Objective-C object's address, class, and ``debugDescription``."""
+        Objective-C object's class and ``debugDescription``."""
         return (
-            f"<{type(self).__module__}.{type(self).__qualname__} {id(self):#x}: "
-            f"{self.objc_class.name} at {self.ptr.value:#x}: {self.debugDescription}>"
+            f"<{type(self).__qualname__}: {self.objc_class.name} at "
+            f"{id(self):#x}: {self.debugDescription}>"
         )
 
     def __getattr__(self, name):
         """Allows accessing Objective-C properties and methods using Python
         attribute syntax.
 
         If ``self`` has a Python attribute with the given name, its value is
@@ -1202,14 +1202,18 @@
     def protocols(self):
         """The protocols adopted by this class."""
 
         out_count = c_uint()
         protocols_ptr = libobjc.class_copyProtocolList(self, byref(out_count))
         return tuple(ObjCProtocol(protocols_ptr[i]) for i in range(out_count.value))
 
+    auto_rename = False
+    """A :any:`bool` value describing whether a defined class should be renamed automatically
+    if a class with the same name already exists in the Objective C runtime."""
+
     @classmethod
     def _new_from_name(cls, name):
         name = ensure_bytes(name)
         ptr = get_class(name)
         if ptr.value is None:
             raise NameError(f"ObjC Class {name} couldn't be found.")
 
@@ -1225,19 +1229,28 @@
                 f"Pointer {ptr} ({ptr.value:#x}) does not refer to a class"
             )
         name = libobjc.class_getName(ptr)
 
         return ptr, name
 
     @classmethod
-    def _new_from_class_statement(cls, name, bases, attrs, *, protocols):
+    def _new_from_class_statement(cls, name, bases, attrs, *, protocols, auto_rename):
+        basename = name
         name = ensure_bytes(name)
 
         if get_class(name).value is not None:
-            raise RuntimeError(f"An Objective-C class named {name!r} already exists")
+            if auto_rename or auto_rename is None and cls.auto_rename:
+                suffix = 1
+                while get_class(name).value is not None:
+                    suffix += 1
+                    name = f"{basename}_{suffix}".encode()
+            else:
+                raise RuntimeError(
+                    f"An Objective-C class named {name!r} already exists"
+                )
 
         try:
             (superclass,) = bases
         except ValueError:
             raise ValueError(
                 f"An Objective-C class must have exactly one base class, not {len(bases)}"
             )
@@ -1312,15 +1325,23 @@
         add_method(ptr, "dealloc", _new_delloc, [None, ObjCInstance, SEL])
 
         # Register the ObjC class
         libobjc.objc_registerClassPair(ptr)
 
         return ptr, name, attrs
 
-    def __new__(cls, name_or_ptr, bases=None, attrs=None, *, protocols=()):
+    def __new__(
+        cls,
+        name_or_ptr,
+        bases=None,
+        attrs=None,
+        *,
+        protocols=(),
+        auto_rename=None,
+    ):
         """The constructor accepts either the name of an Objective-C class to
         look up (as :class:`str` or :class:`bytes`), or a pointer to an existing
         class object (in any form accepted by :class:`ObjCInstance`).
 
         If given a pointer, it must refer to an Objective-C class; pointers to
         other objects are not accepted. (Use :class:`ObjCInstance` to wrap a
         pointer that might also refer to other kinds of objects.) If the pointer
@@ -1332,14 +1353,22 @@
         arguments (name, bases list, namespace mapping). This form is called
         implicitly by Python's ``class`` syntax, and is used to create a new
         Objective-C class from Python (see :ref:`custom-classes-and-protocols`).
         The bases list must contain exactly one :class:`ObjCClass` to be
         extended by the new class. An optional ``protocols`` keyword argument is
         also accepted, which must be a sequence of :class:`ObjCProtocol`\\s for
         the new class to adopt.
+
+        If the name of the class has already registered with the Objective C
+        runtime, the ``auto_rename`` option can be used to ensure that the
+        Objective C name for the new class will be unique. A numeric suffix will
+        be appended to the Objective C name to ensure uniqueness (for example,
+        ``MyClass`` will be renamed to ``MyClass_2``, ``MyClass_3`` etc until a
+        unique name is found). By default, classes will *not* be renamed, unless
+        :attr:`ObjCClass.auto_rename` is set at the class level.
         """
 
         if (bases is None) ^ (attrs is None):
             raise TypeError("ObjCClass arguments 2 and 3 must be given together")
 
         if bases is None and attrs is None:
             # A single argument provided. If it's a string, treat it as
@@ -1358,15 +1387,19 @@
                 ptr, name = cls._new_from_ptr(name_or_ptr)
                 if not issubclass(cls, ObjCMetaClass) and libobjc.class_isMetaClass(
                     ptr
                 ):
                     return ObjCMetaClass(ptr)
         else:
             ptr, name, attrs = cls._new_from_class_statement(
-                name_or_ptr, bases, attrs, protocols=protocols
+                name_or_ptr,
+                bases,
+                attrs,
+                protocols=protocols,
+                auto_rename=auto_rename,
             )
 
         objc_class_name = name.decode("utf-8")
 
         new_attrs = {
             "name": objc_class_name,
             "methods_ptr": None,
@@ -1553,15 +1586,15 @@
         This is equivalent to
         ``self.objc_class.declare_property(name)``.
         """
 
         self.objc_class.forced_properties.add(name)
 
     def __repr__(self):
-        return f"<{type(self).__module__}.{type(self).__qualname__}: {self.name} at {self.ptr.value:#x}>"
+        return f"<{type(self).__qualname__}: {self.name}>"
 
     def __str__(self):
         return f"{type(self).__name__}({self.name!r})"
 
     def __del__(self):
         libc.free(self.methods_ptr)
 
@@ -1848,15 +1881,19 @@
     def protocols(self):
         """The protocols that this protocol extends."""
 
         out_count = c_uint()
         protocols_ptr = libobjc.protocol_copyProtocolList(self, byref(out_count))
         return tuple(ObjCProtocol(protocols_ptr[i]) for i in range(out_count.value))
 
-    def __new__(cls, name_or_ptr, bases=None, ns=None):
+    auto_rename = False
+    """A :class:`bool` value whether a defined protocol should be renamed
+    automatically if a protocol with the same name is already exists."""
+
+    def __new__(cls, name_or_ptr, bases=None, ns=None, auto_rename=None):
         """The constructor accepts either the name of an Objective-C protocol
         to look up (as :class:`str` or :class:`bytes`), or a pointer to an
         existing protocol object (in any form accepted by
         :class:`ObjCInstance`).
 
         If given a pointer, it must refer to an Objective-C protocol; pointers
         to other objects are not accepted. (Use :class:`ObjCInstance` to wrap a
@@ -1866,14 +1903,23 @@
         :class:`ObjCProtocol` can also be called like :class:`type`, with three
         arguments (name, bases list, namespace mapping). This form is called
         implicitly by Python's ``class`` syntax, and is used to create a new
         Objective-C protocol from Python (see
         :ref:`custom-classes-and-protocols`). The bases list can contain any
         number of :class:`ObjCProtocol` objects to be extended by the new
         protocol.
+
+        If the name of the protocol has already registered with the Objective C
+        runtime, the ``auto_rename`` option can be used to ensure that the
+        Objective C name for the new protocol will be unique. A numeric suffix
+        will be appended to the Objective C name to ensure uniqueness (for
+        example, ``MyProtocol`` will be renamed to ``MyProtocol_2``,
+        ``MyProtocol_3`` etc until a unique name is found). By default,
+        protocols will *not* be renamed, unless
+        :attr:`ObjCProtocol.auto_rename` is set at the class level.
         """
 
         if (bases is None) ^ (ns is None):
             raise TypeError("ObjCProtocol arguments 2 and 3 must be given together")
 
         if bases is None and ns is None:
             if isinstance(name_or_ptr, (bytes, str)):
@@ -1888,20 +1934,28 @@
                 elif not send_message(
                     ptr, "isKindOfClass:", Protocol, restype=c_bool, argtypes=[objc_id]
                 ):
                     raise ValueError(
                         f"Pointer {ptr} ({ptr.value:#x}) does not refer to a protocol"
                     )
         else:
+            basename = name_or_ptr
             name = ensure_bytes(name_or_ptr)
 
+            # Rename the protocol that will be defined if the auto_rename option is True.
             if libobjc.objc_getProtocol(name).value is not None:
-                raise RuntimeError(
-                    f"An Objective-C protocol named {name!r} already exists"
-                )
+                if auto_rename or auto_rename is None and cls.auto_rename:
+                    suffix = 1
+                    while libobjc.objc_getProtocol(name).value is not None:
+                        suffix += 1
+                        name = f"{basename}_{suffix}".encode()
+                else:
+                    raise RuntimeError(
+                        f"An Objective-C protocol named {name!r} already exists"
+                    )
 
             # Check that all bases are protocols.
             for base in bases:
                 if not isinstance(base, ObjCProtocol):
                     raise TypeError(
                         f"An Objective-C protocol can only extend ObjCProtocol objects, "
                         f"not {type(base).__module__}.{type(base).__qualname__}"
@@ -1923,15 +1977,15 @@
 
             # Register the protocol object
             libobjc.objc_registerProtocol(ptr)
 
         return super().__new__(cls, ptr)
 
     def __repr__(self):
-        return f"<{type(self).__module__}.{type(self).__qualname__}: {self.name} at {self.ptr.value:#x}>"
+        return f"<{type(self).__qualname__}: {self.name}>"
 
     def __instancecheck__(self, instance):
         """Check whether the given object conforms to this protocol.
 
         If the given object is not an Objective-C object, ``False`` is returned.
 
         This method allows using :class:`ObjCProtocol`\\s as the second argument
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/collections.py` & `rubicon-objc-0.4.8/src/rubicon/objc/collections.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/ctypes_patch.py` & `rubicon-objc-0.4.8/src/rubicon/objc/ctypes_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import sys
 import types
 import warnings
 
 # This module relies on the layout of a few internal Python and ctypes
 # structures. Because of this, it's possible (but not all that likely) that
 # things will break on newer/older Python versions.
-if sys.version_info < (3, 6) or sys.version_info >= (3, 13):
+if sys.version_info < (3, 6) or sys.version_info >= (3, 14):
     v = sys.version_info
     warnings.warn(
-        "rubicon.objc.ctypes_patch has only been tested with Python 3.6 through 3.12. "
+        "rubicon.objc.ctypes_patch has only been tested with Python 3.6 through 3.13. "
         f"You are using Python {v.major}.{v.minor}.{v.micro}. Most likely things will "
         "work properly, but you may experience crashes if Python's internals have "
         "changed significantly."
     )
 
 
 # The PyTypeObject struct from "Include/object.h".
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/eventloop.py` & `rubicon-objc-0.4.8/src/rubicon/objc/eventloop.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             kCFSocketReadCallBack | kCFSocketWriteCallBack | kCFSocketConnectCallBack,
             self._callback,
             None,
         )
         libcf.CFSocketSetSocketFlags(
             self._cf_socket,
             kCFSocketAutomaticallyReenableReadCallBack
-            | kCFSocketAutomaticallyReenableWriteCallBack
+            | kCFSocketAutomaticallyReenableWriteCallBack,
             # # This extra flag is to ensure that CF doesn't (destructively,
             # # because destructively is the only way to do it) retrieve
             # # SO_ERROR
             # 1 << 6
         )
         self._src = libcf.CFSocketCreateRunLoopSource(
             kCFAllocatorDefault, self._cf_socket, 0
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/runtime.py` & `rubicon-objc-0.4.8/src/rubicon/objc/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,16 +662,16 @@
     If no class with the given name is loaded, ``None`` is returned, and
     the Objective-C runtime will log a warning message.
     """
 
     return libobjc.objc_getClass(ensure_bytes(name))
 
 
-# http://www.sealiesoftware.com/blog/archive/2008/10/30/objc_explain_objc_msgSend_stret.html
-# http://www.x86-64.org/documentation/abi-0.99.pdf  (pp.17-23)
+# https://www.sealiesoftware.com/blog/archive/2008/10/30/objc_explain_objc_msgSend_stret.html
+# https://web.archive.org/web/20160810184034/http://www.x86-64.org/documentation/abi-0.99.pdf  (pp.17-23)
 # executive summary: on x86-64, who knows?
 def should_use_stret(restype):
     """Return whether a method returning the given type must be called using
     ``objc_msgSend_stret`` on the current system."""
 
     if type(restype) is not type(Structure):
         # Not needed when restype is not a structure.
@@ -689,15 +689,15 @@
         # On ARM32: Use for all structures, regardless of size.
         return True
     else:
         # Other platforms: Doesn't exist.
         return False
 
 
-# http://www.sealiesoftware.com/blog/archive/2008/11/16/objc_explain_objc_msgSend_fpret.html
+# https://www.sealiesoftware.com/blog/archive/2008/11/16/objc_explain_objc_msgSend_fpret.html
 def should_use_fpret(restype):
     """Return whether a method returning the given type must be called using
     ``objc_msgSend_fpret`` on the current system."""
 
     if __x86_64__:
         # On x86_64: Use only for long double.
         return restype == c_longdouble
@@ -855,15 +855,15 @@
 
     _fields_ = [
         ("receiver", objc_id),
         ("super_class", Class),
     ]
 
 
-# http://stackoverflow.com/questions/3095360/what-exactly-is-super-in-objective-c
+# https://stackoverflow.com/questions/3095360/what-exactly-is-super-in-objective-c
 def send_super(
     cls,
     receiver,
     selector,
     *args,
     restype=c_void_p,
     argtypes=None,
```

### Comparing `rubicon-objc-0.4.7/src/rubicon/objc/types.py` & `rubicon-objc-0.4.8/src/rubicon/objc/types.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/src/rubicon_objc.egg-info/PKG-INFO` & `rubicon-objc-0.4.8/src/rubicon_objc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.7
+Version: 0.4.8
 Summary: A bridge between an Objective C runtime environment and Python.
-Home-page: https://beeware.org/rubicon
-Author: Russell Keith-Magee
-Author-email: russell@keith-magee.com
+Author-email: Russell Keith-Magee <russell@keith-magee.com>
+Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
+Project-URL: Homepage, https://beeware.org/rubicon
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/beeware/rubicon-objc/issues
 Project-URL: Source, https://github.com/beeware/rubicon-objc
+Keywords: macOS,iOS,Objective C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Objective C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: pre-commit==3.5.0; extra == "dev"
-Requires-Dist: pytest==7.4.2; extra == "dev"
+Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-tldr==0.2.5; extra == "dev"
-Requires-Dist: setuptools_scm[toml]==8.0.4; extra == "dev"
-Requires-Dist: tox==4.11.3; extra == "dev"
+Requires-Dist: setuptools_scm==8.0.4; extra == "dev"
+Requires-Dist: tox==4.14.2; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2023.9.10; extra == "docs"
+Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
 Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
-Requires-Dist: sphinx_tabs==3.4.1; extra == "docs"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
+Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
+Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.2.4; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
 .. image:: https://beeware.org/project/projects/bridges/rubicon/rubicon.png
     :width: 72px
     :target: https://beeware.org/rubicon
```

### Comparing `rubicon-objc-0.4.7/src/rubicon_objc.egg-info/SOURCES.txt` & `rubicon-objc-0.4.8/src/rubicon_objc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 .git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
-.travis.yml
 CHANGELOG.rst
 CONTRIBUTING.md
 LICENSE
-MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yml
+.github/workflows/config-file-deps-bump.yml
 .github/workflows/dependabot-changenote.yml
 .github/workflows/pre-commit-update.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 changes/.gitignore
 changes/template.rst
 docs/Makefile
```

### Comparing `rubicon-objc-0.4.7/tests/objc/BaseExample.h` & `rubicon-objc-0.4.8/tests/objc/BaseExample.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/BaseExample.m` & `rubicon-objc-0.4.8/tests/objc/BaseExample.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Blocks.h` & `rubicon-objc-0.4.8/tests/objc/Blocks.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Blocks.m` & `rubicon-objc-0.4.8/tests/objc/Blocks.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/DescriptionTester.m` & `rubicon-objc-0.4.8/tests/objc/DescriptionTester.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Example.h` & `rubicon-objc-0.4.8/tests/objc/Example.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Example.m` & `rubicon-objc-0.4.8/tests/objc/Example.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Makefile` & `rubicon-objc-0.4.8/tests/objc/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/objc/Thing.m` & `rubicon-objc-0.4.8/tests/objc/Thing.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/test_NSArray.py` & `rubicon-objc-0.4.8/tests/test_NSArray.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/test_NSDictionary.py` & `rubicon-objc-0.4.8/tests/test_NSDictionary.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/test_NSString.py` & `rubicon-objc-0.4.8/tests/test_NSString.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/test_async.py` & `rubicon-objc-0.4.8/tests/test_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,10 +185,10 @@
         task = asyncio.ensure_future(list_dir(), loop=self.loop)
         self.loop.run_until_complete(task)
 
         # Check for some files that should exist.
         # Everything in the sample set, less everything from the result,
         # should be an empty set.
         self.assertEqual(
-            {"README.rst", "MANIFEST.in", "setup.cfg"} - task.result(),
+            {"README.rst"} - task.result(),
             set(),
         )
```

### Comparing `rubicon-objc-0.4.7/tests/test_blocks.py` & `rubicon-objc-0.4.8/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.7/tests/test_core.py` & `rubicon-objc-0.4.8/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,17 +400,19 @@
 
         with self.assertRaisesRegex(
             ArgumentError,
             r"mutateIntFieldWithValue: argument 3: "
             + (
                 r"TypeError: 'float' object cannot be interpreted as an integer; argtypes: c_int"
                 if sys.version_info >= (3, 12)
-                else r"TypeError: wrong type; argtypes: c_int"
-                if sys.version_info >= (3, 10)
-                else r"<class 'TypeError'>: wrong type; argtypes: c_int"
+                else (
+                    r"TypeError: wrong type; argtypes: c_int"
+                    if sys.version_info >= (3, 10)
+                    else r"<class 'TypeError'>: wrong type; argtypes: c_int"
+                )
             ),
         ):
             obj.mutateIntFieldWithValue_(1.234)
 
     def test_method_incorrect_argument_count_send(self):
         """Attempting to call a method with send_message with an incorrect
         number of arguments throws an exception."""
@@ -980,39 +982,84 @@
             encoding=4,  # NSUTF8StringEncoding
             options=0,
             range=NSRange(0, 7),
             remainingRange=byref(remaining),
         )
         self.assertEqual(buf.value.decode("utf-8"), pystring)
 
+    def test_objcmethod_str_repr(self):
+        """Test ObjCMethod, ObjCPartialMethod, and ObjCBoundMethod str and repr"""
+
+        obj = NSObject.new()
+
+        # ObjCMethod
+        self.assertEqual(repr(obj.init.method), "<ObjCMethod: init @16@0:8>")
+        self.assertEqual(str(obj.init.method), "<ObjCMethod: init @16@0:8>")
+
+        # ObjCBoundMethod
+        self.assertRegex(
+            repr(obj.init),
+            r"ObjCBoundMethod\(<ObjCMethod: init @16@0:8>, <NSObject: 0x[0-9a-f]{12}>\)",
+        )
+        self.assertRegex(
+            str(obj.init),
+            r"ObjCBoundMethod\(<ObjCMethod: init @16@0:8>, <NSObject: 0x[0-9a-f]{12}>\)",
+        )
+
+        # ObjCPartialMethod
+        self.assertEqual(
+            repr(obj.performSelector.method), "ObjCPartialMethod('performSelector')"
+        )
+        self.assertEqual(
+            str(obj.performSelector.method), "ObjCPartialMethod('performSelector')"
+        )
+
     def test_objcinstance_str_repr(self):
         """An ObjCInstance's str and repr contain the object's description and
         debugDescription, respectively."""
 
         DescriptionTester = ObjCClass("DescriptionTester")
         py_description_string = "normal description string"
         py_debug_description_string = "debug description string"
         tester = DescriptionTester.alloc().initWithDescriptionString(
             py_description_string,
             debugDescriptionString=py_debug_description_string,
         )
+
+        # Check str
         self.assertEqual(str(tester), py_description_string)
-        self.assertIn(py_debug_description_string, repr(tester))
+
+        # Check repr
+        self.assertEqual(
+            repr(tester),
+            f"<ObjCInstance: DescriptionTester at {hex(id(tester))}: {py_debug_description_string}>",
+        )
 
     def test_objcinstance_str_repr_with_nil_descriptions(self):
         """An ObjCInstance's str and repr work even if description and
         debugDescription are nil."""
 
         DescriptionTester = ObjCClass("DescriptionTester")
         tester = DescriptionTester.alloc().initWithDescriptionString(
             None, debugDescriptionString=None
         )
         self.assertIsNot(str(tester), None)
         self.assertIsNot(repr(tester), None)
 
+    def test_objcclass_repr(self):
+        """Test ObjCClass repr and str return correct value."""
+
+        self.assertEqual(repr(NSObject), "<ObjCClass: NSObject>")
+        self.assertEqual(str(NSObject), "ObjCClass('NSObject')")
+
+    def test_objcprotocol_repr(self):
+        """Test ObjCProtocol repr return correct value."""
+
+        self.assertEqual(repr(NSObjectProtocol), "<ObjCProtocol: NSObject>")
+
     def test_nspoint_repr(self):
         """Test NSPoint repr and str returns correct value."""
 
         my_point = NSPoint(10, 20)
         self.assertEqual(repr(my_point), "<NSPoint(10.0, 20.0)>")
         self.assertEqual(str(my_point), "(10.0, 20.0)")
 
@@ -1112,14 +1159,123 @@
         # Second definition will raise an error.
         # Without protection, this is a segfault.
         with self.assertRaises(RuntimeError):
 
             class MyClass(NSObject):  # noqa: F811
                 pass
 
+    def test_class_auto_rename_global(self):
+        """Test the global automatic renaming option of ObjCClass."""
+
+        try:
+            ObjCClass.auto_rename = True
+
+            class TestGlobalRenamedClass(NSObject):
+                @objc_method
+                def oldMethod(self):
+                    pass
+
+            class1 = TestGlobalRenamedClass
+
+            class TestGlobalRenamedClass_2(NSObject):
+                pass
+
+            class TestGlobalRenamedClass(NSObject):  # noqa: F811
+                @objc_method
+                def testMethod(self):
+                    return "TEST1"
+
+            # Check that the class was renamed
+            self.assertEqual(TestGlobalRenamedClass.name, "TestGlobalRenamedClass_3")
+            self.assertIsNot(class1, TestGlobalRenamedClass)
+
+            # Check that methods are updated
+            obj = TestGlobalRenamedClass.new()
+            with self.assertRaises(AttributeError):
+                obj.oldMethod()
+            self.assertEqual(obj.testMethod(), "TEST1")
+
+        finally:
+            ObjCClass.auto_rename = False
+
+    def test_class_auto_rename_per_class(self):
+        """Test the per-class automatic renaming option of ObjCClass."""
+
+        class TestLocalRenamedClass(NSObject):
+            @objc_method
+            def oldMethod(self):
+                pass
+
+        class1 = TestLocalRenamedClass
+
+        class TestLocalRenamedClass_2(NSObject):
+            pass
+
+        class TestLocalRenamedClass(NSObject, auto_rename=True):  # noqa: F811
+            @objc_method
+            def testMethod(self):
+                return "TEST2"
+
+        # Check that the class was renamed
+        self.assertEqual(TestLocalRenamedClass.name, "TestLocalRenamedClass_3")
+        self.assertIsNot(class1, TestLocalRenamedClass)
+
+        # Check that methods are updated
+        obj = TestLocalRenamedClass.new()
+        with self.assertRaises(AttributeError):
+            obj.oldMethod()
+        self.assertEqual(obj.testMethod(), "TEST2")
+
+    def test_protocol_auto_rename_global(self):
+        """Test the global automatic renaming option of ObjCProtocol."""
+
+        try:
+            ObjCProtocol.auto_rename = True
+
+            class TestGlobalRenamedProtocol(metaclass=ObjCProtocol):
+                pass
+
+            protocol1 = TestGlobalRenamedProtocol
+
+            class TestGlobalRenamedProtocol_2(metaclass=ObjCProtocol):
+                pass
+
+            class TestGlobalRenamedProtocol(metaclass=ObjCProtocol):  # noqa: F811
+                pass
+
+            # Check that the protocol was renamed
+            self.assertEqual(
+                TestGlobalRenamedProtocol.name, "TestGlobalRenamedProtocol_3"
+            )
+            self.assertIsNot(protocol1, TestGlobalRenamedProtocol)
+
+        finally:
+            ObjCProtocol.auto_rename = False
+
+    def test_protocol_auto_rename_per_class(self):
+        """Test the per-protocol automatic renaming option of ObjCProtocol."""
+
+        class TestLocalRenamedProtocol(metaclass=ObjCProtocol):
+            pass
+
+        protocol1 = TestLocalRenamedProtocol
+
+        class TestLocalRenamedProtocol_2(metaclass=ObjCProtocol):
+            pass
+
+        class TestLocalRenamedProtocol(
+            metaclass=ObjCProtocol,
+            auto_rename=True,
+        ):  # noqa: F811
+            pass
+
+        # Check that the protocol was renamed
+        self.assertEqual(TestLocalRenamedProtocol.name, "TestLocalRenamedProtocol_3")
+        self.assertIsNot(protocol1, TestLocalRenamedProtocol)
+
     def test_interface(self):
         """An ObjC protocol implementation can be defined in Python."""
 
         Callback = ObjCProtocol("Callback")
         results = {}
 
         class Handler(NSObject, protocols=[Callback]):
```

### Comparing `rubicon-objc-0.4.7/tests/test_ctypes_patch.py` & `rubicon-objc-0.4.8/tests/test_ctypes_patch.py`

 * *Files identical despite different names*

