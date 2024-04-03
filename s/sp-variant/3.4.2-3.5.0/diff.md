# Comparing `tmp/sp_variant-3.4.2.tar.gz` & `tmp/sp_variant-3.5.0.tar.gz`

## Comparing `sp_variant-3.4.2.tar` & `sp_variant-3.5.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.4.2/.editorconfig
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.4.2/mkdocs.yml
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 sp_variant-3.4.2/tox.ini
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.4.2/.reuse/dep5
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.4.2/LICENSES/BSD-2-Clause.txt
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/common/scripts/add-storpool-repo.sh
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/common/scripts/storpool_variant.sh
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/debian/repo/storpool-keyring.gpg
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/debian/repo/storpool.sources
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/redhat/repo/RPM-GPG-KEY-StorPool
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.4.2/data/redhat/repo/storpool-centos.repo
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sp_variant-3.4.2/docs/api.md
--rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 sp_variant-3.4.2/docs/changes.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sp_variant-3.4.2/docs/index.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.4.2/examples/build-repo-overrides.toml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/config/ruff-all/pyproject.toml
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/config/ruff-base/pyproject.toml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/docs.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/ruff.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/test-mypy.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/test-tox-stages.txt
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/test-unit.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/requirements/tools.txt
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_build_repo/__init__.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_build_repo/__main__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_build_repo/diag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_build_repo/py.typed
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_build_repo/subst.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/__init__.py
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/__main__.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/defs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/py.typed
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/variant.py
--rw-r--r--   0        0        0    30252 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/vbuild.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/sp_variant/yaiparser.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/test_docker/__init__.py
--rw-r--r--   0        0        0    17891 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/test_docker/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/unit_tests/__init__.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/unit_tests/test_subst.py
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/unit_tests/test_variant.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.4.2/python/unit_tests/test_yaiparser.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.4.2/.gitignore
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.4.2/README.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 sp_variant-3.4.2/pyproject.toml
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 sp_variant-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.editorconfig
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.5.0/mkdocs.yml
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 sp_variant-3.5.0/tox.ini
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.5.0/LICENSES/BSD-2-Clause.txt
+-rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/common/scripts/add-storpool-repo.sh
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/common/scripts/storpool_variant.sh
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/debian/repo/storpool-keyring.gpg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/debian/repo/storpool.sources
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/redhat/repo/RPM-GPG-KEY-StorPool
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/redhat/repo/storpool-centos.repo
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/api.md
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/changes.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/index.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.5.0/examples/build-repo-overrides.toml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/docs.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/ruff.txt
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-mypy.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-tox-stages.txt
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-unit.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/tools.txt
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/__init__.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/__main__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/diag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/py.typed
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/subst.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/__init__.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/__main__.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/defs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/py.typed
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/variant.py
+-rw-r--r--   0        0        0    27505 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/vbuild.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/yaiparser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/test_docker/__init__.py
+-rw-r--r--   0        0        0    17971 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/test_docker/__main__.py
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/tests/vetox.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/__init__.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_subst.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_variant.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_yaiparser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.gitignore
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.5.0/README.md
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 sp_variant-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 sp_variant-3.5.0/PKG-INFO
```

### Comparing `sp_variant-3.4.2/.editorconfig` & `sp_variant-3.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/mkdocs.yml` & `sp_variant-3.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/LICENSES/BSD-2-Clause.txt` & `sp_variant-3.5.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/data/debian/repo/storpool-keyring.gpg` & `sp_variant-3.5.0/data/debian/repo/storpool-keyring.gpg`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/data/redhat/repo/RPM-GPG-KEY-StorPool` & `sp_variant-3.5.0/data/redhat/repo/RPM-GPG-KEY-StorPool`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/data/redhat/repo/storpool-centos.repo` & `sp_variant-3.5.0/data/redhat/repo/storpool-centos.repo`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/docs/changes.md` & `sp_variant-3.5.0/docs/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,68 @@
 All notable changes to the sp-variant project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.5.0] - 2024-04-03
+
+### Semi-incompatible changes
+
+- use Python 3.x as `min_sys_python` everywhere
+- drop the definitions for CentOS 6, Debian 9, Ubuntu 16.04, and Ubuntu 23.04;
+  they will no longer even be recognized
+
+### Fixes
+
+- mark Debian 10 as unsupported
+- documentation:
+    - correct the changelog link for version 3.4.2
+- python:
+    - library:
+        - re-sort the `sp_variant.variant.__all__` list
+    - test suite:
+        - do not expect Debian 9 and CentOS 6 to be present in the variant data
+        - update the `test-stages` requirements file to use Tox 4.x
+
+### Additions
+
+- all:
+    - add support for Ubuntu 24.04 (Noble Numbat)
+- documentation:
+    - add `publync` configuration to the `pyproject.toml` file
+- python:
+    - tentatively declare Python 3.13 as supported
+
+### Other changes
+
+- documentation:
+    - use `mkdocstrings` 0.24 with no changes
+- python:
+    - test suite:
+        - run the unit tests with pytest 6, 7, and 8, separately
+        - test with Ruff 0.3.4:
+            - simplify the Ruff configuration files layout
+            - override some more checks
+            - push the linter configuration into the `lint.*` TOML hierarchy
+            - use the concise output format even in preview mode
+            - let Ruff insist on trailing commas
+        - add the "docs" environment to the second Tox stage
+        - vendor-import `vetox` version 0.1.3
+- rust:
+    - use the `clap_derive` and `serde_derive` crates instead of features for
+      the respective `clap` and `serde` ones
+    - minor fixes and improvements suggested by Clippy
+- nix:
+    - remove an explanation for not running the Tox tests with Python 3.8;
+      it was dropped from nixpkgs/unstable anyway
+    - also run the Tox tests with Python 3.12
+    - add an expression and a shell helper to run `vetox` with Python 3.9 through 3.13
+
 ## [3.4.2] - 2023-12-19
 
 ### Other changes
 
 - python:
     - use Ruff 0.1.8 for testing with no changes
     - use Ruff instead of Black for source code formatting
@@ -554,16 +608,17 @@
 
 ## [1.3.0] - 2021-09-15
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.4.2...main
-[3.4.1]: https://github.com/storpool/sp-variant/compare/release/3.4.1...release/3.4.2
+[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.5.0...main
+[3.5.0]: https://github.com/storpool/sp-variant/compare/release/3.4.2...release/3.5.0
+[3.4.2]: https://github.com/storpool/sp-variant/compare/release/3.4.1...release/3.4.2
 [3.4.1]: https://github.com/storpool/sp-variant/compare/release/3.4.0...release/3.4.1
 [3.4.0]: https://github.com/storpool/sp-variant/compare/release/3.3.0...release/3.4.0
 [3.3.0]: https://github.com/storpool/sp-variant/compare/release/3.2.3...release/3.3.0
 [3.2.3]: https://github.com/storpool/sp-variant/compare/release/3.2.2...release/3.2.3
 [3.2.2]: https://github.com/storpool/sp-variant/compare/release/3.2.1...release/3.2.2
 [3.2.1]: https://github.com/storpool/sp-variant/compare/release/3.2.0...release/3.2.1
 [3.2.0]: https://github.com/storpool/sp-variant/compare/release/3.1.2...release/3.2.0
```

