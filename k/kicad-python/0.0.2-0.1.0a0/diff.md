# Comparing `tmp/kicad-python-0.0.2.tar.gz` & `tmp/kicad_python-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kicad-python-0.0.2.tar", last modified: Tue Aug 28 19:31:58 2018, max compression
+gzip compressed data, was "kicad_python-0.1.0a0.tar", max compression
```

## Comparing `kicad-python-0.0.2.tar` & `kicad_python-0.1.0a0.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad/
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad/util/
--rw-r--r--   0 thomas    (1000) users      (100)     5481 2018-08-28 17:22:46.000000 kicad-python-0.0.2/kicad/util/point.py
--rw-r--r--   0 thomas    (1000) users      (100)      753 2018-02-17 21:27:48.000000 kicad-python-0.0.2/kicad/util/__init__.py
--rw-r--r--   0 thomas    (1000) users      (100)     4623 2018-08-06 11:12:30.000000 kicad-python-0.0.2/kicad/plotter.py
--rw-r--r--   0 thomas    (1000) users      (100)     1201 2018-03-06 19:39:59.000000 kicad-python-0.0.2/kicad/_native.py
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad/pcbnew/
--rw-r--r--   0 thomas    (1000) users      (100)     3216 2018-08-04 16:54:59.000000 kicad-python-0.0.2/kicad/pcbnew/module.py
--rw-r--r--   0 thomas    (1000) users      (100)     5353 2018-08-06 10:14:09.000000 kicad-python-0.0.2/kicad/pcbnew/board.py
--rw-r--r--   0 thomas    (1000) users      (100)     1959 2018-03-03 21:52:15.000000 kicad-python-0.0.2/kicad/pcbnew/pcbtarget.py
--rw-r--r--   0 thomas    (1000) users      (100)     1751 2018-08-28 17:15:35.000000 kicad-python-0.0.2/kicad/pcbnew/net.py
--rw-r--r--   0 thomas    (1000) users      (100)     7384 2018-03-06 17:55:29.000000 kicad-python-0.0.2/kicad/pcbnew/drawsegment.py
--rw-r--r--   0 thomas    (1000) users      (100)     2737 2018-08-28 15:03:50.000000 kicad-python-0.0.2/kicad/pcbnew/text.py
--rw-r--r--   0 thomas    (1000) users      (100)     1637 2018-08-28 17:24:33.000000 kicad-python-0.0.2/kicad/pcbnew/pad.py
--rw-r--r--   0 thomas    (1000) users      (100)     2270 2018-08-28 15:54:38.000000 kicad-python-0.0.2/kicad/pcbnew/via.py
--rw-r--r--   0 thomas    (1000) users      (100)     5110 2018-08-28 17:18:47.000000 kicad-python-0.0.2/kicad/pcbnew/boarditem.py
--rw-r--r--   0 thomas    (1000) users      (100)     1747 2018-08-28 16:10:05.000000 kicad-python-0.0.2/kicad/pcbnew/__init__.py
--rw-r--r--   0 thomas    (1000) users      (100)     2111 2018-03-06 18:09:46.000000 kicad-python-0.0.2/kicad/pcbnew/dimension.py
--rw-r--r--   0 thomas    (1000) users      (100)     1598 2018-08-28 15:52:33.000000 kicad-python-0.0.2/kicad/pcbnew/zone.py
--rw-r--r--   0 thomas    (1000) users      (100)     4039 2018-08-28 17:20:58.000000 kicad-python-0.0.2/kicad/pcbnew/layer.py
--rw-r--r--   0 thomas    (1000) users      (100)     2286 2018-08-28 15:54:30.000000 kicad-python-0.0.2/kicad/pcbnew/track.py
--rw-r--r--   0 thomas    (1000) users      (100)        0 2018-02-17 21:27:48.000000 kicad-python-0.0.2/kicad/__init__.py
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad/primitives/
--rw-r--r--   0 thomas    (1000) users      (100)      769 2018-08-28 16:10:54.000000 kicad-python-0.0.2/kicad/primitives/__init__.py
--rw-r--r--   0 thomas    (1000) users      (100)     4879 2018-08-28 17:11:23.000000 kicad-python-0.0.2/kicad/primitives/polygon.py
--rw-r--r--   0 thomas    (1000) users      (100)      756 2018-02-17 21:25:46.000000 kicad-python-0.0.2/README.md
--rw-r--r--   0 thomas    (1000) users      (100)     1560 2018-08-28 19:31:58.000000 kicad-python-0.0.2/PKG-INFO
--rw-r--r--   0 thomas    (1000) users      (100)       70 2018-08-28 19:31:58.000000 kicad-python-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas    (1000) users      (100)        0 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad_python.egg-info/
--rw-r--r--   0 thomas    (1000) users      (100)      646 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad_python.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) users      (100)        1 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad_python.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) users      (100)     1560 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad_python.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) users      (100)        6 2018-08-28 19:31:58.000000 kicad-python-0.0.2/kicad_python.egg-info/top_level.txt
--rwxr-xr-x   0 thomas    (1000) users      (100)     1001 2018-08-28 19:30:06.000000 kicad-python-0.0.2/setup.py
+-rw-r--r--   0        0        0    35131 2024-03-09 19:18:11.297062 kicad_python-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1364 2024-03-26 23:12:57.041972 kicad_python-0.1.0a0/README.md
+-rw-r--r--   0        0        0     1047 2024-03-24 18:48:45.402173 kicad_python-0.1.0a0/build.py
+-rw-r--r--   0        0        0      805 2024-03-24 13:07:42.010745 kicad_python-0.1.0a0/kipy/__init__.py
+-rw-r--r--   0        0        0    10189 2024-03-24 14:03:12.782362 kicad_python-0.1.0a0/kipy/board.py
+-rw-r--r--   0        0        0    12483 2024-03-24 18:48:03.062829 kicad_python-0.1.0a0/kipy/board_types.py
+-rw-r--r--   0        0        0     3201 2024-03-24 18:57:15.425165 kicad_python-0.1.0a0/kipy/client.py
+-rw-r--r--   0        0        0     1550 2024-03-23 22:30:16.412692 kicad_python-0.1.0a0/kipy/common_types.py
+-rw-r--r--   0        0        0     2840 2024-03-20 00:48:53.806926 kicad_python-0.1.0a0/kipy/geometry.py
+-rw-r--r--   0        0        0     4176 2024-03-24 13:54:50.109949 kicad_python-0.1.0a0/kipy/kicad.py
+-rw-r--r--   0        0        0     1669 2024-03-14 00:51:46.077751 kicad_python-0.1.0a0/kipy/project.py
+-rw-r--r--   0        0        0     1070 2024-03-15 21:15:06.598355 kicad_python-0.1.0a0/kipy/project_types.py
+-rw-r--r--   0        0        0      791 2024-03-09 19:18:11.298719 kicad_python-0.1.0a0/kipy/proto/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-09 19:18:11.298795 kicad_python-0.1.0a0/kipy/proto/board/__init__.py
+-rw-r--r--   0        0        0     4093 2024-04-03 01:03:37.456567 kicad_python-0.1.0a0/kipy/proto/board/board_commands_pb2.py
+-rw-r--r--   0        0        0    13275 2024-04-03 01:03:37.460321 kicad_python-0.1.0a0/kipy/proto/board/board_commands_pb2.pyi
+-rw-r--r--   0        0        0     4404 2024-04-03 01:03:37.452393 kicad_python-0.1.0a0/kipy/proto/board/board_pb2.py
+-rw-r--r--   0        0        0    11242 2024-04-03 01:03:37.455556 kicad_python-0.1.0a0/kipy/proto/board/board_pb2.pyi
+-rw-r--r--   0        0        0    16782 2024-04-03 01:03:37.437333 kicad_python-0.1.0a0/kipy/proto/board/board_types_pb2.py
+-rw-r--r--   0        0        0    51917 2024-04-03 01:03:37.451469 kicad_python-0.1.0a0/kipy/proto/board/board_types_pb2.pyi
+-rw-r--r--   0        0        0      867 2024-03-09 19:18:11.298877 kicad_python-0.1.0a0/kipy/proto/common/__init__.py
+-rw-r--r--   0        0        0      838 2024-03-09 19:18:11.298958 kicad_python-0.1.0a0/kipy/proto/common/commands/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-03 01:03:37.472861 kicad_python-0.1.0a0/kipy/proto/common/commands/base_commands_pb2.py
+-rw-r--r--   0        0        0     2229 2024-04-03 01:03:37.473502 kicad_python-0.1.0a0/kipy/proto/common/commands/base_commands_pb2.pyi
+-rw-r--r--   0        0        0     8955 2024-04-03 01:03:37.464773 kicad_python-0.1.0a0/kipy/proto/common/commands/editor_commands_pb2.py
+-rw-r--r--   0        0        0    28233 2024-04-03 01:03:37.472394 kicad_python-0.1.0a0/kipy/proto/common/commands/editor_commands_pb2.pyi
+-rw-r--r--   0        0        0     1202 2024-04-03 01:03:37.473935 kicad_python-0.1.0a0/kipy/proto/common/commands/project_commands_pb2.py
+-rw-r--r--   0        0        0     2054 2024-04-03 01:03:37.474505 kicad_python-0.1.0a0/kipy/proto/common/commands/project_commands_pb2.pyi
+-rw-r--r--   0        0        0     2443 2024-04-03 01:03:37.460853 kicad_python-0.1.0a0/kipy/proto/common/envelope_pb2.py
+-rw-r--r--   0        0        0     7861 2024-04-03 01:03:37.462633 kicad_python-0.1.0a0/kipy/proto/common/envelope_pb2.pyi
+-rw-r--r--   0        0        0      861 2024-03-23 15:33:14.626250 kicad_python-0.1.0a0/kipy/proto/common/types/__init__.py
+-rw-r--r--   0        0        0    10011 2024-04-03 01:03:37.423784 kicad_python-0.1.0a0/kipy/proto/common/types/base_types_pb2.py
+-rw-r--r--   0        0        0    30051 2024-04-03 01:03:37.432548 kicad_python-0.1.0a0/kipy/proto/common/types/base_types_pb2.pyi
+-rw-r--r--   0        0        0     3560 2024-04-03 01:03:37.420296 kicad_python-0.1.0a0/kipy/proto/common/types/enums_pb2.py
+-rw-r--r--   0        0        0     8513 2024-04-03 01:03:37.422296 kicad_python-0.1.0a0/kipy/proto/common/types/enums_pb2.pyi
+-rw-r--r--   0        0        0      859 2024-04-03 01:03:37.462974 kicad_python-0.1.0a0/kipy/proto/common/types/project_settings_pb2.py
+-rw-r--r--   0        0        0      907 2024-04-03 01:03:37.463323 kicad_python-0.1.0a0/kipy/proto/common/types/project_settings_pb2.pyi
+-rw-r--r--   0        0        0      709 2024-04-03 01:03:37.419596 kicad_python-0.1.0a0/kipy/proto/schematic/schematic_commands_pb2.py
+-rw-r--r--   0        0        0      925 2024-04-03 01:03:37.419798 kicad_python-0.1.0a0/kipy/proto/schematic/schematic_commands_pb2.pyi
+-rw-r--r--   0        0        0     2841 2024-04-03 01:03:37.433175 kicad_python-0.1.0a0/kipy/proto/schematic/schematic_types_pb2.py
+-rw-r--r--   0        0        0     7552 2024-04-03 01:03:37.435639 kicad_python-0.1.0a0/kipy/proto/schematic/schematic_types_pb2.pyi
+-rw-r--r--   0        0        0      845 2024-03-23 17:32:07.429035 kicad_python-0.1.0a0/kipy/util/__init__.py
+-rw-r--r--   0        0        0     2365 2024-03-23 17:31:57.285951 kicad_python-0.1.0a0/kipy/util/proto.py
+-rw-r--r--   0        0        0     1228 2024-03-15 21:15:06.599400 kicad_python-0.1.0a0/kipy/util/units.py
+-rw-r--r--   0        0        0     1149 2024-03-24 18:47:39.651822 kicad_python-0.1.0a0/kipy/wrapper.py
+-rw-r--r--   0        0        0     1261 2024-03-24 14:35:50.100953 kicad_python-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 kicad_python-0.1.0a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kicad-python-0.0.2/kicad/util/__init__.py` & `kicad_python-0.1.0a0/kipy/proto/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This program source code file is part of KiCad, a free EDA CAD application.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Copyright (C) 2024 KiCad Developers
 #
