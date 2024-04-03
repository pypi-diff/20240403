# Comparing `tmp/dsvenv-1.2.1-py3-none-any.whl.zip` & `tmp/dsvenv-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15041 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        5 b- defN 22-Feb-15 08:47 dsvenv/.version
--rw-rw-rw-  2.0 fat      310 b- defN 22-Feb-14 19:34 dsvenv/__init__.py
--rw-rw-rw-  2.0 fat    53228 b- defN 22-Feb-15 08:42 dsvenv/__main__.py
--rw-rw-rw-  2.0 fat      283 b- defN 22-Feb-15 08:47 dsvenv-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Feb-15 08:47 dsvenv-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       48 b- defN 22-Feb-15 08:47 dsvenv-1.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 22-Feb-15 08:47 dsvenv-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      605 b- defN 22-Feb-15 08:47 dsvenv-1.2.1.dist-info/RECORD
-8 files, 54578 bytes uncompressed, 13983 bytes compressed:  74.4%
+Zip file size: 15659 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-03 08:57 dsvenv/.version
+-rw-rw-rw-  2.0 fat      324 b- defN 24-Apr-03 08:50 dsvenv/__init__.py
+-rw-rw-rw-  2.0 fat    55338 b- defN 24-Apr-03 08:50 dsvenv/__main__.py
+-rw-rw-rw-  2.0 fat      286 b- defN 24-Apr-03 08:57 dsvenv-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 08:57 dsvenv-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       48 b- defN 24-Apr-03 08:57 dsvenv-2.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-03 08:57 dsvenv-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      605 b- defN 24-Apr-03 08:57 dsvenv-2.0.0.dist-info/RECORD
+8 files, 56705 bytes uncompressed, 14601 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dsvenv/__init__.py
 Comment: 
 
 Filename: dsvenv/__main__.py
 Comment: 
 
-Filename: dsvenv-1.2.1.dist-info/METADATA
+Filename: dsvenv-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: dsvenv-1.2.1.dist-info/WHEEL
+Filename: dsvenv-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: dsvenv-1.2.1.dist-info/entry_points.txt
+Filename: dsvenv-2.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dsvenv-1.2.1.dist-info/top_level.txt
+Filename: dsvenv-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dsvenv-1.2.1.dist-info/RECORD
+Filename: dsvenv-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dsvenv/.version

```diff
@@ -1 +1 @@
-1.2.1
+2.0.0
```

## dsvenv/__init__.py

```diff
@@ -3,9 +3,9 @@
 
 try:
     with open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)), '.version'), 'rt'
     ) as fid:
         __version__ = fid.readline().strip()
 except FileNotFoundError:
-    warnings.warn('.version file could not be found')
+    warnings.warn('.version file could not be found', stacklevel=1)
     __version__ = '0.0.0+dev'
```

## dsvenv/__main__.py

