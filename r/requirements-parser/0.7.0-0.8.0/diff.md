# Comparing `tmp/requirements_parser-0.7.0.tar.gz` & `tmp/requirements_parser-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements_parser-0.7.0.tar", max compression
+gzip compressed data, was "requirements_parser-0.8.0.tar", max compression
```

## Comparing `requirements_parser-0.7.0.tar` & `requirements_parser-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,66 @@
--rw-r--r--   0        0        0      251 2021-12-15 20:27:35.000000 requirements_parser-0.7.0/AUTHORS.rst
--rw-r--r--   0        0        0    11356 2021-12-17 14:45:01.000000 requirements_parser-0.7.0/LICENSE
--rw-r--r--   0        0        0     1785 2021-12-17 14:45:01.000000 requirements_parser-0.7.0/README.md
--rw-r--r--   0        0        0     3271 2024-03-28 09:55:10.712600 requirements_parser-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      883 2024-03-28 09:55:10.713191 requirements_parser-0.7.0/requirements/__init__.py
--rw-r--r--   0        0        0     2057 2022-04-25 07:09:51.000000 requirements_parser-0.7.0/requirements/fragment.py
--rw-r--r--   0        0        0     3344 2024-03-27 15:16:54.683683 requirements_parser-0.7.0/requirements/parser.py
--rw-r--r--   0        0        0      810 2022-01-18 09:49:33.000000 requirements_parser-0.7.0/requirements/py.typed
--rw-r--r--   0        0        0    10137 2024-03-27 15:17:00.195134 requirements_parser-0.7.0/requirements/requirement.py
--rw-r--r--   0        0        0     1063 2022-01-18 09:49:46.000000 requirements_parser-0.7.0/requirements/vcs.py
--rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 requirements_parser-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/AUTHORS.rst
+-rw-r--r--   0        0        0    11356 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1785 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/README.md
+-rw-r--r--   0        0        0     3793 2024-04-03 10:02:29.248442 requirements_parser-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      883 2024-04-03 10:02:29.248442 requirements_parser-0.8.0/requirements/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/fragment.py
+-rw-r--r--   0        0        0     3372 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/parser.py
+-rw-r--r--   0        0        0      810 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/py.typed
+-rw-r--r--   0        0        0    10225 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/requirement.py
+-rw-r--r--   0        0        0     1063 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/vcs.py
+-rw-r--r--   0        0        0      657 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/blank_1.expected
+-rw-r--r--   0        0        0        3 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/blank_1.txt
+-rw-r--r--   0        0        0        2 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_1.expected
+-rw-r--r--   0        0        0       20 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_1.txt
+-rw-r--r--   0        0        0      318 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_2.expected
+-rw-r--r--   0        0        0       22 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_2.txt
+-rw-r--r--   0        0        0    20562 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.expected
+-rw-r--r--   0        0        0     2885 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.txt
+-rw-r--r--   0        0        0     1818 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_1.expected
+-rw-r--r--   0        0        0      308 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_1.txt
+-rw-r--r--   0        0        0     1564 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_2.expected
+-rw-r--r--   0        0        0      338 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_2.txt
+-rw-r--r--   0        0        0      635 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/extras_1.expected
+-rw-r--r--   0        0        0       37 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/extras_1.txt
+-rw-r--r--   0        0        0       24 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/fail_1.txt
+-rw-r--r--   0        0        0       58 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/fail_2.txt
+-rw-r--r--   0        0        0     1339 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/file_1.expected
+-rw-r--r--   0        0        0      172 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/file_1.txt
+-rw-r--r--   0        0        0      311 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/global_options_requirements.expected
+-rw-r--r--   0        0        0      168 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/global_options_requirements.txt
+-rw-r--r--   0        0        0     1317 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/illustrative_requirements.expected
+-rw-r--r--   0        0        0      121 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/illustrative_requirements.txt
+-rw-r--r--   0        0        0      948 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_1.expected
+-rw-r--r--   0        0        0       30 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_1.txt
+-rw-r--r--   0        0        0      595 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_2.expected
+-rw-r--r--   0        0        0       24 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_2.txt
+-rw-r--r--   0        0        0      359 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_3.expected
+-rw-r--r--   0        0        0        4 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_3.txt
+-rw-r--r--   0        0        0     1387 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.expected
+-rw-r--r--   0        0        0     1184 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.txt
+-rw-r--r--   0        0        0    10893 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.expected
+-rw-r--r--   0        0        0     2341 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.txt
+-rw-r--r--   0        0        0     1242 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/simple_1.expected
+-rw-r--r--   0        0        0       65 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/simple_1.txt
+-rw-r--r--   0        0        0      408 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/specs_1.expected
+-rw-r--r--   0        0        0       43 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/specs_1.txt
+-rw-r--r--   0        0        0      759 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/subdirectory.expected
+-rw-r--r--   0        0        0      145 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/subdirectory.txt
+-rw-r--r--   0        0        0      305 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/underscores.expected
+-rw-r--r--   0        0        0        9 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/underscores.txt
+-rw-r--r--   0        0        0      926 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/uri.expected
+-rw-r--r--   0        0        0      214 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/uri.txt
+-rw-r--r--   0        0        0     4479 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.expected
+-rw-r--r--   0        0        0      751 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.txt
+-rw-r--r--   0        0        0     4842 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git.expected
+-rw-r--r--   0        0        0      812 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git.txt
+-rw-r--r--   0        0        0      397 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git_extras_require.expected
+-rw-r--r--   0        0        0       73 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git_extras_require.txt
+-rw-r--r--   0        0        0     5078 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_hg.expected
+-rw-r--r--   0        0        0      814 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_hg.txt
+-rw-r--r--   0        0        0     1502 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_svn.expected
+-rw-r--r--   0        0        0      255 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_svn.txt
+-rw-r--r--   0        0        0     2703 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/test_parser.py
+-rw-r--r--   0        0        0     2145 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/test_requirement.py
+-rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 requirements_parser-0.8.0/PKG-INFO
```

### Comparing `requirements_parser-0.7.0/LICENSE` & `requirements_parser-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.7.0/README.md` & `requirements_parser-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.7.0/pyproject.toml` & `requirements_parser-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,46 @@
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "requirements-parser"
-version = "0.7.0"
+# !! version is managed by semantic_release
+version = "0.8.0"
 description = "This is a small Python module for parsing Pip requirement files."
 authors = [
     "Paul Horton <paul@hogr.dev>",
     "David Fischer (@davidfischer)",
     "Trey Hunner (@treyhunner)",
     "Dima Veselov (@dveselov)",
     "Sascha Peilicke (@saschpe)",
     "Jayson Reis (@jaysonsantos)",
     "Max Shenfield (@mshenfield)",
     "Nicolas Delaby (@ticosax)",
     "Stéphane Bidoul (@sbidoul)"
 ]