-# You should have received a copy of the GNU General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation, either version 3 of the License, or (at your
+# option) any later version.
 #
-# (C) 2018 by Thomas Pointhuber, <thomas.pointhuber@gmx.at>
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+# flake8: noqa
 
-from kicad.util.point import Point2D        # noqa: F401
+from .board import *
```

### Comparing `kicad-python-0.0.2/kicad/pcbnew/net.py` & `kicad_python-0.1.0a0/kipy/project.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,50 @@
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This program source code file is part of KiCad, a free EDA CAD application.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Copyright (C) 2024 KiCad Developers
 #
-# You should have received a copy of the GNU General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation, either version 3 of the License, or (at your
+# option) any later version.
 #
-# (C) 2018 by Thomas Pointhuber, <thomas.pointhuber@gmx.at>
-
-from kicad._native import _pcbnew
-
-
-class Net(object):
-    def __init__(self, netinfo):
-        assert isinstance(netinfo, _pcbnew.NETINFO_ITEM)
-        self._obj = netinfo
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    def get_native(self):
-        """Get native object from the low level API
+from typing import List
 
-        :return: :class:`pcbnew.NETINFO_ITEM`
-        """
-        return self._obj
+from kipy.client import KiCadClient
+from kipy.project_types import NetClass
+from kipy.proto.common.types import DocumentSpecifier
+from kipy.proto.common.commands.project_commands_pb2 import (
+    GetNetClasses,
+    NetClassesResponse
+)
+
+
+class Project:
+    def __init__(self, kicad: KiCadClient, document: DocumentSpecifier):
+        self._kicad = kicad
+        self._doc = document
 
     @property