```diff
@@ -1,8 +1,10 @@
 """
+dsvenv - a tool to manage Python virtual environments for DS projects.
+
 dsvenv is created on top of several other Python tools (venv, pip, pre-commit) and
 serves to simplify the setup of the projects for developers. On Windows, it allows
 specifying the Python version (>3.5) that should be used for the virtual environment.
 
 Ideally after cloning the new repository you would need to execute a single command:
   $ dsvenv
 or
@@ -65,58 +67,60 @@
        base venv of the requested version does exist it will be used without the check
        for a possibly newer version. I.e. if you requested Python 3.8.* and you already
        have 3.8.1 - it will be used even if 3.8.9 is available for installation.
 
     4. Any required packages will be installed (possible custom pip configuration). Any
        packages can be specified via the requirement files (using `-r` option) or in the
        configuration file (`requires` option of `dsvenv` section). Additionally the
-       latter option allows to specify `==None` as the package specification - this
+       latter option allows to specify '===None' as the package specification - this
        means that the package won't be installed even if dsvenv usually does it by
        default.
        The order of the package installation is the following:
        - `pip` and `setuptools` (installed with `--upgrade` flag);
        - `keyring` and `artifacts-keyring` - to ensure access to Azure Artifacts;
        - other packages for the build system specified in configuration file;
        - other packages specified in requirements files.
 
     5. The environment will be verified.
 
     6. Pre-commit hooks will be installed if `.pre-commit-config.yaml` can be found.
 """
-from argparse import ArgumentParser
-from collections import namedtuple
-from configparser import ConfigParser, NoSectionError
-from pathlib import Path
-from pip._internal.configuration import CONFIG_BASENAME as _PIP_CONF
-from pkg_resources import Requirement
-from packaging.specifiers import Specifier, InvalidSpecifier
-from packaging.version import Version
-from urllib.request import urlopen
+
 import ast
 import json
 import logging
 import os
 import re
 import shutil
 import subprocess
 import sys
 import traceback
 import zipfile
+from argparse import ArgumentParser, Namespace
+from configparser import ConfigParser, NoSectionError
+from pathlib import Path
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union
+from urllib.request import urlopen
 
+from packaging.requirements import Requirement
+from packaging.specifiers import InvalidSpecifier, SpecifierSet
+from packaging.version import Version
+from pip._internal.configuration import CONFIG_BASENAME as _PIP_CONF
 
 try:
     import colorlog
 except ImportError:
     pass
 
 
+# Local Folder
 from . import __version__
 
 
-def path_or_none(path):
+def path_or_none(path: Path) -> Optional[Path]:
     """
     A small helper that returns a `path` if it exists or `None` otherwise.
     """
     return path if path.exists() else None
 
 
 _DEFAULT_SETUP_CFG = path_or_none(Path.cwd() / 'setup.cfg')
@@ -126,32 +130,45 @@
 _LEGACY_AZURE_PIPELINES_YAML = path_or_none(Path.cwd() / 'azure.yml')
 
 # A base URL for the Nuget package service used to install Python into the base
 # environment on Windows
 _NUGET_PACKAGE_BASE_URL = 'https://api.nuget.org/v3-flatcontainer'
 
 # Any requirements that MUST be present in the virtual environment and cannot be
-# excluded using '==None' syntax
+# excluded using '===None' syntax
 _MANDATORY_DSVENV_REQUIRES = ['pip', 'setuptools']
 
 # The requirements that need to be installed in order to use the Azure Artifacts PyPi.
 # They can be excluded, but pip won't be able to properly handle the custom Azure index
 # without them.
 _MANDATORY_AZURE_ARTIFACTS_REQUIRES = ['keyring', 'artifacts-keyring']
 
+
+def _parse_requirements(requirements: List[str]) -> Dict[str, Requirement]:
+    """
+    Parse the requirements using setuptools and return a dictionary of them.
+
+    Args:
+        requirements: A list of pip requirements.
+
+    Returns:
+        A dictionary with the package names as keys and the full requirement specs as
+            values.
+    """
+    return {Requirement(r).name: Requirement(r) for r in requirements}
+
+
 # These are the default versions specifications of packages needed to be installed.
-_DEFAULT_DSVENV_REQUIRES = [
-    *_MANDATORY_DSVENV_REQUIRES,
-    *_MANDATORY_AZURE_ARTIFACTS_REQUIRES,
-    'dsbuild==0.0.8',
-]
-_DEFAULT_DSVENV_REQUIRES = {
-    Requirement.parse(r).project_name: Requirement.parse(r)
-    for r in _DEFAULT_DSVENV_REQUIRES
-}
+_DEFAULT_DSVENV_REQUIRES = _parse_requirements(
+    [
+        *_MANDATORY_DSVENV_REQUIRES,
+        *_MANDATORY_AZURE_ARTIFACTS_REQUIRES,
+        'dsbuild==0.0.8',
+    ]
+)
 
 _THIS_PYTHON_VERSION = '{}.{}.{}'.format(*sys.version_info[:3])
 
 _VENV_BIN_SEARCH_DIRS = ['.', 'Scripts', 'bin']
 
 if sys.platform == 'win32':
     _BASE_ENVS_DIR = Path(
@@ -160,46 +177,29 @@
             Path(os.environ['LOCALAPPDATA']) / 'dsvenv' / 'base_envs',
         )
     )
 
 
 PipConfig = dict
 
-# Because Python 3.6. is still in play we cannot use the `defaults` parameter of the
-# named tuple, hence the workaround (https://stackoverflow.com/a/18348004/934961):
-try:
-    AzurePipelinesConfig = namedtuple(
-        'AzurePipelinesConfig', 'python_version dsvenv_version', defaults=(None, None)
-    )
-    DSVenvConfig = namedtuple(
-        'DSVenvConfig',
-        'python_version azure_pipelines_yml requires',
-        defaults=(
-            _THIS_PYTHON_VERSION,
-            _DEFAULT_AZURE_PIPELINES_YAML or _LEGACY_AZURE_PIPELINES_YAML,
-            _DEFAULT_DSVENV_REQUIRES,
-        ),
-    )
-except TypeError:
-    AzurePipelinesConfig = namedtuple(
-        'AzurePipelinesConfig', 'python_version dsvenv_version'
-    )
-    DSVenvConfig = namedtuple(
-        'DSVenvConfig', 'python_version azure_pipelines_yml requires'
-    )
 
-    AzurePipelinesConfig.__new__.__defaults__ = (None, None)
-    DSVenvConfig.__new__.__defaults__ = (
-        _THIS_PYTHON_VERSION,
-        _DEFAULT_AZURE_PIPELINES_YAML or _LEGACY_AZURE_PIPELINES_YAML,
-        _DEFAULT_DSVENV_REQUIRES,
+class AzurePipelinesConfig(NamedTuple):
+    python_version: Optional[str] = None
+    dsvenv_version: Optional[str] = None
+
+
+class DSVenvConfig(NamedTuple):
+    python_version: str = _THIS_PYTHON_VERSION
+    azure_pipelines_yml: Optional[Path] = (
+        _DEFAULT_AZURE_PIPELINES_YAML or _LEGACY_AZURE_PIPELINES_YAML
     )
+    requires: Dict[str, Requirement] = _DEFAULT_DSVENV_REQUIRES
 
 
-def setup_logging(loglevel=logging.INFO):
+def setup_logging(loglevel: int = logging.INFO):
     """
     Sets up the logger for the script.
 
     The logs will have a format: TIMESTAMP LEVEL: MESSAGE
     If `colorlog` is installed and running inside a tty the log messages will be
     colored.
 
@@ -215,172 +215,198 @@
     else:
         formatter = logging.Formatter(log_format)
     log_hangler = logging.StreamHandler()
     log_hangler.setFormatter(formatter)
     root.addHandler(log_hangler)
 
 
-def check_call(executable, *args, **kwargs):
+def check_call(executable: Path, *args: str, **kwargs: Dict[str, Any]):
     """
     Runs `subprocess.check_call` ensuring that all the arguments are strings.
 
     This is a convenience wrapper for `subprocessing.check_call`, which allows
     passing any values as the arguments (e.g. pathlib.Path) without the explicit
     conversion to `str`.
 
     All the non-keyword arguments (`executable` and `args`) will be passed to the
     `check_call` as a list. This means that any keyword arguments **must** use the
     keywords, otherwise they will be treated as the arguments for the executable.
 
     Args:
-        executable (Path): A path to the executable to call, e.g. echo.
+        executable: A path to the executable to call, e.g. echo.
 
-        args: any arguments to use for calling the executable,
-            e.g. 'hello', 'world'.
+        args: any arguments to use for calling the executable, e.g. 'hello', 'world'.
 
         kwargs: any keyword arguments to pass to `subprocess.check_call`, e.g. stdin,
-                stdout and stderr.
+            stdout and stderr.
 
     Raises:
         `CalledProcessError` if the return code of the command is not zero.
     """
-    args = [str(a) for a in [executable, *args]]
-    subprocess.check_call(args, **kwargs)
+    args_str = [str(a) for a in [executable, *args]]
+    subprocess.check_call(args_str, **kwargs)  # type: ignore[arg-type]
 
 
-def check_output(executable, *args, **kwargs):
+def check_output(executable: Path, *args: str, **kwargs: Dict[str, Any]) -> str:
     """
     Runs `subprocess.check_output` ensuring that all the arguments are strings.
 
     This is a convenience wrapper for `subprocessing.check_output`, which allows
     passing any values as the arguments (e.g. pathlib.Path) without the explicit
     conversion to `str`.
 
     All the non-keyword arguments (`executable` and `args`) will be passed to the
     `check_call` as a list. This means that any keyword arguments **must** use the
     keywords, otherwise they will be treated as the arguments for the executable.
 
     Args:
-        executable (Path): A path to executable to call, e.g. 'echo'.
+        executable: A path to executable to call, e.g. 'echo'.
 
         args: any arguments to use for calling the executable,
             e.g. 'hello', 'world'.
 
         kwargs: any keyword arguments to pass to `subprocess.check_output`, e.g. stdin,
             stdout and stderr.
 
-    Returns (str):
+    Returns:
         A decoded output of the call.
 
     Raises:
         `CalledProcessError` if the return code of the command is not zero.
     """
-    args = [str(a) for a in [executable, *args]]
-    return subprocess.check_output(args, **kwargs).decode()
+    args_str = [str(a) for a in [executable, *args]]
+    out = subprocess.check_output(args_str, **kwargs)  # type: ignore[call-overload]
+    return out.decode()
 
 
-def version_matches_spec(version_to_check, version_spec):
+def as_specifier(specifier: str) -> SpecifierSet:
     """
-    Checks if a version string fully matches a given version specification.
-
-    'Matching' means 'version matching' according to PEP440 definition (which
-    allows using trailing wildcards and zero-padding):
-    https://www.python.org/dev/peps/pep-0440/#version-matching
+    Try to convert a version specifier to a `SpecifierSet`.
 
     Args:
-        version_to_check (str): A version that should be checked.
-
-        version_spec (str): A version specification (e.g. 1.2.3 or 1.2.*)
+        specifier: A version specifier to convert.
 
-    Returns (Bool):
-        `True` if the versions matches the spec according to the following table:
-        version | spec   | Result
-        ---------------------------
-        1.2.3   | 1.2.3  | True
-        1.2.3   | 1.2.*  | True
-        1.2.3   | 1.*    | True
-        1.2.0   | 1.2    | True
-        1.0.0   | 1      | True
-        1.2     | 1.2.0  | True
-        1       | 1.0.0  | True
-        1.0.0   | 1      | True
-        1.2.3   | 1.2.9  | False
-        1.2.10  | 1.2.1  | False
-        1.2.3   | 1.2    | False
-        1.2.3   | 1      | False
+    Returns:
+        A `SpecifierSet` object.
 
     Raises:
-        ValueError: if the version specification doesn't is not correct (e.g. 1* instead
-            of 1.*).
-
+        InvalidSpecifier: if the version specification is not correct.
     """
-    version = Version(version_to_check)
-
     try:
-        specifier = Specifier(f'=={version_spec}')
+        conv_specifier = SpecifierSet(specifier)
     except InvalidSpecifier:
-        raise ValueError(
-            f'A version specification {version_spec} used to verify a version '
-            f'{version_to_check} is incorrect.'
-        )
+        try:
+            conv_specifier = SpecifierSet(f'=={specifier}')
+        except InvalidSpecifier:
+            raise InvalidSpecifier(
+                f'The version specification {specifier} is incorrect. Supported '
+                f'formats are e.g. 1.2.3, 1.2.*, >=1.2.3, ~=1.2.3, !=1.2.3, '
+                f'<=1.2.3, >1.2.3, <1.2.3, >=1.2, <1.3, >=1.2, <1.3.'
+            )
+    return conv_specifier
+
+
+def version_matches_spec(version_to_check: str, version_spec: str) -> bool:
+    """
+    Checks if a version string matches a given version specification.
 
+    This function allows both 'version matching' and 'version specification' matching.
+    For 'version matching', if the user provides a version number then '==' is added in
+    front and matching is done according to PEP440 definition (which allows using
+    trailing wildcards and zero-padding):
+    https://www.python.org/dev/peps/pep-0440/#version-matching
+    If user provide a version specification e.g. (~=1.2.3, ==1.2.3 or even
+    '>= 1.0, < 2.0') then it is used as is. More examples can be found here:
+    https://peps.python.org/pep-0440/#examples
+
+    Args:
+        version_to_check: A version that should be checked.
+
+        version_spec: A version (e.g. 1.2.3, 1.2.*) or a version specification
+            (>= 1.0).
+
+    Returns:
+        `True` if the versions matches the spec according to the following table:
+        version     | spec  | Result
+        ----------------------------
+        1.2.3       | 1.2.3 | True
+        1.2.3       | 1.2.* | True
+        1.2.3       | 1.*   | True
+        1.2.0       | 1.2   | True
+        1.0.0       | 1     | True
+        1.2         | 1.2.0 | True
+        1           | 1.0.0 | True
+        1.0.0       | 1     | True
+        >1.2.2      | 1.2.3 | True
+        ~=1.2.3     | 1.2.4 | True
+        >=1.0, <2.0 | 1.2.3 | True
+        1.2.3       | 1.2.9 | False
+        1.2.10      | 1.2.1 | False
+        1.2.3       | 1.2   | False
+        1.2.3       | 1     | False
+        >1.2.3      | 1.2.3 | False
+        ~=1.2.3     | 1.3.3 | False
+        >=1.0, <2.0 | 2.2.3 | False
+    """
+    version = Version(version_to_check)
+    specifier = as_specifier(version_spec)
     return version in specifier
 
 
-def python_version_matches_spec(version_to_check, version_spec):
+def python_version_matches_spec(version_to_check: str, version_spec: str) -> bool:
     """
     Checks if a Python version string matches a given version specification.
 
     For the moment it works in exactly the same way as a `version_matches_spec`,
     but this may change in future.
 
     Args:
-        version_to_check (str): A version that should be checked.
+        version_to_check: A version that should be checked.
 
-        version_spec (str): A version specification (e.g. 1.2.3 or 1.2.*)
+        version_spec: A version specification (e.g. 1.2.3 or 1.2.*)
 
-    Returns (Bool):
+    Returns:
         `True` if the versions matches.
     """
     return version_matches_spec(version_to_check, version_spec)
 
 
-def venv_exists(venv_dir):
+def venv_exists(venv_dir: Path) -> bool:
     """
     Verifies if the virtual environment exists in the specified directory.
 
     Args:
-        venv_dir (Path): A path to check.
+        venv_dir: A path to check.
 
-    Returns (Bool):
+    Returns:
         `True` if the virtual environment exists and contains a Python executable.
     """
-    return venv_dir.is_dir() and get_venv_python(venv_dir, required=False) is not None
+    return venv_dir.is_dir() and venv_python_exists(venv_dir)
 
 
-def list_base_venv_python_versions():
+def list_base_venv_python_versions() -> List[str]:
     """
     List all the base python versions in descending order.
     """
     if not _BASE_ENVS_DIR.is_dir():
         return []
 
     dirs = [d.name for d in _BASE_ENVS_DIR.iterdir() if venv_exists(d)]
     versions = sorted((Version(d) for d in dirs), reverse=True)
     return [f'{v}' for v in versions]
 
 
-def list_available_to_download_python_versions():
+def list_available_to_download_python_versions() -> List[str]:
     """
     List all the Python versions available for downloading.
 
     Any of these versions can then be downloaded to create a local base Python
     environment.
 
-    Returns [str]:
+    Returns:
         A list of Python versions in descending order.
 
     Raises:
         EnvironmentError: If running on non-Windows OS.
         RuntimeError: If for any reason cannot retrieve the list of versions online.
     """
     if sys.platform != 'win32':
@@ -401,34 +427,34 @@
     except Exception as e:
         raise RuntimeError(
             f'Error retrieving a list of available Python versions from {versions_url}.'
             f'Exact error: {e}.'
         )
 
 
-def resolve_python_version_spec(python_version_spec):
+def resolve_python_version_spec(python_version_spec: str) -> str:
     """
     Resolves a Python version specification to a version that can be used for venv.
 
     On Windows it first considers the highest compatible version available already
     locally as a base venv. If nothing is suitable, it looks for a the highest
     compatible version online.
 
     On other platforms it will always return a version of the system Python if it is
     compatible with the version specification.
 
     Args:
-        python_version_spec (str): A Python version specification.
-
-    Raises:
-        RuntimeError: If the compatible version cannot be found.
+        python_version_spec: A Python version specification.
 
-    Returns (str)
+    Returns:
         A Python version compatible with the given specification. As a result running
         `create_base_venv` should succeed if provided with this parameter.
+
+    Raises:
+        RuntimeError: If the compatible version cannot be found.
     """
 
     def get_compatible_version(versions, python_version_spec):
         return next(
             (
                 v
                 for v in versions
@@ -455,15 +481,15 @@
 
     compatible_version = get_compatible_version(
         list_base_venv_python_versions(), python_version_spec
     )
     if compatible_version is not None:
         logging.info(
             f'A base environment of Python {compatible_version} found which is '
-            f'compatible with the specification of {python_version_spec}. it will'
+            f'compatible with the specification of {python_version_spec}. it will '
             f'be used to create a virtual environment.'
         )
         return compatible_version
 
     compatible_version = get_compatible_version(
         list_available_to_download_python_versions(), python_version_spec
     )
@@ -478,260 +504,273 @@
     raise RuntimeError(
         f'Unfortunately Python {python_version_spec} is not available '
         f'neither locally (check {str(_BASE_ENVS_DIR)}) nor online (check '
         f'https://www.nuget.org/packages/python).'
     )
 
 
-def base_venv_exists(python_version):
+def base_venv_exists(python_version: str) -> bool:
     """
     Verifies if the base virtual environment of the specified Python version exists.
 
     The base environment stored in `python_version` subdirectory of `_BASE_ENVS_DIR`
     is expected to contain Python of the same version.
 
     Args:
-        python_version (str): A Python version to check.
+        python_version: A Python version to check.
 
-    Returns (Bool):
+    Returns:
         `True` if the base virtual environment exists and contains a Python executable.
     """
     return venv_exists(_BASE_ENVS_DIR / python_version)
 
 
-def venv_is_compatible(venv_dir, python_version_spec):
+def venv_is_compatible(venv_dir: Path, python_version_spec: str) -> bool:
     """
-    Verifies if the virtual environment is compatible with the given Python version
-    specification.
+    Verifies if the venv is compatible with the Python version specification.
 
     Args:
-        venv_dir (Path): A path to check.
+        venv_dir: A path to check.
 
-        python_version_spec (str): A Python version specification.
+        python_version_spec: A Python version specification.
 
-    Returns (Bool):
+    Returns:
         `True` if the virtual environment exists and contains a Python version that is
         compatible with the `python_version_spec`.
     """
     venv_python_version = get_venv_python_version(venv_dir)
     return python_version_matches_spec(venv_python_version, python_version_spec)
 
 
-def get_venv_executable(venv_dir, executable, required=True):
+def get_venv_executable(venv_dir: Path, executable: str) -> Path:
     """
     Return the full path to an executable inside a given virtual environment.
 
     Args:
-        venv_dir (Path): Path to the directory containing the virtual environment.
+        venv_dir: Path to the directory containing the virtual environment.
 
-        executable (str): Name of the executable.
+        executable: Name of the executable.
 
-        required (bool): Whether to consider it a fatal error if the executable is not
-            found.
-
-    Returns (Path or None):
+    Returns:
         Full path to an executable inside the virtual environment.
 
     Raises:
-        FileNotFoundError:  When the executable is `required` and could not be found .
+        FileNotFoundError:  When the executable could not be found.
     """
 
     search_path = [str(venv_dir / p) for p in _VENV_BIN_SEARCH_DIRS]
     venv_executable = shutil.which(cmd=executable, path=os.pathsep.join(search_path))
 
-    if required and venv_executable is None:
+    if venv_executable is None:
         raise FileNotFoundError('The virtual environment executable could not be found')
 
-    if venv_executable is not None:
-        return Path(venv_executable)
-    else:
-        return None
+    return Path(venv_executable)
 
 
-def get_base_venv_executable(python_version, executable, required=True):
+def get_venv_executable_optional(venv_dir: Path, executable: str) -> Optional[Path]:
     """
-    Return the full path to an executable inside a given base virtual environment.
+    Return the full path to an executable inside a given virtual environment.
 
     Args:
-        python_version (Path): A version of base Python environment.
-
-        executable (str):  Name of the executable.
-
-        required (bool):  Whether to consider it a fatal error if the executable is not
-            found.
+        venv_dir: Path to the directory containing the virtual environment.
 
-    Returns (Path or None):
-        Full path to an executable inside the virtual environment.
+        executable: Name of the executable.
 
-    Raises:
-        FileNotFoundError:  When the executable is `required` and could not be found.
+    Returns:
+        Full path to an executable inside the virtual environment, or None if the
+            executable is not found.
     """
-    return get_venv_executable(
-        _BASE_ENVS_DIR / python_version, executable=executable, required=required
-    )
+    try:
+        venv_executable = get_venv_executable(venv_dir=venv_dir, executable=executable)
+    except FileNotFoundError:
+        return None
+    return venv_executable
 
 
-def get_venv_python(venv_dir, required=True):
+def get_venv_python(venv_dir: Path) -> Path:
     """
     Return the Python executable inside a given virtual environment.
 
     Args:
-        venv_dir (Path): Path to the directory containing the virtual environment.
-
-        required (bool): Whether to consider it a fatal error if the executable is not
-            found.
+        venv_dir: Path to the directory containing the virtual environment.
 
     Returns:
-        Path or None: Full path to the Python executable inside the virtual environment.
+        Path: Full path to the Python executable inside the virtual environment.
 
     Raises:
-        FileNotFoundError:  When the executable is `required` and could not be found.
+        FileNotFoundError:  When the executable could not be found.
     """
-    return get_venv_executable(
-        venv_dir=venv_dir, executable=Path(sys.executable).name, required=required,
+    return get_venv_executable(venv_dir=venv_dir, executable=Path(sys.executable).name)
+
+
+def venv_python_exists(venv_dir: Path) -> bool:
+    """
+    Return whether the Python executable exists in a given virtual environment.
+
+    Args:
+        venv_dir: Path to the directory containing the virtual environment.
+
+    Returns:
+        bool: True if the Python executable exists in the virtual environment.
+    """
+    venv_executable = get_venv_executable_optional(
+        venv_dir=venv_dir, executable=Path(sys.executable).name
     )
+    return venv_executable is not None
 
 
-def get_base_python(python_version, required=True):
+def get_base_python(python_version: str) -> Path:
     """
     Return a base Python executable of a certain version.
 
     On Windows this function expects the base virtual environment with the required
     Python version to be present and looks for Python there.
 
     On other systems only system Python version is supported.
 
     Args:
-        python_version (str): A version of the base python to look for.
-
-        required (bool): Whether to consider it a fatal error if the executable is not
-            found.
+        python_version: A version of the base python to look for.
 
     Returns:
-        Path or None: Full path to the base Python executable.
+        Path: Full path to the base Python executable.
 
     Raises:
         EnvironmentError: On non-Windows OS if the `python_version` is different from
-        the system Python version.
-        FileNotFoundError:  When the executable is `required` and could not be found.
+            the system Python version.
     """
     if sys.platform != 'win32':
         if version_matches_spec(_THIS_PYTHON_VERSION, python_version):
             return sys.executable
         else:
             raise EnvironmentError(
                 f'Custom Python version is not supported on your platform '
                 f'({sys.platform}). You can only use system Python '
                 f'{_THIS_PYTHON_VERSION}.'
             )
 
-    return get_venv_python(_BASE_ENVS_DIR / python_version, required=required)
+    return get_venv_python(_BASE_ENVS_DIR / python_version)
 
 
-def run_python(python_executable, *args, **kwargs):
+def run_python(python_executable: Path, *args: str, **kwargs: Dict[str, Any]):
     """
     A convenience function to run a python command.
 
     Args:
-        python_executable (Path): A path to the python executable to call.
+        python_executable: A path to the python executable to call.
 
-        args (list or str): Any arguments to pass to the call, e.g.: '-m', 'pip',
-            'list' or '-m pip list'.
+        args: Any arguments to pass to the call, e.g.: '-m', 'pip', 'list' or
+            '-m pip list'.
 
         kwargs: Any keyword arguments to pass to the underlying `subprocess` call, e.g.
             stdin, stdout and stderr.
     """
-    check_call(python_executable, *args)
+    check_call(python_executable, *args, **kwargs)
 
 
-def run_pip(python_executable, *args):
+def run_pip(python_executable: Path, *args: Any, **kwargs: Dict[str, Any]):
     """
     A convenience function to run a pip command.
 
     Functionally it's equalent to `python -m pip` call.
 
     Args:
-        python_executable (Path): A path to the python executable to call.
+        python_executable: A path to the python executable to call.
 
-        args (list): Any arguments to pass to `pip`, e.g.: 'list'.
+        args: Any arguments to pass to `pip`, e.g.: 'list'.
 
         kwargs: Any keyword arguments to pass to the underlying `subprocess` call, e.g.
                 stdin, stdout and stderr.
     """
-    run_python(python_executable, '-m', 'pip', *args)
+    run_python(python_executable, '-m', 'pip', *args, **kwargs)
 
 
-def get_pip_packages(python_executable):
+def get_pip_packages(python_executable: Path) -> Dict[str, str]:
     """
     Retrieve a list of packages installed by pip.
 
     It gets only the versions of the packages reported as `package==version`. The other
     formats (e.g. the ones installed from git or local files are ignored).
 
     Args:
-        python_executable (Path): A path to the Python executable to check.
+        python_executable: A path to the Python executable to check.
 
-    Returns (dict):
+    Returns:
         A dictionary where the key corresponds to the name of the package and the value
             to its version.
+
+    Raises:
+        ValueError: If the package format is incorrect.
     """
     packages = check_output(python_executable, '-m', 'pip', 'freeze').split()
 
     # The output of `freeze` contains a package per line in a `package==version`
     # format, but there are exceptions (e.g. packages installed from git reviesion) -
     # we filter those out.
-    return dict(tuple(p.split('==')) for p in packages if '==' in p)
+    package_dict = {}
+    for p in packages:
+        if '==' in p:
+            try:
+                name, version = p.split('==')
+            except ValueError:
+                raise ValueError(
+                    f'Incorrect package format: {p}. Package format cannot have more '
+                    f'than one `==`.'
+                )
+            package_dict[name] = version
+
+    return package_dict
 
 
-def get_python_version(python_executable):
+def get_python_version(python_executable: Path) -> str:
     """
     Retrieve a version of the Python executable.
 
     Args:
-        python_executable (Path): A Python to check the version for.
+        python_executable: A Python to check the version for.
 
-    Returns (str):
+    Returns:
         A version in a form of '3.6.8'.
     """
     script = (
         "from sys import version_info as v; print(f'{v.major}.{v.minor}.{v.micro}')"
     )
 
     return check_output(python_executable, '-c', script)
 
 
-def get_venv_python_version(venv_dir):
+def get_venv_python_version(venv_dir: Path) -> str:
     """
     Retrieve a version of Python in a certain virtual environment.
 
     Args:
-        venv_dir (Path): A directory with the virtual environment.
+        venv_dir: A directory with the virtual environment.
 
-    Returns (str):
+    Returns:
         A version of the virtual environment Python executable in a form of '3.6.8'.
     """
     vpython = get_venv_python(venv_dir)
     return get_python_version(vpython).strip()
 
 
-def create_base_venv(target_dir, python_version):
+def create_base_venv(target_dir: Path, python_version: str):
     """
     Create a base virtual environment with the required Python version.
 
     On Windows this function installs only Python inside the required folder. It doesn't
     need for the folder to exist and it doesn't check if the folder is empty, so it will
     overwrite any files already there.
 
     Args:
-        target_dir (Path): A directory where the environment should be created.
+        target_dir: A directory where the environment should be created.
 
-        python_version (str): A Python version that needs to be installed.
+        python_version: A Python version that needs to be installed.
 
     Raises:
         EnvironmentError: If running on non-Windows OS.
+        RuntimeError: If the required Python version is not available for installation.
     """
     if sys.platform != 'win32':
         raise EnvironmentError(
             f'Custom Python version is not supported on your platform '
             f'({sys.platform}). You can only use system Python '
             f'{_THIS_PYTHON_VERSION}.'
         )
@@ -778,29 +817,29 @@
     extract_dir = nuget_dir / 'unzip'
     with zipfile.ZipFile(outfile, 'r') as zf:
         zf.extractall(extract_dir)
         for to_move in (extract_dir / 'tools').iterdir():
             to_move.rename(target_dir / to_move.name)
 
 
-def ensure_base_python(python_version):
+def ensure_base_python(python_version: str):
     """
     Ensures that the base virtual environment of a certain Python version exists.
 
     On Windows the base virtual environment will be created if it doesn't exist yet.
 
     A successful execution of this function means that `get_base_python(python_version)`
     can be called safely.
 
     Args:
-        python_version (str): A required Python version.
+        python_version: A required Python version.
 
     Raises:
         EnvironmentError: If running on non-Windows OS and requiring a Python version
-        different from the system one.
+            different from the system one.
     """
     if sys.platform != 'win32':
         if python_version == _THIS_PYTHON_VERSION:
             return
         else:
             raise EnvironmentError(
                 f'Custom Python version is not supported on your platform '
@@ -810,32 +849,32 @@
 
     if base_venv_exists(python_version):
         return
 
     create_base_venv(_BASE_ENVS_DIR / python_version, python_version)
 
 
-def setup_pip_config_file(venv_dir, pip_config):
+def setup_pip_config_file(venv_dir: Path, pip_config: Dict[str, str]) -> Optional[Path]:
     """
     Setup the pip config file for the virtual environment.
 
     If the `pip_config` argument is provided, the contents will be copied to the
     [global] section of the pip.conf/pip.ini (win/linux,macos) file inside a virtual
     environment. This can be used to provide any extra parameters to pip,
     e.g. `extra-index-url`.
 
     If the `pip_config` is `None` the venv pip configuration file will be removed from
     the virtual environment as well.
 
     Args:
-        venv_dir (Path): A directory with the virtual environment to initialize.
+        venv_dir: A directory with the virtual environment to initialize.
 
-        pip_config (dict): A dictionary with `pip` options.
+        pip_config: A dictionary with `pip` options.
 
-    Returns (Path):
+    Returns:
         A path to the pip configuration file if created, `None` otherwise.
     """
     pip_conf_path = venv_dir / _PIP_CONF
 
     if pip_config is None:
         if pip_conf_path.exists():
             pip_conf_path.unlink()
@@ -848,67 +887,72 @@
 
     with pip_conf_path.open('w') as fid:
         pip_conf.write(fid)
 
     return pip_conf_path
 
 
-def clear_venv(venv_dir):
+def clear_venv(venv_dir: Path):
     """
     Remove the virtual environment.
 
     Args:
-        venv_dir (Path): A directory containina a virtual environment.
+        venv_dir: A directory containina a virtual environment.
     """
     shutil.rmtree(venv_dir)
 
 
-def create_venv(venv_dir, dsvenv_config):
+def create_venv(venv_dir: Path, dsvenv_config: DSVenvConfig):
     """
     Create a bare virtual environment in a given directory.
 
     The function ensures that the base Python of the required version exists in the
     system and creates a virtual environment out of it at a specified location.
 
     Args:
-        venv_dir (Path): A directory where the virtual environment should be created.
+        venv_dir: A directory where the virtual environment should be created.
 
-        dsvenv_config (DsVenvConfig): A configuration containing various venv options.
+        dsvenv_config: A configuration containing various venv options.
     """
     python_version_spec = dsvenv_config.python_version
     python_version = resolve_python_version_spec(python_version_spec)
     ensure_base_python(python_version=python_version)
 
     # Create a virtual environment
     base_python = get_base_python(python_version=python_version)
     run_python(base_python, '-m', 'venv', f'{venv_dir}')
 
 
-def initialize_venv(venv_dir, dsvenv_config, pip_config, requirements):
+def initialize_venv(
+    venv_dir: Path,
+    dsvenv_config: DSVenvConfig,
+    pip_config: Dict[str, str],
+    requirements: List[Path],
+):
     """
     Initialize a virtual environment by installing the necessary requirements.
 
     The requirements installation goes in stages:
 
     1. Mandatory requirements (e.g. pip, setuptools) and present Azure PyPi
         requirements (artifacts-keyring) as specified in setup.cfg.
     2. Virtual environment pip configuration file is updated.
     3. All the rest required packages from setup.cfg.
     4. All the requirements files.
 
     Args:
-        venv_dir (Path):  Path to a virtual environment.
+        venv_dir:  Path to a virtual environment.
 
-        dsvenv_config (DsVenvConfig): additional venv options. All the requirements from
+        dsvenv_config: additional venv options. All the requirements from
             `_MANDATORY_DSVENV_REQUIRES` must be present in the config `requires`
             section.
 
-        pip_config (dict): Additional `pip` options for the environment.
+        pip_config: Additional `pip` options for the environment.
 
-        requirements (List[Path]): A list of paths to the existing requirements files.
+        requirements: A list of paths to the existing requirements files.
     """
 
     # Get the venv python executable
     vpython = get_venv_python(venv_dir)
     requires = dsvenv_config.requires
 
     # Ensure that all the required reqs will be installed.
@@ -947,29 +991,30 @@
     # Add a `-r` option before each requirement file.
     if requirements:
         vpython = get_venv_python(venv_dir)
         requirement_args = [a for r in requirements for a in ['-r', r]]
         run_pip(vpython, 'install', *requirement_args)
 
 
-def verify_venv(venv_dir, azure_pipelines_config):
+def verify_venv(venv_dir: Path, azure_pipelines_config: AzurePipelinesConfig):
     """
     Perform a sanity check on the interpreter executing this script.
 
     Verify if the environment that is being used is based on the correct version of
     Python and `dsvenv` (the ones stored in `azure.yml` if present).
 
     The function has no side effects and only writes warnings about any inconsistencies
     to the log.
 
     Args:
-        azure_pipelines_config (AzurePipelinesConfig): An Azure pipeline configuration
+        venv_dir: A path to the virtual environment directory.
+
+        azure_pipelines_config: An Azure pipeline configuration
             to verify the environment against (e.g. python version, dsvenv version).
     """
-
     required_python, required_dsvenv = azure_pipelines_config
     existing_python = get_venv_python_version(venv_dir)
     existing_dsvenv = __version__
 
     if required_python is not None:
         if not version_matches_spec(existing_python, required_python):
             logging.warning(
@@ -983,27 +1028,27 @@
             logging.warning(
                 f'The current dsvenv version ({existing_dsvenv}) is not the same as '
                 f'the version specified in Azure pipelines configuration '
                 f'({required_dsvenv}).'
             )
 
 
-def install_pre_commit_hooks(venv_dir):
+def install_pre_commit_hooks(venv_dir: Path):
     """
     Install the `pre-commit` hooks.
 
     This function assumes that when pre-commit hooks are configured for the repo, the
     `requirements.txt` file contains a pre-commit requirement
     (eg. `pre-commit==<version>`).
 
     Args:
-        venv_dir (str): The path to the virtual environment directory.
+        venv_dir: The path to the virtual environment directory.
 
     Raises:
-        Environment: When the pre-commit package is not installed.
+        EnvironmentError: When the pre-commit package is not installed.
     """
     vpython = get_venv_python(venv_dir)
 
     # Verify if pre-commit package itself is installed.
     if 'pre-commit' not in get_pip_packages(vpython):
         raise EnvironmentError(
             'The pre-commit package cannot be found in your virtual environment.\n'
@@ -1012,21 +1057,21 @@
         )
 
     # Then actually install the hooks.
     run_python(vpython, '-m', 'pre_commit', 'install')
 
 
 def ensure_venv(
-    venv_dir,
-    dsvenv_config,
-    pip_config,
-    requirements,
-    azure_pipelines_config,
-    clear,
-    should_install_pre_commit_hooks,
+    venv_dir: Path,
+    dsvenv_config: DSVenvConfig,
+    pip_config: Dict[str, str],
+    requirements: List[Path],
+    azure_pipelines_config: AzurePipelinesConfig,
+    clear: bool,
+    should_install_pre_commit_hooks: bool,
 ):
     """
     This function ensures existing of a compatible virtual environment.
 
     The existing virtual environment will be removed only if explicitly requested.
 
     The function will allow to proceed with the existing environment only if its Python
@@ -1039,31 +1084,35 @@
 
     The environment is verified to be in sync with `azure_pipelines_config` (used for
     CI builds of the package) if it exists.
 
     The pre-commit hooks will be created if requested.
 
     Args:
-        venv_dir (Path): A directory for the virtual environment should exist.
+        venv_dir: A directory for the virtual environment should exist.
 
-        dsvenv_config (DsVenvConfig): An additional configuration for the venv itself,
-            e.g. Python version, additional build packages.
+        dsvenv_config: An additional configuration for the venv itself, e.g. Python
+            version, additional build packages.
 
-        pip_config (dict): A pip configuration for the virtual environment.
+        pip_config: A pip configuration for the virtual environment.
 
-        requirements (List[Path]): A list of paths to the files with requirements that
-            will be installed in the environment.
+        requirements: A list of paths to the files with requirements that will be
+            installed in the environment.
 
-        azure_pipelines_config (AzurePipelinesConfig): An Azure pipelines config to
-            verify the environment against.
+        azure_pipelines_config: An Azure pipelines config to verify the environment
+            against.
 
-        clear (Bool): If `True`, any existing environment will be removed.
+        clear: If `True`, any existing environment will be removed.
 
-        should_install_pre_commit_hooks (Bool): If `True` the pre-commit hooks will be
+        should_install_pre_commit_hooks: If `True` the pre-commit hooks will be
             configured according to the `.pre-commit-config.yaml` file.
+
+    Raises:
+        EnvironmentError: If the existing environment is not compatible with the
+            required Python version.
     """
     if venv_exists(venv_dir) and clear:
         logging.warning(
             f'Existing environment at {venv_dir} will be removed as requested'
             f' by --clear flag.'
         )
         clear_venv(venv_dir)
@@ -1090,15 +1139,17 @@
 
     verify_venv(venv_dir, azure_pipelines_config)
 
     if should_install_pre_commit_hooks:
         install_pre_commit_hooks(venv_dir)
 
 
-def parse_setup_cfg(setup_cfg_path, python_version, venv_dir):
+def parse_setup_cfg(
+    setup_cfg_path: Path, python_version: str, venv_dir: Path
+) -> Tuple[Optional[PipConfig], DSVenvConfig]:
     """
     Parse the configuration file for pip and dsvenv config.
 
     The purpose of this function is to contain a lot of ugly code resulting in a fact
     that dsvenv operates over multiple config files (and command line arguments in
     addition), some of which are implicit and some may reference others.
 
@@ -1113,63 +1164,62 @@
         - a version from the configuration file;
         - a version from existing environment at `venv_dir`
         - a default version.
 
     2. parses any `requires` packages and resolves defaults and `None` packages.
 
     Args:
-        setup_cfg_path (Path): A path to the configuration file.
+        setup_cfg_path: A path to the configuration file.
 
-        python_version (str): Any explicitly provided Python version.
+        python_version: Any explicitly provided Python version.
 
-        venv_dir (Path): A venv directory.
+        venv_dir: A venv directory.
 
-    Returns (PipConfig, DsVenvConfig):
+    Returns:
         pip and dsvenv configurations.
     """
 
-    def prepare_requirements(requirements):
+    def prepare_requirements(requirements: List[str]) -> Dict[str, Requirement]:
         """
         A function that parses a requirement string and resolves defaults.
 
         First we use the `setuptools` functionality to parse the requirement specs
         and merge them with the default requirements (overwriting any defaults).
 
-        Then we throw away any requirements with '==None' spec allowing to override even
-        the defaults.
+        Then we throw away any requirements with '===None' spec allowing to override
+        even the defaults.
 
         Args:
-            requirements (Iterable[str]): A list of pip requirements.
+            requirements: A list of pip requirements.
 
-        Returns (Dict[str, Requirement]):
+        Returns:
             A dictionary, where keys are the package names and the values are full
             requirement specs, e.g.: { 'dsbuild': Requirement('dsbuild==0.0.7') }.
         """
         # Parse all the reqs together with specs
-        requirements = {
-            Requirement.parse(r).project_name: Requirement.parse(r)
-            for r in requirements
-        }
+        parsed_requirements = _parse_requirements(requirements)
 
         # Now combine them together allowing `requirements` to override any defaults.
-        requirements = {**_DEFAULT_DSVENV_REQUIRES, **requirements}
+        parsed_requirements = {**_DEFAULT_DSVENV_REQUIRES, **parsed_requirements}
 
-        # And finally throw away anything with a spec of '==None'
-        requirements = {
-            k: v for k, v in requirements.items() if v.specs != [('==', 'None')]
+        # And finally throw away anything with a spec of '===None'
+        parsed_requirements = {
+            k: v
+            for k, v in parsed_requirements.items()
+            if str(v.specifier) != '===None'
         }
 
-        return requirements
+        return parsed_requirements
 
     # Setting sensible defaults for the results
     # `dsvenv_config` will be used later to create a DsVenvConfig named tuple, which
     # already has the default values for the missing values, that's why we don't need
     # to add anything.
     pip_config = None
-    dsvenv_config = {}
+    dsvenv_config: Dict[str, Union[str, Path, Dict[str, Requirement]]] = {}
 
     if setup_cfg_path is not None:
         setup_cfg = ConfigParser()
         setup_cfg.read(setup_cfg_path)
 
         # Read pip config if it exists
         try:
@@ -1188,49 +1238,50 @@
                 logging.warning(
                     f'The following options specified in "dsvenv" section of the '
                     f'configuration file {setup_cfg_path} are unknown and will be'
                     f' ignored: {unknown_options}.'
                 )
 
             if 'azure_pipelines_yml' in dsvenv_config:
-                dsvenv_config['azure_pipelines_yml'] = (
-                    Path.cwd() / dsvenv_config['azure_pipelines_yml']
+                dsvenv_config['azure_pipelines_yml'] = Path.cwd() / str(
+                    dsvenv_config['azure_pipelines_yml']
                 )
 
             # Prepare the requirements
             # Since INI is not TOML, it cannot resolve a list option into a Python list.
             # Instead we receive it as a multiline string of format "[\n'dsbuild'\n]".
             # That's why we first convert it into a valid list.
             dsvenv_config['requires'] = prepare_requirements(
-                ast.literal_eval(dsvenv_config.get('requires', '[]'))
+                ast.literal_eval(str(dsvenv_config.get('requires', '[]')))
             )
         except NoSectionError:
             pass
 
     # And now we finally resolve the Python version:
     if python_version is not None:
         dsvenv_config['python_version'] = python_version
     elif 'python_version' not in dsvenv_config:
         if venv_exists(venv_dir):
             dsvenv_config['python_version'] = get_venv_python_version(venv_dir)
 
-    return pip_config, DSVenvConfig(**dsvenv_config)
+    dsvenv_conf = DSVenvConfig(**dsvenv_config)  # type: ignore[arg-type, return-value]
+    return pip_config, dsvenv_conf
 
 
-def parse_azure_pipelines(azure_pipelines_path):
+def parse_azure_pipelines(azure_pipelines_path: Optional[Path]) -> AzurePipelinesConfig:
     """
     Parse the Azure pipelines file if it exists.
 
     If `azure_pipelines_path` is explicitly `None` the function will check if either
     default `azure-pipelines.yml` or legacy `azure.yml` exists and use that one instead.
 
     Args:
-        azure_pipelines_path (Path): A path to Azure pipelines file.
+        azure_pipelines_path: A path to Azure pipelines file.
 
-    Return (AzurePipelinesConf):
+    Return:
         Azure pipelines configuration.
     """
     if azure_pipelines_path is None:
         return AzurePipelinesConfig()
 
     if azure_pipelines_path == _LEGACY_AZURE_PIPELINES_YAML:
         logging.warning(
@@ -1238,43 +1289,43 @@
             f'at {azure_pipelines_path}. Please rename it to "azure-pipelines.yml" '
             f'to silence this warning (do not forget to point the DevOps pipeline '
             f'to the new file).'
         )
 
     azure_pipeline_yaml = azure_pipelines_path.read_text()
 
-    azure_python_version = re.search(r'python_version:\s+(\S+)', azure_pipeline_yaml)
-    if azure_python_version is not None:
-        azure_python_version = azure_python_version.group(1)
-
-    azure_dsvenv_version = re.search(r'dsvenv_version:\s+(\S+)', azure_pipeline_yaml)
-    if azure_dsvenv_version is not None:
-        azure_dsvenv_version = azure_dsvenv_version.group(1)
+    match = re.search(r'python_version:\s+(\S+)', azure_pipeline_yaml)
+    azure_python_version = match.group(1) if match is not None else None
+
+    match = re.search(r'dsvenv_version:\s+(\S+)', azure_pipeline_yaml)
+    azure_dsvenv_version = match.group(1) if match is not None else None
 
     return AzurePipelinesConfig(azure_python_version, azure_dsvenv_version)
 
 
-def parse_args():
+def parse_args() -> Namespace:
     """
     Parse the input argumens and validate them.
 
     Parses the argument according to the parser configuration below providing a few
     tweaks.
 
     If no requirement files were provided and `requirements.txt` exists it will be used
     by default. Any explicitly provided file must exist.
 
     If no config file was provided and `setup.cfg` exists it will be used by default. If
     provided explicitly the file must exist.
 
-    Return (Namespace):
+    Return:
         All the args parsed.
 
     Raises:
         FileNotFoundError: If any of explicitly provided files does not exist.
+        ValueError: If any of the mandatory requirements is missing.
+        RuntimeError: If the pre-commit hooks are requested and `git` is not available.
     """
     parser = ArgumentParser(
         description=(
             'Create and initialize a virtual environment based on a requirements file. '
             'If a `.pre-commit-config.yaml` is present, pre-commit hooks will be '
             'installed.'
         ),
@@ -1289,15 +1340,19 @@
         type=Path,
         default=Path.cwd() / '.venv',
         help='Directory containing the virtual environment.',
     )
     parser.add_argument(
         '--python-version',
         '-p',
-        help='The desired Python version of the virtual environment.',
+        help=(
+            'The desired Python version of the virtual environment. This can also be a '
+            'specifier e.g. ~=3.10 or >=3.8,<3.9. If not provided, the version will be '
+            'resolved from the configuration file or the existing environment.'
+        ),
     )
     parser.add_argument(
         '--requirement',
         '-r',
         dest='requirements',
         type=Path,
         default=[_DEFAULT_REQUIREMENTS_TXT] if _DEFAULT_REQUIREMENTS_TXT else [],
@@ -1323,18 +1378,18 @@
             'section will be written to a pip configuration file inside the virtual '
             'environment (if the section is not present, this file will be removed). '
             'The [dsvenv] section may contain the following options: "python_version" '
             '(specifies the desired venv Python version), "azure_pipelines_yml" (a name'
             ' of the Azure pipelines file) and "requires" (a list of pip package '
             'specifications required for the build, e.g. "dsbuild" or "pip==20.0.1"). '
             '"requires" syntax comes from pyproject.toml. It additionally allows to '
-            'specify "==None" as a package version, which means that the package won\'t'
-            ' be installed during the environment initialization even if dsvenv does it'
-            ' by default (e.g. "dsbuild==None" prevents the default installation of '
-            '"dsbuild").'
+            'specify "===None" as a package version, which means that the package '
+            'will not be installed during the environment initialization even if '
+            'dsvenv does it by default (e.g. "dsbuild===None" prevents the default '
+            'installation of "dsbuild").'
         ),
     )
     parser.add_argument(
         '--no-pre-commit',
         '--no-install-pre-commit-hooks',
         dest='install_pre_commit_hooks',
         default=(_DEFAULT_PRE_COMMIT_YAML is not None),
@@ -1372,15 +1427,15 @@
     # Verify if any mandatory requirements are missing
     missing_reqs = [
         r for r in _MANDATORY_DSVENV_REQUIRES if r not in args.dsvenv_config.requires
     ]
     if missing_reqs:
         raise ValueError(
             f'The following requirements are mandatory and cannot be excluded using'
-            f' the "==None" syntax: {missing_reqs}.'
+            f' the "===None" syntax: {missing_reqs}.'
         )
 
     args.azure_pipelines_config = parse_azure_pipelines(
         args.dsvenv_config.azure_pipelines_yml
     )
 
     # Check if git exists if the pre-commit hooks are needed
@@ -1392,15 +1447,15 @@
                 f'disable pre-commit hooks by removing the "{_DEFAULT_PRE_COMMIT_YAML}"'
                 'configuration file or using "--no-pre-commit" option.'
             )
 
     return args
 
 
-def error_print(func):
+def error_print(func: Callable) -> Callable:
     """
     This decorator function captures all exceptions of `func` and displays them nicely.
 
     First the traceback will be displayed, then the error message.
     """
 
     def inner():
```