### Comparing `sp_variant-3.4.2/docs/index.md` & `sp_variant-3.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/python/sp_build_repo/__main__.py` & `sp_variant-3.5.0/python/sp_build_repo/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Build the "add StorPool repository" archive."""
 
 from __future__ import annotations
 
 import dataclasses
 import datetime
@@ -48,17 +48,17 @@
     (0, 1): {
         "?repo": {
             "*": {
                 "?slug": str,
                 "?url": str,
                 "?vendor": str,
                 "?codename": str,
-            }
-        }
-    }
+            },
+        },
+    },
 }
 
 
 @dataclasses.dataclass(frozen=True)
 class DataFormatVersion:
     """The version of the data format specification."""
 
@@ -157,15 +157,15 @@
         shutil.copy2(src, dst)
     except (OSError, subprocess.CalledProcessError) as err:
         raise variant.VariantFileError(f"Could not copy {src} to {dst}: {err}") from err
     try:
         dst.chmod(0o755 if executable else 0o644)
     except OSError as err:
         raise variant.VariantFileError(
-            f"Could not set the permissions mode on {dst}: {err}"
+            f"Could not set the permissions mode on {dst}: {err}",
         ) from err
 
 
 def subst_debian_sources(
     cfg: Config,
     var: variant.Variant,
     src: pathlib.Path,
@@ -179,15 +179,16 @@
     dst: Final = dstdir / (src.stem + rtype.extension + src.suffix)
     logging.debug(
         "%(src)s -> %(dst)s [vendor %(vendor)s, codename %(codename)s]",
         {"src": src, "dst": dst, "vendor": vendor, "codename": codename},
     )
 
     ovr: Final = cfg.overrides.repo.get(
-        rtype.name, OverrideRepo(url=None, slug=None, vendor=None, codename=None)
+        rtype.name,
+        OverrideRepo(url=None, slug=None, vendor=None, codename=None),
     )
     try:
         result: Final = (
             Singles.jinja2_env(src.parent)
             .get_template(src.name)
             .render(
                 url=rtype.url if ovr.url is None else ovr.url,
@@ -215,15 +216,16 @@
 ) -> None:
     """Substitute the placeholder vars in a Debian sources list file."""
     assert isinstance(var.repo, defs.YumRepo)  # noqa: S101  # mypy needs this
     dst: Final = dstdir / (src.stem + rtype.extension + src.suffix)
     logging.debug("%(src)s -> %(dst)s []", {"src": src, "dst": dst})
 
     ovr: Final = cfg.overrides.repo.get(
-        rtype.name, OverrideRepo(url=None, slug=None, vendor=None, codename=None)
+        rtype.name,
+        OverrideRepo(url=None, slug=None, vendor=None, codename=None),
     )
     try:
         result: Final = (
             Singles.jinja2_env(src.parent)
             .get_template(src.name)
             .render(
                 url=rtype.url if ovr.url is None else ovr.url,
@@ -286,28 +288,28 @@
             copy_file(cfg.datadir / var.repo.keyring, vardir)
         elif isinstance(var.repo, defs.YumRepo):
             for rtype in defs.REPO_TYPES:
                 subst_yum_repo(cfg, var, cfg.datadir / var.repo.yumdef, vardir, rtype)
             copy_file(cfg.datadir / var.repo.keyring, vardir)
         else:
             raise NotImplementedError(
-                f"No idea how to handle {type(var.repo).__name__} for {var.name}"
+                f"No idea how to handle {type(var.repo).__name__} for {var.name}",
             )
 
     distfile: Final = (cfg.destdir / distname).with_suffix(".tar.gz")
     ensure_none(distfile)
     logging.debug("Creating %(distfile)s", {"distfile": distfile})
     try:
         subprocess.check_call(
             ["tar", "-caf", distfile, "-C", cfg.destdir, distname],
             shell=False,
         )
     except subprocess.CalledProcessError as err:
         raise variant.VariantFileError(
-            f"Could not package {distdir} up into {distfile}: {err}"
+            f"Could not package {distdir} up into {distfile}: {err}",
         ) from err
     return distfile
 
 
 @functools.lru_cache(maxsize=2)
 def typed_loader(*, failonextra: bool = False) -> typedload.dataloader.Loader:
     """Prepare a loader that can parse annotated types."""
@@ -331,15 +333,15 @@
     try:
         data_format: Final = typed_loader().load(raw_format, DataFormat)
     except (TypeError, AttributeError, KeyError, ValueError) as err:
         sys.exit(f"Could not read the 'format' section of the {path} overrides file: {err}")
     if (data_format.version.major, data_format.version.minor) != (0, 1):
         sys.exit(
             f"Unsupported format version for the {path} override files, "
-            f"only 0.1 supported so far"
+            f"only 0.1 supported so far",
         )
 
     try:
         return typed_loader(failonextra=True).load(raw, Overrides)
     except (TypeError, AttributeError, KeyError, ValueError) as err:
         sys.exit(f"Invalid format for the {path} overrides file: {err}")
```

### Comparing `sp_variant-3.4.2/python/sp_build_repo/diag.py` & `sp_variant-3.5.0/python/sp_build_repo/diag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2023, 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Provide a class that outputs diagnostic messages if configured to."""
 
 from __future__ import annotations
 
 import functools
 import logging
@@ -24,15 +24,18 @@
     handler.setLevel(logging.DEBUG)
 
     logger.addHandler(handler)
     return logger
 
 
 def setup_logger(
-    name: str | None = None, *, verbose: bool, propagate: bool = False
+    name: str | None = None,
+    *,
+    verbose: bool,
+    propagate: bool = False,
 ) -> logging.Logger:
     """Set up a logger that sends messages to the standard error stream.
 
     If the `verbose` parameter is false, debug-level messages are ignored.
 
     Note that the logger will NOT propagate messages to parent loggers unless
     the `propagate` parameter is true.
```

### Comparing `sp_variant-3.4.2/python/sp_build_repo/subst.py` & `sp_variant-3.5.0/python/sp_build_repo/subst.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Substitute variant data using Jinja2 templates."""
 
 from __future__ import annotations
 
 import dataclasses
 import functools
@@ -112,15 +112,18 @@
 
 class OctalInteger(click.ParamType):
     """Convert a string value to an integer using base 8."""
 
     name = "octal"
 
     def convert(
-        self, value: str | int, param: click.Parameter | None, ctx: click.Context | None
+        self,
+        value: str | int,
+        param: click.Parameter | None,
+        ctx: click.Context | None,
     ) -> int:
         """Convert a string to an integer using base 8."""
         if isinstance(value, int):
             return value
 
         try:
             return int(value, 8)
@@ -139,15 +142,19 @@
     default=0o644,
     help="the octal permissions mode of the output file",
 )
 @click.option(
     "-o",
     "--output",
     type=click.Path(
-        dir_okay=False, file_okay=True, writable=True, resolve_path=True, path_type=pathlib.Path
+        dir_okay=False,
+        file_okay=True,
+        writable=True,
+        resolve_path=True,
+        path_type=pathlib.Path,
     ),
     required=True,
     help="the output file to generate",
 )
 @click.option(
     "-t",
     "--template",
```

### Comparing `sp_variant-3.4.2/python/sp_variant/__main__.py` & `sp_variant-3.5.0/python/sp_variant/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Support for different OS distributions and StorPool build variants."""
 
 from __future__ import annotations
 
 import argparse
 import json
@@ -69,28 +69,28 @@
         raise variant.VariantFileError(f"Could not copy {src} over to {dst}: {err}") from err
 
 
 def repo_name_with_extension(cfg: defs.Config, path: pathlib.Path) -> str:
     """Get the path basename, add the extension for the specified repository type."""
     if len(path.suffixes) != 1:
         raise variant.VariantFileError(
-            f"Unexpected repository file name without an extension: {path}"
+            f"Unexpected repository file name without an extension: {path}",
         )
     return f"{path.stem}{cfg.repotype.extension}{path.suffix}"
 
 
 def repo_add_deb(cfg: defs.Config, var: defs.Variant, vardir: pathlib.Path) -> None:
     """Install the StorPool Debian-like repo configuration."""
     assert isinstance(var.repo, defs.DebRepo)  # noqa: S101  # mypy needs this
 
     try:
         subprocess.check_call(var.commands.package.install + var.repo.req_packages, shell=False)
     except subprocess.CalledProcessError as err:
         raise variant.VariantFileError(
-            f"Could not install the required packages {' '.join(var.repo.req_packages)}: {err}"
+            f"Could not install the required packages {' '.join(var.repo.req_packages)}: {err}",
         ) from err
 
     copy_file(
         cfg,
         vardir / repo_name_with_extension(cfg, pathlib.Path(var.repo.sources)),
         _PATH_APT_SOURCES,
     )
@@ -120,15 +120,15 @@
                 "-y",
                 "ca-certificates",
             ],
             shell=False,
         )
     except subprocess.CalledProcessError as err:
         raise variant.VariantFileError(
-            f"Could not install the required ca-certificates package: {err}"
+            f"Could not install the required ca-certificates package: {err}",
         ) from err
 
     copy_file(
         cfg,
         vardir / repo_name_with_extension(cfg, pathlib.Path(var.repo.yumdef)),
         _PATH_YUM_REPOS,
     )
@@ -160,15 +160,15 @@
                 "clean",
                 "metadata",
             ],
             shell=False,
         )
     except subprocess.CalledProcessError as err:
         raise variant.VariantFileError(
-            f"Could not clean the Yum repository metadata: {err}"
+            f"Could not clean the Yum repository metadata: {err}",
         ) from err
 
 
 def repo_add(cfg: defs.Config) -> None:
     """Install the StorPool repository configuration."""
     assert cfg.repodir is not None  # noqa: S101  # mypy needs this
     var: Final = variant.detect_variant(cfg)