-    def name(self):
-        """Name of Net
-
-        :return: ``unicode``
-        """
-        return self._obj.GetNetname()
-
-    def __eq__(self, other):
-        if not isinstance(self, other.__class__):
-            return False
-
-        if not isinstance(self._obj, other._obj.__class__):
-            return False
+    def document(self) -> DocumentSpecifier:
+        return self._doc
 
-        if self._obj == other._obj:
-            return True
-
-        return self.name == other.name
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
-        return hash(self.name)
-
-    def __repr__(self):
-        return "kicad.pcbnew.Net({})".format(self._obj)
-
-    def __str__(self):
-        return "kicad.pcbnew.Net(\"{}\")".format(self.name)
+    @property
+    def name(self) -> str:
+        """Returns the name of the project"""
+        return self._doc.project.name
+    
+    @property
+    def path(self) -> str:
+        return self._doc.project.path
+    
+    def get_net_classes(self) -> List[NetClass]:
+        command = GetNetClasses()
+        response = self._kicad.send(command, NetClassesResponse)
+        return [NetClass(p) for p in response.net_classes]
```

### Comparing `kicad-python-0.0.2/kicad/primitives/__init__.py` & `kicad_python-0.1.0a0/kipy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This program source code file is part of KiCad, a free EDA CAD application.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Copyright (C) 2024 KiCad Developers
 #
-# You should have received a copy of the GNU General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation, either version 3 of the License, or (at your
+# option) any later version.
 #
-# (C) 2018 by Thomas Pointhuber, <thomas.pointhuber@gmx.at>
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from kipy.kicad import KiCad
 
-from kicad.primitives.polygon import Polygon, PolygonSet    # noqa: F401
+__all__ = ("KiCad",)
```

