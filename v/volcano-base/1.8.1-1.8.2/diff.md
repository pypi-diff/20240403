# Comparing `tmp/volcano_base-1.8.1.tar.gz` & `tmp/volcano_base-1.8.2.tar.gz`

## Comparing `volcano_base-1.8.1.tar` & `volcano_base-1.8.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.mise.local.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.mise.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.release-please-manifest.json
--rw-r--r--   0        0        0    17385 2020-02-02 00:00:00.000000 volcano_base-1.8.1/CHANGELOG.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.1/release-please-config.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-1.8.1/requirements-dev.lock
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-1.8.1/requirements.lock
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.github/release-please/release-please-config.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.github/release-please/release-please-manifest.json
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/__init__.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/config.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/down/__init__.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/down/cesm2.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/down/historic_so2.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/down/ob16.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/load/__init__.py
--rw-r--r--   0        0        0    21670 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/load/load_c2w_files.py
--rw-r--r--   0        0        0    31462 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/load/load_ob16.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/manipulate/__init__.py
--rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-1.8.1/src/volcano_base/manipulate/time_series.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-1.8.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-1.8.1/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-1.8.1/README.md
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.mise.local.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.mise.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.release-please-manifest.json
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 volcano_base-1.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.2/release-please-config.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-1.8.2/requirements-dev.lock
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-1.8.2/requirements.lock
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.github/release-please/release-please-config.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.github/release-please/release-please-manifest.json
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/__init__.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/config.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/down/__init__.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/down/cesm2.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/down/historic_so2.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/down/ob16.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/load/__init__.py
+-rw-r--r--   0        0        0    22053 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/load/load_c2w_files.py
+-rw-r--r--   0        0        0    31462 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/load/load_ob16.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/manipulate/__init__.py
+-rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-1.8.2/src/volcano_base/manipulate/time_series.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-1.8.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-1.8.2/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-1.8.2/README.md
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-1.8.2/PKG-INFO
```

### Comparing `volcano_base-1.8.1/.mise.toml` & `volcano_base-1.8.2/.mise.toml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/.pre-commit-config.yaml` & `volcano_base-1.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/CHANGELOG.md` & `volcano_base-1.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [1.8.2](https://github.com/engeir/volcano-base/compare/v1.8.1...v1.8.2) (2024-04-03)
+
+
+### Code Refactoring
+
+* **cesm2 load:** better error message that hints to where files can be dowloaded ([404c952](https://github.com/engeir/volcano-base/commit/404c9521f58e57df48f3c8b32bcfb0ba17fa7ffb))
+
 ## [1.8.1](https://github.com/engeir/volcano-base/compare/v1.8.0...v1.8.1) (2024-03-22)
 
 
 ### Bug Fixes
 
 * **time series:** expose subtract_climatology to the manipulate module ([1d48f98](https://github.com/engeir/volcano-base/commit/1d48f98ae91677221ce576c63d834414627041f8))
```

### Comparing `volcano_base-1.8.1/release-please-config.json` & `volcano_base-1.8.2/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/requirements-dev.lock` & `volcano_base-1.8.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/requirements.lock` & `volcano_base-1.8.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/.github/release-please/release-please-config.json` & `volcano_base-1.8.2/.github/release-please/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/.github/workflows/release.yml` & `volcano_base-1.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/config.py` & `volcano_base-1.8.2/src/volcano_base/config.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/down/cesm2.py` & `volcano_base-1.8.2/src/volcano_base/down/cesm2.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,36 +37,33 @@
         link = tag.get("href")
         if link.endswith(".nc") or link.endswith(".md"):
             files.append(link)
             # print(_URL + link)
     return files
 
 
-def save_cesm_files(path: pathlib.Path) -> None:
+def _save_cesm_files(path: pathlib.Path) -> None:
     """Save the CESM2 NIRD archive files to disk.
 
-    This function is used by functions inside the `volcano_base.load` module, and should
-    not be needed to be called by the user.
-
     Parameters
     ----------
     path : pathlib.Path
         Path to the file to download.
     """
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-    if not path.exists():
-        path.mkdir(parents=False)
     answer = input(
-        f"Is it ok that I download all CESM2 NIRD archive files to {path.resolve()}? [y/N] "
+        f"Is it ok that I create the directory and download all CESM2 NIRD archive files to {path.resolve()}? [y/N] "
     ).lower()
     if answer not in ["y", "yes"]:
         sys.exit(
             "Ok, I will not download anything. The files are needed to run the script,"
             f" and can be downloaded manually from {_URL}."
         )
+    if not path.exists():
+        path.mkdir(parents=True)
     for file in _find_files():
         # Input file with injected SO2.
         _download_cesm_file(path, file)
     print("Done!")
 
 
 def _download_cesm_file(path: pathlib.Path, file_name: str) -> None:
@@ -96,24 +93,24 @@
         chunk_size = 8192
         total = int(total_length) // chunk_size if total_length is not None else 0
         with progress:
             progress.console.print(f"[progress.description]Downloading {file_name}")
             with open(file, "wb") as f:
                 for chunk in progress.track(
                     r.iter_content(chunk_size=chunk_size),
-                    # total=20851,
                     total=total,
                     description=f"[cyan]Downloading {file_name}",
                 ):
                     # If you have chunk encoded response uncomment if
                     # and set chunk_size parameter to None.
                     # if chunk:
                     f.write(chunk)
 
 
-def _main() -> None:
+def save_cesm_files() -> None:
+    """Save the CESM2 NIRD archive files to disk."""
     path: pathlib.Path = volcano_base.config.DATA_PATH / "nird-archive"
-    save_cesm_files(path)
+    _save_cesm_files(path)
 
 
 if __name__ == "__main__":
-    _main()
+    save_cesm_files()
```

### Comparing `volcano_base-1.8.1/src/volcano_base/down/historic_so2.py` & `volcano_base-1.8.2/src/volcano_base/down/historic_so2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/down/ob16.py` & `volcano_base-1.8.2/src/volcano_base/down/ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/load/load_c2w_files.py` & `volcano_base-1.8.2/src/volcano_base/load/load_c2w_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 import xarray as xr
 from returns.result import Failure, Result, Success
 from xarray.core.types import T_Xarray
 
 import volcano_base
 
 
+class CESM2FileNotFound(FileNotFoundError):
+    """Raise an error if one of the CESM2 files are not found."""
+
+    def __init__(self, *args: object) -> None:
+        if args:
+            msg = f'Cannot find the file "{args[0]}", which is a nescessary CESM2 file.'
+        else:
+            msg = "Cannot find the necessary CESM2 files."
+        self.message = f"{msg} Please run the `save_cesm_files` function within `down.cesm2` to see what files are missing."
+        super().__init__(self.message)
+
+
 class FindFiles:
     """Find files that match a pre-defined regular expression.
 
     Parameters
     ----------
     ft : str
         file type to look for
@@ -34,15 +46,15 @@
     _bad_files : files that were candidates but that did not match the regex
     _matched_files : files that have been looked up among the files found with the regex
     _sort_order : tuple with the sorting that is applied to the files
     _sort_reverse : bool stating if the sorting of the files should be reversed
 
     Raises
     ------
-    ConnectionError
+    CESM2FileNotFound
         If the files cannot be found the hard disk might not be mounted
 
     Examples
     --------
     >>> ff = FindFiles()
 
     You find nothing since the date is wrong.
@@ -141,18 +153,15 @@
             -
             # Match for date
             # Match exactly 8 digits
             (\d{8})"""
         pattern = re.compile(regex + self.ft, re.X)
         self.root_path = pathlib.Path(volcano_base.config.DATA_PATH)
         if not self.root_path.exists():
-            raise ConnectionError(
-                "The file path could not be found. Are you sure the harddisk is"
-                " connected?"
-            )
+            raise CESM2FileNotFound()
         files = self.root_path.rglob(f"**/*{self.ft}")
         self._initial_file_lookup(files, pattern)
         self._matched_files: list[tuple[str, str, str, str, str, str]] | None = None
         self._sort_order: tuple[str, ...] | None = None
         self._sort_reverse: bool = False
 
     def copy(self) -> Self:
```

### Comparing `volcano_base-1.8.1/src/volcano_base/load/load_ob16.py` & `volcano_base-1.8.2/src/volcano_base/load/load_ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/manipulate/__init__.py` & `volcano_base-1.8.2/src/volcano_base/manipulate/__init__.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/src/volcano_base/manipulate/time_series.py` & `volcano_base-1.8.2/src/volcano_base/manipulate/time_series.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/.gitignore` & `volcano_base-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/LICENSE` & `volcano_base-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.1/README.md` & `volcano_base-1.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.1</sup> <!-- x-release-please-version -->
+<sup>Latest version: v1.8.2</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

### Comparing `volcano_base-1.8.1/pyproject.toml` & `volcano_base-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "volcano-base"
-version = "1.8.1"
+version = "1.8.2"
 description = "Download, find and manipulate volcano and climate related time series"
 authors = [{ name = "engeir", email = "engeir@pm.me" }]
 license = "MIT"
 readme = "README.md"
 requires-python = ">= 3.12"
 dependencies = [
     "returns>=0.22.0",
```

### Comparing `volcano_base-1.8.1/PKG-INFO` & `volcano_base-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: volcano-base
-Version: 1.8.1
+Version: 1.8.2
 Summary: Download, find and manipulate volcano and climate related time series
 Author-email: engeir <engeir@pm.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: cftime>=1.6.3
@@ -19,15 +19,15 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: xarray>=2024.1.1
 Description-Content-Type: text/markdown
 
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.1</sup> <!-- x-release-please-version -->
+<sup>Latest version: v1.8.2</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

