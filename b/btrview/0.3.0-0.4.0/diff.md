# Comparing `tmp/btrview-0.3.0.tar.gz` & `tmp/btrview-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.3.0.tar", last modified: Tue Apr  2 00:14:34 2024, max compression
+gzip compressed data, was "btrview-0.4.0.tar", last modified: Wed Apr  3 01:49:02 2024, max compression
```

## Comparing `btrview-0.3.0.tar` & `btrview-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.899686 btrview-0.3.0/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.3.0/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-02 00:14:34.896350 btrview-0.3.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     5932 2024-04-01 23:56:02.000000 btrview-0.3.0/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       65 2024-04-02 00:03:20.000000 btrview-0.3.0/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2372 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6215 2024-04-01 23:13:39.000000 btrview-0.3.0/btrview/btrfs.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-03-12 18:06:35.000000 btrview-0.3.0/btrview/scripts/btrsend.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2372 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6827 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-03-21 15:13:50.000000 btrview-0.3.0/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      923 2024-04-02 00:03:20.000000 btrview-0.3.0/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-02 00:14:34.899686 btrview-0.3.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.4.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-03 01:49:02.182009 btrview-0.4.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     5932 2024-04-02 00:28:22.000000 btrview-0.4.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       65 2024-04-03 01:44:27.000000 btrview-0.4.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2402 2024-04-03 01:44:21.000000 btrview-0.4.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6911 2024-04-03 01:22:12.000000 btrview-0.4.0/btrview/btrfs.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-03-12 18:06:35.000000 btrview-0.4.0/btrview/scripts/btrsend.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2402 2024-04-03 01:44:21.000000 btrview-0.4.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7202 2024-04-03 01:44:27.000000 btrview-0.4.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-03 01:10:36.000000 btrview-0.4.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-03 01:49:02.182009 btrview-0.4.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-03 01:49:02.000000 btrview-0.4.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      923 2024-04-03 01:44:27.000000 btrview-0.4.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-03 01:49:02.182009 btrview-0.4.0/setup.cfg
```

### Comparing `btrview-0.3.0/LICENSE.md` & `btrview-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.3.0/PKG-INFO` & `btrview-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.3.0
+Version: 0.4.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2022 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.3.0/README.md` & `btrview-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `btrview-0.3.0/btrview/__main__.py` & `btrview-0.4.0/btrview/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import textwrap
 from itertools import zip_longest
 
 import btrview
 from btrview.utils import check_root
-from btrview.btrfs import Btrfs
+from btrview.btrfs import Btrfs, get_forest
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
@@ -34,26 +34,27 @@
     return arg_parser
 
 def logic(labels: list[str], root, deleted, unreachable, prop) -> None:
     check_root()
     filesystems = Btrfs.get_filesystems(labels)
     for fs in filesystems:
         print(f"{fs}")
-        subvol_tree = fs.forest(False, root, deleted, unreachable)
-        subvol_str = get_forest_string(subvol_tree, False, prop)
+        subvols = fs.subvolumes(root,deleted,unreachable)
+        subvol_tree = get_forest([s for s in subvols if not s.deleted],"subvol")
+        subvol_str = get_forest_string(subvol_tree, "Subvolumes", prop)
 
-        snap_tree = fs.forest(True, root, deleted, unreachable)
-        snap_str = get_forest_string(snap_tree, True, prop)
+        snap_tree = get_forest(subvols,"snap")
+        snap_str = get_forest_string(snap_tree, "Snapshots", prop)
 
         zipper = zip_longest(subvol_str.splitlines(),snap_str.splitlines(),fillvalue="")
         for subvol_line, snap_line in zipper:
             print(f"{subvol_line:<50}{snap_line:}")
 
-def get_forest_string(forest, snapshot: bool = False, prop: str = ""):
-    forest_str = "Snapshots: \n" if snapshot else "Subvolumes: \n"
+def get_forest_string(forest, header, prop: str = ""):
+    forest_str = f"{header}:\n"
     for tree in forest:
         #stdout=False is only needed because of bug
         #see https://github.com/caesar0301/treelib/issues/221
         tree_str = tree.show(data_property=prop, stdout=False)
         forest_str += textwrap.indent(str(tree_str), "  ")
     return forest_str
```

### Comparing `btrview-0.3.0/btrview/btrfs.py` & `btrview-0.4.0/btrview/btrfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     _UUIDs:  dict[str,str] = dict()
     _all_mounts: defaultdict[str,set[Mount]] = defaultdict(set)
 
     def __init__(self, uuid: str, label: str|None = None) -> None:
         """Initialist with the filesystem uuid, and label if it exists."""
         self.uuid = uuid
         self.label = label