@@ -199,22 +199,22 @@
     for comp in cfg.command.split("."):
         if not isinstance(current, tuple):
             raise defs.VariantConfigError("Too many command components")
 
         fields: tuple[str, ...] = current._fields
         if comp not in fields:
             raise defs.VariantConfigError(
-                f"Invalid command component '{comp}', should be one of {' '.join(fields)}"
+                f"Invalid command component '{comp}', should be one of {' '.join(fields)}",
             )
         current = getattr(current, comp)
 
     if not isinstance(current, list):
         fields = current._fields
         raise defs.VariantConfigError(
-            f"Incomplete command specification, should continue with one of {' '.join(fields)}"
+            f"Incomplete command specification, should continue with one of {' '.join(fields)}",
         )
 
     return current
 
 
 def command_run(cfg: defs.Config) -> None:
     """Run a distribution-specific command."""
@@ -257,15 +257,15 @@
         sys.exit(1)
 
 
 def cmd_features(_cfg: defs.Config) -> None:
     """Display the features supported by storpool_variant."""
     print(
         f"Features: repo=0.2 variant={defs.VERSION} "
-        f"format={defs.FORMAT_VERSION[0]}.{defs.FORMAT_VERSION[1]}"
+        f"format={defs.FORMAT_VERSION[0]}.{defs.FORMAT_VERSION[1]}",
     )
 
 
 def cmd_show(cfg: defs.Config) -> None:
     """Display information about a single build variant."""
     vbuild.build_variants(cfg)
 