## Comparing `dsvenv-1.2.1.dist-info/RECORD` & `dsvenv-2.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dsvenv/.version,sha256=IGYgplfxzMivcrhm_c7yDmQcSPOc4n8zjOgxOUnGPlM,5
-dsvenv/__init__.py,sha256=kFCbC9sLEVVj-QXVyaecPCQ7cNOTahuIQ31JSCQxEAI,310
-dsvenv/__main__.py,sha256=9hExMlp1mpLA53zf0IIjK050_9y4h05Pe37nS8lHJOY,53228
-dsvenv-1.2.1.dist-info/METADATA,sha256=15trveCT8Ra14enE6zs5vMlmz7I3zNd_BwsHOgsY6mg,283
-dsvenv-1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dsvenv-1.2.1.dist-info/entry_points.txt,sha256=91gUHtcrYbNXkByhbqSm0eb7sJNANQo3V14bzYMC2h4,48
-dsvenv-1.2.1.dist-info/top_level.txt,sha256=RaeZdyjfZYUPKmhOjDjRUDWRufNih7EMcYN6Y9o23kk,7
-dsvenv-1.2.1.dist-info/RECORD,,
+dsvenv/.version,sha256=8iq9Z3OrIyhpMhrUseR6wMkI_r9POivRDIBmFA90EmE,5
+dsvenv/__init__.py,sha256=fBRmj09fShgE3KZpePCQE94zNpbPhIHjjfN4sIXkEYY,324
+dsvenv/__main__.py,sha256=cAX1ImDeuv2l7tPLCxUAkh34rkB0rmi4gkCgPBAeBdo,55338
+dsvenv-2.0.0.dist-info/METADATA,sha256=BHOqycWzrXFYoG7dXHMINz04po3n_4V1X0UHwjt_oAE,286
+dsvenv-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dsvenv-2.0.0.dist-info/entry_points.txt,sha256=91gUHtcrYbNXkByhbqSm0eb7sJNANQo3V14bzYMC2h4,48
+dsvenv-2.0.0.dist-info/top_level.txt,sha256=RaeZdyjfZYUPKmhOjDjRUDWRufNih7EMcYN6Y9o23kk,7
+dsvenv-2.0.0.dist-info/RECORD,,
```