-        self._get_mounts()
+        if not self._UUIDs:
+            self._get_mounts()
 
     @classmethod
     def _get_mounts(cls) -> None:
         """Generates all the mount points for each filesystem"""
         headings = "label,uuid,fsroot,target"
         #Why parse all mounts instead of just one using the --source flag?
         #Some of the FSes weren't showing up for some reason with that flag. Also
@@ -43,46 +44,56 @@
         #cast to tuple makes for easier referencing, also has the benefit of
         #preventing direct access to the set object
         return tuple(self._all_mounts[self.uuid])
 
     @classmethod
     def get_filesystems(cls, labels:list[str] | None = None) -> list[Self]:
         """Returns a list of each filesystem on the system."""
-        cls._get_mounts() #had to be here in case nothing gets initialized
+        #had to be here in case nothing gets initialized
+        if not cls._UUIDs:
+            cls._get_mounts() 
         filesystems = []
         for uuid,label in cls._UUIDs.items():
             if not labels or (label in labels):
                 fs = cls(uuid,label)
                 filesystems.append(fs)
         return filesystems
 
     @classmethod
     def _get_deleted_subvols(cls, subvols: list[Subvolume]) -> list[Subvolume]:
         """Returns a list of deleted subvolumes"""
-        uuids = {s["UUID"] for s in subvols}
+        uuids = {s.id("snap") for s in subvols}
         puuids = set()
         for subvol in subvols:
-            puuid = subvol["Parent UUID"]
+            puuid = subvol.parent("snap")
             if puuid and (puuid not in uuids):
                 puuids.add(puuid)
         return [Subvolume({"UUID":puuid}, tuple(), deleted=True) for puuid in puuids]
             
     def subvolumes(self, root: bool, deleted: bool, unreachable: bool,) -> list[Subvolume]:
         """Return a list of subvolumes on the file system"""
         mount_point = self.mounts[0].target 
-        out = run(f"btrfs subvolume list -u {mount_point}")
-        fs_uuids = []
+        out = run(f"sudo btrfs subvolume list -apcguqR {mount_point}")
+
         subvols = []
+        keys = "ID,gen,cgen,parent,parent_uuid,received_uuid,uuid".split(",")
+        vals = "Subvolume ID,Generation,Gen at creation,Parent ID,Parent UUID,Received UUID,UUID".split(",")
+        key_dict = {key:val for key,val in zip(keys,vals)}
         for line in out.stdout.splitlines():
-            match = re.search(r"uuid\s*(\S*)",line)
-            if match:
-                fs_uuids.append(match.group(1))
-        for uuid in fs_uuids:
-            subvol = Subvolume.from_UUID(uuid, mount_point, self.mounts)
-            subvols.append(subvol)
+            match_dict = {}
+            for key,val in key_dict.items():
+                match = re.search(f"\\b{key}\\s+(\\S+)",line)
+                if match and match.group(1) == "-":
+                    match_dict[val] = None
+                elif match :
+                    match_dict[val] = match.group(1)
+            path_match = re.search(r"path\s*(.*)",line).group(1).removeprefix("<FS_TREE>")
+            match_dict["btrfs Path"] = Path(f"/{path_match}".replace("//","/",1))
+            match_dict["Name"] = match_dict["btrfs Path"].name
+            subvols.append(Subvolume(match_dict,self.mounts))
         if not unreachable:
             to_remove = []
             for subvol in subvols:
                 if not subvol.mounted:
                     to_remove.append(subvol)
             for subvol in to_remove:
                 subvols.remove(subvol)
@@ -140,11 +151,12 @@
         trees.append(tree)
         tree.create_node(name, subvol_id, data=subvol)
     return tree
 
 def get_forest(subvolumes: list[Subvolume], kind = "subvol") -> list[Tree]:
     """Turns a flat list of subvolumes into a forest of trees."""
     trees: list[Tree] = []
+    subvolumes = subvolumes.copy()
     while subvolumes:
         subvol = subvolumes[0]
         get_tree(subvol, subvolumes, trees, kind)
     return trees
```

### Comparing `btrview-0.3.0/btrview/scripts/btrsend.py` & `btrview-0.4.0/btrview/scripts/btrsend.py`

 * *Files identical despite different names*

### Comparing `btrview-0.3.0/btrview/scripts/btrview.py` & `btrview-0.4.0/btrview/scripts/btrview.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import textwrap
 from itertools import zip_longest
 
 import btrview
 from btrview.utils import check_root
-from btrview.btrfs import Btrfs
+from btrview.btrfs import Btrfs, get_forest
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
@@ -34,26 +34,27 @@
     return arg_parser
 
 def logic(labels: list[str], root, deleted, unreachable, prop) -> None:
     check_root()
     filesystems = Btrfs.get_filesystems(labels)
     for fs in filesystems:
         print(f"{fs}")
