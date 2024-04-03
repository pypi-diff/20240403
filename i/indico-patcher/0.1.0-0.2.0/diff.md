# Comparing `tmp/indico_patcher-0.1.0-py3-none-any.whl.zip` & `tmp/indico_patcher-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10087 bytes, number of entries: 11
--rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 indico_patcher/__init__.py
--rw-r--r--  2.0 unx     1754 b- defN 80-Jan-01 00:00 indico_patcher/classes.py
--rw-r--r--  2.0 unx     3397 b- defN 80-Jan-01 00:00 indico_patcher/enums.py
--rw-r--r--  2.0 unx      527 b- defN 80-Jan-01 00:00 indico_patcher/main.py
+Zip file size: 10187 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 indico_patcher/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 80-Jan-01 00:00 indico_patcher/classes.py
+-rw-r--r--  2.0 unx     3404 b- defN 80-Jan-01 00:00 indico_patcher/enums.py
+-rw-r--r--  2.0 unx      534 b- defN 80-Jan-01 00:00 indico_patcher/main.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 indico_patcher/py.typed
--rw-r--r--  2.0 unx      832 b- defN 80-Jan-01 00:00 indico_patcher/types.py
--rw-r--r--  2.0 unx     8136 b- defN 80-Jan-01 00:00 indico_patcher/util.py
--rw-r--r--  2.0 unx     1085 b- defN 80-Jan-01 00:00 indico_patcher-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5872 b- defN 80-Jan-01 00:00 indico_patcher-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 indico_patcher-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      879 b- defN 16-Jan-01 00:00 indico_patcher-0.1.0.dist-info/RECORD
-11 files, 22691 bytes uncompressed, 8601 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx      839 b- defN 80-Jan-01 00:00 indico_patcher/types.py
+-rw-r--r--  2.0 unx     8143 b- defN 80-Jan-01 00:00 indico_patcher/util.py
+-rw-r--r--  2.0 unx     1085 b- defN 80-Jan-01 00:00 indico_patcher-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6092 b- defN 80-Jan-01 00:00 indico_patcher-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 indico_patcher-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      879 b- defN 16-Jan-01 00:00 indico_patcher-0.2.0.dist-info/RECORD
+11 files, 22953 bytes uncompressed, 8701 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: indico_patcher/types.py
 Comment: 
 
 Filename: indico_patcher/util.py
 Comment: 
 
-Filename: indico_patcher-0.1.0.dist-info/LICENSE
+Filename: indico_patcher-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: indico_patcher-0.1.0.dist-info/METADATA
+Filename: indico_patcher-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: indico_patcher-0.1.0.dist-info/WHEEL
+Filename: indico_patcher-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: indico_patcher-0.1.0.dist-info/RECORD
+Filename: indico_patcher-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_patcher/__init__.py

```diff
@@ -1,6 +1,6 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 from .main import patch
 
 __all__ = ["patch"]
```

## indico_patcher/classes.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 from collections import defaultdict
 from typing import cast
 
 from .types import ClassWrapper
 from .types import PatchedClass
 from .util import get_members
```

## indico_patcher/enums.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 from collections.abc import Iterable
 from enum import Enum
 from enum import EnumMeta
 from typing import cast
 
 from aenum import extend_enum
```

## indico_patcher/main.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 from __future__ import annotations
 
 from enum import EnumMeta
 from typing import Any
 
 from .classes import patch_class
```

## indico_patcher/types.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 # TODO: Use explicit TypeAlias and | when support for Python 3.9 is dropped
 
 from collections.abc import Callable
 from enum import EnumMeta
 from types import FunctionType
 from typing import Any
```

## indico_patcher/util.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of indico-patcher.
-# Copyright (C) 2023 UNCONVENTIONAL
+# Copyright (C) 2023 - 2024 UNCONVENTIONAL
 
 from __future__ import annotations
 
 import sys
 from collections.abc import Callable
 from functools import partial
 from types import FrameType
```

## Comparing `indico_patcher-0.1.0.dist-info/LICENSE` & `indico_patcher-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `indico_patcher-0.1.0.dist-info/METADATA` & `indico_patcher-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: indico-patcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Swiss Army knife to customize Indico
 Home-page: https://github.com/unconventionaldotdev/indico-patcher
 License: MIT
 Author: Alejandro Avilés
 Author-email: ome@unconventional.dev
-Requires-Python: >=3.9.0,<3.12
+Requires-Python: >=3.12.2,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aenum (>=3.1.15)
-Requires-Dist: indico (>=3.2)
+Requires-Dist: indico (>=3.3)
 Project-URL: Repository, https://github.com/unconventionaldotdev/indico-patcher
 Description-Content-Type: text/markdown
 
 # Indico Patcher
 
+<!-- XXX: All the links must remain absolute. This README.md file is used to generate the description for the project in PyPI. Relative links will not work in PyPI. -->
+
 The Swiss Army knife for [Indico](https://getindico.io/) plugin development.
 
 Indico plugin development primarily relies on [`flask-pluginengine`](https://github.com/indico/flask-pluginengine), [Jinja](https://github.com/pallets/jinja) template hooks or core [signals](https://github.com/indico/indico/tree/master/indico/core/signals) to extend and modify system functionality. This, however, falls short in many other cases. Indico Patcher offers a clean interface to patch Indico code at runtime, allowing for things such as:
 
 - Adding or overriding properties and intercepting methods in classes
 - Reordering, modifying and removing fields in WTForms forms
 - Adding new columns and relationships to SQLAlchemy models
 - Adding new members to Enums
 
-For more examples and usage information, please refer to the [patching guide](doc/README.md). For general information about Indico plugin development, please refer to the [official guide](https://docs.getindico.io/en/stable/plugins/). Not yet supported cases are tracked in [TODO.md](TODO.md).
+For more examples and usage information, please refer to the [patching guide](https://github.com/unconventionaldotdev/indico-patcher/blob/master/doc/README.md). For general information about Indico plugin development, please refer to the [official guide](https://docs.getindico.io/en/stable/plugins/). Not yet supported cases are tracked in [TODO.md](https://github.com/unconventionaldotdev/indico-patcher/blob/master/TODO.md).
 
 ## Installation
 
 Indico Patcher is available on PyPI as [`indico-patcher`](https://pypi.org/project/indico-patcher/) and can be installed with `pip`:
 
 ```sh
 pip install indico-patcher
@@ -81,15 +80,15 @@
 class _UserTitle(RichIntEnum):
     __titles__ = [None, 'Madam', 'Sir', 'Rev.']
     madam = 1
     sir = 2
     rev = 3
 ```
 
-For more examples and usage information, please refer to the [patching guide](doc/README.md).
+For more examples and usage information, please refer to the [patching guide](https://github.com/unconventionaldotdev/indico-patcher/blob/master/doc/README.md).
 
 ### Caveats
 
 > [!WARNING]
 > With great power comes great responsibility.
 
 Runtime patching is a powerful and flexible strategy but it will lead to code that may break without notice as the Indico project evolves. Indico Patcher makes patching Indico dangerously easy so keep in mind a few things when using it.
```