@@ -274,20 +274,20 @@
         if cfg.command == "all":
             return defs.jsonify(
                 {
                     "format": {
                         "version": {
                             "major": defs.FORMAT_VERSION[0],
                             "minor": defs.FORMAT_VERSION[1],
-                        }
+                        },
                     },
                     "version": defs.VERSION,
                     "variants": vbuild.VARIANTS,
                     "order": [var.name for var in vbuild.DETECT_ORDER],
-                }
+                },
             )
 
         assert cfg.command is not None  # noqa: S101  # mypy needs this
         var: Final[defs.Variant | None] = (
             variant.detect_variant(cfg)
             if cfg.command == "current"
             else vbuild.VARIANTS.get(cfg.command)
@@ -297,19 +297,19 @@
 
         return defs.jsonify(
             {
                 "format": {
                     "version": {
                         "major": defs.FORMAT_VERSION[0],
                         "minor": defs.FORMAT_VERSION[1],
-                    }
+                    },
                 },
                 "version": defs.VERSION,
                 "variant": var,
-            }
+            },
         )
 
     print(json.dumps(get_data(), sort_keys=True, indent=2))
 
 
 def parse_arguments() -> tuple[defs.Config, Callable[[defs.Config], None]]:
     """Parse the command-line arguments."""
```

### Comparing `sp_variant-3.4.2/python/sp_variant/defs.py` & `sp_variant-3.5.0/python/sp_variant/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     extension: str
     """The extension to be used in filenames for configurating the package manager."""
 
     url: str
     """The base URL of the StorPool package repository."""
 
 
-VERSION: Final = "3.4.2"
+VERSION: Final = "3.5.0"
 FORMAT_VERSION: Final = (1, 4)
 
 REPO_TYPES: Final = [
     RepoType(name="contrib", extension="", url="https://repo.storpool.com/public/"),
     RepoType(
         name="staging",
         extension="-staging",
```

### Comparing `sp_variant-3.4.2/python/sp_variant/variant.py` & `sp_variant-3.5.0/python/sp_variant/variant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Build variant definitions and commands."""
 
 from __future__ import annotations
 
 import errno
 import pathlib
@@ -95,15 +95,15 @@
             for line in pathlib.Path(var.detect.filename).read_text(encoding=SAFEENC).splitlines():
                 if var.detect.regex.match(line):
                     cfg.diag(f"  - found it: {line}")
                     return var
         except OSError as err:
             if err.errno != errno.ENOENT:
                 raise VariantDetectError(
-                    f"Could not read the {var.detect.filename} file: {err}"
+                    f"Could not read the {var.detect.filename} file: {err}",
                 ) from err
             cfg.diag(f"  - no {var.detect.filename}")
 
     return None
 
 
 def detect_variant(cfg: Config = _DEFAULT_CONFIG) -> Variant:
@@ -167,25 +167,25 @@
 
         res.append(
             defs.OSPackage(
                 name=fields[0],
                 version=fields[1],
                 arch=fields[2],
                 status="installed",
-            )
+            ),
         )
 
     return res
 
 
 __all__ = (
+    "VERSION",
     "Config",
     "Variant",
     "VariantError",
-    "VERSION",
     "detect_variant",
     "get_all_variants",
     "get_all_variants_in_order",
     "get_by_alias",
     "get_variant",
     "list_all_packages",
     "update_namedtuple",
```

### Comparing `sp_variant-3.4.2/python/sp_variant/vbuild.py` & `sp_variant-3.5.0/python/sp_variant/vbuild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Build the hierarchical structure of variant definitions."""
 
 from __future__ import annotations
 
 import pathlib
 import re
@@ -97,15 +97,15 @@
                     "env DEBIAN_FRONTEND=noninteractive apt-get install "
                     "--no-install-recommends --reinstall -y "
                     "-o DPkg::Options::=--force-confnew "
                     "-- $packages",
                 ],
             ),
         ),
-        min_sys_python="3.9",
+        min_sys_python="3.11",
         repo=defs.DebRepo(
             vendor="debian",
             codename="unstable",
             sources="debian/repo/storpool.sources",
             keyring="debian/repo/storpool-keyring.gpg",
             req_packages=["ca-certificates"],
         ),
@@ -170,15 +170,15 @@
                 """,
                 re.X,
             ),
             os_id="debian",
             os_version_regex=re.compile(r"^11$"),
         ),
         updates={
-            "supported": {"repo": True},
+            "min_sys_python": "3.9",
             "repo": {"codename": "bullseye"},
             "package": {
                 "LIBSSL": "libssl1.1",
             },
             "builder": {
                 "alias": "debian11",
                 "base_image": "debian:bullseye",
@@ -200,103 +200,77 @@
                 """,
                 re.X,
             ),
             os_id="debian",
             os_version_regex=re.compile(r"^10$"),
         ),
         updates={
+            "supported": {"repo": False},
             "repo": {
                 "codename": "buster",
             },
-            "min_sys_python": "2.7",
+            "min_sys_python": "3.7",
             "package": {
                 "BINDINGS_PYTHON": "python",
                 "BINDINGS_PYTHON_CONFGET": "python-confget",
                 "BINDINGS_PYTHON_SIMPLEJSON": "python-simplejson",
             },
             "builder": {
                 "alias": "debian10",
                 "base_image": "debian:buster",
                 "branch": "debian/buster",
             },
         },
     ),
     defs.VariantUpdate(
-        name="DEBIAN9",
-        descr="Debian 9.x (stretch)",
-        parent="DEBIAN10",
-        detect=defs.Detect(
-            filename="/etc/os-release",
-            regex=re.compile(
-                r"""^
-                    PRETTY_NAME= .*
-                    Debian \s+ GNU/Linux \s+
-                    (?: stretch | 9 ) (?: \s | / )
-                """,
-                re.X,
-            ),
-            os_id="debian",
-            os_version_regex=re.compile(r"^9$"),
-        ),
-        updates={
-            "supported": {"repo": False},
-            "repo": {
-                "codename": "stretch",
-                "req_packages": ["apt-transport-https", "ca-certificates"],
-            },
-            "builder": {
-                "alias": "debian9",
-                "base_image": "debian:stretch",
-                "branch": "debian/stretch",
-            },
-        },
-    ),
-    defs.VariantUpdate(
-        name="UBUNTU2304",
-        descr="Ubuntu 23.04 LTS (Lunar Lobster)",
-        parent="DEBIAN12",
+        name="UBUNTU2404",
+        descr="Ubuntu 24.04 LTS (Noble Numbat)",
+        parent="DEBIAN13",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
-                r"^ PRETTY_NAME= .* Ubuntu \s+ 23 \. 04 ",
+                r"^ PRETTY_NAME= .* Ubuntu \s+ .* Noble ",
                 re.X,
             ),
             os_id="ubuntu",