-        subvol_tree = fs.forest(False, root, deleted, unreachable)
-        subvol_str = get_forest_string(subvol_tree, False, prop)
+        subvols = fs.subvolumes(root,deleted,unreachable)
+        subvol_tree = get_forest([s for s in subvols if not s.deleted],"subvol")
+        subvol_str = get_forest_string(subvol_tree, "Subvolumes", prop)
 
-        snap_tree = fs.forest(True, root, deleted, unreachable)
-        snap_str = get_forest_string(snap_tree, True, prop)
+        snap_tree = get_forest(subvols,"snap")
+        snap_str = get_forest_string(snap_tree, "Snapshots", prop)
 
         zipper = zip_longest(subvol_str.splitlines(),snap_str.splitlines(),fillvalue="")
         for subvol_line, snap_line in zipper:
             print(f"{subvol_line:<50}{snap_line:}")
 
-def get_forest_string(forest, snapshot: bool = False, prop: str = ""):
-    forest_str = "Snapshots: \n" if snapshot else "Subvolumes: \n"
+def get_forest_string(forest, header, prop: str = ""):
+    forest_str = f"{header}:\n"
     for tree in forest:
         #stdout=False is only needed because of bug
         #see https://github.com/caesar0301/treelib/issues/221
         tree_str = tree.show(data_property=prop, stdout=False)
         forest_str += textwrap.indent(str(tree_str), "  ")
     return forest_str
```

### Comparing `btrview-0.3.0/btrview/subvolume.py` & `btrview-0.4.0/btrview/subvolume.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 
     def __str__(self) -> str:
         return f"{self.fsroot} on {self.target}"
 
 class Subvolume:
     """Class representing a btrfs subvolume"""
     def __init__(self, props: dict[str,str|None], mounts: tuple[Mount, ...],
-                 deleted: bool = False,) -> None:
+                 deleted: bool = False, show: bool = False) -> None:
         self.props = props
         self.mounts = mounts
         self.deleted = deleted
+        self._show = show
 
     @property
     def paths(self) -> list[Path]:
         if not self["btrfs Path"]:
             return []
         btr_path = Path(self["btrfs Path"])
         return [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
@@ -54,15 +55,15 @@
         targets = [mount.target for mount in self.mounts]
         return tuple(path for path in self.paths if path in targets)
 
     def parent(self, p_type: str) -> str | None:
         """Returns parent UUID or ID string"""
         match p_type:
             case "snap":
-                parent = self["Recieved UUID"] or self["Parent UUID"]
+                parent = self["Received UUID"] or self["Parent UUID"]
             case "subvol":
                 parent = self["Parent ID"]
             case _:
                 parent = None
         return parent
 
     def id(self, p_type: str) -> str | None:
@@ -77,22 +78,22 @@
         return ID
 
     @classmethod
     def from_UUID(cls, uuid: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from the subvolumes UUID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -u {uuid} {path}"
         props = cls._run_cmd(cmd)
-        return cls(props, mounts)
+        return cls(props, mounts, show = True)
 
     @classmethod
     def from_ID(cls, ID: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from subvolume's ID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -r {ID} {path}"
         props = cls._run_cmd(cmd)
-        return cls(props, mounts)
+        return cls(props, mounts, show = True)
 
     @classmethod
     def _run_cmd(cls, cmd: str) -> dict[str, str | None]:
         """Runs the shell command and returns the prop dictionary
         if the command doesn't error"""
         out = run(cmd)
         if out.returncode != 0:
@@ -121,14 +122,21 @@
         """Returns true if path is part of a btrfs filesystem."""
         response = run(f"btrfs filesystem usage '{path}'")
         return response.returncode == 0
 
     def __getitem__(self, key: str) -> str | None:
         """Returns the item from the props dictionary, but instead
         of throwing a key error, returns None"""
+        if key in self.props:
+            return self.props.get(key)
+        elif not self._show and not self.deleted:
+            cmd = f"btrfs subvolume show -u {self['UUID']} {self.mounts[0].target}"
+            props = self._run_cmd(cmd)
+            self.props |= props
+            self._show = True
         return self.props.get(key)
 
     def __str__(self) -> str:
         string = self["Name"] or str(self["UUID"])
         if mps := self.mount_points:
             mp_string = ", ".join(str(mp) for mp in mps)
             string = f"{string} on: {mp_string}"
```

### Comparing `btrview-0.3.0/btrview/utils.py` & `btrview-0.4.0/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.3.0/btrview.egg-info/PKG-INFO` & `btrview-0.4.0/btrview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.3.0
+Version: 0.4.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2022 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.3.0/pyproject.toml` & `btrview-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.3.0"
+version = "0.4.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,15 +20,15 @@
 btrview = "btrview.scripts.btrview:main"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