-maintainers = ["Paul Horton <simplyecommerce@gmail.com>"]
+maintainers = ["Paul Horton <paul@hogr.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/madpah/requirements-parser"
+homepage = "https://github.com/madpah/requirements-parser/#readme"
 repository = "https://github.com/madpah/requirements-parser"
+documentation = "https://requirements-parser.readthedocs.io/"
 packages = [
-    { include = "requirements" }
+    { include = "requirements" },
+    { include = "tests", format = "sdist" },
 ]
 include = [
-    "AUTHORS.rst",
-    "LICENSE",
-    "README.md"
+    { path = "AUTHORS.rst", format = "sdist" },
+    { path = "LICENSE", format = "sdist" },
+    { path = "README.md", format = "sdist" },
+]
+exclude = [
+  # exclude dotfiles and dotfolders
+  "**/.*",
+  "docs/_build", "docs/processes",
 ]
 classifiers = [
     # Trove classifiers - https://packaging.python.org/specifications/core-metadata/#metadata-classifier
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
@@ -37,40 +49,41 @@
     'Topic :: System :: Software Distribution',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Typing :: Typed'
 ]
 keywords = [
     "Pip", "requirements", "parse"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/madpah/requirements-parser/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-setuptools = ">= 59.7.0"
-types-setuptools = ">= 59.7.0"
+python = "^3.8"
+types-setuptools = ">=69.1.0"
 
-[tool.poetry.dev-dependencies]
-tox = "^3.24.3"
-coverage = "^6.2"
-mypy = "^0.920"
-autopep8 = "^1.6.0"
-flake8 = "^4.0.1"
-flake8-annotations = {version = "^2.7.0", python = ">= 3.6.2"}
-flake8-bugbear = "^21.11.29"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.group.dev.dependencies]
+coverage = "7.4.4"
+flake8 = { version="7.0.0", python=">=3.8.1" }
+flake8-annotations = { version="3.0.1", python=">=3.8.1" }
+flake8-bugbear = { version="24.2.6", python=">=3.8.1" }
+flake8-isort = "6.1.1"
+flake8-quotes = "3.4.0"
+flake8-use-fstring = "1.4"
+pep8-naming = "0.13.3"
+isort = "5.13.2"
+autopep8 = "2.1.0"
+mypy = "1.9.0"
+tox = "4.14.2"
 
 [tool.semantic_release]
 # see https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 commit_author = "semantic-release <semantic-release>"
 commit_message = "chore(release): {version}\n\nAutomatically generated by python-semantic-release\n\nSigned-off-by: semantic-release <semantic-release>"
 upload_to_vcs_release = true
 build_command = "pip install poetry && poetry build"
```

### Comparing `requirements_parser-0.7.0/requirements/__init__.py` & `requirements_parser-0.8.0/requirements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 __all__ = [
     'parse'
 ]
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "0.7.0"  # noqa:Q000
+__version__ = "0.8.0"  # noqa:Q000
```

### Comparing `requirements_parser-0.7.0/requirements/fragment.py` & `requirements_parser-0.8.0/requirements/fragment.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import re
-from typing import cast, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple, cast
 
 # Copied from pip
 # https://github.com/pypa/pip/blob/281eb61b09d87765d7c2b92f6982b3fe76ccb0af/pip/index.py#L947
 HASH_ALGORITHMS = set(['sha1', 'sha224', 'sha384', 'sha256', 'sha512', 'md5'])
 
 extras_require_search = re.compile(r'(?P<name>.+)\[(?P<extras>[^\]]+)\]')
```

### Comparing `requirements_parser-0.7.0/requirements/parser.py` & `requirements_parser-0.8.0/requirements/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,19 +69,19 @@
             with open(new_file_path) as f:
                 for requirement in parse(f):
                     yield requirement
         elif line.startswith('-f') or line.startswith('--find-links') or \
                 line.startswith('-i') or line.startswith('--index-url') or \
                 line.startswith('--extra-index-url') or \
                 line.startswith('--no-index'):
-            warnings.warn('Private repos not supported. Skipping.')
+            warnings.warn('Private repos not supported. Skipping.', stacklevel=2)
             continue
         else:
             unsupported: bool = False
             for param in _UNSUPPORTED_OPTIONS.keys():
                 if line.startswith(param):
-                    warnings.warn(str(_UNSUPPORTED_OPTIONS.get(param)))
+                    warnings.warn(str(_UNSUPPORTED_OPTIONS.get(param)), stacklevel=2)
                     unsupported = True
 
             # Otherwise, parse it
             if not unsupported:
                 yield Requirement.parse(line)
```

### Comparing `requirements_parser-0.7.0/requirements/py.typed` & `requirements_parser-0.8.0/requirements/py.typed`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.7.0/requirements/requirement.py` & `requirements_parser-0.8.0/requirements/requirement.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import unicode_literals
 
 import re
-from typing import Any, cast, Dict, List, Match, Optional
+from typing import Any, Dict, List, Match, Optional, Tuple, cast
 
 from pkg_resources import Requirement as Req
 
-from .fragment import get_hash_info, parse_fragment, parse_extras_require
+from .fragment import get_hash_info, parse_extras_require, parse_fragment
 from .vcs import VCS, VCS_SCHEMES
 
 URI_REGEX = re.compile(
     r'^(?P<scheme>https?|file|ftps?)://(?P<path>[^#]+)'
     r'(#(?P<fragment>\S+))?'
 )
 
@@ -83,18 +83,18 @@
         self.subdirectory = None
         self.uri = None
         self.path = None
         self.revision = None
         self.hash_name = None
         self.hash = None
         self.extras: List[str] = []
-        self.specs: List[str] = []
+        self.specs: List[Tuple[str, str]] = []
 
     def __repr__(self) -> str:
-        return '<Requirement: "{0}">'.format(self.line)
+        return f'<Requirement: "{self.line}">'
 
     def __getitem__(self, key: str) -> Any:
         return getattr(self, key)
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, Requirement):
             return all([
@@ -124,50 +124,52 @@
         See: pip/req.py:from_editable()
 
         :param line: an "editable" requirement
         :returns: a Requirement instance for the given line
         :raises: ValueError on an invalid requirement
         """
 
-        req = cls('-e {0}'.format(line))
+        req = cls(f'-e {line}')
         req.editable = True
 
         if ' #' in line:
             line = line[:line.find(' #')]
 
         vcs_match: Optional[Match[str]] = VCS_REGEX.match(line)
         local_match: Optional[Match[str]] = LOCAL_REGEX.match(line)
 
         if vcs_match is not None:
             groups: Dict[str, str] = vcs_match.groupdict()
             if groups.get('login'):
-                req.uri = '{scheme}://{login}@{path}'.format(**groups)  # type: ignore
+                req.uri = f'{groups["scheme"]}://{groups["login"]}@{groups["path"]}'  # type: ignore
             else:
-                req.uri = '{scheme}://{path}'.format(**groups)  # type: ignore
+                req.uri = f'{groups["scheme"]}://{groups["path"]}'  # type: ignore
             req.revision = groups['revision']  # type: ignore
             if groups['fragment']:
                 fragment = parse_fragment(groups['fragment'])
                 egg = cast(str, fragment.get('egg'))
                 req.name, req.extras = parse_extras_require(egg)  # type: ignore
-                req.hash_name, req.hash = get_hash_info(fragment)     # type: ignore
+                req.hash_name, req.hash = get_hash_info(fragment)  # type: ignore
                 req.subdirectory = fragment.get('subdirectory')  # type: ignore
             for vcs in VCS:
                 if str(req.uri).startswith(vcs):
                     req.vcs = vcs  # type: ignore
-        else:
-            assert local_match is not None, 'This should match everything'
+        elif local_match is not None:
             groups = local_match.groupdict()
             req.local_file = True
             if groups['fragment']:
                 fragment = parse_fragment(groups['fragment'])
                 egg = cast(str, fragment.get('egg'))
                 req.name, req.extras = parse_extras_require(egg)  # type: ignore
                 req.hash_name, req.hash = get_hash_info(fragment)  # type: ignore
                 req.subdirectory = fragment.get('subdirectory')  # type: ignore
             req.path = cast(str, groups['path'])  # type: ignore
+        else:
+            req.local_file = True
+            req.path, req.name = line.rsplit('/', 1)  # type: ignore
 
         return req
 
     @classmethod
     def parse_line(cls, line: str) -> 'Requirement':
         """
         Parses a Requirement from a non-editable requirement.
@@ -184,30 +186,30 @@
         vcs_match: Optional[Match[str]] = VCS_REGEX.match(line)
         uri_match: Optional[Match[str]] = URI_REGEX.match(line)
         local_match: Optional[Match[str]] = LOCAL_REGEX.match(line)
 
         if vcs_match is not None:
             groups = vcs_match.groupdict()
             if groups.get('login'):
-                req.uri = '{scheme}://{login}@{path}'.format(**groups)  # type: ignore
+                req.uri = f'{groups["scheme"]}://{groups["login"]}@{groups["path"]}'  # type: ignore
             else:
-                req.uri = '{scheme}://{path}'.format(**groups)  # type: ignore
+                req.uri = f'{groups["scheme"]}://{groups["path"]}'  # type: ignore
             req.revision = groups['revision']  # type: ignore
             if groups['fragment']:
                 fragment = parse_fragment(groups['fragment'])
                 egg = fragment.get('egg')
                 req.name, req.extras = parse_extras_require(egg)  # type: ignore
                 req.hash_name, req.hash = get_hash_info(fragment)  # type: ignore
                 req.subdirectory = fragment.get('subdirectory')  # type: ignore
             for vcs in VCS:
                 if str(req.uri).startswith(vcs):
                     req.vcs = vcs  # type: ignore
         elif uri_match is not None:
             groups = uri_match.groupdict()
-            req.uri = '{scheme}://{path}'.format(**groups)  # type: ignore
+            req.uri = f'{groups["scheme"]}://{groups["path"]}'  # type: ignore
             if groups['fragment']:
                 fragment = parse_fragment(groups['fragment'])
                 egg = fragment.get('egg')
                 req.name, req.extras = parse_extras_require(egg)  # type: ignore
                 req.hash_name, req.hash = get_hash_info(fragment)  # type: ignore
                 req.subdirectory = fragment.get('subdirectory')  # type: ignore
             if groups['scheme'] == 'file':
@@ -228,15 +230,15 @@
         else:
             # This is a requirement specifier.
             # Delegate to pkg_resources and hope for the best
             req.specifier = True
             pkg_req = Req.parse(line)
             req.name = pkg_req.unsafe_name  # type: ignore
             req.extras = list(pkg_req.extras)
-            req.specs = pkg_req.specs  # type: ignore
+            req.specs = pkg_req.specs
         return req
 
     @classmethod
     def parse(cls, line: str) -> 'Requirement':
         """
         Parses a Requirement from a line of a requirement file.
```

### Comparing `requirements_parser-0.7.0/requirements/vcs.py` & `requirements_parser-0.8.0/requirements/vcs.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.7.0/PKG-INFO` & `requirements_parser-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: requirements-parser
-Version: 0.7.0
+Version: 0.8.0
 Summary: This is a small Python module for parsing Pip requirement files.
-Home-page: https://github.com/madpah/requirements-parser
+Home-page: https://github.com/madpah/requirements-parser/#readme
 License: Apache-2.0
 Keywords: Pip,requirements,parse
 Author: Paul Horton
 Author-email: paul@hogr.dev
 Maintainer: Paul Horton
-Maintainer-email: simplyecommerce@gmail.com
-Requires-Python: >=3.7,<4.0
+Maintainer-email: paul@hogr.dev
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Dist: setuptools (>=59.7.0)
-Requires-Dist: types-setuptools (>=59.7.0)
+Requires-Dist: types-setuptools (>=69.1.0)
 Project-URL: Bug Tracker, https://github.com/madpah/requirements-parser/issues
+Project-URL: Documentation, https://requirements-parser.readthedocs.io/
 Project-URL: Repository, https://github.com/madpah/requirements-parser
 Description-Content-Type: text/markdown
 
 Requirements Parser
 ===================
 
 [![Python CI](https://github.com/madpah/requirements-parser/actions/workflows/poetry.yml/badge.svg)](https://github.com/madpah/requirements-parser/actions/workflows/poetry.yml)
```