-            os_version_regex=re.compile(r"^23\.04$"),
+            os_version_regex=re.compile(r"^24\.04$"),
         ),
         updates={
+            "supported": {"repo": False},
             "repo": {
                 "vendor": "ubuntu",
-                "codename": "lunar",
+                "codename": "noble",
             },
+            "min_sys_python": "3.12",
             "package": {
                 "CPUPOWER": "linux-tools-generic",
             },
             "builder": {
-                "alias": "ubuntu-23.04",
-                "base_image": "ubuntu:lunar",
-                "branch": "ubuntu/lunar",
+                "alias": "ubuntu-24.04",
+                "base_image": "ubuntu:noble",
+                "branch": "ubuntu/noble",
             },
         },
     ),
     defs.VariantUpdate(
         name="UBUNTU2204",
         descr="Ubuntu 22.04 LTS (Jammy Jellyfish)",
-        parent="UBUNTU2304",
+        parent="UBUNTU2404",
         detect=defs.Detect(
             filename="/etc/os-release",
             regex=re.compile(
                 r"^ PRETTY_NAME= .* (?: Ubuntu \s+ 22 \. 04 | Mint \s+ 21 ) ",
                 re.X,
             ),
             os_id="ubuntu",
             os_version_regex=re.compile(r"^22\.04$"),
         ),
         updates={
             "supported": {"repo": True},
+            "min_sys_python": "3.10",
             "repo": {
                 "vendor": "ubuntu",
                 "codename": "jammy",
             },
             "builder": {
                 "alias": "ubuntu-22.04",
                 "base_image": "ubuntu:jammy",
@@ -347,57 +321,27 @@
             os_id="ubuntu",
             os_version_regex=re.compile(r"^18\.04$"),
         ),
         updates={
             "repo": {
                 "codename": "bionic",
             },
-            "min_sys_python": "2.7",
+            "min_sys_python": "3.6",
             "package": {
                 "BINDINGS_PYTHON": "python",
                 "BINDINGS_PYTHON_CONFGET": "python-confget",
                 "BINDINGS_PYTHON_SIMPLEJSON": "python-simplejson",
             },
             "builder": {
                 "alias": "ubuntu-18.04",
                 "base_image": "ubuntu:bionic",
                 "branch": "ubuntu/bionic",
             },
         },
     ),
-    defs.VariantUpdate(
-        name="UBUNTU1604",
-        descr="Ubuntu 16.04 LTS (Xenial Xerus)",
-        parent="UBUNTU1804",
-        detect=defs.Detect(
-            filename="/etc/os-release",
-            regex=re.compile(
-                r"^ PRETTY_NAME= .* Ubuntu \s+ 16 \. 04 ",
-                re.X,
-            ),
-            os_id="ubuntu",
-            os_version_regex=re.compile(r"^16\.04$"),
-        ),
-        updates={
-            "supported": {"repo": False},
-            "repo": {
-                "codename": "xenial",
-                "req_packages": ["apt-transport-https", "ca-certificates"],
-            },
-            "package": {
-                "LIBSSL": "libssl1.0.0",
-                "mcelog": "mcelog",
-            },
-            "builder": {
-                "alias": "ubuntu-16.04",
-                "base_image": "ubuntu:xenial",
-                "branch": "ubuntu/xenial",
-            },
-        },
-    ),
     defs.Variant(
         name="ALMA9",
         descr="AlmaLinux 9.x",
         parent="",
         family="redhat",
         detect=defs.Detect(
             filename="/etc/redhat-release",
@@ -474,15 +418,15 @@
 if [ -n "$to_reinstall" ]; then
     dnf reinstall -y --disablerepo='*' --enablerepo=appstream,baseos,crb,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
 """,  # noqa: E501
                 ],
             ),
         ),
-        min_sys_python="2.7",
+        min_sys_python="3.9",
         repo=defs.YumRepo(
             yumdef="redhat/repo/storpool-centos.repo",
             keyring="redhat/repo/RPM-GPG-KEY-StorPool",
         ),
         package={
             "KMOD": "kmod",
             "LIBCGROUP": "bash",
@@ -519,14 +463,15 @@
         ),
         updates={
             "supported": {"repo": True},
             "package": {
                 "LIBCGROUP": "libcgroup-tools",
                 "PYTHON_SIMPLEJSON": "python2-simplejson",
             },
+            "min_sys_python": "3.6",
             "commands": {
                 "package": {
                     "install": [
                         "dnf",
                         "--disablerepo=*",
                         "--enablerepo=appstream",
                         "--enablerepo=baseos",
@@ -659,47 +604,14 @@
                 "branch": "centos/7",
                 "kernel_package": "kernel",
                 "utf8_locale": "en_US.utf8",
             },
         },
     ),
     defs.VariantUpdate(
-        name="CENTOS6",
-        descr="CentOS 6.x",
-        parent="CENTOS7",
-        detect=defs.Detect(
-            filename="/etc/redhat-release",
-            regex=re.compile(r"^ CentOS \s .* \s 6 \.", re.X),
-            os_id="centos",
-            os_version_regex=re.compile(r"^6(?:$|\.[0-9])"),
-        ),
-        updates={
-            "supported": {"repo": False},
-            "min_sys_python": "2.6",
-            "package": {
-                "KMOD": "module-init-tools",
-                "LIBCGROUP": "libcgroup",
-                "LIBUDEV": "libudev",
-                "OPENSSL": "openssl",
-                "PERL_AUTODIE": "perl",
-                "PERL_FILE_PATH": "perl",
-                "PERL_LWP_PROTO_HTTPS": "perl",
-                "PERL_SYS_SYSLOG": "perl",
-                "PYTHON_SIMPLEJSON": "python-simplejson",
-                "PROCPS": "procps",
-                "UDEV": "udev",
-            },
-            "builder": {
-                "alias": "centos6",
-                "base_image": "centos:6",
-                "branch": "centos/6",
-            },
-        },
-    ),
-    defs.VariantUpdate(
         name="ORACLE7",
         descr="Oracle Linux 7.x",
         parent="CENTOS7",
         detect=defs.Detect(
             filename="/etc/oracle-release",
             regex=re.compile(r"^ Oracle \s+ Linux \s .* \s 7 \.", re.X),
             os_id="ol",
@@ -737,15 +649,15 @@
                         "--enablerepo=baseos",
                         "--enablerepo=storpool-contrib",
                         "--enablerepo=codeready-builder-for-rhel-8-x86_64-rpms",
                         "install",
                         "-q",
                         "-y",
                         "--",
-                    ]
+                    ],
                 },
                 "pkgfile": {
                     "install": [
                         "sh",
                         "-c",
                         """
 unset to_install to_reinstall
@@ -761,15 +673,15 @@
 if [ -n "$to_install" ]; then
     dnf install -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,codeready-builder-for-rhel-8-x86_64-rpms --setopt=localpkg_gpgcheck=0 -- $to_install
 fi
 if [ -n "$to_reinstall" ]; then
     dnf reinstall -y --disablerepo='*' --enablerepo=appstream,baseos,storpool-contrib,codeready-builder-for-rhel-8-x86_64-rpms --setopt=localpkg_gpgcheck=0 -- $to_reinstall
 fi
 """,  # noqa: E501
-                    ]
+                    ],
                 },
             },
             "builder": {
                 "alias": "rhel8",
                 "base_image": "redhat/ubi8:reg",
                 "branch": "",
             },
@@ -898,23 +810,25 @@
 
         for vtype, handler in _UPDATE_HANDLERS:
             if isinstance(value, vtype):
                 newv[name] = handler(prefix, name, orig, value)
                 break
         else:
             raise defs.VariantConfigError(
-                f"{prefix}: weird {type(value).__name__} update for {name}"
+                f"{prefix}: weird {type(value).__name__} update for {name}",
             )
 
     updated: Final[_TNamedTuple] = type(data)(**newv)  # type: ignore[call-overload]
     return updated
 
 
 def merge_into_parent(
-    cfg: defs.Config, parent: defs.Variant, child: defs.VariantUpdate
+    cfg: defs.Config,
+    parent: defs.Variant,
+    child: defs.VariantUpdate,
 ) -> defs.Variant:
     """Merge a child's definitions into the parent."""
     cfg.diag(f"- merging {child.name} into {parent.name}")
     return update_namedtuple(
         defs.Variant(
             name=child.name,
             descr=child.descr,
```

### Comparing `sp_variant-3.4.2/python/sp_variant/yaiparser.py` & `sp_variant-3.5.0/python/sp_variant/yaiparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Yet Another INI-style-file Parser."""
 
 from __future__ import annotations
 
 import pathlib
 import re
@@ -56,30 +56,34 @@
         if isinstance(line, str):
             return self._parse_line_str(line)
 
         try:
             str_line: Final = line.decode("UTF-8")
         except UnicodeDecodeError as err:
             raise VariantYAIError(
-                f"Invalid {self.filename} line, not a valid UTF-8 string: {line!r}: {err}"
+                f"Invalid {self.filename} line, not a valid UTF-8 string: {line!r}: {err}",
             ) from err
         return self._parse_line_str(str_line)
 
     def _parse_line_quoted_single(
-        self, line: str, varname: str, quoted: str, cquot: str
+        self,
+        line: str,
+        varname: str,
+        quoted: str,
+        cquot: str,
     ) -> tuple[str, str] | None:
         """Parse a value enclosed in single quotes."""
         if _SINGLE_QUOTE in quoted:
             raise VariantYAIError(
                 f"Weird {self.filename} line, the quoted content "
-                f"contains the quote character: {line!r}"
+                f"contains the quote character: {line!r}",
             )
         if cquot != _SINGLE_QUOTE:
             raise VariantYAIError(
-                f"Weird {self.filename} line, open/close quote mismatch: {line!r}"
+                f"Weird {self.filename} line, open/close quote mismatch: {line!r}",
             )
 
         return (varname, quoted)
 
     def _parse_line_unquoted(self, line: str, varname: str, quoted: str) -> tuple[str, str] | None:
         """Escape any characters preceded by a backslash."""
         res = ""
@@ -89,15 +93,15 @@
             except ValueError:
                 res += quoted
                 break
 
             if idx == len(quoted) - 1:
                 raise VariantYAIError(
                     f"Weird {self.filename} line, backslash at "
-                    f"the end of the quoted string: {line!r}"
+                    f"the end of the quoted string: {line!r}",
                 )
             res += quoted[:idx] + quoted[idx + 1]
             quoted = quoted[idx + 2 :]
 
         return (varname, res)
 
     def _parse_line_str(self, line: str) -> tuple[str, str] | None:
@@ -118,15 +122,15 @@
         if oquot == _SINGLE_QUOTE:
             return self._parse_line_quoted_single(line, varname, quoted, cquot)
 
         if oquot is None:
             quoted = full
         elif cquot != oquot:
             raise VariantYAIError(
-                f"Weird {self.filename} line, open/close quote mismatch: {line!r}"
+                f"Weird {self.filename} line, open/close quote mismatch: {line!r}",
             )
 
         return self._parse_line_unquoted(line, varname, quoted)
 
     def parse(self) -> dict[str, str]:
         """Parse a file, store and return the result."""
         contents: Final = self.filename.read_text(encoding="UTF-8")
```

### Comparing `sp_variant-3.4.2/python/test_docker/__main__.py` & `sp_variant-3.5.0/python/test_docker/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Run some sp_variant tests using Docker containers."""
 
 from __future__ import annotations
 
 import asyncio
 import asyncio.subprocess as aprocess
@@ -47,37 +47,41 @@
     """A part of the variants representation."""
 
     name: str
     builder: SimpleBuilder
 
 
 def extract_variants_data(
-    cfg: Config, tempd: pathlib.Path
+    cfg: Config,
+    tempd: pathlib.Path,
 ) -> tuple[pathlib.Path, dict[str, SimpleVariant]]:
     """Extract the variants data into the specified directory."""
     logging.debug("Making sure the %(tempd)s directory is empty", {"tempd": tempd})
     if found := list(tempd.iterdir()):
         sys.exit(f"Unexpected stuff found in {tempd}: {found!r}")
 
     logging.debug(
-        "Extracting %(repo_file)s into %(tempd)s", {"repo_file": cfg.repo_file, "tempd": tempd}
+        "Extracting %(repo_file)s into %(tempd)s",
+        {"repo_file": cfg.repo_file, "tempd": tempd},
     )
     subprocess.check_call(["tar", "-xaf", cfg.repo_file, "-C", tempd], env=cfg.utf8_env)
     logging.debug("Looking for a single directory")
     found = list(tempd.iterdir())
     if len(found) != 1 or not found[0].is_dir() or found[0].name != "add-storpool-repo":
         sys.exit(f"Expected a single add-storpool-repo directory in {tempd}: {found!r}")
     spdir: Final = found[0]
 
     spvar: Final = spdir / "storpool_variant"
     if not spvar.is_file() or (spvar.stat().st_mode & 0o555) != 0o555:
         sys.exit(f"Expected an executable {spvar} file")
 
     output: Final = subprocess.check_output(
-        [spvar, "show", "all"], encoding="UTF-8", env=cfg.utf8_env
+        [spvar, "show", "all"],
+        encoding="UTF-8",
+        env=cfg.utf8_env,
     )
     try:
         data: Final = json.loads(output)
     except ValueError as err:
         sys.exit(f"Failed to decode the output of `{spvar} show all`: {err}")
 
     if (
@@ -107,15 +111,15 @@
     """Find the Docker images present on this system."""
     logging.debug("Querying Docker for the available images")
     all_images: Final = set(
         subprocess.check_output(
             ["docker", "image", "ls", "--format", "{{.Repository}}:{{.Tag}}"],
             encoding="UTF-8",
             env=cfg.utf8_env,
-        ).splitlines()
+        ).splitlines(),
     )
     images: Final = (
         all_images
         if not cfg.images_filter
         else {name for name in all_images if any(word in name for word in cfg.images_filter)}
     )
 
@@ -128,29 +132,31 @@
             if image in images:
                 res[image] = var.name
 
     return res
 
 
 async def process_detect_lines(
-    image: str, proc: aprocess.Process
+    image: str,
+    proc: aprocess.Process,
 ) -> tuple[bytes | None, list[str]]:
     """Read the lines output by `storpool_variant detect`, see if they look okay."""
     assert proc.stdout is not None  # noqa: S101  # mypy needs this
 
     first_line = None
     rest = b""
     errors: Final = []
     try:
         try:
             first_line = await proc.stdout.readline()
         except Exception as err:  # noqa: BLE001
             errors.append(f"Could not read the first line: {err}")
         logging.debug(
-            "%(image)s: first line %(first_line)r", {"image": image, "first_line": first_line}
+            "%(image)s: first line %(first_line)r",
+            {"image": image, "first_line": first_line},
         )
 
         if first_line:
             first_line = first_line.rstrip(b"\n")
             while True:
                 try:
                     more = await proc.stdout.readline()
@@ -172,15 +178,17 @@
         if res:
             errors.append(f"Non-zero exit code {res}")
 
     return first_line, errors
 
 
 async def run_detect_for_image(
-    cfg: Config, spdir: pathlib.Path, image: str
+    cfg: Config,
+    spdir: pathlib.Path,
+    image: str,
 ) -> tuple[str | None, str | None]:
     """Run `storpool_variant detect` in a single new Docker container."""
     logging.debug("%(image)s: starting a container", {"image": image})
     proc: Final = await aprocess.create_subprocess_exec(
         "docker",
         "run",
         "--rm",
@@ -225,15 +233,17 @@
         return [f"{image}: expected {expected!r}, got {r_first!r}"]
 
     logging.debug("%(image)s: OK: %(r_first)r", {"image": image, "r_first": r_first})
     return []
 
 
 async def test_detect(
-    cfg: Config, spdir: pathlib.Path, ordered: list[tuple[str, str]]
+    cfg: Config,
+    spdir: pathlib.Path,
+    ordered: list[tuple[str, str]],
 ) -> list[str]:
     """Run `storpool_variant detect` for all the images."""
     logging.debug("Spawning the detect containers")
     gathering: Final = asyncio.gather(
         *(run_detect_for_image(cfg, spdir, image) for image, _ in ordered),
         return_exceptions=True,
     )
@@ -243,15 +253,15 @@
     logging.debug("Analyzing %(count)d detect results", {"count": len(res)})
     errors: Final = []
     for (image, expected), received in zip(ordered, res):
         errors.extend(analyze_detect_single(image, expected, received))
 
     if len(res) != len(ordered):
         errors.append(
-            f"Internal error: expected {len(ordered)} detect results, got {len(res)} ones"
+            f"Internal error: expected {len(ordered)} detect results, got {len(res)} ones",
         )
 
     return errors
 
 
 async def run_add_repo_for_image(
     cfg: Config,
@@ -295,15 +305,16 @@
                 {"image": image, "stype": stype, "line": line},
             )
             res += line
 
         return res
 
     r_out, r_err = await asyncio.gather(
-        read_stream("stdout", proc.stdout), read_stream("stderr", proc.stderr)
+        read_stream("stdout", proc.stdout),
+        read_stream("stderr", proc.stderr),
     )
     res: Final = await proc.wait()
     return (r_out, r_err, res)
 
 
 def analyze_add_repo_single(
     image: str,
@@ -315,15 +326,15 @@
     if not isinstance(received, tuple) or len(received) != 3:
         return [f"{image}: unexpected result {received!r}"]
 
     r_out, r_err, r_res = received
     if r_res:
         return [
             f"{image}: the script failed with exit code {r_res}; "
-            f"stdout: {r_out!r} stderr {r_err!r}"
+            f"stdout: {r_out!r} stderr {r_err!r}",
         ]
 
     logging.debug("%(image)s: OK", {"image": image})
     return []
 
 
 async def test_add_repo(
@@ -487,15 +498,15 @@
     logging.debug("Analyzing %(count)d add-repo results", {"count": len(res)})
     errors: Final = []
     for (image, _), received in zip(ordered, res):
         errors.extend(analyze_add_repo_single(image, received))
 
     if len(res) != len(ordered):
         errors.append(
-            f"Internal error: expected {len(ordered)} add-repo results, got {len(res)} ones"
+            f"Internal error: expected {len(ordered)} add-repo results, got {len(res)} ones",
         )
 
     return errors
 
 
 async def run_tests(
     cfg: Config,
```

### Comparing `sp_variant-3.4.2/python/unit_tests/test_subst.py` & `sp_variant-3.5.0/python/unit_tests/test_subst.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/python/unit_tests/test_variant.py` & `sp_variant-3.5.0/python/unit_tests/test_variant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 """Test the functions in the sp.variant module."""
 
 from __future__ import annotations
 
 import collections
 import dataclasses
@@ -26,26 +26,26 @@
 _MSG_NOT_SEEN = "This should not be seen"
 _MSG_SEEN = "This should be seen"
 _RE_CENTOS_VER = re.compile(r"^ .*? (?P<ver> \d+ ) $", re.X)
 
 
 def test_get() -> None:
     """Test the operation of get_variant()."""
-    assert variant.get_variant("CENTOS7").name == "CENTOS7"
-    assert variant.get_variant("CENTOS6").name == "CENTOS6"
+    assert variant.get_variant("CENTOS9").name == "CENTOS9"
+    assert variant.get_variant("CENTOS8").name == "CENTOS8"
 
     repo = variant.get_variant("UBUNTU1804").repo
     assert isinstance(repo, defs.DebRepo)
     assert repo.vendor == "ubuntu"
     assert repo.codename == "bionic"
 
-    repo = variant.get_variant("DEBIAN9").repo
+    repo = variant.get_variant("DEBIAN12").repo
     assert isinstance(repo, defs.DebRepo)
     assert repo.vendor == "debian"
-    assert repo.codename == "stretch"
+    assert repo.codename == "bookworm"
 
     with pytest.raises(variant.VariantKeyError):
         variant.get_variant("whee")
 
 
 def test_roundtrip() -> None:
     """Run through the variants with some minimal sanity checks."""
@@ -174,15 +174,15 @@
         vdata: Final = _RE_CENTOS_VER.match(var.name)
         assert vdata
         ver: Final = vdata.group("ver")
         assert ver
         return ver
 
     versions: Final = sorted(
-        {extract_version(var) for var in all_variants if var.family == "redhat"}
+        {extract_version(var) for var in all_variants if var.family == "redhat"},
     )
     assert versions
     missing_branches: Final = [
         branch
         for branch in (f"centos/{ver}" for ver in versions)
         if all(var.builder.branch != branch for var in all_variants)
     ]
```

### Comparing `sp_variant-3.4.2/python/unit_tests/test_yaiparser.py` & `sp_variant-3.5.0/python/unit_tests/test_yaiparser.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/README.md` & `sp_variant-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sp_variant-3.4.2/pyproject.toml` & `sp_variant-3.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 - 2023  StorPool <support@storpool.com>
+# SPDX-FileCopyrightText: 2021 - 2024  StorPool <support@storpool.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [build-system]
 requires = [
   "hatchling >= 1.8, < 2",
 ]
 build-backend = "hatchling.build"
@@ -26,14 +26,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: System :: Systems Administration",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
@@ -69,9 +70,26 @@
 [tool.hatch.version]
 path = "python/sp_variant/defs.py"
 pattern = 'VERSION: Final = "(?P<version>[^"]+)"'
 
 [tool.mypy]
 strict = true
 
+[tool.publync.format.version]
+major = 0
+minor = 1
+
+[tool.publync.build.tox]
+
+[tool.publync.sync.rsync]
+remote = "root@https-sof.sof-vm.storpool.local:/var/www/repo/public/doc/sp-variant"
+
+[tool.ruff]
+extend = "ruff-base.toml"
+output-format = "concise"
+preview = true
+
+[tool.ruff.lint]
+select = ["ALL"]
+
 [tool.test-stages]
 stages = ["@check and @quick and not @manual", "@check and not @manual", "@tests and not @manual"]
```

### Comparing `sp_variant-3.4.2/PKG-INFO` & `sp_variant-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sp-variant
-Version: 3.4.2
+Version: 3.5.0
 Summary: Detect the Linux distribution for the StorPool build system
 Project-URL: Homepage, https://repo.storpool.com/public/doc/sp-variant/
 Project-URL: Changelog, https://github.com/storpool/sp-variant/blob/main/docs/changes.md
 Project-URL: Source Code, https://github.com/storpool/sp-variant
 Author-email: StorPool <support@storpool.com>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

