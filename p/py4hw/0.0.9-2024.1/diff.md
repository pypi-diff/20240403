# Comparing `tmp/py4hw-0.0.9.tar.gz` & `tmp/py4hw-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c:\Projects\Research\INT_Py4hw\py4hw\dist\tmpdloz20u2\py4hw-0.0.9.tar", last modified: Sat Jul 23 19:39:09 2022, max compression
+gzip compressed data, was "py4hw-2024.1.tar", last modified: Wed Apr  3 10:54:59 2024, max compression
```

## Comparing `py4hw-0.0.9.tar` & `py4hw-2024.1.tar`

### file list

```diff
@@ -1,31 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-07-23 19:39:09.000000 py4hw-0.0.9/
--rw-rw-rw-   0        0        0    35149 2021-06-17 16:52:58.000000 py4hw-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1014 2022-07-23 19:39:09.000000 py4hw-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      573 2022-01-30 16:19:40.000000 py4hw-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw/
--rw-rw-rw-   0        0        0      421 2022-02-13 19:59:59.000000 py4hw-0.0.9/py4hw/__init__.py
--rw-rw-rw-   0        0        0    15126 2022-07-22 08:12:10.000000 py4hw-0.0.9/py4hw/base.py
--rw-rw-rw-   0        0        0     5214 2022-02-08 09:58:34.000000 py4hw-0.0.9/py4hw/debug.py
--rw-rw-rw-   0        0        0     9623 2022-07-04 05:10:47.000000 py4hw-0.0.9/py4hw/gui.py
--rw-rw-rw-   0        0        0     7143 2022-07-23 17:21:36.000000 py4hw-0.0.9/py4hw/helper.py
-drwxrwxrwx   0        0        0        0 2022-07-23 19:39:09.000000 py4hw-0.0.9/py4hw/logic/
--rw-rw-rw-   0        0        0      233 2022-01-27 13:06:32.000000 py4hw-0.0.9/py4hw/logic/__init__.py
--rw-rw-rw-   0        0        0    11271 2022-06-07 06:59:38.000000 py4hw-0.0.9/py4hw/logic/arithmetic.py
--rw-rw-rw-   0        0        0    17792 2022-02-09 12:40:38.000000 py4hw-0.0.9/py4hw/logic/bitwise.py
--rw-rw-rw-   0        0        0      509 2022-01-29 12:22:03.000000 py4hw-0.0.9/py4hw/logic/clock.py
--rw-rw-rw-   0        0        0    10364 2022-02-04 15:02:28.000000 py4hw-0.0.9/py4hw/logic/relational.py
--rw-rw-rw-   0        0        0    14390 2022-07-23 07:19:59.000000 py4hw-0.0.9/py4hw/logic/simulation.py
--rw-rw-rw-   0        0        0     2501 2022-03-04 14:46:48.000000 py4hw-0.0.9/py4hw/logic/storage.py
--rw-rw-rw-   0        0        0    29666 2022-07-18 15:35:28.000000 py4hw-0.0.9/py4hw/rtl_generation.py
--rw-rw-rw-   0        0        0    45392 2022-07-04 05:25:42.000000 py4hw-0.0.9/py4hw/schematic.py
--rw-rw-rw-   0        0        0    22417 2022-03-08 07:49:57.000000 py4hw-0.0.9/py4hw/schematic_symbols.py
--rw-rw-rw-   0        0        0     5758 2022-01-28 17:43:42.000000 py4hw-0.0.9/py4hw/simulation.py
-drwxrwxrwx   0        0        0        0 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/
--rw-rw-rw-   0        0        0     1014 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-23 19:39:08.000000 py4hw-0.0.9/py4hw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-06-10 10:55:08.000000 py4hw-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      490 2022-07-23 19:39:09.000000 py4hw-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      815 2022-07-23 19:38:25.000000 py4hw-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.331527 py4hw-2024.1/
+-rw-rw-rw-   0        0        0    35149 2021-06-17 16:52:58.000000 py4hw-2024.1/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-10-05 15:22:53.000000 py4hw-2024.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1226 2024-04-03 10:54:59.329526 py4hw-2024.1/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2022-01-30 16:19:40.000000 py4hw-2024.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.007711 py4hw-2024.1/py4hw/
+-rw-rw-rw-   0        0        0      534 2023-05-10 09:47:00.000000 py4hw-2024.1/py4hw/__init__.py
+-rw-rw-rw-   0        0        0    22222 2023-12-04 22:30:16.000000 py4hw-2024.1/py4hw/base.py
+-rw-rw-rw-   0        0        0    27343 2023-04-07 08:22:39.000000 py4hw-2024.1/py4hw/code_generation.py
+-rw-rw-rw-   0        0        0     5381 2022-11-20 10:25:09.000000 py4hw-2024.1/py4hw/debug.py
+-rw-rw-rw-   0        0        0    11151 2024-02-16 15:11:29.000000 py4hw-2024.1/py4hw/gui.py
+-rw-rw-rw-   0        0        0    25105 2023-12-04 22:30:16.000000 py4hw-2024.1/py4hw/helper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.148632 py4hw-2024.1/py4hw/logic/
+-rw-rw-rw-   0        0        0      294 2023-03-19 09:35:30.000000 py4hw-2024.1/py4hw/logic/__init__.py
+-rw-rw-rw-   0        0        0    17588 2024-03-23 08:42:37.000000 py4hw-2024.1/py4hw/logic/arithmetic.py
+-rw-rw-rw-   0        0        0    13229 2023-03-19 08:52:48.000000 py4hw-2024.1/py4hw/logic/arithmetic_fp.py
+-rw-rw-rw-   0        0        0     2535 2023-03-19 19:29:08.000000 py4hw-2024.1/py4hw/logic/arithmetic_fxp.py
+-rw-rw-rw-   0        0        0    25059 2024-03-24 11:59:06.000000 py4hw-2024.1/py4hw/logic/bitwise.py
+-rw-rw-rw-   0        0        0     1616 2023-04-28 09:24:58.000000 py4hw-2024.1/py4hw/logic/clock.py
+-rw-rw-rw-   0        0        0    12701 2023-04-28 08:59:53.000000 py4hw-2024.1/py4hw/logic/relational.py
+-rw-rw-rw-   0        0        0    17573 2024-03-25 11:05:26.000000 py4hw-2024.1/py4hw/logic/simulation.py
+-rw-rw-rw-   0        0        0     5188 2024-03-26 06:13:28.000000 py4hw-2024.1/py4hw/logic/storage.py
+-rw-rw-rw-   0        0        0    29389 2024-03-25 16:08:37.000000 py4hw-2024.1/py4hw/rtl_generation.py
+-rw-rw-rw-   0        0        0    63168 2024-02-12 17:48:36.000000 py4hw-2024.1/py4hw/schematic.py
+-rw-rw-rw-   0        0        0    28055 2024-02-06 16:04:55.000000 py4hw-2024.1/py4hw/schematic_symbols.py
+-rw-rw-rw-   0        0        0     6237 2023-05-25 08:24:27.000000 py4hw-2024.1/py4hw/simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.316533 py4hw-2024.1/py4hw/transpilation/
+-rw-rw-rw-   0        0        0      106 2023-04-02 13:11:02.000000 py4hw-2024.1/py4hw/transpilation/__init__.py
+-rw-rw-rw-   0        0        0     2564 2023-04-03 11:16:36.000000 py4hw-2024.1/py4hw/transpilation/ast2xml.py
+-rw-rw-rw-   0        0        0      402 2023-04-05 11:03:14.000000 py4hw-2024.1/py4hw/transpilation/astutils.py
+-rw-rw-rw-   0        0        0    17990 2023-04-07 08:22:39.000000 py4hw-2024.1/py4hw/transpilation/python2cflexhdl_transpilation.py
+-rw-rw-rw-   0        0        0     5474 2023-04-05 11:03:14.000000 py4hw-2024.1/py4hw/transpilation/python2structural.py
+-rw-rw-rw-   0        0        0    28050 2024-03-19 17:05:40.000000 py4hw-2024.1/py4hw/transpilation/python2verilog_transpilation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:54:59.320535 py4hw-2024.1/py4hw.egg-info/
+-rw-rw-rw-   0        0        0     1226 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 10:54:58.000000 py4hw-2024.1/py4hw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-06-10 10:55:08.000000 py4hw-2024.1/pyproject.toml
+-rw-rw-rw-   0        0        0       83 2023-12-04 22:30:16.000000 py4hw-2024.1/requires.txt
+-rw-rw-rw-   0        0        0      490 2024-04-03 10:54:59.342525 py4hw-2024.1/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-02-12 15:40:49.000000 py4hw-2024.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py4hw-0.0.9/LICENSE` & `py4hw-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py4hw-0.0.9/PKG-INFO` & `py4hw-2024.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: py4hw
-Version: 0.0.9
+Version: 2024.1
 Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.
 Home-page: https://github.com/davidcastells/py4hw
 Author: David Castells-Rufas
 Author-email: david.castells@uab.cat
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nbwavedrom==0.2.0
+Requires-Dist: ipywidgets
+Requires-Dist: matplotlib
+Requires-Dist: deprecated
+Requires-Dist: scipy
+Requires-Dist: pytest
+Requires-Dist: edalize
+Requires-Dist: setuptools
 
 # py4hw
 
 [![PyPI version](https://badge.fury.io/py/py4hw.svg)](https://badge.fury.io/py/py4hw)
 [![Join the chat at https://gitter.im/davidcastells/py4hw](https://badges.gitter.im/davidcastells/py4hw.svg)](https://gitter.im/davidcastells/py4hw?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 py4hw is an HDL library based on python to create digital circuits (mainly) following a structural design methodology.
```

### Comparing `py4hw-0.0.9/README.md` & `py4hw-2024.1/README.md`

 * *Files identical despite different names*

### Comparing `py4hw-0.0.9/py4hw/base.py` & `py4hw-2024.1/py4hw/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,49 +6,66 @@
     """
     
     def __init__(self, parent, instanceName:str):
         self.parent = parent
         self.name = instanceName
         
         if (not(parent is None)):
+            if not(isinstance(parent, Logic)):
+                raise Exception('parent object must be a Logic object not a {}'.format(type(parent)))
+                
             # Add this object as a parent's child
             if (instanceName in parent.children.keys()):
                 raise Exception('there is already a child named {} in {}'.format(instanceName, parent.getFullPath() ))
 
             parent.children[instanceName] = self
 
         self.inPorts = []   # in ports are a sorted list
         self.outPorts = []  # out ports are a sorted list
+        self.inOutPorts = [] # in/out ports
         self.sources = []   # list of InterfaceSource objects
         self.sinks = []     # List of InterfaceSink objects
     
         self.children = {}          # children are keyed by name
         self.clockDriver = None     # every circuit has a clock driver, if None it is inherited from parent
         
+        self._wires = {}        # dictionary of wires created by the object
+        
     def addIn(self, name , wire):
         port = InPort(self, name, wire)
         self.inPorts.append(port)
         return wire;
     
     def getInPortByName(self, name):
         for port in self.inPorts:
             if (port.name == name):
                 return port
         return None
+
+    def getOutPortByName(self, name):
+        for port in self.outPorts:
+            if (port.name == name):
+                return port
+        return None
         
     def reconnectIn(self, name, wire):
         # there is already a port with this name, but we just one to change the wire assigned
         port = self.getInPortByName(name)
         port.wire = wire
         
         
     def addOut(self, name, wire):
         port = OutPort(self, name, wire)
         self.outPorts.append(port)
         return wire;
+    
+    def addInOut(self, name, wire):
+        port = InOutPort(self, name, wire)
+        self.inOutPorts.append(port)
+        return wire;
 
     def addInterfaceSource(self, name:str, interface):
         """
         Adds the source ports of the interface to the 
 
         Parameters
         ----------
@@ -57,24 +74,27 @@
 
         Returns
         -------
         None.
 
         """
         ports = []
+        if (len(name) > 0):
+            name = name + '_'
+            
         for obj in interface.sourceToSink:
             wire = obj[1]
-            portname = name + "_" +obj[0]
+            portname = name + obj[0]
             port = OutPort(self, portname, wire)
             self.outPorts.append(port)
             ports.append(port)
         
         for obj in interface.sinkToSource:
             wire = obj[1]
-            portname = name + "_" +obj[0]
+            portname = name + obj[0]
             port = InPort(self, portname, wire)
             self.inPorts.append(port)
             ports.append(port)
 
         self.sources.append(InterfaceSource(name, ports))
             
         return interface;
@@ -90,35 +110,66 @@
 
         Returns
         -------
         None.
 
         """
         ports = []
+        if (len(name) > 0):
+            name = name + '_'
+            
         for obj in interface.sourceToSink:
             wire = obj[1]
-            portname = name + "_" +obj[0]
+            portname = name + obj[0]
             port = InPort(self, portname, wire)
             self.inPorts.append(port)
             ports.append(port)
         for obj in interface.sinkToSource:
             wire = obj[1]
-            portname = name + "_" +obj[0]
+            portname = name + obj[0]
             port = OutPort(self, portname, wire)
             self.outPorts.append(port)
             ports.append(port)
             
         self.sinks.append(InterfaceSink(name, ports))
         
         return interface;
         
+    def appendWire(self, wire):
+        #print('checking if ', wire.name, 'is already in', [x for x in self._wires.keys()])
+        if (wire.name in self._wires.keys()):
+            raise Exception('a wire named {} already exist'.format(wire.name))
+            
+        self._wires[wire.name] = wire
+        
+    def bidir_wire(self, name, width=1):
+        return BidirWire(self, name, width)
+    
     def wire(self, name, width=1):
         return Wire(self, name, width);
     
-    def wires(self, name:str, num:int, width:int):
+    def wires(self, name:str, num:int, width:int) -> list:
+        """
+        Creates a number of wires
+
+        Parameters
+        ----------
+        name : str
+            prefix of the wire names, it will be suffixed by _0, _1, etc.
+        num : int
+            numer of wires to create.
+        width : int
+            width of the wires to create.
+
+        Returns
+        -------
+        list
+            a list with the created wires.
+
+        """
         ret = []
         for i in range(num):
             ret.append(self.wire('{}_{}'.format(name,i), width))
         return ret;
     
     def allLeaves(self):
         acum = []
@@ -218,27 +269,33 @@
         if (pos2 >= 0):
             return objFound.getFromFullPath( path[pos1:])
         else:
             return objFound;
         
 class Wire:
     """
-    Wires in py4hw connect one source with one (or more) sinks
+    Wires in py4hw connect one source with one (or more) sinks.
+    For many-to-many connections use BidirWire
     """
     
     # this is the list of prepared wires, 
     prepared = []
     
     def __init__(self, parent, name : str, width: int = 1 ):
+        # the following should not be necessary if python checks types
+        assert(isinstance(name, str))
+        assert(isinstance(width, int))
+        
         self.parent = parent
         self.name = name
         self.width = width
         self.value = 0 # should be None      # reset state
         self.sinks = []
         self.source = None
+        parent.appendWire(self)
         
     def getFullPath(self)->str:
         return self.parent.getFullPath() + '[{}]'.format(self.name)
     
     def getWidth(self) -> int:
         return self.width
     
@@ -255,18 +312,20 @@
         self.value = self.next
         
     def get(self) -> int:
         return self.value
     
     def setSource(self, source):
         if (self.source != None):
-            raise Exception('Source already connected to ' + self.source.parent.getFullPath())
+            raise Exception('Source of wire {} already connected to {}'.format(self.getFullPath(), self.source.parent.getFullPath()))
 
         self.source = source
         
+    def addSource(self, source):
+        self.setSource(source)
         
     def getSource(self):
         """
         Returns the OutPort that drives this wire
 
         Returns
         -------
@@ -316,16 +375,150 @@
         """
         for w in Wire.prepared:
             w.settle()
             
         # empty list
         Wire.prepared = []
     
+    def rename(self, newname):
+        del self.parent._wires[self.name]
+        self.name = newname
+        self.parent.appendWire(self)
+        
+    def reparent(self, newparent):
+        del self.parent._wires[self.name]
+        self.parent = newparent
+        newparent.appendWire(self)
+
+    def reparentAndRename(self, newparent, newname):
+        del self.parent._wires[self.name]
+        self.name = newname
+        self.parent = newparent
+        newparent.appendWire(self)
+
+class BidirWire(Wire):
+    """
+    Wires in py4hw connect one source with one (or more) sinks.
+    For many-to-many connections use BidirWire
+    """
+    
+    # this is the list of prepared wires, 
+    # @todo what for ??
+    prepared = []
+    
+    def __init__(self, parent, name : str, width: int = 1 ):
+        # the following should not be necessary if python checks types
+        assert(isinstance(name, str))
+        assert(isinstance(width, int))
+        
+        self.parent = parent
+        self.name = name
+        self.width = width
+        self.value = 0 # should be None      # reset state
+        self.sinks = []
+        self.sources = []
+        parent.appendWire(self)
+        
+    def getFullPath(self)->str:
+        return self.parent.getFullPath() + '[{}]'.format(self.name)
+    
+    def getWidth(self) -> int:
+        return self.width
     
+    def put(self, val:int):
+        mask = (1<<self.width) -1
+        self.value = val & mask
 
+    def prepare(self, val:int):
+        mask = (1<<self.width) -1
+        self.next = val & mask
+        Wire.prepared.append(self)
+        
+    def settle(self):
+        self.value = self.next
+        
+    def get(self) -> int:
+        return self.value
+    
+    def addSource(self, source):        
+        self.sources.append(source)
+        
+        
+    def getSource(self):
+        """
+        Returns the OutPort that drives this wire
+
+        Returns
+        -------
+        TYPE
+            DESCRIPTION.
+
+        """
+        return self.source
+    
+    def addSink(self, sink):
+        """
+        Adds a sink to the wire
+
+        Parameters
+        ----------
+        sink : TYPE
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.sinks.append(sink)
+        
+    def getSinks(self):
+        """
+        Gets all the sinks from a wire
+
+        Returns
+        -------
+        TYPE
+            DESCRIPTION.
+
+        """
+        return self.sinks;
+    
+
+    def settleAll():
+        """
+        Settles all pending wires that were changed by clock methods
+
+        Returns
+        -------
+        None.
+
+        """
+        for w in Wire.prepared:
+            w.settle()
+            
+        # empty list
+        Wire.prepared = []
+    
+    def rename(self, newname):
+        del self.parent._wires[self.name]
+        self.name = newname
+        self.parent.appendWire(self)
+        
+    def reparent(self, newparent):
+        del self.parent._wires[self.name]
+        self.parent = newparent
+        newparent.appendWire(self)
+
+    def reparentAndRename(self, newparent, newname):
+        del self.parent._wires[self.name]
+        self.name = newname
+        self.parent = newparent
+        newparent.appendWire(self)
+        
 class InPort:
     """
     An Input port
     """
     
     def __init__(self, parent:Logic, name, wire:Wire):
         """
@@ -358,15 +551,15 @@
     def getFullPath(self):
         return self.parent.getFullPath() + '[{}]'.format(self.name)
     
 class OutPort:
     """
     An output port
     """
-    def __init__(self, parent:Logic, name:str, wire:Wire):
+    def __init__(self, parent:Logic, name:str, wire):
         """
         Creates an out port to the cell.
         The cell will be registered as source of the wire only if it
         is a leaf (a primitive) in the hierarchy 
 
         Parameters
         ----------
@@ -384,15 +577,52 @@
         """
         #print('out port')
         self.name = name
         self.parent = parent
         self.wire = wire
         
         if (parent.isPrimitive()):
-            wire.setSource(self)
+            wire.addSource(self)
+
+    def getFullPath(self):
+        return self.parent.getFullPath() + '[{}]'.format(self.name)
+
+class InOutPort:
+    """
+    An input/output port
+    """
+    def __init__(self, parent:Logic, name:str, wire:Wire):
+        """
+        Creates an in/out port to the cell.
+        The cell will be registered as source of the wire only if it
+        is a leaf (a primitive) in the hierarchy 
+
+        Parameters
+        ----------
+        parent : Logic
+            Parent Cell of the port
+        name : str
+            name of the port.
+        wire : Wire
+            Wire associated with the port
+
+        Returns
+        -------
+        None.
+
+        """
+        #print('out port')
+        self.name = name
+        self.parent = parent
+        self.wire = wire
+        
+        if (parent.isPrimitive()):
+            wire.addSource(self)
+            wire.addSink(self)
+
 
     def getFullPath(self):
         return self.parent.getFullPath() + '[{}]'.format(self.name)
 
 class InterfaceSource:
     def __init__(self, name:str, ports):
         self.name = name
@@ -405,21 +635,24 @@
         self.name = name
         self.ports = ports
     
 class HWSystem(Logic):
     """
     A Hardware system is the top level entity of all designs 
     """
-    def __init__(self, clock_driver=None):
+    def __init__(self, clock_driver=None, name=None):
         super().__init__(None, "HWSystem")
         self.simulator = None
         if (clock_driver is None):
-            clock_driver = ClockDriver('clk50', 50E6, 0) # we create a 50MHz clock driver by default
+            clock_driver = ClockDriver('clk50', 50E6, 0, wire=self.wire('clk50')) # we create a 50MHz clock driver by default
+        if not(name is None):
+            self.name = name
         self.clockDriver = clock_driver
         
+        
     def getSimulator(self):
         """
         Returns the singleton simulator instance
 
         Returns
         -------
         TYPE
@@ -437,15 +670,15 @@
         
     
 class ClockDriver():
     """
     A clock driver
     """
     
-    def __init__(self, name:str, freq=50E6, phaseOffset=0, base=None, enable=None):
+    def __init__(self, name:str, freq=50E6, phaseOffset=0, base=None, enable=None, wire=None):
         """
         Creates a clock driver
 
         Parameters
         ----------
         name : str
             Name of the clock driver.
@@ -454,14 +687,16 @@
         phaseOffset : number, optional
             phase offset (in %) of the positive edge of the clock
         base : ClockDriver, optional
             ClockDriver that this clock driver is based on. This is useful for gated clocks.
         enable : Wire, optional
             Wire controling the gating of the clock. When enable is 0, the clock
             will be gated
+        wire : Wire, optional
+            Wire that contains the clock
 
         Returns
         -------
         None.
 
         """
         self.name = name
@@ -471,15 +706,15 @@
             self.freq = freq
             self.phaseOffset = phaseOffset
         else:
             self.freq = base.freq;
             self.phaseOffset = base.phaseOffset
             
         self.enable = enable
-        
+        self.wire = wire
 
 def has_method(o, name):
     return callable(getattr(o, name, None))
 
 
 class Interface:
     """
@@ -507,14 +742,34 @@
         -------
         None.
 
         """
         w = self.parent.wire(self.name + "_" + name, width)
         self.sourceToSink.append([name, w])
         return w;
+    
+    def getSourceToSink(self, name):
+        if len(self.sourceToSink) == 0:
+            raise Exception('No source-to-sink elements in this interface')
+            
+        for p in self.sourceToSink:
+            if (p[0] == name):
+                return p[1]
+            
+        raise Exception('SourceToSink {} not found'.format(name))
+    
+    def getSinkToSource(self, name):
+        if len(self.sinkToSource) == 0:
+            raise Exception('No sink-to-source elements in this interface')
+            
+        for p in self.sinkToSource:
+            if (p[0] == name):
+                return p[1]
+                
+        raise Exception('SinkToSource {} not found'.format(name))
         
     def addSinkToSource(self, name:str, width:int):
         """
         Adds a source wire to the definition of the interface
 
         Parameters
         ----------
```

### Comparing `py4hw-0.0.9/py4hw/debug.py` & `py4hw-2024.1/py4hw/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,24 @@
         
         for child in obj.children.values():
             indent = oldindent + 1
             _printElementWithValues(child, include=include, format=format)
             
         indent = oldindent
     
+def getPorts(obj:Logic):
+    ret = []
+    for ip in obj.inPorts:
+        ret.append(ip)
+
+    for ip in obj.outPorts:
+        ret.append(ip)
+
+    return ret
+
 def getPortWires(obj:Logic):
     ret = []
     for ip in obj.inPorts:
         ret.append(ip.wire)
 
     for ip in obj.outPorts:
         ret.append(ip.wire)
```

### Comparing `py4hw-0.0.9/py4hw/gui.py` & `py4hw-2024.1/py4hw/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import tkinter 
 import tkinter.font
 from tkinter import *
 from tkinter import ttk
-
+from PIL import Image, ImageTk
+import os
 from .base import Logic
 from .schematic import Schematic
     
 class Workbench():
     
-    
+    def getIcon(self, path):
+        script_directory = os.path.dirname(os.path.abspath(__file__))
+        icon_path = os.path.join(script_directory, path)
+        
+        icon = Image.open(icon_path)
+        icon = ImageTk.PhotoImage(icon)
+        return icon
+        
     def __init__(self, sys:Logic):
     
         self.sys = sys
         self.detailObj = None
         
         root = tkinter.Tk()
         root.title('py4hw Interactive Workbench')
@@ -21,62 +29,77 @@
         
         ttk.Style().configure("Treeview", fg="light yellow")
         font = tkinter.font.Font(size=8)
         ttk.Style().configure("Prolepsis.Treeview", font=font)
         
         self.topPane = PanedWindow(root, orient=HORIZONTAL)
         
-        self.hierarchyPane = PanedWindow(self.topPane, relief = SUNKEN, width=50, height=100)
+        self.hierarchyPane = Frame(self.topPane) # PanedWindow(self.topPane, relief = SUNKEN, width=50, height=100)
         self.topPane.add(self.hierarchyPane)
         
+        self.buttonPane = Frame(self.hierarchyPane) #, relief = SUNKEN, width=100, height=100)
+        
+        self.txtClocks = tkinter.StringVar(value='1')
         #print(ttk.Style().lookup("Prolepsis.Treeview", "font"))
+        txtClocks = ttk.Entry(self.buttonPane, width=10, textvariable=self.txtClocks)
+        #txtClocks.grid(row=0, column=0)
+        txtClocks.pack(side=tkinter.LEFT, padx=10, pady=(10,5))
+        
+        btnClock = ttk.Button(self.buttonPane, text="Clock", command=self.guiClk)
+        btnClock.pack(side=tkinter.RIGHT, padx=(10,0), pady=(10,5))
+        #btnClock.grid(row=0, column=1)
         
-        btnClock = ttk.Button(self.hierarchyPane, text="Clock", command=self.guiClk)
-        self.hierarchyPane.add(btnClock)
-        btnClock.pack()
+        #self.hierarchyPane.add(self.buttonPane)
         
-        self.hierarchyTree()
+        self.buttonPane.pack(side=tkinter.TOP)
+        
+        self.createHierarchyTree()
         
         self.rightPane = PanedWindow(self.topPane, orient=VERTICAL, relief = SUNKEN, width=100, height=100)
         self.topPane.add(self.rightPane)
         
         self.interfacePane = PanedWindow(self.rightPane, relief = SUNKEN, width=100, height=100)
         
         self.schematicAreaPane = PanedWindow(self.rightPane,  orient=VERTICAL, relief = SUNKEN, width=100, heigh=20)
-        self.schematicToolbarPane = PanedWindow(self.schematicAreaPane,  orient=HORIZONTAL, relief = SUNKEN, width=100, heigh=20)
+        self.schematicToolbarPane = Frame(self.schematicAreaPane) #,  orient=HORIZONTAL, relief = SUNKEN, width=100, heigh=20)
                 
         self.rightPane.add(self.interfacePane)
         self.rightPane.add(self.schematicAreaPane)
         self.schematicAreaPane.add(self.schematicToolbarPane) 
         
-        btnZoomOut = ttk.Button(self.schematicToolbarPane, text="Zoom out", command=self.guiZoomOut)
-        btnZoomIn = ttk.Button(self.schematicToolbarPane, text="Zoom in", command=self.guiZoomIn)
-
-        self.schematicToolbarPane.add(btnZoomOut)
-        self.schematicToolbarPane.add(btnZoomIn)
-
-#        btnZoomOut.pack()
+        icon_zo = self.getIcon('zoomout24.png')
+        icon_zi = self.getIcon('zoomin24.png')
+        
+        btnZoomIn = ttk.Button(self.schematicToolbarPane,  image=icon_zi, text="Zoom in", command=self.guiZoomIn)
+        btnZoomOut = ttk.Button(self.schematicToolbarPane, image=icon_zo, text="Zoom out", command=self.guiZoomOut)
+        
+        btnZoomIn.pack(side=tkinter.LEFT)
+        btnZoomOut.pack(side=tkinter.LEFT)
         
         self.schematicPane = PanedWindow(self.schematicAreaPane, relief = SUNKEN, width=100, height=100)
         self.schematicAreaPane.add(self.schematicPane)
         
         #pane2.pack(fill=BOTH, expand=YES, side=RIGHT)
         
         self.circuitDetail(None)
         
         self.topPane.pack(fill=BOTH, expand=True)
         
-        sys.getSimulator().addListener(self)
+        # explicitelly update
+        # sys.getSimulator().addListener(self)
         
         
         root.mainloop()
         
     def guiClk(self):
+        clks = int(self.txtClocks.get())
         sim = self.sys.getSimulator()
-        sim.clk(1)
+        sim.clk(clks)
+        #explicitelly update
+        self.simulatorUpdated()
 
     def guiZoomOut(self):
         self.schematicDiagram.scale("all", 0, 0, 0.9, 0.9)
 
     def guiZoomIn(self):
         self.schematicDiagram.scale("all", 0, 0, 1.1, 1.1)
 
@@ -91,14 +114,17 @@
         None.
 
         """
         if (self.detailObj != None):
             self.setCircuitDetail(self.detailObj)
         
     def circuitDetail(self, obj:Logic):
+
+        # this is called just once now (?)        
+        print('Circuit detail on ', obj)
         
         # Create the Circuit Interface pane
         # @todo we are creating this every time we focus on a circuit, could we
         # just create it once and clear the tree view and populate it as necessary ?
         self.detail_tv = ttk.Treeview(self.interfacePane)
         
         detail_tv = self.detail_tv
@@ -122,47 +148,49 @@
         
         detail_tv.config(selectmode=tkinter.NONE)
         detail_tv.tag_configure("ally", background="green")
         #detail_tv.tag_bind("char", "<Double-Button-1>", event)
         #tv.config(style="Prolepsis.Treeview")
         detail_tv["style"] = "Prolepsis.Treeview"
 
-        self.debugTkinterHierarchy(self.root, 0)
+        #self.debugTkinterHierarchy(self.root, 0)
         
         if (obj == None):
             return
         
         self.setCircuitDetail(obj)
         
         
     def debugTkinterHierarchy(self, obj, ii):
         indent = '|' * ii + '+'
-        print('[INFO] {} tkinter obj {}'.format(indent, type(obj)));
+        print('[INFO] {} tkinter obj {} {}'.format(indent, type(obj), obj._name if (hasattr(obj, '_name')) else ''));
         
         try:
             for child in obj.children.values():
                 self.debugTkinterHierarchy(child, ii+1)
         except:
             pass
                 
     def setCircuitDetail(self, obj:Logic):
         
         if (obj != None):
             for pane in self.schematicPane.panes():
                 self.schematicPane.forget(pane)
                 
-            if not(obj.isStructural()):
+            if (obj.isStructural()):
                 # ignore non structural circuits
-                return
-                
-            sch = Schematic(obj, render='tkinter', parent=self.schematicPane)
-
-            self.schematicDiagram = sch.canvas.canvas
-            self.schematicPane.add(self.schematicDiagram)
-            #self.schematicPane.pack()
+                sch = Schematic(obj, render='tkinter', parent=self.schematicPane, showValues=True)
+    
+                sch.drawAll()
+                self.schematicDiagram = sch.canvas.canvas
+                self.schematicPane.add(self.schematicDiagram)
+                #self.schematicPane.pack()
+            elif (hasattr(obj, 'tkinter_gui')):
+                sch = obj.tkinter_gui(self.schematicPane)
+                self.schematicPane.add(sch)
             
         self.detailObj = obj
         self.detail_tv.delete(*self.detail_tv.get_children())
         
         detail_tv = self.detail_tv
         
         visitedPorts = []
@@ -221,23 +249,28 @@
                 circuitType = 'Clockable'
             elif (child.isPropagatable()):
                 circuitType = 'Propagatable'
             childid = tv.insert(tvid, tkinter.END, text=type(child).__name__, values=[instanceName, circuitType, child.getFullPath()], tags=["ally","char"])
             self.map_id_obj[childid] = child
             self.populateTree(tv, childid, child)
 
-    def hierarchyTree(self):
+    def createHierarchyTree(self):
         self.hierarchyTree = ttk.Treeview(self.hierarchyPane)
     
         tv = self.hierarchyTree  
         self.map_id_obj = {}
     
+        
         tv.bind('<<TreeviewSelect>>', self.callback)
-        self.hierarchyPane.add(tv)
+        #self.hierarchyPane.add(tv)
         tv.pack(fill=BOTH, expand=YES)
+        #tv.grid(row=1, column=0, columnspan=2, sticky='nsew')
+        
+        
+        
         dc_iid = tv.insert("", tkinter.END, text="HWSystem", values=['Top', 'Top level'], open=True)
         
         self.map_id_obj[dc_iid] = self.sys
     
         self.populateTree(tv, dc_iid, self.sys)
         
         print(tv.cget("displaycolumns"))
```

### Comparing `py4hw-0.0.9/py4hw/logic/arithmetic.py` & `py4hw-2024.1/py4hw/logic/arithmetic.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,52 @@
 """
 Created on Wed Jan 19 12:53:47 2022
 
 @author: dcr
 """
 from .. import *
 from .bitwise import *
+
 from deprecated import deprecated
 
 
+class Add(Logic):
+    """
+    Combinational Arithmetic Add
+    """
+
+    def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire, ci=None, co=None):
+        super().__init__(parent, name)
+        self.a = self.addIn("a", a)
+        self.b = self.addIn("b", b)
+        self.r = self.addOut("r", r)
+        
+        if (ci is None):
+            self.ci = None
+        else:
+            self.ci = self.addIn('ci', ci)
+            
+        if (co is None):
+            self.co = None
+        else:
+            self.co = self.addOut('co', co)
+
+    def propagate(self):
+        if (not(self.ci is None)):
+            vci = self.ci.get()
+        else:
+            vci = 0
+
+        vr = self.a.get() + self.b.get() + vci
+        
+        if (not(self.co is None)):
+            self.co.put(vr >> self.r.getWidth())
+            
+        self.r.put(vr)
+
 class Abs(Logic):
     """
     Absolute value
     """
     def __init__(self, parent, name: str, a: Wire, r: Wire, inverted:Wire=None):
         """
         Creates ans absolute value circuit r = abs(a), inverted=sign(a)
@@ -42,18 +77,31 @@
         if not(inverted is None):
             s = self.addOut('inverted', inverted)
         else:
             s = self.wire('sign')
 
         zero = self.wire('zero', r.getWidth())
         neg = self.wire('neg', a.getWidth())
+        Constant(self, 'zero', 0, zero)
         Sign(self, 'sign', a, s)
         Sub(self, 'sub', zero, a, neg)
         Mux2(self, 'mux', s, a, neg, r)
 
+
+class Neg(Logic):
+    def __init__(self, parent, name: str, a: Wire, r: Wire):
+        super().__init__(parent, name)
+
+        self.addIn("a", a)
+        self.addOut("r", r)
+
+        zero = self.wire('zero', r.getWidth())
+        Constant(self, 'zero', 0, zero)    
+        Sub(self, 'sub', zero, a, r)
+
 class Sign(Logic):
     """
     Sign test.
     r = 0 if a >= 0 (positive)
     t = 1 if a < 0 (negative)
     """
 
@@ -62,14 +110,17 @@
         self.a = self.addIn("a", a)
         self.r = self.addOut("r", r)
 
         Bit(self, "signBit", a, a.getWidth() - 1, r)
         
 
 class SignExtend(Logic):
+    """
+    Behaviouraly modeled sign extend
+    """
     def __init__(self, parent: Logic, name: str, a: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn('a', a)
         self.r = self.addOut('r', r)
 
     def propagate(self):
         value = self.a.get()
@@ -77,114 +128,199 @@
         for i in range(self.a.getWidth(), self.r.getWidth()):
             value = value | (hb << i)
 
         self.r.put(value)
 
 
 class ZeroExtend(Logic):
+    """
+    Behaviouraly modeled zero extend
+    """
     def __init__(self, parent: Logic, name: str, a: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn('a', a)
         self.r = self.addOut('r', r)
 
     def propagate(self):
         value = self.a.get()
         self.r.put(value)
 
 
 
-class Add(Logic):
+
+
+class Mul(Logic):
     """
-    Combinational Arithmetic Add
+    Combinational Arithmetic Multiplier
     """
 
     def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn("a", a)
         self.b = self.addIn("b", b)
         self.r = self.addOut("r", r)
 
     def propagate(self):
-        self.r.put(self.a.get() + self.b.get())
+        self.r.put(self.a.get() * self.b.get())
 
+class SignedMul(Logic):
+    """
+    Arithmetic Signed Multiplier
+    """
+    def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
+        super().__init__(parent, name)
+        self.a = self.addIn("a", a)
+        self.b = self.addIn("b", b)
+        self.r = self.addOut("r", r)
 
-class Mul(Logic):
+    def propagate(self):
+        from ..helper import IntegerHelper    
+        
+        sa = IntegerHelper.c2_to_signed(self.a.get(), self.a.getWidth())
+        sb = IntegerHelper.c2_to_signed(self.b.get(), self.b.getWidth())
+        mask = (1 << self.r.getWidth()) - 1
+        newValue = (sa * sb) & mask
+        self.r.put(newValue)
+        
+class Div(Logic):
     """
-    Combinational Arithmetic Multiplier
+    Combinational Arithmetic Divider
     """
 
     def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn("a", a)
         self.b = self.addIn("b", b)
         self.r = self.addOut("r", r)
 
     def propagate(self):
-        self.r.put(self.a.get() * self.b.get())
-
+        self.r.put(self.a.get() // self.b.get())
 
-class Div(Logic):
+class Mod(Logic):
     """
-    Combinational Arithmetic Multiplier
+    Combinational Arithmetic Modulo (reminder of div)
     """
 
     def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn("a", a)
         self.b = self.addIn("b", b)
         self.r = self.addOut("r", r)
 
     def propagate(self):
-        self.r.put(self.a.get() // self.b.get())
+        self.r.put(self.a.get() % self.b.get())
 
 
+class SignedDiv(Logic):
+    """
+    Combinational Arithmetic Divider
+    """
+
+    def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
+        super().__init__(parent, name)
+        self.a = self.addIn("a", a)
+        self.b = self.addIn("b", b)
+        self.r = self.addOut("r", r)
+
+        abs_a = self.wire('abs_a', a.getWidth())
+        abs_b = self.wire('abs_b', b.getWidth())
+        
+        Abs(self, 'abs_a', a, abs_a)
+        Abs(self, 'abs_b', b, abs_b)
+        
+        sign_a = self.wire('sign_a')
+        sign_b = self.wire('sign_b')
+        
+        Sign(self, 'sign_a', a, sign_a)
+        Sign(self, 'sign_b', b, sign_b)
+       
+        q = self.wire('q', r.getWidth())        
+        neg_q = self.wire('neg_q', r.getWidth())
+        
+        Div(self, 'div', abs_a, abs_b, q)
+        Neg(self, 'neg', q, neg_q)
+        
+        sign_r = self.wire('sign_r')
+        Xor2(self, 'sign_r', sign_a, sign_b, sign_r) 
+        
+        Mux2(self, 'r', sign_r, q, neg_q, r)        
+        
+
 class Sub(Logic):
     """
-    Arithmetic Add
+    Arithmetic Sub
     """
 
     def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
         super().__init__(parent, name)
         self.a = self.addIn("a", a)
         self.b = self.addIn("b", b)
         self.r = self.addOut("r", r)
 
     def propagate(self):
         mask = (1 << self.r.getWidth()) - 1
         newValue = (self.a.get() - self.b.get()) & mask
         self.r.put(newValue)
 
 
+class SignedSub(Logic):
+    """
+    Arithmetic Sub
+    """
+    
+
+    def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
+        super().__init__(parent, name)
+        self.a = self.addIn("a", a)
+        self.b = self.addIn("b", b)
+        self.r = self.addOut("r", r)
 
+    def propagate(self):
+        from ..helper import IntegerHelper    
+        
+        sa = IntegerHelper.c2_to_signed(self.a.get(), self.a.getWidth())
+        sb = IntegerHelper.c2_to_signed(self.b.get(), self.b.getWidth())
+        mask = (1 << self.r.getWidth()) - 1
+        newValue = (sa - sb) & mask
+        self.r.put(newValue)
+        
 class Counter(Logic):
     """
     Counts up to the value mod and returns to zero
     """
     def __init__(self, parent, name : str, reset:Wire , inc:Wire , q:Wire ):
         super().__init__(parent, name)
         
         from .bitwise import Constant
         from .bitwise import Or2
         from .bitwise import Mux2
         from .storage import Reg
         
-        reset = self.addIn('reset', reset)
-        inc = self.addIn('inc', inc)
+        if not(reset is None):
+            reset = self.addIn('reset', reset)
+        if not(inc is None):
+            inc = self.addIn('inc', inc)
+        
         q = self.addOut('q', q)
     
         one = self.wire('one', q.getWidth())
         zero = self.wire('zero', q.getWidth())
         add = self.wire('add', q.getWidth())
         d = self.wire('d', q.getWidth())
         d1 = self.wire('d1', q.getWidth())
         e_add = self.wire('e_add', 1)
         
         Constant(self, 'one', 1, one)
         Constant(self, 'zero', 0, zero)
         
+        if (inc is None):
+            inc = one
+        if (reset is None):
+            reset = zero
+            
         Mux2(self, 'muxinc', inc, q, add, d1)
         Mux2(self, 'muxreset', reset, d1, zero, d)
 
         #py4hw.Select(self, 'select', [reset, inc], [zero, add], d)
         Or2(self, 'e_add', reset, inc, e_add)
         #py4hw.Mux(self, 'mux', )
         Add(self, 'add', q, one, add)
@@ -246,136 +382,201 @@
         
         for i in range(num):
             shifted = self.wire('shifted{}'.format(i), r.getWidth())
             ShiftRightConstant(self, 'shifted{}'.format(i), a, i, shifted)
             ins.append(shifted)
             
         Mux(self, 'mux', b, ins, r)
+
+class ShiftLeft(Logic):
+    def __init__(self, parent:Logic, name:str, a, b, r):
+        super().__init__(parent, name)
+
+        a = self.addIn('a', a)
+        b = self.addIn('b', b)
+        r = self.addOut('r', r)
+            
+        wb = b.getWidth()
+        
+        num = int(math.pow(2, wb))
+        ins = []
+        
+        for i in range(num):
+            shifted = self.wire('shifted{}'.format(i), r.getWidth())
+            ShiftLeftConstant(self, 'shifted{}'.format(i), a, i, shifted)
+            ins.append(shifted)
+            
+        Mux(self, 'mux', b, ins, r)
         
 class BinaryToBCD(Logic):
     """
     Converts a binary number into BCD digits
     """
     
     def __init__(self, parent, name : str, a: Wire, r:Wire):
+        from ..helper import LogicHelper    
+
         super().__init__(parent, name)
         
         a = self.addIn('a', a)
         r = self.addOut('r', r)
     
-class FPAdder_SP(Logic):
-    
-    def __init__(self, parent:Logic, name:str, a:Wire, b:Wire, r:Wire):
-        super().__init__(parent, name)
+        hlp = LogicHelper(self)
         
-        # This is really cumbersome
-        import sys
-        if not('..' in sys.path):
-            sys.path.append ('..')
+        w = a.getWidth()
+        assert(r.getWidth() % 4 == 0)
+        digits = r.getWidth() // 4 # int(math.ceil(math.log10((2**w)-1)))
+        print('Number of BCD digits:', digits)
+        print('r width:', r.getWidth())
+        
+        assert(r.getWidth() >= (digits*4))
+        
+        ret = []
+        v = a
+        k10 = hlp.hw_constant(4, 10)
+        
+        for i in range(digits):
+            rem = self.wire('mod{}'.format(i), 4)
+            div = self.wire('div{}'.format(i), w)
+            Mod(self, 'mod{}'.format(i), v, k10, rem)
+            Div(self, 'div{}'.format(i), v, k10, div)
+            ret.append(rem)
+            v = div
             
-        import py4hw.helper
-        
-        a = self.addIn('a', a)
-        b = self.addIn('b', b)
-        r = self.addOut('r', r)
-        
-        igt = self.wire('igt')
-        ieq = self.wire('ieq')
-        ilt = self.wire('ilt')
-
-        FPComparator_SP(self, 'cmp', a, b, igt, ieq, ilt, absolute=True)
-        
-        a2 = self.wire('a2', a.getWidth())
-        b2 = self.wire('b2', b.getWidth())
-        
-        Swap(self, 'swap', a, b, ilt, a2, b2)
-        
-        a = a2
-        b = b2
-        
-        sa = self.wire('sa')
-        sb = self.wire('sb')
-        ea = self.wire('ea', 8)
-        eb = self.wire('eb', 8)
-        ma = self.wire('ma', 23)
-        mb = self.wire('mb', 23)
-        
-        Bit(self, 'sa',a, 31, sa)
-        Bit(self, 'sb',b, 31, sb)
-        Range(self, 'ea', a, 30, 23, ea)
-        Range(self, 'eb', b, 30, 23, eb)
-        Range(self, 'ma', a, 22, 0, ma)
-        Range(self, 'mb', b, 22, 0, mb)
-        
-        one = self.wire('one', 1)
-        Constant(self, 'one', 1, one)
-        
-        ma2 = self.wire('ma2', ma.getWidth()+1)
-        mb2 = self.wire('mb2', ma.getWidth()+1)
+        ConcatenateLSBF(self, 'r', ret, r)
         
-        ConcatenateMSBF(self, 'ma2', [one, ma], ma2)
-        ConcatenateMSBF(self, 'mb2', [one, mb], mb2)
-        
-        ma = ma2
-        mb = mb2
-        
-        # Maximum possible shifting is 23 bits (of the mantisa), so
-        # it is enough with 5 bits for ediff
-        # Also we know ediff will be always positive
 
-        ediff = self.wire('ediff', 5)
-        Sub(self, 'ediff', ea, eb, ediff)
-        
-        mb3 = self.wire('mb3', mb.getWidth())
-        
-        ShiftRight(self, 'preshift', mb, ediff, mb3)
+class _FFunction(Logic):
+    """
+    F function described in the paper DOI: 10.1109/TVLSI.2008.2000458
+    """
+    def __init__(self, parent, name : str, a: list, r:Wire):
+        super().__init__(parent, name)
+
+        w = len(a)
+        an = []
         
-        mb = mb3
+        for i in range(w):
+            self.addIn('in{}'.format(i), a[i])
+            ann = self.wire('an{}'.format(i))
+            Not(self, 'an{}'.format(i), a[i], ann)
+            an.append(ann)
+            
+        self.addOut('r', r)
         
-        s_eq = self.wire('s_eq')
-        Equal(self, 's_eq', sa, sb, s_eq)
+        products = []
+        notcount = 0
+        idx = w-1
+        negidx_start = w-2
+        negidx_stop = w-2
+        
+        while (True):
+            prodsig = [a[idx]]
+            #print('positive:', idx, 'negative:', end='')
+            
+            for j in range(negidx_start, negidx_stop, -2):
+                #print(j, end=',')
+                prodsig.append(an[j])
+                
+            #print()
+            prod = self.wire('prod{}'.format(idx))
+            
+            if (len(prodsig) > 1):
+                And(self, 'and{}'.format(idx), prodsig, prod)
+                products.append(prod)
+            else:
+                products.append(prodsig[0])
+                
+            idx -= 2
+            negidx_stop -= 2
+            
+            if (idx < 0):
+                break;
         
-        m_a_plus_b = self.wire('m_a_plus_b', ma.getWidth()+1)
-        m_a_minus_b = self.wire('m_a_minus_b', ma.getWidth()+1)
-        m_b_minus_a = self.wire('m_b_minus_a', ma.getWidth()+1)
+        if (len(products) > 1):
+            Or(self, 'or', products, r)
+        else:
+            Buf(self, 'r', products[0], r)
         
-        Add(self, 'm_a_plus_b', ma, mb, m_a_plus_b)
-        Sub(self, 'm_a_minus_b', ma, mb, m_a_minus_b)
-        Sub(self, 'm_b_minus_a', mb, ma, m_b_minus_a)
+class CountLeadingZeros(Logic):
+    """
+    Count leading zero bits
+    We implement the design described in 
+    Dimitrakopoulos, Giorgos, Kostas Galanopoulos, Christos Mavrokefalidis, 
+    and Dimitris Nikolos. "Low-power leading-zero counting and anticipation 
+    logic for high-speed floating point units." IEEE transactions on very large 
+    scale integration (VLSI) systems 16, no. 7 (2008): 837-850.
+    https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=4539802    
+    DOI: 10.1109/TVLSI.2008.2000458
+    """
+    def __init__(self, parent, name : str, a: Wire, r:Wire, z:Wire):
+        super().__init__(parent, name)
         
-        samb = self.wire('samb')
-        sbma = self.wire('sbma')
+        a = self.addIn('a', a)
+        r = self.addOut('r', r)
+        z = self.addOut('z', z)
+
+        aw = a.getWidth()
+        rw = r.getWidth()
         
-        Sign(self, 'samb', m_a_minus_b, samb)
-        Sign(self, 'sbma', m_b_minus_a, sbma)
+        r_intern_w = int(math.ceil(math.log2(aw)))
+        if (r_intern_w > rw):
+            raise Exception('r with too small for a input')
+            
+        # we must extend the input to a power of 2
+        # if we do that, we should subtract the extra bits from the result
+        a_intern_w = int(math.pow(2, r_intern_w))
+        a_intern = self.wire('a_intern', a_intern_w)
         
+        ZeroExtend(self, 'zexta', a, a_intern)
+            
+        r_intern = self.wire('r_intern', r_intern_w)
         
-        mr = self.wire('mr', m_a_plus_b.getWidth())
-        sr = self.wire('sr')
+        r_preout = self.wire('r_preout', r.getWidth())
         
-        g = py4hw.helper.LogicHelper(self)
-        sel_apb = g.hw_buf(s_eq)
-        sel_amb = g.hw_and2(sa, g.hw_not(sb))
-        sel_bma = g.hw_and2(g.hw_not(sa), sb)
+        # we support bigger than necessary outputs by automatically
+        # zero extending
+        ZeroExtend(self, 'zextr', r_intern, r_preout)
         
-        Select(self, 'select_mr', [sel_apb, sel_amb, sel_bma], [m_a_plus_b, m_a_minus_b, m_b_minus_a], mr)
-        Select(self, 'select_sr', [sel_apb, sel_amb, sel_bma], [sa, sb, sa], sr)
+        # Work with individual a wires
+        a_bits = self.wires('a', a_intern_w, 1)
+        BitsLSBF(self, 'a_bits', a_intern, a_bits)
         
-        # invert result
-        inverted = self.wire('inverted')
-        mr2 = self.wire('mr2', mr.getWidth())
-        Abs(self, 'abs', mr, mr2, inverted)
+        # Work with indidual wires , and concatenate them into the r_intern
+        r_bits = self.wires('r_intern', r_intern_w, 1)
         
-        mr = mr2
+        ConcatenateLSBF(self, 'concat', r_bits, r_intern)
         
-        # invert the sign if necessary
-        sr = g.hw_xor2(inverted, sr)
+        f_bits = a_bits
         
-        # shrink wire
-        mr3 = self.wire('mr3', 23)
-        Buf(self, 'mr3', mr, mr3)
-        mr = mr3
+        #print('len f_bits:', len(f_bits))
         
-        maxe = self.wire('maxe', ea.getWidth())
-        Max2(self, 'maxe', ea, eb, maxe)
+        for i in range(r_intern_w):
+            fvalue = self.wire('f{}'.format(i))
+            _FFunction(self, 'f_{}'.format(i), f_bits, fvalue)
+            Not(self, 'z_{}'.format(i), fvalue, r_bits[i])
+            
+            next_f_bits_w = len(f_bits)//2
+            next_f_bits = self.wires('f{}'.format(i), next_f_bits_w, 1)
+            
+            #print('level', i, next_f_bits_w)
+            for j in range(next_f_bits_w):
+
+                Or2(self, 'o{}_{}'.format(i,j), f_bits[j*2], f_bits[j*2+1], next_f_bits[j])
+            
+            f_bits = next_f_bits
+            
+        # we should end with a single wire in f_bits
+        Not(self, 'not_z', f_bits[0], z)
         
-        ConcatenateMSBF(self, 'final_r', [sr, maxe, mr], r)
+        allZeroK = self.wire('allZeroK', r.getWidth())
+        Constant(self, 'allZeroK', a.getWidth(), allZeroK)
+
+        if (a_intern_w > aw):
+            r_preout2 = self.wire('preout2', rw)
+            extra = self.wire('extra', rw)
+            Constant(self, 'extra', a_intern_w-aw, extra)
+            Sub(self, 'sub', r_preout, extra, r_preout2)
+            r_preout = r_preout2
+
+        Mux2(self, 'final', z, r_preout, allZeroK, r)
+
```

### Comparing `py4hw-0.0.9/py4hw/logic/bitwise.py` & `py4hw-2024.1/py4hw/logic/bitwise.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,21 +40,22 @@
 
         # store inputs/outputs for RTL generation
         self.r = r
         self.ins = lins
         
         num = len(ins)
 
+        if (num == 1):
+            Buf(self, 'and1', ins[0], r)
+            return
+        
         if (num == 2):
             And2(self, 'and2', ins[0], ins[1], r)
             return
             
-        if (num < 3):
-            raise Exception('List should be > 2')
-
         # by now we do an inefficient ladder structure, we should
         # do a more fancy logarithmic design
         
         auxin = lins[0]
         auxout = self.wire('and{}'.format(0), w)
         
         for i in range(num-1):
@@ -150,14 +151,49 @@
         super().__init__(parent, name)
         self.a = self.addIn('a', a)
         self.r = self.addOut('r', r)
 
     def propagate(self):
         self.r.put(self.a.get())
 
+class BidirBuf(Logic):
+    
+    def __init__(self, parent, name: str, pin : Wire , pout : Wire, poe : Wire, bidir : BidirWire):
+        super().__init__(parent, name)
+        
+        self.bidir = self.addInOut('bidir', bidir)
+        self.pin = self.addOut('pin', pin)
+        self.pout = self.addIn('pout', pout)
+        self.poe = self.addIn('poe', poe)
+        
+    def propagate(self):
+        if (self.poe.get() ==1):
+            self.bidir.put(self.pout.get())
+        else:
+            self.pin.put(self.bidir.get())
+
+class BufEnable(Logic):
+    # This is just a way to control set to zero all bits of a signal
+    # depending on an enable signal
+    def __init__(self, parent, name, a, en, r):
+        super().__init__(parent, name)
+        
+        self.a = self.addIn('a', a)
+        self.en = self.addIn('en', en)
+        self.r = self.addOut('r', r)
+   
+        assert(a.getWidth() == r.getWidth())
+    
+        re = self.wire('re', r.getWidth())
+        Repeat(self, 're', en, re)
+        And2(self, 'r', a, re, r)
+        
+    def structureName(self):
+        return 'BufEnable{}'.format(self.a.getWidth())
+    
 
 class Constant(Logic):
     """
     A constant value
     """
 
     def __init__(self, parent: Logic, name: str, value: int, r: Wire):
@@ -165,14 +201,31 @@
         self.value = value
         self.r = self.addOut("r", r)
 
     def propagate(self):
         self.r.put(self.value)
         #print(self.name, '=', self.value)
         
+class Demux(Logic):
+    def __init__(self, parent, name, a, sel, r):
+        super().__init__(parent, name)
+        
+        self.addIn('a', a)
+        self.addIn('sel', sel)
+        
+        assert(2**sel.getWidth() == len(r))
+        
+        ss = self.wires('ss', 2**sel.getWidth(), 1)
+        Decoder(self, 'decoder', sel, ss)
+        
+        for idx, ri in enumerate(r):
+            self.addOut('r{}'.format(idx), ri)
+            
+            BufEnable(self, 'en{}'.format(idx), a, ss[idx], ri)
+            
 class Nand2(Logic):
     """
     Binary Nand
     """
 
     def __init__(self, parent, name: str, a: Wire, b: Wire, r: Wire):
         super().__init__(parent, name)
@@ -249,14 +302,25 @@
         self.a = self.addIn("a", a)
         self.b = self.addIn("b", b)
         self.r = self.addOut("r", r)
 
     def propagate(self):
         self.r.put(self.a.get() | self.b.get())
 
+class OrBits(Logic):
+    def __init__(self, parent, name:str, a: Wire, r: Wire):
+        super().__init__(parent, name)
+        
+        self.addIn('a', a)
+        self.addOut('r', r)
+        
+        ab = self.wires('ab', a.getWidth(), 1)
+        BitsLSBF(self, 'bits', a, ab)
+        Or(self, 'or', ab, r)
+    
 class Or(Logic):
     def __init__(self, parent, name:str, ins, r: Wire):
         super().__init__(parent, name)
         lins = []
         r = self.addOut('r', r)
         w = r.getWidth()
         
@@ -265,21 +329,22 @@
 
         # save inputs/outputs for RTL generation
         self.r = r
         self.ins = lins
         
         num = len(ins)
 
+        if (num == 1):
+            Buf(self, 'or1', ins[0], r)
+            return 
+        
         if (num == 2):
-            Or2(self, 'and2', ins[0], ins[1], r)
+            Or2(self, 'or2', ins[0], ins[1], r)
             return
-            
-        if (num < 3):
-            raise Exception('List should be > 2')
-
+                    
         # by now we do an inefficient ladder structure, we should
         # do a more fancy logarithmic design
         
         auxin = lins[0]
         auxout = self.wire('and{}'.format(0), w)
         
         for i in range(num-1):
@@ -373,14 +438,17 @@
                 auxout = self.wire('and{}'.format(i+1), w)
                 
 
 class Mux(Logic):
     def __init__(self, parent, name: str, sel: Wire, ins, r: Wire):
         super().__init__(parent, name)
         
+        if (sel.getWidth() != int(math.log2(len(ins)))):
+            raise Exception('Invalid length sel bits: {} # ins: {}'.format(sel.getWidth(), int(math.log2(len(ins)))))
+
         sel = self.addIn('sel', sel)
         r = self.addOut('r', r)
 
         lins = []
         for idx, inv in enumerate(ins):
             lins.append(self.addIn('in{}'.format(idx), inv))
         
@@ -391,16 +459,14 @@
             
         # bits contain all the bits from the selection wire
         # which will be the base for creating a logarithmic
         # selection tree
         bits = BitsLSBF.fromWire(self, 'sel', sel)
 
 
-        if (len(bits) != int(math.log2(len(ins)))):
-            raise Exception('Invalid length sel bits: {} # ins: {}'.format(len(bits), int(math.log2(len(ins)))))
             
         fp, ip = math.modf(math.log2(len(ins)))
         
         if (fp != 0):
             raise Exception('Input wires are not a power of 2')
 
         w = len(ins) // 2
@@ -449,15 +515,15 @@
 
         v = self.i.get()
         if (v):
             self.r.put(wp)
         else:
             self.r.put(wf)
 
-
+# deprecated use OneHotMux
 class Select(Logic):
     def __init__(self, parent, name: str, sels:list, ins:list, r: Wire):
         super().__init__(parent, name)
 
         final = []
 
         for idx, sel in enumerate(sels):
@@ -471,16 +537,72 @@
             And2(self, 'and{}'.format(idx), selx, inv, and_sel)
             final.append(and_sel)
 
         self.addOut('r', r)
         Or(self, 'or', final, r)
 
 
+class OneHotMux(Logic):
+    def __init__(self, parent, name: str, sels:list, ins:list, r: Wire):
+        super().__init__(parent, name)
+
+        final = []
 
+        for idx, sel in enumerate(sels):
+            inv = ins[idx]
+            self.addIn('sel{}'.format(idx), sel)
+            self.addIn('in{}'.format(idx), inv)
+            selx = self.wire('selx{}'.format(idx), inv.getWidth())
+            and_sel = self.wire('and_sel{}'.format(idx), inv.getWidth())
+
+            Repeat(self, 'sel{}'.format(idx), sel, selx)
+            And2(self, 'and{}'.format(idx), selx, inv, and_sel)
+            final.append(and_sel)
+
+        self.addOut('r', r)
+        Or(self, 'or', final, r)
+
+
+class OneHotDemux(Logic):
+    def __init__(self, parent, name: str, sels:list, a:Wire, outs: list):
+        super().__init__(parent, name)
+
+        final = []
+
+        a = self.addIn('a', a)
+
+        for idx, sel in enumerate(sels):
+            self.addIn('sel{}'.format(idx), sel)
+            self.addOut('out{}'.format(idx), outs[idx])
+            
+            selx = self.wire('selx{}'.format(idx), a.getWidth())
+
+            Repeat(self, 'sel{}'.format(idx), sel, selx)
+            And2(self, 'and{}'.format(idx), selx, a, outs[idx])
+            
+        
+class SelectDefault(Logic):
+    def __init__(self, parent, name, sels, ins, default, r):
+        super().__init__(parent, name)
+        
+        self.addIn('default', default)
+        self.addOut('r', r)
         
+        nextoutput = r
+        
+        for idx, sel in enumerate(sels):
+            inv = ins[idx]
+            self.addIn('sel{}'.format(idx), sel)
+            self.addIn('in{}'.format(idx), inv)
+            previnput = self.wire('t{}'.format(idx), r.getWidth())
+            Mux2(self, 'mux{}'.format(idx), sel, previnput, inv, nextoutput)
+            
+            nextoutput = previnput
+            
+        Buf(self, 'buf', default, previnput)
 
 
 
 class Decoder(Logic):
     """
     A decoder
     """
@@ -553,32 +675,53 @@
                 parts.append(nbit)
             else:
                 parts.append(lbits[i])
 
         And(self, 'prod', parts, r)
         
 
+class SumOfMinterms(Logic):
+    def __init__(self, parent, name, a, minterms:list, r):
+        super().__init__(parent, name)
+        
+        self.addIn('a', a)
+        self.addOut('r', r)
+        
+        bits = self.wires('bits', a.getWidth(), 1)
+        BitsLSBF(self, 'bits', a, bits)
+        
+        acum = []
+        for idx, minterm in enumerate(minterms):
+            v = self.wire('s{}'.format(idx))
+            
+            Minterm(self, 'minterm{}'.format(idx), bits, minterm, v)
+            acum.append(v)
+            
+        Or(self, 'sum', acum, r)
+        
 class ConcatenateMSBF(Logic):
     """
     Concatenate wires circuit in MSBF order
     """
     def __init__(self, parent: Logic, name: str, ins:list, r: Wire):
         super().__init__(parent, name)
 
+        ind_w = []
         total_w = 0
         max_w = r.getWidth()
         
         self.ins = []
 
         for idx, item in enumerate(ins):
             self.ins.append(self.addIn('in{}'.format(idx), item))
             total_w += item.getWidth()
+            ind_w.append(item.getWidth())
 
         if (total_w > max_w):
-            raise Exception('Combined input widths larger than result width {}>{}'.format(total_w, max_w))
+            raise Exception('Combined input widths {} larger than result width {}>{}'.format(ind_w, total_w, max_w))
             
         self.r = self.addOut('r', r)
 
     def propagate(self):
         value = 0
         last = 0
         for idx, item in enumerate(self.ins):
@@ -630,7 +773,82 @@
 
     def propagate(self):
         value = self.a.get()
         mask = (1 << (self.high - self.low + 1)) - 1
         newvalue = (value >> self.low) & mask
         self.r.put(newvalue)
 
+class Digit7Segment(Logic):
+    def __init__(self, parent, name, v, led):
+        super().__init__(parent, name)
+        
+        assert(led.getWidth() == 7)
+        
+        self.addIn('v', v)
+        self.addOut('led', led)
+        
+        
+        a_minterms = [0,2,3,5,6,7,8,9,0xA,0xC,0xE,0xF]
+        b_minterms = [0,1,2,3,4,7,8,9,0xA,0xd]
+        c_minterms = [0,1,3,4,5,6,7,8,9,0xA,0xb,0xd]
+        d_minterms = [0,2,3,5,6,8,0xb,0xC,0xd,0xE]
+        e_minterms = [0,2,6,8,0xA,0xb,0xC,0xd,0xE,0xF]
+        f_minterms = [0,4,5,6,8,9,0xA,0xb,0xC,0xE,0xF]
+        g_minterms = [2,3,4,5,6,8,9,0xA,0xb,0xd,0xE,0xF]
+        
+        
+        a = self.wire('a')
+        b = self.wire('b')
+        c = self.wire('c')
+        d = self.wire('d')
+        e = self.wire('e')
+        f = self.wire('f')
+        g = self.wire('g')
+        
+        na = self.wire('na')
+        nb = self.wire('nb')
+        nc = self.wire('nc')
+        nd = self.wire('nd')
+        ne = self.wire('ne')
+        nf = self.wire('nf')
+        ng = self.wire('ng')
+        
+        ConcatenateLSBF(self, 'led', [a,b,c,d,e,f,g], led)
+        
+        SumOfMinterms(self, 'a', v, a_minterms, a)
+        SumOfMinterms(self, 'b', v, b_minterms, b)
+        SumOfMinterms(self, 'c', v, c_minterms, c)
+        SumOfMinterms(self, 'd', v, d_minterms, d)
+        SumOfMinterms(self, 'e', v, e_minterms, e)
+        SumOfMinterms(self, 'f', v, f_minterms, f)
+        SumOfMinterms(self, 'g', v, g_minterms, g)
+        
+class PriorityEncoder(Logic):
+    def __init__(self, parent, name, a, r, inc_priority=True):
+        from ..helper import LogicHelper
+        super().__init__(parent, name)
+        assert(len(a) == len(r))
+
+        # Make a copy so that reverse does not affect the original list
+        a = a.copy()
+        r = r.copy()
+        
+        # It the priority is decreasing, the a[0] is the more priorized
+        # Otherwise is the higher index
+        if (inc_priority):
+            a.reverse()
+            r.reverse()
+        
+        hlp = LogicHelper(self)
+        
+        last = None
+        
+        for i in range(len(a)):
+            self.addIn('a{}'.format(i), a[i])
+            self.addOut('r{}'.format(i), r[i])
+            
+            if (last is None):
+                Buf(self, 'r{}'.format(i), a[i], r[i])
+                last = hlp.hw_buf(a[i])
+            else:
+                And2(self, 'r{}'.format(i), a[i], hlp.hw_not(last), r[i])
+                last = hlp.hw_or2(last, a[i])
```

### Comparing `py4hw-0.0.9/py4hw/logic/relational.py` & `py4hw-2024.1/py4hw/logic/relational.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,26 +30,44 @@
             for j in range(num):
                 if (i != j):
                     rp = self.wire('eq_{}_{}'.format(i,j), 1)
                     Equal(self, 'eq_{}_{}'.format(i,j), lins[i], lins[j], rp)
                     checks.append(rp)
 
         Or(self, 'anyEqual', checks, r)
+
+class NotEqualConstant(Logic):
+    """
+    An Equal comparator circuit
+    """
+
+    def __init__(self, parent, name: str, a: Wire, v: int, r: Wire):
+        super().__init__(parent, name)
+
+        from .bitwise import Not
+
+        self.addIn("a", a)
+        self.addOut("r", r)
+        
+        eq = self.wire('eq')
+        EqualConstant(self, 'eq', a, v, eq)
+        Not(self, 'r', eq, r)
                 
 class EqualConstant(Logic):
     """
     An Equal comparator circuit
     """
 
     def __init__(self, parent, name: str, a: Wire, v: int, r: Wire):
         super().__init__(parent, name)
 
         from .bitwise import BitsLSBF
         from .bitwise import Minterm
         from .bitwise import Buf
+        from .bitwise import Not
 
         # we save the values for Verilog generation
         self.a = self.addIn("a", a)
         self.r = self.addOut("r", r)
         self.v = v
 
         w = a.getWidth()
@@ -58,15 +76,15 @@
             # very simple case
             if (v == 0):
                 Not(self, 'buf', a, r)
             else:
                 Buf(self, 'not', a, r)
                 
         else:
-            bits = self.wires('b', a.getWidth(), 1)
+            bits = self.wires('b', a.getWidth(), 1)   
             BitsLSBF(self, "bits", a, bits)
             Minterm(self, 'm{}'.format(v), bits, v, r)
 
 
 
 class Equal(Logic):
     """
@@ -380,8 +398,79 @@
         swap = self.addIn('swap', swap)
         ra = self.addOut('ra', ra)
         rb = self.addOut('rb', rb)
         
         Mux2(self, 'muxa', swap, a, b, ra)
         Mux2(self, 'muxb', swap, b, a, rb)
         
+
+class FixedPointComparator(Logic):
+    """
+    A Greater Than, Equal and Less Than comparator circuit
+    """
+
+    def __init__(self, parent:Logic, name: str, a: Wire, af, b: Wire, bf, gt: Wire, eq: Wire, lt: Wire):
+        """
+        Constructor of the comparator circuit
+
+        Parameters
+        ----------
+        parent : Logic
+            parent circuit.
+        name : str
+            instance name.
+        a : Wire
+            operand a.
+        b : Wire
+            operand b.
+        gt : Wire
+            1 if a > b.
+        eq : Wire
+            1 if a == b.
+        lt : Wire
+            1 if a < b.
+
+        Returns
+        -------
+        the object.
+
+        """
+        
+        from .bitwise import Equal
+        from .bitwise import And2
+        from .bitwise import Not
+        from .bitwise import Mux2
+        from .arithmetic_fxp import FixedPointSub
+        from .arithmetic_fxp import FixedPointSign
+
+        super().__init__(parent, name)
+        
+        if (a.getWidth() != b.getWidth()):
+            raise Exception('a and b must have equal width')
+            
+        a = self.addIn("a", a)
+        b = self.addIn("b", b)
+        gt = self.addOut("gt", gt)
+        eq = self.addOut("eq", eq)
+        lt = self.addOut("lt", lt)
+
+        sub = Wire(self, "sub", a.getWidth())
+        notLT = Wire(self, "nLT", 1)
+        notEQ = Wire(self, "nEQ", 1)
+
+        FixedPointSub(self, "Comparison", a, af, b, bf, sub, af)
+
+        # LT
+        if (not(lt is None)):
+            FixedPointSign(self, "LessThan", sub, af, lt)
+
+        # EQ
+        if (not(eq is None)):
+            EqualConstant(self, "Equal", sub, 0, eq)
+
+        # GT
+        if (not(gt is None)):
+            Not(self, "nLT", lt, notLT)
+            Not(self, "nEQ", eq, notEQ)
+            And2(self, "GT", notEQ, notLT, gt)
+
```

### Comparing `py4hw-0.0.9/py4hw/logic/simulation.py` & `py4hw-2024.1/py4hw/logic/simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,18 +11,33 @@
 
 import numpy as np
 import tkinter
 import tkinter.font
 from tkinter import *
 from tkinter import ttk
     
+class FieldInspector:
+    def __init__(self, obj, field):
+        self.obj = obj
+        self.field = field
+        
+    def getFormat(self):
+        return '{}'
+    
+    def get(self):
+        return getattr(self.obj, self.field)
+    
+    def getFullPath(self):
+        return self.obj.getFullPath() + '/' + self.field
+        
 class Waveform(Logic):
     def __init__(self, parent, name, wires):
         """
-        
+        Collects the progress of signals along the time.
+        We try to reduce data by avoiding data duplication.
 
         Parameters
         ----------
         parent : TYPE
             DESCRIPTION.
         name : TYPE
             DESCRIPTION.
@@ -31,46 +46,83 @@
 
         Returns
         -------
         None.
 
         """
         super().__init__(parent, name)
+        
+        # wires contain all the elements of the input list, there might be repeatitions
         self.wires = wires if isinstance(wires, list) else [wires]
+        self.format = []
         self.data = {}  # this is a dictionary of obj (wire or port) -> data, list of wire values 
 
+        self.uniqueWires = []
+        
         for x in self.wires:
+            
             if isinstance(x, Wire):
-                self.addIn(x.name, x)
+                w = x
+                if not(x in self.uniqueWires):
+                    self.addIn(x.name, x)
+                    self.uniqueWires.append(x)
+                    self.data[x] = []            
             elif isinstance(x, InPort) or isinstance(x, OutPort):
                 w = x.wire
                 if (w is None):
                     raise Exception('Wire is null for port', x.getFullPath())
-                self.addIn(w.name, w)
+                if not (w in self.uniqueWires):
+                    self.addIn(w.name, w)
+                    self.uniqueWires.append(w)
+                    self.data[w] = []     
+            elif isinstance(x, FieldInspector):
+                w = None
+                if not(x in self.uniqueWires):
+                    self.uniqueWires.append(x)
+                    self.data[x] = []                                                
             else:
-                raise Exception('Unsupported object class to watch ' + type(x))
+                raise Exception('Unsupported object class to watch: {}'.format(type(x)))
                 
-            self.data[x] = []            
+
+            if isinstance(x, FieldInspector):
+               self.format.append(x.getFormat()) 
+            elif (w.getWidth() == 1):
+                self.format.append('')
+            else:
+                self.format.append('{:X}')
 
     @staticmethod
     def getwire(x):
         if isinstance(x, Wire):
             w = x
         elif isinstance(x, InPort) or isinstance(x, OutPort):
             w = x.wire
         else:
             raise Exception('Object is not wire {}'.format(x))
             
         return w
     
+    def clear(self):
+        for key in self.data.keys():
+            self.data[key] = []
+        
+        
     def clock(self):
-        for x in self.wires:
-            w = Waveform.getwire(x)
+        # Data is indexed by wire (or field inspector) to avoid repeats
+        # For ports, the value used for x will be its wire
+        for x in self.uniqueWires:
+            if isinstance(x, FieldInspector):
+                self.data[x].append(x.get())
+            else:
+                w = Waveform.getwire(x)
                 
-            self.data[x].append(w.get())
+                if not(w in self.data):
+                    raise Exception('Wire {}/{} not in data list {}'.format(x, w, self.data.keys()))
+                    
+                self.data[w].append(w.get())
             
     def getDict(self):
         return self.data
 
     def draw(self):
         import matplotlib.pyplot as plt
         fig, axs = plt.subplots(len(self.data.keys())+1, sharex=True)
@@ -86,38 +138,88 @@
         
         for idx, x in enumerate(self.wires):
            axs[idx+1].step(t, self.data[x], linewidth=2, where='post')
            axs[idx+1].set_ylabel(x.name, rotation=0)
         
         return fig, axs
     
-    def draw_wavedrom(self):
+    def draw_wavedrom(self, shortNames=False):
+        """
+        
+
+        Parameters
+        ----------
+        shortNames : bool, optional
+            Indicates that the names of the wires should be short (instead of the full
+            path). The default is False.
+
+        Returns
+        -------
+        TYPE
+            a widget.
+
+        """
         import nbwavedrom as wave
-        return wave.draw(self.get_wavedrom())
+        return wave.draw(self.get_wavedrom(shortNames))
     
-    def get_wavedrom(self):
+    
+    
+    def get_wavedrom(self, shortNames=False):
+        """
+        
+
+        Parameters
+        ----------
+        shortNames : TYPE, optional
+            DESCRIPTION. The default is False.
+
+        Returns
+        -------
+        ret : TYPE
+            DESCRIPTION.
+
+        """
+        
         signals = [{"name": "clk", 'wave': 'P'}]
         
-        for obj in self.wires:
-            w = Waveform.getwire(obj)
+        for idx, obj in enumerate(self.wires):
+            if (isinstance(obj, FieldInspector)):
+                w = obj
+                ww = -1
+            else:
+                w = Waveform.getwire(obj)
+                ww = w.getWidth()
+                
+            fmt = self.format[idx]
             wavedata = 'x'
+            wavedatadata = []
             
-            data = self.data[obj]
+            data = self.data[w]
             last = 'x'
             numclks = len(data)
             for i in range(numclks):
                 v = data[i]
                 if (v != last):
-                    wavedata += '{}'.format(v)
+                    if (ww == 1):
+                        wavedata += '{}'.format(v)
+                    else:
+                        wavedata += '{}'.format(2)
+                        wavedatadata.append(fmt.format(v))
                 else:
                     wavedata += '.'
                 last = v
                     
             wavedata += 'x'
-            signals.append({'name': obj.getFullPath(), 'wave':wavedata})
+            
+            if (shortNames):
+                name = obj.name
+            else:
+                name = obj.getFullPath()
+                
+            signals.append({'name': name, 'wave':wavedata, 'data':wavedatadata})
 
         wavedata = 'P'
         for i in range(numclks):
             wavedata += '.'
         wavedata += 'x'
 
         signals[0]['wave'] = wavedata
@@ -265,15 +367,15 @@
         
         hclock = self.hclock
         vsig = 15
         vtext = 7
         htrans = 3
         
         for idx, wav in enumerate(wd.keys()):
-            if isinstance(wav, py4hw.Wire):
+            if isinstance(wav, Wire):
                 w = wav.getWidth()
             else:
                 w = wav.wire.getWidth()
                 
             data = wd[wav]
             
             if (w == 1):
```

### Comparing `py4hw-0.0.9/py4hw/rtl_generation.py` & `py4hw-2024.1/py4hw/rtl_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,39 @@
 """
 
 from .base import *
 from .logic import *
 from .logic.bitwise import *
 from .logic.storage import *
 from .schematic_symbols import *
+from .transpilation.python2verilog_transpilation import *
 
 def getVerilogModuleName(obj:Logic, noInstanceNumber=False):
+    '''
+    Returns the module name of an object.
+    Logic classes can provide their module name by implementing the method structureName,
+    if it is not provided the structure is unique for every instance, hence the number
+    of structures is significantly increase (which is generally bad for reading)
+
+    Parameters
+    ----------
+    obj : Logic
+        DESCRIPTION.
+    noInstanceNumber : TYPE, optional
+        DESCRIPTION. The default is False.
+
+    Returns
+    -------
+    str : TYPE
+        DESCRIPTION.
+
+    '''
+    if (has_method(obj, 'structureName')):
+        return obj.structureName()
+    
     str = type(obj).__name__  
     if (not(noInstanceNumber)):
         sid = hex(id(obj))
         str += "_" +sid[2:] 
         
     return str
 
@@ -117,19 +140,23 @@
     for inp in obj.inPorts:
         ret[inp.wire]= getPortName(inp) 
         link = ","
 
     for outp in obj.outPorts:
         ret[outp.wire] = getPortName(outp) 
         
+    for outp in obj.inOutPorts:
+        ret[outp.wire] = getPortName(outp) 
+        
     return ret
     
 def collectPortWires( obj:Logic):
     """
-    Return the wires of the object interface
+    Return the wires of the object interface.
+    @todo where is this used ?
 
     Parameters
     ----------
     obj : Logic
         DESCRIPTION.
 
     Returns
@@ -142,14 +169,18 @@
     for inp in obj.inPorts:
         if (not(inp.wire is None)):
             ret.append(inp.wire)
 
     for outp in obj.outPorts:
         if (not(outp.wire is None)):
             ret.append(outp.wire)
+            
+    for outp in obj.inOutPorts:
+        if (not(outp.wire is None)):
+            ret.append(outp.wire)
 
     return ret
 
 def collectLocalWires(obj:Logic):
     """
     Collects local wires
 
@@ -183,29 +214,44 @@
     return name
     
 def getPortName(p):
     return getValidVerilogName(p.name)
 
 def getWireName(scope:Logic, w:Wire):
     wNames = getWireNames(scope)
+    
+    if not(w in wNames.keys()):
+        print('ERROR: wire ', w.getFullPath(), 'not in the wires of ', scope.getFullPath()) 
+        for w2 in wNames.keys():
+            print(wNames[w2], w2 )
+        raise Exception('Wire wire {} not in the wires of {}'.format( w.getFullPath(), scope.getFullPath())) 
+        
     return wNames[w]
 
 def getParentWireName(child:Logic, w:Wire):
     wNames = getWireNames(child.parent)
     return wNames[w]
     
 def InlineConstant(obj:Logic):
     return "assign {} = {};\n".format(getParentWireName(obj, obj.r) + getWidthInfo(obj.r), obj.value)
 
 def InlineNot(obj:Logic):
     return "assign {} = ~{};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a))
 
+def InlineBidirBuf(obj:Logic):
+    str =  "assign {} = {};\n".format(getParentWireName(obj, obj.pin), getParentWireName(obj, obj.bidir))
+    str += "assign {} = ({}) ? {} : {}'bZ;\n".format(getParentWireName(obj, obj.bidir), getParentWireName(obj, obj.poe), getParentWireName(obj, obj.pout), obj.bidir.getWidth())
+    return str
+
 def InlineBuf(obj:Logic):
     return "assign {} = {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a))
 
+def InlineSignExtend(obj:Logic):
+    return "assign {} = {{ {{ {} {{ {}[{}] }} }}, {} }};\n".format(getParentWireName(obj, obj.r), obj.r.getWidth() - obj.a.getWidth(),  getParentWireName(obj, obj.a), obj.a.getWidth()-1, getParentWireName(obj, obj.a))
+
 def InlineZeroExtend(obj:Logic):
     return "assign {} = {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a))
     
 def InlineAnd2(obj:Logic):
     return "assign {} = {} & {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
 
 def InlineNand2(obj:Logic):
@@ -222,17 +268,23 @@
 
 def InlineMux2(obj:Logic):
     return "assign {} = ({})? {} : {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.sel), getParentWireName(obj, obj.sel1) , getParentWireName(obj, obj.sel0))
 
 def InlineAdd(obj:Logic):
     return "assign {} = {} + {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
 
+def InlineMul(obj:Logic):
+    return "assign {} = {} * {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
+
 def InlineDiv(obj:Logic):
     return "assign {} = {} / {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
 
+def InlineMod(obj:Logic):
+    return "assign {} = {} % {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
+
 def InlineSub(obj:Logic):
     return "assign {} = {} - {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a) , getParentWireName(obj, obj.b))
 
 def InlineEqualConstant(obj:Logic):
     return "assign {} = ({} == {})? 1 : 0;\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a), obj.v )
 
 def InlineRange(obj:Logic):
@@ -276,20 +328,36 @@
         str += link + "{}".format(getParentWireName(obj, obj.i))
         link = ','
     str += '};\n'
     
     return str
 
 def InlineConcatenateMSBF(obj:Logic):
-    str = ""
+    str = '' # "# MSBF \n"
     w = len(obj.ins)
     if (w == 1):
         return "assign {} = {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.ins[0]))
 
-    str = 'assign {} ='.format(getParentWireName(obj, obj.r))
+    str += 'assign {} ='.format(getParentWireName(obj, obj.r))
+    
+    link = '{'
+    for i in range(w):
+        str += link + "{}".format(getParentWireName(obj, obj.ins[i]))
+        link = ','
+    str += '};\n'
+    
+    return str
+
+def InlineConcatenateLSBF(obj:Logic):
+    str = '' # "# LSBF \n"
+    w = len(obj.ins)
+    if (w == 1):
+        return "assign {} = {};\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.ins[0]))
+
+    str += 'assign {} ='.format(getParentWireName(obj, obj.r))
     
     link = '{'
     for i in range(w):
         str += link + "{}".format(getParentWireName(obj, obj.ins[i]))
         link = ','
     str += '};\n'
     
@@ -321,17 +389,20 @@
         link = "|";
     str += ");\n"
     return str
 
 def InlineEqual(obj:Logic):
     return "assign {} = ({} == {})? 1:0;\n".format(getParentWireName(obj, obj.r), getParentWireName(obj, obj.a), getParentWireName(obj, obj.b))
 
+def InlineVerilogCommnent(obj:Logic):
+    return '// {}\n'.format(obj.comment)
+    
 def BodyReg(obj:Logic):
     clkname = getObjectClockDriver(obj).name
-    str = "reg "+getWidthInfo(obj.q) + " rq = 0;\n"
+    str = "reg "+getWidthInfo(obj.q) + " rq = {};\n".format(obj.reset_value)
     str += "always @(posedge {})\n".format(clkname)
     close = ""
     if not(obj.r is None):
         str += "if (r == 1)\n"
         str += "begin\n"
         str += "   rq <= 0;\n"
         str += "end\n";
@@ -366,73 +437,125 @@
     def __init__(self, obj:Logic):
         #print('Testing Verilog Generation')
         self.obj = obj
         
         self.inlinablePrimitives = {}
         
         self.inlinablePrimitives[Add] = InlineAdd
+        
         self.inlinablePrimitives[And2] = InlineAnd2
         self.inlinablePrimitives[And] = InlineAnd
-        self.inlinablePrimitives[Buf] = InlineBuf
+        self.inlinablePrimitives[BidirBuf] = InlineBidirBuf
         self.inlinablePrimitives[Bit] = InlineBit
         self.inlinablePrimitives[BitsLSBF] = InlineBitsLSBF
         self.inlinablePrimitives[BitsMSBF] = InlineBitsMSBF
+        self.inlinablePrimitives[Buf] = InlineBuf
         self.inlinablePrimitives[ConcatenateMSBF] = InlineConcatenateMSBF
+        self.inlinablePrimitives[ConcatenateLSBF] = InlineConcatenateLSBF
         self.inlinablePrimitives[Constant] = InlineConstant
         self.inlinablePrimitives[Div] = InlineDiv
         self.inlinablePrimitives[Equal] = InlineEqual
         self.inlinablePrimitives[EqualConstant] = InlineEqualConstant
+        self.inlinablePrimitives[Mod] = InlineMod
+        self.inlinablePrimitives[Mul] = InlineMul
+        self.inlinablePrimitives[Mux2] = InlineMux2
         self.inlinablePrimitives[Nand2] = InlineNand2
         self.inlinablePrimitives[Not] = InlineNot
         self.inlinablePrimitives[Nor] = InlineNor
         self.inlinablePrimitives[Nor2] = InlineNor2
         self.inlinablePrimitives[Or] = InlineOr
         self.inlinablePrimitives[Or2] = InlineOr2
-        self.inlinablePrimitives[Mux2] = InlineMux2
         self.inlinablePrimitives[Sub] = InlineSub
-        self.inlinablePrimitives[Xor2] = InlineXor2
         self.inlinablePrimitives[Range] = InlineRange
         self.inlinablePrimitives[Repeat] = InlineRepeat
+        self.inlinablePrimitives[SignExtend] = InlineSignExtend
         self.inlinablePrimitives[ZeroExtend] = InlineZeroExtend
+        self.inlinablePrimitives[VerilogComment] = InlineVerilogCommnent
+        self.inlinablePrimitives[Xor2] = InlineXor2
         
         self.providingBody = {}
         
         self.providingBody[Reg] = BodyReg 
         self.providingBody[GatedClock] = BodyGatedClock
         
-    def getVerilogForHierarchy(self, obj=None, noInstanceNumberInTopEntity=False):
+    def getVerilogForHierarchy(self, obj=None, noInstanceNumberInTopEntity=True, forceName=None):
         """
         Generates Verilog for all entities of the object hierarchy
 
         Returns
         -------
-        None.
+        An string with the Verilog for the Hierarchy.
 
         """
+        
+        self.created_structures = []
+        return self._getVerilogForHierarchy(obj, noInstanceNumberInTopEntity, forceName)
+    
+    def _getVerilogForHierarchy(self, obj=None, noInstanceNumberInTopEntity=True, forceName=None):
+        
+        
         if (obj is None):
             obj = self.obj
+        
+        #print('generating {}'.format(obj.getFullPath()))
             
-        str = self.getVerilog(obj, noInstanceNumber = noInstanceNumberInTopEntity)
+        str = self._getVerilog(obj, noInstanceNumber = noInstanceNumberInTopEntity, forceName=forceName)
         
         for child in obj.children.values():
-            if (not(self.isInlinable(child))):
+            if (self.isInlinable(child)):
+                #print('inlining {}'.format(child.name))
+                pass
+            else:
                 # skip inlinable modules from verilog generation
-                str += "\n"
-                str += self.getVerilogForHierarchy(child, noInstanceNumberInTopEntity=False)
+                part = self._getVerilogForHierarchy(child, noInstanceNumberInTopEntity=False)
+                
+                if len(part) > 0:
+                    str += "\n"
+                    str += part
 
         return str        
         
-    def getVerilog(self, obj=None, noInstanceNumber=False):
+    def getVerilog(self, obj=None, noInstanceNumber=False, forceName=None):
+        '''
+        Create Verilog for a module
+
+        Parameters
+        ----------
+        obj : TYPE, optional
+            DESCRIPTION. The default is None.
+        noInstanceNumber : TYPE, optional
+            DESCRIPTION. The default is False.
+
+        Returns
+        -------
+        str : TYPE
+            DESCRIPTION.
+
+        '''
+        self.created_structures = []
+        return self._getVerilog(obj, noInstanceNumber, forceName)
+    
+    def _getVerilog(self, obj=None, noInstanceNumber=False, forceName=None):
+        
         str = "// This file was automatically created by py4hw RTL generator\n"
         
         if (obj is None):
             obj = self.obj
             
+        # check if structure was already generated
+        
+        if not(forceName is None):
+            structure_name = forceName
+        else:
+            structure_name = getVerilogModuleName(obj, noInstanceNumber=noInstanceNumber)
+        
+        if (structure_name in self.created_structures):
+            return ''
             
-        str += self.createModuleHeader(obj, noInstanceNumber=noInstanceNumber)
+        str += self.createModuleHeader(obj, structure_name)
         
         localWires = collectLocalWires(obj)
         wireNames = getWireNames(obj)
         
         for wire in localWires:
             name = wireNames[wire]
             ww = wire.getWidth()
@@ -458,14 +581,16 @@
 
         else:
             # structural circuit
             str += self.createModuleInstances(obj)
         
         str += "endmodule\n"
         
+        self.created_structures.append(structure_name)
+        
         return str
         
     def anyClockableDescendant(self, obj:Logic):
         """
         Checks it any of the descendants of obj is clockable
 
         Parameters
@@ -483,41 +608,45 @@
         
         for child in obj.children.values():
             if (self.anyClockableDescendant(child)):
                 return True
             
         return False
         
-    def createModuleHeader(self, obj:Logic, noInstanceNumber=None):
-        str = "module " + getVerilogModuleName(obj, noInstanceNumber=noInstanceNumber) + " (\n\t"
+    def createModuleHeader(self, obj:Logic, structureName):
+        str = "module " + structureName + " (\n\t"
 
         link = ""
         
         if (isinstance(obj, GatedClock)):
             drv = obj.drv
             str += link + "input clk_in".format(drv.base.name)
             link = ",\n\t"
             str += link + "output clk_out".format(drv.name)
             
         reg = ""
-        if (obj.isClockable() and not(self.isProvidingBody(obj))):
+        if ((obj.isClockable() or obj.isPropagatable()) and not(self.isProvidingBody(obj))):
             reg = " reg "
         
         if (self.anyClockableDescendant(obj)):
             clkname = getObjectClockDriver(obj).name
             str += "input {}".format(clkname)
             link = ",\n\t"
         
         for inp in obj.inPorts:
             str += link +  "input " + getWidthInfo(inp.wire) + " " + getPortName(inp)+ ""
             link = ",\n\t"
 
         for outp in obj.outPorts:
             str += link + "output " + reg + getWidthInfo(outp.wire) + " " + getPortName(outp)+ ""
             link = ",\n\t"
+
+        for outp in obj.inOutPorts:
+            str += link + "inout " + reg + getWidthInfo(outp.wire) + " " + getPortName(outp)+ ""
+            link = ",\n\t"
             
         str += ");\n"
         
         return str
     
 
     
@@ -532,58 +661,93 @@
             return False
         
         return True
     
     def isProvidingBody(self, obj:Logic):
         # if (not(obj.isPrimitive())):
         #     return False
+
+        if (has_method(obj, 'verilogBody')):
+            return True
         
         try:
             ret = self.providingBody[type(obj)]
         except:
             return False
         
         return True
 
     def inlinePrimitive(self, obj:Logic):
         ret = self.inlinablePrimitives[type(obj)]
         return ret(obj)
 
     def provideBody(self, obj:Logic):
+
+        if (has_method(obj, 'verilogBody')):
+            return obj.verilogBody()
+
         ret = self.providingBody[type(obj)]
         return ret(obj)
         
     def createModuleInstances(self, obj:Logic):
+        '''
+        Instantiate the child instances of the module
+
+        Parameters
+        ----------
+        obj : Logic
+            DESCRIPTION.
+
+        Returns
+        -------
+        str
+            The Verilog of sub-circuit instantiation.
+
+        '''
         str = "\n"
         
         for child in obj.children.values():
-            
             if (self.isInlinable(child)):
+                #print('create inlinable instance {}'.format(child.name))
+                #print('>>', self.inlinePrimitive(child))
+
                 str += self.inlinePrimitive(child)
             else:
                 str += self.instantiateStructural(child)
 
         return str;
 
     def instantiateStructural(self, child:Logic):
+        parent = child.parent
         str = getVerilogModuleName(child) + " " +  getInstanceName(child)
         str += "("
         link = ""
         
         if (isinstance(child, GatedClock)):
             # ClockGate elements are special
             drv:ClockDriver = child.drv
             str += link + ".clk_in({})".format(drv.base.name)
             link = ","
             str += link + ".clk_out({})".format(drv.name)
             
         elif (self.anyClockableDescendant(child)):
             # Clock is an implicit parameter
-            clkname = getObjectClockDriver(child).name
-            str += link + ".{}({})".format(clkname, clkname)
+            drv:ClockDriver = getObjectClockDriver(child)
+            clkname = drv.name
+            if (drv.wire is None):
+                raise Exception('None clk driver wire for', clkname, child.getFullPath())
+                
+            parentDrv:ClockDriver = getObjectClockDriver(child.parent)
+            
+            if (drv.wire == parentDrv.wire):
+                wirename = clkname
+            else:
+                wirename = getWireName(parent, drv.wire)
+                
+            str += link + ".{}({})".format(clkname, wirename)
             link = ","
         
 
         # get the wire names from the instantiator
         wireName = getWireNames(child.parent)
         
         for inp in child.inPorts:
@@ -603,56 +767,51 @@
             if (not(outp.wire in wireName)):
                 raise Exception('Output port wire {} not part of the wires of the parent {}'.format(outp.wire.getFullPath(), child.parent.getFullPath()))
 
             str += link + "." + getPortName(outp) + "("+wireName[outp.wire]+")"
  
             link = ","
         
+        for outp in child.inOutPorts:
+            if (outp.wire is None):
+                raise Exception('Input/Output port {} from {} not connected to any wire'.format(outp.name, child.getFullPath()));
+
+            if (not(outp.wire in wireName)):
+                raise Exception('Input/Output port wire {} {} not part of the wires of the parent {}'.format(outp.wire.getFullPath(), outp.wire, child.parent.getFullPath()))
+
+            str += link + "." + getPortName(outp) + "("+wireName[outp.wire]+")"
+ 
+            link = ","
+            
         str += ");\n"
 
         return str                
     
     
     def generateCodeFromClock(self, obj:Logic):
         str = "// Code generated from clock method\n"
-        clkname = getObjectClockDriver(obj).name
         
-        tr = Python2VerilogTranspiler(obj, 'clock')
+        tr = Python2VerilogTranspiler(obj)
         
-        transpiled = tr.transpile() ;
-        
-        str += "// local declarations\n"
-        str += tr.getExtraDeclarations() + "\n";
-        str += "// sequential process\n"
-        str += "always @(posedge {})\n".format(clkname)
-        str += "begin\n"
-        str += transpiled + "\n"
-        str += "end\n"
+        node = tr.transpileSequential()
+        str += tr.toVerilog(node)
         
-        str += "\n"
+        str = tr.format(str)
         
         return str
 
     def generateCodeFromPropagate(self, obj:Logic):
-        str = "// Code generated from clock method\n"
-        clkname = getObjectClockDriver(obj).name
-        
-        tr = Python2VerilogTranspiler(obj, 'propagate')
+        str = "// Code generated from propagate method\n"
         
-        transpiled = tr.transpile() ;
+        tr = Python2VerilogTranspiler(obj)
         
-        str += "// local declarations\n"
-        str += tr.getExtraDeclarations() + "\n";
-        str += "// combinational process\n"
-        str += "always @(*)\n".format(clkname)
-        str += "begin\n"
-        str += transpiled + "\n"
-        str += "end\n"
+        node = tr.transpileCombinational()
+        str += tr.toVerilog(node)
         
-        str += "\n"
+        str = tr.format(str)
         
         return str
 import inspect
 import ast
 import textwrap
     
 
@@ -680,197 +839,11 @@
         if (len(obj)>1):
             raise Exception('multiple names in {}'.format(obj))
         
         return getAstName(obj[0])
     else:
         raise Exception('unknown type {}'.format(type(obj)))
 
-class Python2VerilogTranspiler:
-
-    def __init__(self, obj:Logic, methodName:str):
-        self.obj = obj
-        self.methodName = methodName
-        self.signals = {}
-        self.indent = 0
-
-    def getIndent(self):
-        return ' ' * (self.indent * 4)
-        
-    def transpile(self):
-        
-        methods = inspect.getmembers(self.obj, inspect.ismethod)
-        method = [x[1] for x in methods if x[0] == self.methodName ][0]
-
-        source = textwrap.dedent(inspect.getsource(method))
-        module = ast.parse(source)
-
-        
-        module = ReplaceWireGets().visit(module)
-        module = ReplaceWirePrepare().visit(module)
-        module = ReplaceWirePut().visit(module)
-        
-        func = module.body[0].body
-        
-        return self.transpileUnknown(func)
-        
-    def getExtraDeclarations(self):
-        str = ""
-        
-        portNames = []
-        
-        
-        for inp in self.obj.inPorts:
-            portNames.append(getValidVerilogName(inp.name))
-
-        for outp in self.obj.outPorts:
-            portNames.append(getValidVerilogName(outp.name))        
-        
-        #print('SIGNALS:', self.signals)
-        #print('PORT NAMES:', portNames)
-
-        extra = [x for x in self.signals if x not in portNames]
-        
-        # @todo we should analyze the number of possible values of 
-        # extra signals to decide their width. By now we consider a worst
-        # case scenario with extra signals all requiring a maximum of 8 bits
-        # this will be simplyfied during synthesis if less bits are required
-        # but it will cause a BUG if the required bits are higher
-        for sig in extra:
-            str += "reg [7:0] " + sig + " = 0;\n" 
-            
-        return str
-    
-    def transpileUnknown(self, line):
-        
-        if (type(line) == ast.If):
-            return self.transpileIf(line);
-        if (type(line) == ast.Compare):
-            return self.transpileCompare(line)
-        if (type(line) == ast.Assign):
-            return self.transpileAssign(line)
-        if (type(line) == ast.BinOp):
-            return self.transpileBinOp(line)
-        if (type(line) == ast.Attribute):
-            return self.transpileAttribute(line)
-        if (isinstance(line, ast.Name)):
-            return self.transpileName(line)
-        if (type(line) == ast.Eq):
-            return "==";
-        if (type(line) == ast.Constant):
-            return "{}".format(getAstValue(line))
-        if (type(line) == ast.Num):
-            return "{}".format(int(line.n))
-        
-        if (type(line) == list):
-            str = ""
-            for item in line:
-                str += self.transpileUnknown(item) 
-            return str
-
-        if (type(line) == ast.Expr):
-            return self.transpileExpr(line)
-        
-        else:
-            str= "type = {}\n".format(type(line))
-            
-            str += ast.dump(line) + "\n"
-            
-            return str
-        
-    def transpileAttribute(self, line:ast.Attribute):
-        return line.attr
-            
-    def transpileExpr(self, line:ast.Expr):
-        return self.transpileUnknown(line.value)
-        
-    def transpileBinOp(self, line:ast.BinOp):
-        return "(" + self.transpileUnknown(line.left) + self.transpileOp(line.op) + self.transpileUnknown(line.right) + ")";
-
-    def transpileOp(self, op):
-        if (isinstance(op, ast.BitAnd)):
-            return '&'
-        elif (isinstance(op, ast.BitOr)):
-            return '|'
-        elif (isinstance(op, ast.BitXor)):
-            return '^'
-        else:
-            raise Exception('Op not supported: {}'.format(op))
-        
-    def transpileAssign(self, line:ast.Assign):
-        targets = line.targets 
-        if (len(targets) > 1):
-            return ast.dump(line)
-        
-        var = getAstName(targets[0])
-        
-        self.signals[var] = var
-        
-        return var + " <= " + self.transpileUnknown(line.value) + ";\n" + self.getIndent()  ;
-    
-    def transpileIf(self, line:ast.If):
-        str = "if " + self.transpileUnknown(line.test) + "\n"
-        str += self.getIndent() + "begin\n"
-        self.indent += 1
-        str += self.getIndent() + self.transpileUnknown(line.body)
-        self.indent -= 1
-        str +=  "end\n"
-        
-        if (not(line.orelse is None)):
-            str += self.getIndent() + "else \n"
-            str += self.getIndent() + "begin\n"
-            self.indent += 1
-            str += self.getIndent() + self.transpileUnknown(line.orelse)
-            self.indent -= 1
-            str +=  "end\n"
-
-        return str
-    
-    def transpileCompare(self, line:ast.Compare):
-        str = "("
-        str += self.transpileUnknown(line.left)
-        str += self.transpileUnknown(line.ops)
-        str += self.transpileUnknown(line.comparators)
-        str += ")"
-        return str;
-    
-    def transpileName(self, line:ast.Name):
-        str =  getValidVerilogName(line.id)
-        self.signals[str] = str
-        return str
-    
-    
-    
-
-class ReplaceWireGets(ast.NodeTransformer):
-    def visit_Call(self, node):
-        attr = getAstName(node.func)
-        
-        if (attr == 'get'):
-            #if isinstance(node.func.value, ast.Attribute):
-            wirename = getAstName(node.func.value)
-            #print('REPLACING GET ', wirename)
-            return ast.Name(wirename, ast.Load)
-        
-        return node
-    
-    
-class ReplaceWirePrepare(ast.NodeTransformer):
-    def visit_Call(self, node):
-        attr = getAstName(node.func)
-        
-        if (attr == 'prepare'):
-            #print('REPLACE WIRE PUTS FUNC:', attr , node.func.value.attr, node.args)
-            return ast.Assign([node.func.value], node.args[0])
-        
-        
-        return node
-    
-class ReplaceWirePut(ast.NodeTransformer):
-    def visit_Call(self, node):
-        attr = getAstName(node.func)
-        
-        if (attr == 'put'):
-            #print('REPLACE WIRE PUTS FUNC:', attr , node.func.value.attr, node.args)
-            return ast.Assign([node.func.value], node.args[0])
-        
-        
-        return node
+class VerilogComment(Logic):
+    def __init__(self, parent, name: str, comment:str):
+        super().__init__(parent, name)
+        self.comment = comment
```

### Comparing `py4hw-0.0.9/py4hw/schematic.py` & `py4hw-2024.1/py4hw/schematic.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,52 +5,65 @@
 @author: dcr
 """
 import matplotlib.pyplot as plt
 import numpy as np
         
 from matplotlib.lines import Line2D
 from matplotlib.patches import *
+from matplotlib import colors
 from .base import *
 from .logic import *
 from .logic.bitwise import *
 from .logic.storage import *
 from .schematic_symbols import *
 
 gridsize = 5
 cellmargin = 50
 cellmargin_initial = 150
 netmargin = 40
 netspacing = 10
 nettrackspacing = 10
+portvaluemargin = 10
 
 class MatplotlibRender:
-    def __init__(self, shape):
-        w = shape[0]
-        h = shape[1]
-        dpi = 100
-        iw = w / dpi 
-        ih = h / dpi
+    def __init__(self, shape, physical_shape=None, dpi=None):
+        w = shape[1]
+        h = shape[0]
+        if (physical_shape is None):
+            if (dpi is None):
+                dpi = 100
+            iw = w / dpi 
+            ih = h / dpi
+            #print('w/h = ',w,h, 'iw/ih', iw,ih)
+        else:
+            iw = physical_shape[1]
+            ih = physical_shape[0]
+            if (dpi is None):
+                dpi = max(w / iw, h / ih)
+            
         pmax = max(w,h)
         imax = max(iw, ih)
-        f = plt.figure(figsize=(imax,imax), dpi=dpi)
+        f = plt.figure(figsize=(iw,ih), dpi=dpi)
         self.canvas = f.add_subplot()
-        self.canvas.set_xlim(0, pmax)
-        self.canvas.set_ylim(0, pmax)
+        self.canvas.set_xlim(0, w)
+        self.canvas.set_ylim(0, h)
         self.canvas.invert_yaxis()
         plt.axis('off')
         
-        self.color = 'k'
-        self.fillcolor = 'k'
+        self.setForecolor('k')
+        self.setFillcolor('k')
         self.linewidth = 2
         
     def setForecolor(self, color):
-        self.color = color
+        #print('color {} = {}'.format(color, colors.rgb2hex(colors.to_rgb(color))))
+        self.color = colors.rgb2hex(colors.to_rgb(color))
         
     def setFillcolor(self, color):
-        self.fillcolor = color
+        #print('color {} = {}'.format(color, colors.rgb2hex(colors.to_rgb(color))))
+        self.fillcolor = colors.rgb2hex(colors.to_rgb(color))
         
     def setLineWidth(self, w):
         self.linewidth = w
         
     def drawText(self, x, y, text, anchor):
         """
         
@@ -97,138 +110,191 @@
         self.drawPolygon([x0, x1, x1, x0, x0],[y0,y0, y1,y1, y0], fill)
         
     def drawRoundRectangle(self, x0, y0, x1, y1, radius=5, fill=False):
         box = FancyBboxPatch((x0,y0), width=x1-x0, height=y1-y0,
               boxstyle=BoxStyle("Round", pad=radius), facecolor=self.fillcolor)
         self.canvas.add_patch(box)
         
-    def drawArc(self, x0, y0, x1, y1, start, extent):
-        arc = Arc(((x0+x1)//2, (y0+y1)//2), x1-x0, y1-y0, angle=0, theta1=start, theta2=extent, linewidth=self.linewidth)
+    def drawArc(self, x0, y0, x1, y1, start, stop):
+        arc = Arc(((x0+x1)//2, (y0+y1)//2), x1-x0, y1-y0, angle=0, theta1=start, theta2=stop, linewidth=self.linewidth)
         self.canvas.add_patch(arc)
 
     def drawEllipse (self, x0, y0, x1, y1, outline=None, fill=None):
         el = Ellipse(((x0+x1)/2, (y0+y1)/2), x1-x0, y1-y0, edgecolor=self.color, facecolor='none', linewidth=self.linewidth)
         self.canvas.add_artist(el)
         
     def drawSpline(self, x, y):
         from scipy import interpolate
         tck,u     = interpolate.splprep( [x,y] ,s = 0 )
         xnew,ynew = interpolate.splev( np.linspace( 0, 1, 20 ), tck,der = 0)
         self.canvas.plot( xnew ,ynew , color=self.color, linewidth=self.linewidth)
         
+    def drawImage(self, x, y, img ):
+        w = img.shape[1]
+        h = img.shape[0]
+        self.canvas.imshow(img, extent=[x,x+w,y+h,y], origin='upper')
+        
 
 class TkinterRender:
     # check https://zetcode.com/tkinter/drawing/
     
     def __init__(self, parent, shape):
         from tkinter import Canvas
         self.canvas = Canvas(parent, bg='white')
+        
+        self.canvas.bind("<ButtonPress-1>", self.on_press)
+        self.canvas.bind("<B1-Motion>", self.on_drag)
+
+        self.start_x = None
+        self.start_y = None
+        
         w = shape[0]
         h = shape[1]
         dpi = 100
         iw = w / dpi 
         ih = h / dpi
         pmax = max(w,h)
         imax = max(iw, ih)
         # f = plt.figure(figsize=(imax,imax), dpi=dpi)
         # self.canvas = f.add_subplot()
         # self.canvas.set_xlim(0, pmax)
         # self.canvas.set_ylim(0, pmax)
         # self.canvas.invert_yaxis()
         # plt.axis('off')
         
-        self.color = 'k'
-        self.fillcolor = 'k'
+        self.setForecolor('k')
+        self.setFillcolor('k')
         self.linewidth = 2
+        self.xmargin = 50
+        self.ymargin = 50
+
+    def on_press(self, event):
+        self.start_x = int(self.canvas.canvasx(event.x))
+        self.start_y = int(self.canvas.canvasy(event.y))
+
+    def on_drag(self, event):
+        if self.start_x is not None and self.start_y is not None:
+            cur_x = int(self.canvas.canvasx(event.x))
+            cur_y = int(self.canvas.canvasy(event.y))
+
+            delta_x = cur_x - self.start_x
+            delta_y = cur_y - self.start_y
+
+            self.canvas.scan_mark(self.start_x, self.start_y)
+            self.canvas.scan_dragto(cur_x, cur_y, gain=1)
+
+    def reset_start_coords(self):
+        self.start_x = None
+        self.start_y = None
         
     def setForecolor(self, color):
-        self.color = color
+        #print('color {} = {}'.format(color, colors.rgb2hex(colors.to_rgb(color))))
+        self.color = colors.rgb2hex(colors.to_rgb(color))
         
     def setFillcolor(self, color):
-        self.fillcolor = color
+        #print('color {} = {}'.format(color, colors.rgb2hex(colors.to_rgb(color))))
+        self.fillcolor = colors.rgb2hex(colors.to_rgb(color))
         
     def setLineWidth(self, w):
         self.linewidth = w
         
     def drawText(self, x, y, text, anchor):
         if (anchor == 'w'):
             ha = 'left'
         elif (anchor == 'e'):
             ha = 'right'
         elif (anchor == 'c'):
             ha = 'center'
             
-        self.canvas.create_text(x,y, anchor=anchor, text=text)
+        self.canvas.create_text(x + self.xmargin, y+self.ymargin, anchor=anchor, text=text)
         
     def drawPolygon(self, x, y, fill=False):
         
-        # points = []
-        
-        # for i in range(len(x)):
-        #     points.append(x[i])
-        #     points.append(y[i])
+        if (fill):
+            points = []
+            
+            for i in range(len(x)):
+                points.append(self.xmargin + x[i])
+                points.append(self.ymargin + y[i])
             
         # #lines = Line2D(x,y, color=self.color, linewidth=self.linewidth)
         # # if (fill):
         # #    self.canvas.fill(x, y, self.fillcolor)
 
-        # self.canvas.create_polygon(points)
-        x0 = x[0]
-        y0 = y[0]
-        for i in range(1, len(x)):
-            x1 = x[i]
-            y1 = y[i]
-            self.drawLine(x0, y0, x1, y1)
-            x0 = x1
-            y0 = y1
+            self.canvas.create_polygon(points, outline=self.color, fill=self.fillcolor, width=self.linewidth)
+            
+        else:            
+            x0 = x[0]
+            y0 = y[0]
+            for i in range(1, len(x)):
+                x1 = x[i]
+                y1 = y[i]
+                self.drawLine(x0 , y0 , x1 , y1 )
+                x0 = x1
+                y0 = y1
         #     points.append(x[i])
         #     points.append(y[i])
         
 
     def drawLine(self, x0, y0, x1, y1):
-        self.canvas.create_line(x0, y0, x1, y1)
+        self.canvas.create_line(x0 + self.xmargin, y0 + self.ymargin, x1 + self.xmargin, y1 + self.ymargin, fill=self.color, width=self.linewidth)
         #self.drawPolygon([x0, x1], [y0, y1])
         
     def drawRectangle(self , x0, y0, x1, y1, fill=False):
         #print('rect', x0, y0, x1, y1)
         #self.drawPolygon([x0, x1, x1, x0, x0],[y0,y0, y1,y1, y0], fill)
-        self.canvas.create_rectangle(x0, y0, x1, y1)
+        self.canvas.create_rectangle(x0 + self.xmargin, y0 + self.ymargin, x1 + self.xmargin, y1 + self.ymargin, width=self.linewidth)
         
     def drawRoundRectangle(self, x0, y0, x1, y1, radius=5, fill=False):
         #box = FancyBboxPatch((x0,y0), width=x1-x0, height=y1-y0,
         #      boxstyle=BoxStyle("Round", pad=radius), facecolor=self.fillcolor)
         #self.canvas.add_patch(box)
         print('[WARNING] round rectangle not supported yet')
         
-    def drawArc(self, x0, y0, x1, y1, start, extent):
+    def drawArc(self, x0, y0, x1, y1, start, stop):
         import tkinter
         # arc = Arc(((x0+x1)//2, (y0+y1)//2), x1-x0, y1-y0, angle=0, theta1=start, theta2=extent, linewidth=self.linewidth)
         # self.canvas.add_patch(arc)
-        print('draw arc', x0, y0, x1, y1, start, extent)
-        self.canvas.create_arc(x0, y0, x1, y1, start=start, extent=extent-start, style=tkinter.ARC)
+        self.canvas.create_arc(x0 + self.xmargin, y0 + self.ymargin, x1 + self.xmargin, y1 + self.ymargin, start=start, extent=stop-start, style=tkinter.ARC, width=self.linewidth)
 
     def drawEllipse (self, x0, y0, x1, y1, outline=None, fill=None):
         # el = Ellipse(((x0+x1)/2, (y0+y1)/2), x1-x0, y1-y0, edgecolor=self.color, facecolor='none', linewidth=self.linewidth)
         # self.canvas.add_artist(el)
-        self.canvas.create_oval(x0, y0, x1, y1)
+        self.canvas.create_oval(x0 + self.xmargin, y0 + self.ymargin, x1 + self.xmargin, y1 + self.ymargin, width=self.linewidth)
         
     def drawSpline(self, x, y):
-        # from scipy import interpolate
-        # tck,u     = interpolate.splprep( [x,y] ,s = 0 )
-        # xnew,ynew = interpolate.splev( np.linspace( 0, 1, 20 ), tck,der = 0)
-        # self.canvas.plot( xnew ,ynew , color=self.color, linewidth=self.linewidth)
-        print('[WARNING] spline not supported yet')
+        from scipy import interpolate
+        tck,u     = interpolate.splprep( [x,y] ,s = 0 )
+        xnew,ynew = interpolate.splev( np.linspace( 0, 1, 20 ), tck,der = 0)
+        self.drawPolygon( xnew ,ynew)
 
+    def drawImage(self, x, y, np_img ):
+        from tkinter import PhotoImage
+        from PIL import Image, ImageTk
+        w = np_img.shape[1]
+        h = np_img.shape[0]
+        
+        #print('drawImage', np_img.shape, type(np_img), type(np_img[0][0][0]))
+
+        pil_img = Image.fromarray(np_img)
+        tk_img = ImageTk.PhotoImage(image=pil_img)
+        # Display the image on the canvas
+        self.canvas.create_image(x, y, anchor="nw", image=tk_img)
+        self.canvas.image = tk_img
         
 class Schematic:
     """
     Class that controls the schematic drawing
     """
+
+    step_timeout = 10 # any step of the schematic rendering cannot take more than this value (seconds)
+
+    mapping = {} # maaping from object class to symbol
     
-    def __init__(self, obj:Logic, render='matplotlib', parent=None):
+    def __init__(self, obj:Logic, render='matplotlib', parent=None, placeAndRoute=True, showValues=False):
    
         if not(obj.isStructural()):
             raise Exception('Schematics are only available to structural circuits')
 
         self.sys = obj
         self.x = 0
         self.y = 0
@@ -246,47 +312,64 @@
         # vbar.config(command=canvas.yview)
         # canvas.config(width=300,height=900)
         # canvas.config(xscrollcommand=hbar.set, yscrollcommand=vbar.set)
         # canvas.pack(side=LEFT,expand=True,fill=BOTH)
 
         self.objs = []      # a list of the logic symbols displayed
         self.nets = []      # a list of the nets
-        self.sources = []   # a list of net sources with tuples [symbol, x, y, wire]
-        self.sinks = []     # a list of net sinks with tuples   [symbol, x, y, wire]
+        self.sources = []   # a list of net sources with tuples [symbol, x, y, port]
+        self.sinks = []     # a list of net sinks with tuples   [symbol, x, y, port]
         
-        self.mapping = {}
-        self.mapping[And2] = AndSymbol
-        self.mapping[Not] = NotSymbol
-        self.mapping[Or2] = OrSymbol
-        self.mapping[Or] = OrSymbol
-        self.mapping[Nor2] = NorSymbol
-        self.mapping[Xor2] = XorSymbol
-        
-        self.mapping[Add] = AddSymbol
-        self.mapping[Sub] = SubSymbol
-        self.mapping[Mul] = MulSymbol
-        
-        self.mapping[Reg] = RegSymbol
-        self.mapping[Scope] = ScopeSymbol
-        self.mapping[Buf] = BufSymbol
-        self.mapping[Bit] = BitSymbol
-        self.mapping[Mux2] = Mux2Symbol
-        self.mapping[Range] = RangeSymbol
+        Schematic.mapping[And2] = AndSymbol
+        Schematic.mapping[And] = AndSymbol
+        Schematic.mapping[Not] = NotSymbol
+        Schematic.mapping[Or2] = OrSymbol
+        Schematic.mapping[Or] = OrSymbol
+        Schematic.mapping[Nor2] = NorSymbol
+        Schematic.mapping[Xor2] = XorSymbol
+        
+        Schematic.mapping[Add] = AddSymbol
+        Schematic.mapping[Sub] = SubSymbol
+        Schematic.mapping[Mul] = MulSymbol
+        
+        Schematic.mapping[Reg] = RegSymbol
+        Schematic.mapping[Scope] = ScopeSymbol
+        Schematic.mapping[Buf] = BufSymbol
+        Schematic.mapping[Bit] = BitSymbol
+        Schematic.mapping[Mux2] = Mux2Symbol
+        Schematic.mapping[Range] = RangeSymbol
 
         self.mapping[Waveform] = ScopeSymbol # Temp solution
+
+        self.parent = parent
+        self.render = render        
+        self.canvas = None
+
+        self.showValues = showValues
+
+        if (placeAndRoute):
+            self.placeAndRoute()
+        
+        
+        # schematics are created but not directly drawn to allow 
+        # the manipulation of the graphical objects
         
+        #self.drawAll()
         
+        #mainloop()
+
+    def placeAndRoute(self, debug=False):
         self.placeInputPorts()
         self.placeInstances()
         self.placeOutputPorts()
 
         self.bruteForceSort()
         self.columnAssignment()
         
-        self.createNets()
+        self.createNets(debug=debug) 
         self.passthroughCreation()
         self.removeArrowsSpecialCases()
         
         self.rowAssignment()
         
 
         self.trackAssignment()
@@ -299,28 +382,16 @@
         #self.replaceVerticalCompress()
         # #self.replaceHorizontalCompress()
         
 
         self.routeNets()
         
         
-        if (render == 'matplotlib'):
-            self.canvas = MatplotlibRender(self.getOccupancyGrid().shape)
-        elif (render == 'tkinter'):
-            self.canvas = TkinterRender(parent, self.getOccupancyGrid().shape)
-        else:
-            raise Exception('Unsupported render {}'.format(render))
-            
-        self.canvas.setForecolor('k')
-        self.drawAll()
-        
-        #mainloop()
-        
-        
     def draw(self):
+        self.drawAll()
         import matplotlib.pyplot as plt
         return plt.show()
     
     def removeArrowsSpecialCases(self):
         """
         Remove the arrows from some nets like the ones
         connected to selection ports of muxes 
@@ -347,40 +418,46 @@
 
         """
         nets = self.getNets()
         numCols = len(self.columns)
         self.channels = [] 
         
         #print('cols', self.columns)
-        for colidx in range(1, numCols):
+        for colidx in range(0, numCols):
             track = 0
-            netsInCol = [n for n in nets if n.sink in self.columns[colidx]]
+            netsInCol = [n for n in nets if n.sourcecol == colidx]
             
-            # temporal object to check if several nets are created from the same
-            # source
+            # temporal object to check if several nets are created from the 
+            # same source
             channeltracks = {}
             
             #print('Nets is column', colidx, netsInCol )
             for net in netsInCol:
                 try:
-                    existingtrack = channeltracks[net.source['wire']]
+                    existingtrack = channeltracks[net.wire]
+                    
                 except:
                     existingtrack = None
                     
+                
                 if (existingtrack == None):
+                    # There is not track for this wire
                     net.track = track
                     track = track + 1
                     channeltracks[net.wire]={'num':net.track, 'nets':[net]}
+                    #print('track:', net.track, 'channel tracks:', channeltracks)
                 else:
                     net.track = existingtrack['num']
                     existingtrack['nets'].append(net)
+                 
+                # do not update the sourcecol
+                #net.sourcecol = colidx - 1
                     
-                net.sourcecol = colidx - 1
-                    
-                
+            #print('col:', colidx, ['{}->{}'.format(type(x.source).__name__, type(x.sink).__name__)  for x in netsInCol])
+            #print('track:', track, 'channel tracks:', channeltracks)
             self.channels.append({'tracks':track, 'track':channeltracks})
         
     def getAllInstanceSources(self, sym:LogicSymbol):
         """
         Return all the instance objects that are connected
         as sources to this symbol
 
@@ -399,15 +476,15 @@
         
         ret = []
         
         for inp in obj.inPorts:
             wire = inp.wire
             
             for src in self.sources:
-                if (src['wire'] == wire):
+                if (src['port'].wire == wire):
                     ret.append(src['symbol'])
         
         return ret
     
     def getAllInstanceSinks(self, sym:LogicSymbol):
         """
         Return all the instance objects that are connected
@@ -431,26 +508,30 @@
         if (isinstance(obj, InPort)):
             # an input port is a single driver
             outports = [obj]
         elif (isinstance(obj, OutPort)):
             # an output port cannot drive anything (at the circuit level)
             # so, no dependent instances 
             return []
+        elif (isinstance(obj, InOutPort)):
+            outports = [obj]
         else:
             if (not(hasattr(obj, 'outPorts'))):
                 raise Exception('obj {} from type {} {} has not out ports'.format(obj.getFullPath(), type(obj), isinstance(obj, InPort)))
                 
             outports = obj.outPorts
         
         for outp in outports:
             wire = outp.wire
             
-            for src in self.sinks:
-                if (src['wire'] == wire):
-                    ret.append(src['symbol'])
+            if not(wire in self.maxfanoutwires):
+                # avoid to report elements connected by pruned wires
+                for src in self.sinks:
+                    if (src['port'].wire == wire):
+                        ret.append(src['symbol'])
         
         # if multiple wires connect between two symbols, there will be repetitions
         # so remove duplicates
         ret = list(set(ret))
         
         return ret
         
@@ -470,20 +551,70 @@
 
         """
         for colidx, col in enumerate(self.columns):
             if (sym in col):
                 return colidx
             
         return -1
-                            
+                          
+    def columnManualAssignment(self, inlist, inslist, outlist):
+        self.columns = []
+        
+        
+        # Process inputs
+        unsorted = {}
+        currentCol = []
+        for idx, obj in enumerate(self.objs):
+            if (idx < self.numInputs):
+                unsorted[obj.obj.name] = obj
+                
+        for name in inlist:
+            currentCol.append(unsorted[name])
+        self.columns.append(currentCol)
+        
+        # Process instances
+        for inskeys in inslist:
+            unsorted = {}
+            currentCol = []
+            for idx, obj in enumerate(self.objs):
+                if (idx < self.numInputs):
+                    pass
+                elif (idx < self.firstOutput):
+                    if (obj.obj.name in inskeys):
+                        unsorted[obj.obj.name] = obj
+            
+            for name in inskeys:
+                currentCol.append(unsorted[name])
+            self.columns.append(currentCol)    
+        
+        # Process outputs
+        unsorted = {}
+        currentCol = []
+        for idx, obj in enumerate(self.objs):
+            if (idx >= self.firstOutput):
+                unsorted[obj.obj.name] = obj
+        for name in outlist:
+            currentCol.append(unsorted[name])
+        self.columns.append(currentCol)
+        
     def columnAssignment(self):
+        """
+        Creates the columns structure and assigns inputs, instances and outputs 
+        to a column
+
+        Returns
+        -------
+        None.
+
+        """
         self.columns = []
         currentCol = []
         
-        # append inputs
+        # append inputs. We know that inputs are always at the start
+        # of the object list
         for idx, obj in enumerate(self.objs):
             if (idx < self.numInputs):
                 currentCol.append(obj)
 
         self.columns.append(currentCol)
                 
         # append instances
@@ -548,15 +679,15 @@
             
             if (colidx < len(self.channels)):
                 x = x + self.channels[colidx]['tracks'] * nettrackspacing
 
             if (colidx < len(self.channels)):
                 self.channels[colidx]['sourcewidth'] = maxw
     
-    def passthroughCreation(self):
+    def passthroughCreation(self, debug=False):
         """
         Create passthrough entities.
         For connected entities that are separated by more than 1 column
         we create passthrough entities.
         For entities connected to previous columns we create feedback 
         entities.
 
@@ -564,36 +695,38 @@
         -------
         None.
 
         """
 
         for colidx, col in enumerate(self.columns):
             for obj in col:
+                # We list the objects in the column 
                 if (isinstance(obj, PassthroughSymbol)):
                     continue
                 if (isinstance(obj, FeedbackStartSymbol)):
                     continue
                 if (isinstance(obj, FeedbackStopSymbol)):
                     continue
                 
                 sinks = self.getAllInstanceSinks(obj)
                 
                 for sink in sinks:
                     sinkcol = self.getSymbolColumn(sink)
                     
                     if (sinkcol > colidx +1):
                         #print('WARNING: passthrough required between: [{}]'.format(colidx), type(obj).__name__, '[{}]'.format(sinkcol), type(sink).__name__, )
-                        self.insertPassthrough(obj, colidx, sink, sinkcol)
+                        self.insertPassthrough(obj, colidx, sink, sinkcol, debug)
                     if (sinkcol <= colidx):
                         #print('WARNING: feedback required between: [{}]'.format(colidx), type(obj).__name__, '[{}]'.format(sinkcol), type(sink).__name__)
-                        self.insertFeedback(obj, colidx, sink, sinkcol)
+                        self.insertFeedback(obj, colidx, sink, sinkcol, debug)
 
-    def insertPassthrough(self, source:LogicSymbol, sourcecol:int, sink:LogicSymbol, sinkcol:int):
+    def insertPassthrough(self, source:LogicSymbol, sourcecol:int, sink:LogicSymbol, sinkcol:int, debug=False):
         """
-        A passthrough instance has to be inserted for every wire connecting both entities
+        A passthrough instance has to be inserted for every wire connecting 
+        entities source and sink
 
         Parameters
         ----------
         source : LogicSymbol
             DESCRIPTION.
         sourcecol : int
             DESCRIPTION.
@@ -611,51 +744,67 @@
     
         source_wires = self.getWiresFromSource(source)
         sink_wires = self.getWiresFromSink(sink)
         intersection = Intersection(source_wires, sink_wires)
               
         
         for wire in intersection:
+            if (wire is None):
+                continue
+            
             # remove the original net
             removeNets = [x for x in self.nets if x.wire== wire and x.source == source and x.sink == sink]
 
             if (len(removeNets) == 0):
                 self.dumpNets()
                 raise Exception('Wire:{} with source:{} {} and sink:{} {} not in remove nets'.format(wire.getFullPath(), id(source), source.obj.getFullPath(), id(sink), sink.obj.getFullPath()))
             
-            self.nets.remove(removeNets[0])
+            if (len(removeNets) > 1):
+                self.dumpNets()
+                raise Exception('Muliple nets between source:{} {} and sink:{} {}'.format( type(source).__name__, source.obj.getFullPath(), type(sink).__name__, sink.obj.getFullPath()))
+
+            netToRemove = removeNets[0]
+            self.nets.remove(netToRemove)
         
             lastSymbol = source
+            lastSourcePort = netToRemove.sourcePort
             
             for col in range(sourcecol+1, sinkcol):
                 pts = PassthroughSymbol()
+
                 self.objs.append(pts)
                 self.columns[col].append(pts)
-                self.sources.append({'symbol':pts, 'wire':wire})
-                self.sinks.append({'symbol':pts, 'wire':wire})
+
+                # raise Exception('TODO get the port of this wire')
+                # self.sources.append({'symbol':pts, 'port':wire})
+                # self.sinks.append({'symbol':pts, 'port':wire})
                 
-                net1 = NetSymbol(wire, lastSymbol, pts)
+                # TODO what to do here with the port info ??
+                net1 = NetSymbol(wire, lastSourcePort, None, lastSymbol, pts)
                 net1.sourcecol = col-1
                 net1.arrow = False
                 self.nets.append(net1)
                 
                 lastSymbol = pts
+                lastSourcePort = None
                 
                 
             if (lastSymbol != None):
-                net2 = NetSymbol(wire, pts, sink)
+                # TODO what to do here with the port info 
+                net2 = NetSymbol(wire, None, netToRemove.sinkPort, pts, sink)
+                net2.sourcecol = sinkcol-1
                 self.nets.append(net2)
                                 
     def dumpNets(self):
         for idx, net in enumerate(self.nets):
             print('Net {} wire:{} source:{} {}  sink:{} {}'.format(idx, net.wire.getFullPath(), id(net.source), type(net.source).__name__ , id(net.sink), type(net.sink).__name__))
             
-    def insertFeedback(self, source:LogicSymbol, sourcecol:int, sink:LogicSymbol, sinkcol:int):
+    def insertFeedback(self, source:LogicSymbol, sourcecol:int, sink:LogicSymbol, sinkcol:int, debug=False):
         """
-        A passthrough instance has to be inserted for every wire connecting both entities
+        Create feedback nets between source and sink
 
         Parameters
         ----------
         source : LogicSymbol
             DESCRIPTION.
         sourcecol : int
             DESCRIPTION.
@@ -671,82 +820,96 @@
         """
         #return
     
         source_wires = self.getWiresFromSource(source)
         sink_wires = self.getWiresFromSink(sink)
         intersection = Intersection(source_wires, sink_wires)
         
-       
+        # intersection wires are wires that connect source and sink
+        # but take care, because the same wire can have multiple sink ports
         
         for wire in intersection:
             # remove the original net
             removeNets = [x for x in self.nets if x.wire == wire and x.source == source and x.sink == sink]
             
             if (len(removeNets) == 0):
                 self.dumpNets()
                 raise Exception('Wire:{} with source:{} {} and sink:{} {} not in remove nets'.format(wire.getFullPath(), type(source).__name__, source.obj.getFullPath(), type(sink).__name__, sink.obj.getFullPath()))
 
-            self.nets.remove(removeNets[0])
+            if (len(removeNets) > 1):
+                self.dumpNets()
+                raise Exception('Muliple nets between source:{} {} and sink:{} {}'.format( type(source).__name__, source.obj.getFullPath(), type(sink).__name__, sink.obj.getFullPath()))
+
+            netToRemove = removeNets[0]
+            self.nets.remove(netToRemove)
         
             lastSymbol = source
             
             #insert feedback channel if necessary
             
             #self.channels[sourcecol+1]
             fb_start = FeedbackStartSymbol()
+            fb_start.debug = debug
             self.objs.append(fb_start)
-            self.columns[sourcecol+1].append(fb_start)
+            self.columns[sourcecol].append(fb_start)
             #self.sources.append({'symbol':fb_start, 'wire':wire})
             #self.sinks.append({'symbol':fb_start, 'wire':wire})
             
-            net1 = NetSymbol(wire, lastSymbol, fb_start)
+            # TODO: what to do here with the port info ???
+            net1 = NetSymbol(wire, netToRemove.sourcePort, None , lastSymbol, fb_start)
             net1.sourcecol = sourcecol
             net1.arrow = False
-            self.nets.append(net1)
-            
+            self.nets.append(net1)            
             
             fb_end = FeedbackStopSymbol()
+            fb_end.debug = debug
             self.objs.append(fb_end)
-            self.columns[sinkcol-1].append(fb_end)
+            self.columns[sinkcol].append(fb_end)
             #self.sources.append({'symbol':fb_start, 'wire':wire})
             #self.sinks.append({'symbol':fb_start, 'wire':wire})
             
-            net2 = NetSymbol(wire, fb_end, sink)
-            net2.sourcecol = sinkcol-1
+            # TODO what to do here with the port info ????
+            net2 = NetSymbol(wire, None, netToRemove.sinkPort, fb_end, sink)
+            net2.sourcecol = sinkcol
             net2.arrow = True
             self.nets.append(net2)
             
             lastSymbol = fb_end
             
             
-            for col in range(sinkcol, sourcecol+1):
-                  pts = PassthroughSymbol()
-                  self.objs.append(pts)
-                  self.columns[col].append(pts)
-                  self.sources.append({'symbol':pts, 'wire':wire})
-                  self.sinks.append({'symbol':pts, 'wire':wire})
-                
-                  net1 = NetSymbol(wire, lastSymbol, pts)
-                  net1.sourcecol = col-1
-                  net1.arrow = False
-                  self.nets.append(net1)
-                
-                  lastSymbol = pts
+            for col in range(sinkcol+1, sourcecol):
+                pts = PassthroughSymbol()
+                self.objs.append(pts)
+                self.columns[col].append(pts)
+
+                #raise Exception('TODO get the port of this wire')
+                #self.sources.append({'symbol':pts, 'port':wire})
+                #self.sinks.append({'symbol':pts, 'port':wire})
+              
+                # TODO what to do here with the port info ???
+                net1 = NetSymbol(wire, None, None, lastSymbol, pts)
+                net1.sourcecol = col-1
+                net1.arrow = False
+                self.nets.append(net1)
+              
+                lastSymbol = pts
                 
                 
             if (lastSymbol != None):
-                 net2 = NetSymbol(wire, lastSymbol, fb_start)
-                 net2.arrow = False
-                 self.nets.append(net2)
+                # TODO What to do here with the port info ???
+                net2 = NetSymbol(wire, None, None, lastSymbol, fb_start)
+                net2.sourcecol = sourcecol
+                net2.arrow = False
+                self.nets.append(net2)
 
     def getWiresFromSource(self, source):
-        return [x['wire'] for x in self.sources if x['symbol'] == source]
+        return [x['port'].wire for x in self.sources if x['symbol'] == source]
 
     def getWiresFromSink(self, sink):
-        return [x['wire'] for x in self.sinks if x['symbol'] == sink]
+        return [x['port'].wire for x in self.sinks if x['symbol'] == sink]
     
     def replaceByAdjacencyMatrix(self):
         am = self.getAdjacencyMatrix()
         
         x = 0
         y = 0
         
@@ -859,15 +1022,15 @@
         changed = True
         iterNum = 0
         
         while (changed and iterNum < 2):
             iterNum = iterNum + 1
             changed = False
             for sourceTuple in self.sources:
-                sinks = self.findSinkTuples(sourceTuple['wire'])
+                sinks = self.findSinkTuples(sourceTuple['port'].wire)
                 sourceObj = sourceTuple['symbol']
                 
                 
                 for sinkTuple in sinks:
                     sinkObj = sinkTuple['symbol']
                     candidatex = sourceObj.x + sourceObj.getWidth() + cellmargin
     
@@ -888,16 +1051,18 @@
                         #print('Sink Obj:', sinkObj.obj.name)
                         #print('direct', directCount, 'reverse', reverseCount)
                         sinkObj.x = candidatex + cellmargin
                         changed = True
                 
         
     def countNetsBetweenSymbols(self, sourceSym, sinkSym):
-        wiresFromSource = [source['wire'] for source in self.sources if source['symbol'] == sourceSym]
-        wiresToSink = [sink['wire'] for sink in self.sinks if sink['symbol'] == sinkSym]
+        raise Exception('This counts wires, not ports')
+
+        wiresFromSource = [source['port'].wire for source in self.sources if source['symbol'] == sourceSym]
+        wiresToSink = [sink['port'].wire for sink in self.sinks if sink['symbol'] == sinkSym]
         common = [wire for wire in wiresFromSource if wire in wiresToSink ]
         return len(common)
     
     def placeInputPorts(self):
         """
         Place the input ports of the module 
 
@@ -908,152 +1073,330 @@
         """
         self.x = gridsize
         self.y = gridsize * 5
         
         for inp in self.sys.inPorts:
             isym = InPortSymbol(inp, self.x, self.y)
             self.objs.append(isym)
-            self.y = self.y + gridsize * portSeparation
-            self.sources.append({'symbol':isym, 'x':15, 'y':8+5, 'wire':inp.wire})
+            self.y = self.y + gridsize * LogicSymbol.portSeparation
+            self.sources.append({'symbol':isym, 'x':15, 'y':8+5, 'port':inp})
         
         if (len(self.sys.inPorts) > 0):
             self.x = self.x + 25 * gridsize
             
         # g = genGraph(self.sources)
         # g.add_edge(self.sources)
         # print("Executed")
         # g.col_assignment()
         # g.print_graph()
         self.numInputs = len(self.objs)
         
     def getSymbol(self, obj, x, y):
         try:
-            ret = self.mapping[type(obj)]
+            ret = Schematic.mapping[type(obj)]
     
             #print('getSymbol -> good', obj)
                 
         except:
             #print('getSymbol -> none for object', type(obj))
             return None
 
         return ret(obj, x, y)
         
 
+    def placeInstance(self, child):
+        isym = self.getSymbol(child, self.x, self.y)
+        
+        if (isym is None):
+            isym = InstanceSymbol(child, self.x, self.y)
+        
+        self.objs.append(isym)
+        self.y = self.y + isym.getHeight() + cellmargin * 2 
+
+        i = 0
+        for inp in child.inPorts:
+            #print('adding inport ', child, inp.name)
+            self.sinks.append({'symbol':isym, 'x':0, 'y':8+8+8+5+i*LogicSymbol.portpitch, 'port':inp})
+            i = i+1
+        i = 0
+        for inp in child.outPorts:
+            #print('adding outport ', child, inp.name)
+            self.sources.append({'symbol':isym, 'x':isym.getWidth(), 'y':8+8+8+5+i*LogicSymbol.portpitch, 'port':inp})
+            i = i+1
+                
+        return isym
+    
     def placeInstances(self):
         maxx = 0
         self.y = gridsize*3
         
         #print('placeInstances', self.sys)
+        if (self.showValues):
+            self.x += portvaluemargin
         
         for child in self.sys.children.values():
-            #print('child', child)
-            isym = self.getSymbol(child, self.x, self.y)
-            
-            if (isym is None):
-                isym = InstanceSymbol(child, self.x, self.y)
-            
-            self.objs.append(isym)
-            self.y = self.y + isym.getHeight() + cellmargin * 2 
- 
-            i = 0
-            for inp in child.inPorts:
-                #print('adding inport ', child, inp.name)
-                self.sinks.append({'symbol':isym, 'x':0, 'y':8+8+8+5+i*portpitch, 'wire':inp.wire})
-                i = i+1
-            i = 0
-            for inp in child.outPorts:
-                #print('adding outport ', child, inp.name)
-                self.sources.append({'symbol':isym, 'x':isym.getWidth(), 'y':8+8+8+5+i*portpitch, 'wire':inp.wire})
-                i = i+1
-                    
-    
+            isym = self.placeInstance(child)
             maxx = max(maxx, isym.getWidth())
             
-        self.x = self.x + maxx + gridsize*10 + cellmargin
-        self.grid_yunits = self.y / gridsize
+        self.x += maxx + gridsize*10 + cellmargin + portvaluemargin
         self.grid_yunits = self.y / gridsize
+        self.grid_yunits = self.y / gridsize # @todo should this be x ??
         
     def placeOutputPorts(self):
+        '''
+        Place Output Ports and InOutPorts.
+        This basically means creating an output port symbol for each port and
+        assigning the its y coordinate 
+
+        Returns
+        -------
+        None.
+
+        '''
         #self.x = 1
         self.y = gridsize * 5
         
         self.firstOutput = len(self.objs)
         
         for inp in self.sys.outPorts:
             osym = OutPortSymbol(inp, self.x, self.y)
             self.objs.append(osym)
-            self.y = self.y + gridsize * portSeparation
-            self.sinks.append({'symbol':osym, 'x':0, 'y':8+5, 'wire':inp.wire})
-        
+            self.y = self.y + gridsize * LogicSymbol.portSeparation
+            self.sinks.append({'symbol':osym, 'x':0, 'y':8+5, 'port':inp})
+
+        for inp in self.sys.inOutPorts:
+            osym = InOutPortSymbol(inp, self.x, self.y)
+            self.objs.append(osym)
+            self.y = self.y + gridsize * LogicSymbol.portSeparation
+            self.sinks.append({'symbol':osym, 'x':0, 'y':8+5, 'port':inp})
+            self.sources.append({'symbol':osym, 'x':0, 'y':8+5, 'port':inp})
+
         #self.x = self.x + 3
 
         self.lastOutput = len(self.objs)
 
         
     def findSourceTuple(self, sinkWire:Wire):
         for source in self.sources:
-            if (source['wire'] == sinkWire):
+            if (source['port'].wire == sinkWire):
                 return source
             
         sourceNames = [x['wire'].getFullPath() for x in self.sources]
-        raise Exception('No source to wire "{}" in {}'.format(sinkWire.getFullPath(), sourceNames ) )
+        raise Exception('Could not find a source to wire "{}" in the sources collection {}'.format(sinkWire.getFullPath(), sourceNames ) )
             
     def findSinkTuples(self, sourceWire):
         ret = []
         for sink in self.sinks:
-            if (sink['wire'] == sourceWire):
+            if (sink['port'].wire == sourceWire):
                 ret.append(sink)
         return ret;
             
-    def createNets(self):
+    def createNets(self, debug=False):
         """
         Create nets for all entities in the drawing.
-        It potulates the self.nets list by analyzing the sinks
+        It populates the self.nets list by analyzing the sinks
         list which was collected in function createOutputPorts
 
         Returns
         -------
         None.
 
         """
         for sink in self.sinks:
             try:
-                wire = sink['wire']
+                if (debug):
+                    print('Sink:', sink)
+                    
+                wire = sink['port'].wire
                 source = self.findSourceTuple(wire)
-                self.nets.append(NetSymbol(wire, source['symbol'], sink['symbol']))   
+                sourcecol = self.getSymbolColumn(source['symbol'])
+                sinkcol = self.getSymbolColumn(sink['symbol'])
+
+                net = NetSymbol(wire, source['port'], sink['port'], source['symbol'], sink['symbol'])
+                net.sourcecol = sourcecol
+                net.sinkcol = sinkcol
+                self.nets.append(net)   
             except Exception as err:
                 print('Exception', err)
+                
+        self.maxfanoutwires = []
+
+    # def createNetsWithJoints(self):
+    #     """
+    #     Create nets for all entities in the drawing.
+    #     It populates the self.nets list by analyzing the sinks
+    #     list which was collected in function createOutputPorts
+
+    #     Returns
+    #     -------
+    #     None.
+
+    #     """
+        
+    #     # build a list for all the sinks of a wire
+    #     netSinks = {}
+    #     for src in self.sinks:
+    #         wire = src['wire']
+    #         try:
+    #             symlist = netSinks[wire]
+    #         except:
+    #             symlist = []
+    #         symlist.append(src['symbol'])
+    #         netSinks[wire] = symlist
+
+
+    #     for sink in self.sinks:
+    #         try:
+    #             wire = sink['wire']
+                
+    #             wireSinks = netSinks[wire]
+                
+    #             if (len(wireSinks) == 1):
+    #                 source = self.findSourceTuple(wire)
+    #                 self.nets.append(NetSymbol(wire, source['symbol'], sink['symbol']))   
+    #             else:
+                    
+    #         except Exception as err:
+    #             print('Exception', err)
+                
+    #     self.maxfanoutwires = []
 
+    def createNetsWithMaxFanout(self, maxfanout):
+        """
+        Create nets for all entities in the drawing.
+        It populates the self.nets list by analyzing the sinks
+        list which was collected in function createOutputPorts
+    
+        Returns
+        -------
+        None.
+    
+        """
+        sourceWires = {}
+        for src in self.sinks:
+            wire = src['port'].wire
+            try:
+                symlist = sourceWires[wire]
+            except:
+                symlist = []
+            symlist.append(src['symbol'])
+            sourceWires[wire] = symlist
+            
+        self.maxfanoutwires = [x for x in sourceWires.keys() if len(sourceWires[x]) > maxfanout] 
+            
+        for sink in self.sinks:
+            try:
+                wire = sink['port'].wire
+                
+                fanout = len(sourceWires[wire])
+                
+                if (fanout <= maxfanout):
+                    source = self.findSourceTuple(wire)
+                    self.nets.append(NetSymbol(wire, source['port'], sink['port'], source['symbol'], sink['symbol']))   
+                else:
+                    print('skip wire {} fanout: {}'.format(wire.getFullPath(), fanout))
+                    
+            except Exception as err:
+                print('Exception', err)
+                
     def getNets(self):
         #oa = np.array(self.objs)
         #ba = np.array([isinstance(x, NetSymbol) for x in self.objs])
         #return list(oa[ba])
         return self.nets
     
     def getNonNets(self):
         #oa = np.array(self.objs)
         #ba = np.array([not isinstance(x, NetSymbol) for x in self.objs])
         #return list(oa[ba])
         return self.objs
-    
-    def drawAll(self):
+
+    def createRender(self, physical_shape=None, dpi=None) :
+        """
+        Creates the renderer object
+
+        Parameters
+        ----------
+        physical_shape : tuple, optional
+            Dimension of the physical canvas (in inches). The default is None.
+        dpi : dots per inch, optional
+            Dots per inch of the drawing canvas. The default is None, and it is calculated.
+
+        Raises
+        ------
+        Exception
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
+        render = self.render
+        if (render == 'matplotlib'):
+            self.canvas = MatplotlibRender(self.getOccupancyGrid().shape, physical_shape, dpi)
+        elif (render == 'tkinter'):
+            self.canvas = TkinterRender(self.parent, self.getOccupancyGrid().shape)
+        else:
+            raise Exception('Unsupported render {}'.format(render))
+
+    def drawValues(self, symbol):
+        if (symbol.obj is None):
+            #print('WARNING: no symbol for object', type(symbol))
+            return
+        if not(hasattr(symbol.obj, 'inPorts')):
+            return
+        
+        for port in symbol.obj.inPorts:
+            wire = port.wire
+            pos = symbol.getPortSinkPos(port)
+            self.canvas.drawText(symbol.x + pos[0] - portvaluemargin,
+                                 symbol.y + pos[1] - gridsize * 2,
+                                 '{:X}'.format(wire.get()), 'w')
+        for port in symbol.obj.outPorts:
+            wire = port.wire
+            pos = symbol.getPortSourcePos(port)
+            self.canvas.drawText(symbol.x + pos[0] + portvaluemargin,
+                                 symbol.y + pos[1] - gridsize * 2,
+                                 '{:X}'.format(wire.get()), 'e')
+
+
+    def drawAll(self, debug=False):
+        if (self.canvas is None):
+            self.createRender()
+            
+        self.canvas.setForecolor('k')
+
         # Draw Instances
+        
+        # @todo the color and line properties should be assigned during creation 
+        # so that they can later be manipulated by applications before drawing
         for obj in self.getNonNets():
             self.canvas.setForecolor('k')  
             self.canvas.setFillcolor('k')
             self.canvas.setLineWidth(2)
-            obj.draw(self.canvas)
+            if (debug):
+                print('draw', type(obj))
+            
+            obj.draw(self.canvas, debug=debug)
+            
+            if (self.showValues):
+                self.drawValues(obj)
 
         # Draw Nets
         for obj in self.getNets():
-            self.canvas.setForecolor('blueviolet')  
-            self.canvas.setFillcolor('blueviolet')
+            
+            self.canvas.setForecolor(obj.color)  
+            self.canvas.setFillcolor(obj.color)
             self.canvas.setLineWidth(1)
+
+            if (debug):
+                print('draw', type(obj))
             
-            obj.draw(self.canvas)
+            obj.draw(self.canvas, debug=debug)
         
         return self.canvas
     
     def getAdjacencyMatrix(self):
         """
         
         Returns
@@ -1086,14 +1429,23 @@
 
         return cost
     
     def swap(self, a, b):
         self.objs[a], self.objs[b] = self.objs[b], self.objs[a] 
 
     def bruteForceSort(self):
+        """
+        Sort the object list
+
+        Returns
+        -------
+        am : TYPE
+            DESCRIPTION.
+
+        """
         am = self.getAdjacencyMatrix()
         nc = am.shape[0]
 
         timelimit = 10
 
         import time
         
@@ -1127,34 +1479,39 @@
                             anychange = True
                             
                             #print(self.getAdjacencyMatrix())
 
             #print('iter', k, 'cost:', cost, anychange)
                     
             if ((time.time() - t0) > timelimit):
+                print('WARNING: time limit reached in sort')
                 anychange = False
                 
             if (not anychange):
                 break
 
         am = self.getAdjacencyMatrix()
         return am
 
     def areSourceTarget(self, srcobj, trgobj):
         if (isinstance(srcobj, InPortSymbol)):
             outwires = [srcobj.obj.wire]
         elif (isinstance(srcobj, OutPortSymbol)):
             outwires = []
+        elif (isinstance(srcobj, InOutPortSymbol)):
+            outwires = [srcobj.obj.wire] # @todo is this what we should do ?
         else:
             outwires = [outport.wire for outport in srcobj.obj.outPorts]
         
         if (isinstance(trgobj, InPortSymbol)):
             inwires = []
         elif (isinstance(trgobj, OutPortSymbol)):
             inwires = [trgobj.obj.wire]
+        elif (isinstance(trgobj, InOutPortSymbol)):
+            inwires = [trgobj.obj.wire] # @todo check this, not sure if we should put more wires here
         else:
             inwires = [inport.wire for inport in trgobj.obj.inPorts]
         
         inter = Intersection(inwires, outwires)
         
         #print('Intersection ', srcobj.obj.getFullPath(), trgobj.obj.getFullPath(), '=', len(inter))
         
@@ -1187,15 +1544,16 @@
             h = obj.y + obj.getHeight() + cellmargin
             if (w > maxw): maxw = w
             if (h > maxh): maxh = h
             
         if (mode == 'prerouting'):
             maxh = maxh*2
             
-        grid = np.zeros((maxh,maxw))
+        #print('ocupancy grid = ', maxh, maxw)
+        grid = np.zeros((maxh, maxw))
         
         for obj in self.getNonNets():
             if (obj in discard):
                 continue
 
             x = obj.x
             y = obj.y
@@ -1241,15 +1599,29 @@
             
             v = np.max(og[y0:y1+1, x0:x1+1])
         except:
             return False
         
         return v == 0
         
-    def routeNet(self, net:NetSymbol):
+    def routeNetSquare(self, net:NetSymbol):
+        """
+        Route a single net. The process consist in assigning 
+        a collection of points (path) to go from a source to a destination
+
+        Parameters
+        ----------
+        net : NetSymbol
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
         p0 = net.getStartPoint()
         pf = net.getEndPoint()
         
 
         sw = 0
         try:
             sw = self.channels[net.sourcecol]['sourcewidth'] 
@@ -1262,40 +1634,122 @@
                 net.track = 0
             else:
                 print('error sourcecol=', net.sourcecol)
                 print('channels[{}]'.format(net.sourcecol), self.channels[net.sourcecol])
                 print('source sym', net.source)
         
         if (hasattr(net, 'track') == False):
-            print('WARNING: net', net.source['wire'].getFullPath(), 'with not track')
+            print('WARNING: net', net.source, 'with not track')
             net.track = 0
 
-        mp = (net.source.x + sw + netspacing + net.track * nettrackspacing, (p0[1]+pf[1])//2)    
             
         if (isinstance(net.source, FeedbackStopSymbol)):
-            #print('Feedback-stop track:', net.track, mp[0])
-            net.setPath([mp[0], mp[0], pf[0]], [p0[1],pf[1],pf[1]])
+            # In stop symbols, the source and sink are in the same column
+            if (isinstance(net.sink, FeedbackStartSymbol) or isinstance(net.sink, PassthroughSymbol)):
+                # Normal case, midpoint is between both elements
+                mp = (net.source.x + sw + netspacing + net.track * nettrackspacing, (p0[1]+pf[1])//2)                
+                net.setPath([p0[0], mp[0], mp[0], pf[0]], [p0[1],p0[1],pf[1],pf[1]])
+            else:
+                mp = (net.source.x  - netspacing - net.track * nettrackspacing, -1)
+    
+                #print('Feedback-stop track:', net.track, mp[0])
+                #net.setPath([mp[0], mp[0], pf[0]], [p0[1],pf[1],pf[1]])
+                net.setPath([p0[0], mp[0], mp[0], pf[0]], [p0[1], p0[1], pf[1], pf[1]])
         elif (isinstance(net.sink, FeedbackStartSymbol)):
+            # In start symbols, the source and sink are in the same column, 
+            # midpoint is similar to normal case (in x)
+            mp = (net.source.x + sw + netspacing + net.track * nettrackspacing, -1)                
+            
             #print('Feedback-start track:', net.track, mp[0])
-            net.setPath([p0[0], mp[0], mp[0]], [p0[1],p0[1],pf[1]])
-        else:                  
+            net.setPath([p0[0], mp[0], mp[0], pf[0]], [p0[1], p0[1], pf[1], pf[1]])
+        else:                 
+            # Normal case, midpoint is between both elements
+            mp = (net.source.x + sw + netspacing + net.track * nettrackspacing, (p0[1]+pf[1])//2)                
             net.setPath([p0[0], mp[0], mp[0], pf[0]], [p0[1],p0[1],pf[1],pf[1]])
 
         #mp[0] = p0[0] + net.track * nettrackspacing
         
         net.routed = True
     
+    def routeNetDirect(self, net:NetSymbol):
+        """
+        Route a single net. The process consist in assigning 
+        a collection of points (path) to go from a source to a destination
+
+        Parameters
+        ----------
+        net : NetSymbol
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
+        p0 = net.getStartPoint()
+        pf = net.getEndPoint()
+        
+
+        # sw = 0
+        # try:
+        #     sw = self.channels[net.sourcecol]['sourcewidth'] 
+        #     #sw = sw - net.source['symbol'].getWidth() + netspacing
+        #     #print('sw[{}]={}'.format(net.sourcecol, sw))
+        # except:
+        #     if (hasattr(net, 'sourcecol') == False):
+        #         # this net was not assigned a sourcecol
+        #         print('WARNING: net', net.source['wire'].getFullPath(), 'without source column')
+        #         net.track = 0
+        #     else:
+        #         print('error sourcecol=', net.sourcecol)
+        #         print('channels[{}]'.format(net.sourcecol), self.channels[net.sourcecol])
+        #         print('source sym', net.source)
+        
+        # if (hasattr(net, 'track') == False):
+        #     print('WARNING: net', net.source['wire'].getFullPath(), 'with not track')
+        #     net.track = 0
+
+        # mp = (net.source.x + sw + netspacing + net.track * nettrackspacing, (p0[1]+pf[1])//2)    
+            
+        # if (isinstance(net.source, FeedbackStopSymbol)):
+        #     #print('Feedback-stop track:', net.track, mp[0])
+        #     net.setPath([mp[0], mp[0], pf[0]], [p0[1],pf[1],pf[1]])
+        # elif (isinstance(net.sink, FeedbackStartSymbol)):
+        #     #print('Feedback-start track:', net.track, mp[0])
+        #     net.setPath([p0[0], mp[0], mp[0]], [p0[1],p0[1],pf[1]])
+        # else:                  
+        #     net.setPath([p0[0], mp[0], mp[0], pf[0]], [p0[1],p0[1],pf[1],pf[1]])
+
+        net.setPath([p0[0], pf[0]], [p0[1],pf[1]])
+
+        #mp[0] = p0[0] + net.track * nettrackspacing
+        
+        net.routed = True
     
-    def routeNets(self):
+    def routeNets(self, mode='square'):
+        """
+        Route all the nets
+
+        Returns
+        -------
+        None.
+
+        """
         nets = self.getNets()
         
-        for net in nets:
-            # route net
-            self.routeNet(net)
-                        
+        if (mode == 'square'):
+            for net in nets:
+                # route net
+                self.routeNetSquare(net)
+        elif (mode == 'direct'):
+            for net in nets:
+                # route net
+                self.routeNetDirect(net)
+        else:
+            raise Exception('Unsupported net routing mode {}'.format(mode))
 
         # for inp in self.obj.outPorts:
         #     canvas.create_text(x+15-2, y, text=inp.name , anchor='e')
         #     y = y+8
         #     canvas.create_polygon(x, y, x+10, y, x+15, y+5, x+10, y+10, x, y+10)
         #     y = y+portpitch-8
```

### Comparing `py4hw-0.0.9/py4hw/schematic_symbols.py` & `py4hw-2024.1/py4hw/schematic_symbols.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,118 +4,181 @@
 
 @author: dcr
 """
 from .logic.bitwise import *
 from .base import Wire
 import math
 
-gridsize = 5
-portpitch = 28
-cellmargin = 50
-portSeparation = 10
-
-namemargin = 8
-portmargin = 8
-instanceportwidth = 4
-instanceportheight = 10
-instanceporttextmargin = 10
+
  
 #
 #  name              name margin
 #  +------------+
 #  |            |   portmargin          \
 #  | i0      o0 |   instanceportheight  |
 #  |            |                       |
 #  | i1         |                       /- port pitch
 #  |            |
 #  +------------+
 
 class LogicSymbol:
+    gridsize = 5
+    portpitch = 28
+    cellmargin = 50
+    portSeparation = 10
+
+    namemargin = 8
+    portmargin = 8
+    instanceportwidth = 4
+    instanceportheight = 10
+    instanceporttextmargin = 10
+
     def __init__(self, obj:Logic, x:int, y:int):
         self.obj = obj
         self.x = x
         self.y = y
+        self.instanceWidth = self.computeWidth() 
+        #print('instance width:', self.instanceWidth)
+        
+    def getTextExtend(self, text):
+        from matplotlib.textpath import TextPath
+
+        fontsize = 12
+        
+        path = TextPath((0, 0), text, size=fontsize)
+        
+        text_width = path.get_extents().width
+        #text_height = path.get_extents().height
+        return text_width
+
+    def getInPortsWidth(self):
+        inMaxWidth = 0
+        if (hasattr(self.obj, 'inPorts')):
+            for idx, port in enumerate(self.obj.inPorts):
+                inMaxWidth = max(inMaxWidth, self.getTextExtend(port.name))
+        return inMaxWidth
+    
+    def getOutPortsWidth(self):
+        outMaxWidth = 0
+        if (hasattr(self.obj, 'outPorts')):
+            for idx, port in enumerate(self.obj.outPorts):
+                outMaxWidth = max(outMaxWidth, self.getTextExtend(port.name))
+        return outMaxWidth
+                                
+    
+    def computeWidth(self):
+        outMaxWidth = self.getOutPortsWidth()
+        inMaxWidth = self.getInPortsWidth()
+        
+        return int(outMaxWidth * 1.5  +  LogicSymbol.gridsize*10 + inMaxWidth * 1.5 )
+
+    def getPortSourcePos(self, refport):
+        selidx = -1
+        for idx, port in enumerate(self.obj.outPorts):
+            if (port.name == refport.name):
+                selidx = idx
                 
+        if (selidx == -1):
+            raise Exception('out port {} not found in {}'.format(refport.name, self.obj.getFullPath()) )
+
+
+        return (self.getWidth(), LogicSymbol.namemargin + LogicSymbol.portmargin + selidx*LogicSymbol.portpitch + LogicSymbol.instanceportheight//2)
         
     def getWireSourcePos(self, wire:Wire):
+        # TODO remove
+        raise Exception('use port one')
         selidx = -1
         for idx, port in enumerate(self.obj.outPorts):
             if (port.wire == wire):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('out port not found in {}'.format(self.obj.getFullPath()) )
 
 
-        return (self.getWidth(), namemargin + portmargin + selidx*portpitch + instanceportheight//2)
+        return (self.getWidth(), LogicSymbol.namemargin + LogicSymbol.portmargin + selidx*LogicSymbol.portpitch + LogicSymbol.instanceportheight//2)
+
+    def getPortSinkPos(self, portref):
+        selidx = -1
+        for idx, port in enumerate(self.obj.inPorts):
+            if (port == portref):
+                selidx = idx
+                
+        if (selidx == -1):
+            raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
+
+        
+        return (0, LogicSymbol.namemargin + LogicSymbol.portmargin + selidx*LogicSymbol.portpitch + LogicSymbol.instanceportheight//2)
     
     def getWireSinkPos(self, wire:Wire):
+        # TODO remove
+        raise Exception('use port one')
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
             if (port.wire == wire):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
 
         
-        return (0, namemargin + portmargin + selidx*portpitch + instanceportheight//2)
+        return (0, LogicSymbol.namemargin + LogicSymbol.portmargin + selidx*LogicSymbol.portpitch + LogicSymbol.instanceportheight//2)
 
     def getHeight(self):
-        return namemargin + 2*portmargin + max(len(self.obj.inPorts), len(self.obj.outPorts)) * portpitch 
+        return LogicSymbol.namemargin + 2*LogicSymbol.portmargin + max(len(self.obj.inPorts), len(self.obj.outPorts)) * LogicSymbol.portpitch 
     
     def getWidth(self):
-        return 25 * gridsize    
+        return self.instanceWidth    
 
     def getOccupancy(self):
         return {'x':self.x, 'y':self.y, 'w':self.getWidth(), 'h':self.getHeight()}
 
 class BinaryOperatorSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         canvas.drawText(x+25, y+25+5, self.operator, anchor='c')
         canvas.drawEllipse(x, y, x+50, y+50)
         #canvas.drawLine(x, y, x + 40, y)
         #canvas.drawLine(x, y + 40, x + 40, y + 40)
         #canvas.drawLine(x, y, x, y + 40)
         #canvas.drawArc(x + 20, y, x + 50, y + 40, start=-90, extent=180) #, style=tkinter.ARC, outline='black', fill='white')
 
     def getHeight(self):
-        return 50 + namemargin
+        return 50 + LogicSymbol.namemargin
 
     def getWidth(self):
         return 50 
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + 25)
+    def gePortSourcePos(self, wire:Wire):
+        return (self.getWidth(), LogicSymbol.namemargin + 25)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
-            raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
+            raise Exception('in port {} not found in {}'.format(self.obj.getFullPath()) )
 
         x = int(math.cos(math.pi/4)*25)
         y = int(math.sin(math.pi/4)*25)
 
         if (selidx == 0):
             y = -y
 
-        return (25-x, namemargin + 25 + y)
+        return (25-x, LogicSymbol.namemargin + 25 + y)
 
 
 class AddSymbol(BinaryOperatorSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         self.operator = '+'
 
@@ -128,383 +191,423 @@
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         self.operator = '*'
     
 class AndSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
-        self.h = 40
 
-    def draw(self, canvas):
+        if (isinstance(obj, And2)):
+            self.nins = 2
+        else:
+            self.nins = len(obj.ins)
+
+        self.h = 20 * self.nins
+
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         # the and box would be x[0:50] y[0:30]
         canvas.drawLine(x, y, x + 25, y)
         canvas.drawLine(x, y + self.h, x + 25, y + self.h)
         canvas.drawLine(x, y, x, y + self.h)
-        canvas.drawArc(x , y+2, x + 50, y + self.h, start=-90, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
+        canvas.drawArc(x , y+2, x + 50, y + self.h, start=-90, stop=90) #, style=tkinter.ARC, outline='black', fill='white')
 
     def getHeight(self):
-        return namemargin + self.h
+        return LogicSymbol.namemargin + self.h
 
     def getWidth(self):
         return 50
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + self.h//2)
+    def getPortSourcePos(self, refport):
+        return (self.getWidth(), LogicSymbol.namemargin + self.h//2)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
+        inlist = []
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            inlist.append(port.name)
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
-            raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
+            raise Exception('in port {} not found in {}. Object in ports: {}'.format(refport.name, self.obj.getFullPath(), inlist) )
 
-        if (selidx == 0):
-            y = self.h//2 - 10
-        else:
-            y = self.h//2 + 10 
+        y = 10 + selidx * 20
 
-        return (0, namemargin + y)
+        return (5, LogicSymbol.namemargin + y)
 
 class NotSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin 
+        y = y + LogicSymbol.namemargin 
 
         y = y + 10
 
         canvas.drawPolygon([x, x + 30, x, x], [y, y + 15, y + 30, y])
         canvas.drawEllipse(x + 30, y + 10, x + 40, y + 20)
 
     def getHeight(self):
         return 30
 
     def getWidth(self):
         return 40
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + 25)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + 25)
     
-    def getWireSinkPos(self, wire:Wire):
-        return (0, namemargin + 25)
+    def getPortSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 25)
     
     
 class BufSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin 
+        y = y + LogicSymbol.namemargin 
 
         canvas.drawPolygon([x, x + 20, x, x], [y, y + 10, y + 20, y])
         
     def getHeight(self):
         return 20
 
     def getWidth(self):
         return 20
 
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + 10)
+    def getWireSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + 10)
     
-    def getWireSinkPos(self, wire:Wire):
-        return (0, namemargin + 10)
+    def getWireSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 10)
     
 class BitSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text='[{}]'.format(self.obj.bit), anchor='w')
-        y = y + namemargin 
+        y = y + LogicSymbol.namemargin 
 
         canvas.drawLine(x+10,y, x, y+20)
         #canvas.drawPolygon([x, x + 20, x, x], [y, y + 10, y + 20, y])
         
     def getHeight(self):
         return 20
 
     def getWidth(self):
         return 20
 
-    def getWireSourcePos(self, wire:Wire):
-        return (10, namemargin + 10)
+    def getPortSourcePos(self, port):
+        return (10, LogicSymbol.namemargin + 10)
     
-    def getWireSinkPos(self, wire:Wire):
-        return (0, namemargin + 10)
+    def getPortSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 10)
     
 class RangeSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text='[{}:{}]'.format(self.obj.high, self.obj.low), anchor='w')
-        y = y + namemargin 
+        y = y + LogicSymbol.namemargin 
 
         canvas.drawLine(x+10,y, x, y+20)
         #canvas.drawPolygon([x, x + 20, x, x], [y, y + 10, y + 20, y])
         
     def getHeight(self):
         return 20
 
     def getWidth(self):
         return 20
 
-    def getWireSourcePos(self, wire:Wire):
-        return (10, namemargin + 10)
+    def getPortSourcePos(self, port):
+        return (10, LogicSymbol.namemargin + 10)
     
-    def getWireSinkPos(self, wire:Wire):
-        return (0, namemargin + 10)
+    def getPortSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 10)
     
 class NorSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         self.h = 40
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         # the and box would be x[0:50] y[0:30]
         canvas.drawLine(x, y, x + 20, y)
         canvas.drawLine(x, y + self.h, x + 20, y + self.h)
         canvas.drawArc(x-10 , y, x + 10, y + self.h, start=-90, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
 
         #canvas.drawLine(x, y, x, y + self.h)
         canvas.drawArc(x-30 , y, x + 50+20, y + self.h*4, start=-90, extent=-60) #, style=tkinter.ARC, outline='black', fill='white')
         canvas.drawArc(x-30 , y-self.h*3, x + 50+20, y + self.h, start=60, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
 
         canvas.drawEllipse(x + 55, y + 15, x + 65, y + 25)
 
     def getHeight(self):
-        return namemargin + self.h
+        return LogicSymbol.namemargin + self.h
 
     def getWidth(self):
         return 65
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + self.h//2)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + self.h//2)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
 
         if (selidx == 0):
             y = self.h//2 - 10
         else:
             y = self.h//2 + 10 
 
-        return (5, namemargin + y)
+        return (5, LogicSymbol.namemargin + y)
     
 class OrSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         
         if (isinstance(obj, Or2)):
             self.nins = 2
         else:
             self.nins = len(obj.ins)
 
         self.h = 20 * self.nins
         
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         # the and box would be x[0:50] y[0:30]
         canvas.drawLine(x, y, x + 20, y)
         canvas.drawLine(x, y + self.h, x + 20, y + self.h)
-        canvas.drawArc(x-10 , y, x + 10, y + self.h, start=-90, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
+        canvas.drawArc(x-10 , y, x + 10, y + self.h, start=-90, stop=90) #, style=tkinter.ARC, outline='black', fill='white')
 
         #canvas.drawLine(x, y, x, y + self.h)
         #canvas.drawArc(x-30 , y, x + 50+20, y + self.h + (self.nins+1)*40, start=-90, extent=-60) #, style=tkinter.ARC, outline='black', fill='white')
         #canvas.drawArc(x-30 , y - (self.nins+1)*40, x + 50+20, y + self.h, start=60, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
         canvas.drawSpline([x+20, x+30, x+42, x+50], [y,  y+2, y+self.h//4, y+self.h//2])
         canvas.drawSpline([x+20, x+30, x+42, x+50], [y+self.h,  y+self.h-2, y+self.h-self.h//4, y+self.h//2])
 
     def getHeight(self):
-        return namemargin + self.h
+        return LogicSymbol.namemargin + self.h
 
     def getWidth(self):
         return 50
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + self.h//2)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + self.h//2)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
 
         y = 10 + selidx * 20
 
-        return (5, namemargin + y)
+        return (5, LogicSymbol.namemargin + y)
     
 class XorSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         self.h = 40
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         # the and box would be x[0:50] y[0:30]
         canvas.drawLine(x+10, y, x + 20+10, y)
         canvas.drawLine(x+10, y + self.h, x + 20+10, y + self.h)
-        canvas.drawArc(x-10 , y, x + 10, y + self.h, start=-90, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
-        canvas.drawArc(x , y, x + 20, y + self.h, start=-90, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
+        canvas.drawArc(x-10 , y, x + 10, y + self.h, start=-90, stop=90) #, style=tkinter.ARC, outline='black', fill='white')
+        canvas.drawArc(x , y, x + 20, y + self.h, start=-90, stop=90) #, style=tkinter.ARC, outline='black', fill='white')
 
-        canvas.drawArc(x-30 +10, y, x + 50+20+10, y + self.h*4, start=-90, extent=-60) #, style=tkinter.ARC, outline='black', fill='white')
-        canvas.drawArc(x-30 +10, y-self.h*3, x + 50+20+10, y + self.h, start=60, extent=90) #, style=tkinter.ARC, outline='black', fill='white')
+        #canvas.drawArc(x-30 +10, y, x + 50+20+10, y + self.h*4, start=-90, stop=-60) #, style=tkinter.ARC, outline='black', fill='white')
+        #canvas.drawArc(x-30 +10, y-self.h*3, x + 50+20+10, y + self.h, start=60, stop=90) #, style=tkinter.ARC, outline='black', fill='white')
+        canvas.drawSpline([x+20+10, x+30+10, x+42+10, x+50+10], [y,  y+2, y+self.h//4, y+self.h//2])
+        canvas.drawSpline([x+20+10, x+30+10, x+42+10, x+50+10], [y+self.h,  y+self.h-2, y+self.h-self.h//4, y+self.h//2])
 
 
 
     def getHeight(self):
-        return namemargin + self.h
+        return LogicSymbol.namemargin + self.h
 
     def getWidth(self):
         return 50+10
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + self.h//2)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + self.h//2)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
 
         if (selidx == 0):
             y = self.h//2 - 10
         else:
             y = self.h//2 + 10 
 
-        return (5, namemargin + y)
+        return (5, LogicSymbol.namemargin + y)
     
 class InPortSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x 
         y = self.y 
         canvas.drawText(x, y, text=self.obj.name , anchor='w')
-        y = y+namemargin 
+        y = y+LogicSymbol.namemargin 
         
         canvas.drawPolygon([x, x+10, x+15, x+10,x,x], [y, y, y+5, y+10, y+10, y])
 
     def getWidth(self):
         return 15;
     
     def getHeight(self):
         return 20;
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin +5)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin +5)
     
 class OutPortSymbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x 
         y = self.y 
         canvas.drawText(x, y, text=self.obj.name , anchor='w')
-        y = y+namemargin 
+        y = y+LogicSymbol.namemargin 
         
         canvas.drawPolygon([x, x+10, x+15, x+10, x, x], [y, y, y+5, y+10, y+10, y])
 
     def getWidth(self):
         return 15;
     
     def getHeight(self):
         return 20;
     
-    def getWireSinkPos(self, wire:Wire):
-        return (0, namemargin + 5)
+    def getPortSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 5)
+
+class InOutPortSymbol(LogicSymbol):
+    def __init__(self, obj, x, y):
+        super().__init__(obj, x, y)
+        
+    def draw(self, canvas, debug=False):
+        x = self.x 
+        y = self.y 
+        canvas.drawText(x, y, text=self.obj.name , anchor='w')
+        y = y+LogicSymbol.namemargin 
+        
+        canvas.drawPolygon([x, x+5, x+10, x+15, x+10, x+5, x], [y+5, y, y, y+5, y+10, y+10, y+5])
+
+    def getWidth(self):
+        return 20;
+    
+    def getHeight(self):
+        return 20;
+    
+    def getPortSinkPos(self, port):
+        return (0, LogicSymbol.namemargin + 5)
+    
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin +5)
+
     
 class InstanceSymbol(LogicSymbol):
     def __init__(self, obj:Logic, x:int, y:int):
         super().__init__(obj, x, y)
     
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x 
         y = self.y 
         
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y+namemargin 
+        y = y + LogicSymbol.namemargin 
         
-        canvas.drawRectangle(x, y, x + self.getWidth(), y + self.getHeight() - namemargin)
+        #print('instance symbol width:', self.getWidth())
+        canvas.drawRectangle(x, y, x + self.getWidth(), y + self.getHeight() - LogicSymbol.namemargin)
 
-        ipw = instanceportwidth 
-        iph = instanceportheight
+        ipw = LogicSymbol.instanceportwidth 
+        iph = LogicSymbol.instanceportheight
         iphh = iph//2
-        iptm = instanceporttextmargin
+        iptm = LogicSymbol.instanceporttextmargin
 
-        y = y + portmargin
+        y = y + LogicSymbol.portmargin
         
         for inp in self.obj.inPorts:
             canvas.drawPolygon([x, x+ipw, x+ipw+iphh, x+ipw, x,x], [y, y, y+iphh, y+iph, y+iph,y])
             canvas.drawText(x+ipw+iph, y+iptm, text=inp.name , anchor='w')
-            y = y+portpitch
+            y = y+LogicSymbol.portpitch
             
-        y = self.y + namemargin + portmargin
+        y = self.y + LogicSymbol.namemargin + LogicSymbol.portmargin
         
 
         for inp in self.obj.outPorts:
             x = self.x + self.getWidth() - ipw - iphh 
             canvas.drawPolygon([x, x+ipw, x+ipw+iphh, x+ipw, x, x], [y, y, y+iphh, y+iph, y+iph, y])
             x = self.x + self.getWidth() - ipw - iph -iphh
             canvas.drawText(x, y+iptm, text=inp.name , anchor='e')
-            y = y+portpitch
+            y = y+LogicSymbol.portpitch
+
+        for inp in self.obj.inOutPorts:
+            x = self.x + self.getWidth() - ipw - iphh 
+            canvas.drawPolygon([x, x+ipw, x+ipw+iphh, x+ipw, x, x], [y, y, y+iphh, y+iph, y+iph, y])
+            x = self.x + self.getWidth() - ipw - iph -iphh
+            canvas.drawText(x, y+iptm, text=inp.name , anchor='e')
+            y = y+LogicSymbol.portpitch
         
         
 class RegSymbol(InstanceSymbol):
     def __init__(self, obj:Logic, x:int, y:int):
         super().__init__(obj, x, y)
         
     def getWidth(self):
@@ -516,52 +619,52 @@
         
     def getWidth(self):
         return 80
     
     def getHeight(self):
         return 80
     
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x 
         y = self.y 
         
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y+namemargin 
+        y = y+LogicSymbol.namemargin 
 
         canvas.setFillcolor('lightsalmon')
-        canvas.drawRectangle(x, y, x + self.getWidth(), y + self.getHeight() - namemargin, fill=True)
+        canvas.drawRectangle(x, y, x + self.getWidth(), y + self.getHeight() - LogicSymbol.namemargin, fill=True)
 
-        ipw = instanceportwidth 
-        iph = instanceportheight
+        ipw = LogicSymbol.instanceportwidth 
+        iph = LogicSymbol.instanceportheight
         iphh = iph//2
-        iptm = instanceporttextmargin
+        iptm = LogicSymbol.instanceporttextmargin
 
-        y = y + portmargin
+        y = y + LogicSymbol.portmargin
         
         for inp in self.obj.inPorts:
             canvas.drawPolygon([x, x+ipw, x+ipw+iphh, x+ipw, x,x], [y, y, y+iphh, y+iph, y+iph,y])
             #canvas.drawText(x+ipw+iph, y+iptm, text=inp.name , anchor='w')
-            y = y+portpitch
+            y = y+LogicSymbol.portpitch
             
-        y = self.y + namemargin + portmargin
+        y = self.y + LogicSymbol.namemargin + LogicSymbol.portmargin
         
         canvas.setFillcolor('white')
-        canvas.drawRoundRectangle(x+25, y+20, x+self.getWidth()-25, y-20+self.getHeight()-namemargin-20, radius=10, fill=True)
+        canvas.drawRoundRectangle(x+25, y+20, x+self.getWidth()-25, y-20+self.getHeight()-LogicSymbol.namemargin-20, radius=10, fill=True)
         
 class Mux2Symbol(LogicSymbol):
     def __init__(self, obj, x, y):
         super().__init__(obj, x, y)
         self.h = 20*3
 
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
 
         canvas.drawText(x, y, text=self.obj.name, anchor='w')
-        y = y + namemargin
+        y = y + LogicSymbol.namemargin
 
         canvas.setForecolor('blueviolet')  
         canvas.setLineWidth(1)
         canvas.drawLine(x, y+10, x+15, y+10)
         canvas.drawLine(x+15, y+10, x+15, y+25)
 
         y = y+20
@@ -581,132 +684,145 @@
         ars = 3
         x = x + 15
         y = y + 5
         canvas.drawPolygon([x-ars+1,x+1,x+ars+1, x-ars+1], [y-ars*2, y, y-ars*2, y-ars*2], fill=True)
 
 
     def getHeight(self):
-        return namemargin + self.h
+        return LogicSymbol.namemargin + self.h
 
     def getWidth(self):
         return 20
     
-    def getWireSourcePos(self, wire:Wire):
-        return (self.getWidth(), namemargin + 40)
+    def getPortSourcePos(self, port):
+        return (self.getWidth(), LogicSymbol.namemargin + 40)
     
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, refport):
         selidx = -1
         for idx, port in enumerate(self.obj.inPorts):
-            if (port.wire == wire):
+            if (port.name == refport.name):
                 selidx = idx
                 
         if (selidx == -1):
             raise Exception('in port not found in {}'.format(self.obj.getFullPath()) )
 
         if (selidx == 0):
             y = 10
         elif (selidx == 1):
             y = 30 
         else:
             y = 50 
 
-        return (0, namemargin + y)
+        return (0, LogicSymbol.namemargin + y)
 
 class PassthroughSymbol(LogicSymbol):
     def __init__(self):
         super().__init__(None, 0, 0)
         
     def getHeight(self):
         return 30
     
     def getWidth(self):
         return 30
     
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
-        
-        canvas.setForecolor('blueviolet')  
-        canvas.setLineWidth(1)
-        
-        #canvas.drawRectangle(x, y, x+30, y+30)
-        canvas.drawLine(x, y+15, x+30, y+15)
 
-        canvas.setForecolor('k')  
-        canvas.setLineWidth(2)
+        if (debug):       
+            canvas.setFillcolor('yellow')  
+            canvas.drawRectangle(x, y, x+30, y+30, fill=True)
+        else:
+            canvas.setForecolor('blueviolet')  
+            canvas.setLineWidth(1)
+            
+            canvas.drawLine(x, y+15, x+30, y+15)
+    
+            canvas.setForecolor('k')  
+            canvas.setLineWidth(2)
         
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, port):
         return (0, 15);
     
-    def getWireSourcePos(self, wire:Wire):
+    def getPortSourcePos(self, port):
         return (30, 15);
     
 class FeedbackStartSymbol(LogicSymbol):
     def __init__(self):
         super().__init__(None, 0, 0)
         
     def getHeight(self):
         return 30
     
     def getWidth(self):
         return 30
     
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
-        
-        canvas.setForecolor('red')  
-        canvas.setLineWidth(1)
-        
-        #canvas.drawRectangle(x, y, x+30, y+30)
-        canvas.drawLine(x, y+15, x+30, y+15)
 
-        canvas.setForecolor('k')  
-        canvas.setLineWidth(2)
+        if (debug):       
+            canvas.setFillcolor('lightgreen')  
+            canvas.drawRectangle(x, y, x+30, y+30, fill=True)
+        else:            
+            # canvas.setForecolor('red')  
+            # canvas.setLineWidth(1)
+            
+            # canvas.drawLine(x, y+15, x+30, y+15)
         
-    def getWireSinkPos(self, wire:Wire):
+            # canvas.setForecolor('k')  
+            # canvas.setLineWidth(2)
+            pass
+        
+    def getPortSinkPos(self, port):
         return (0, 15);
     
-    def getWireSourcePos(self, wire:Wire):
+    def getPortSourcePos(self, port):
         return (30, 15);
     
 class FeedbackStopSymbol(LogicSymbol):
     def __init__(self):
         super().__init__(None, 0, 0)
+        self.debug = False
         
     def getHeight(self):
         return 30
     
     def getWidth(self):
         return 30
     
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         x = self.x
         y = self.y
-        
-        canvas.setForecolor('red')  
-        canvas.setLineWidth(1)
-        
-        #canvas.drawRectangle(x, y, x+30, y+30)
-        canvas.drawLine(x, y+15, x+30, y+15)
 
-        canvas.setForecolor('k')  
-        canvas.setLineWidth(2)
+        if (debug):       
+            canvas.setFillcolor('red')  
+            canvas.drawRectangle(x, y, x+30, y+30, fill=True)
+        else:
+            # canvas.setForecolor('red')  
+            # canvas.setLineWidth(1)
+            
+            # #canvas.drawRectangle(x, y, x+30, y+30)
+            # canvas.drawLine(x, y+15, x+30, y+15)
+    
+            # canvas.setForecolor('k')  
+            # canvas.setLineWidth(2)
+            pass
         
-    def getWireSinkPos(self, wire:Wire):
+    def getPortSinkPos(self, port):
         return (0, 15);
     
-    def getWireSourcePos(self, wire:Wire):
+    def getPortSourcePos(self, port):
         return (30, 15);
     
     
 class NetSymbol:
-    def __init__(self, wire:Wire, source:LogicSymbol, sink:LogicSymbol):
+    def __init__(self, wire:Wire, sourcePort, sinkPort, source:LogicSymbol, sink:LogicSymbol):
         """
-        Constructor of net symbol
+        A net symbol connects two entities.
 
         Parameters
         ----------
         wire : Wire
             Associated wire.
         source : LogicSymbol
             source logic symbol.
@@ -715,36 +831,41 @@
 
         Returns
         -------
         None.
 
         """
         self.wire = wire
+        self.sourcePort = sourcePort
+        self.sinkPort = sinkPort
         self.source = source
         self.sink = sink
         self.x = None
         self.y = None
         self.routed = False
         self.arrow = True
+        self.color = 'blueviolet'
+        self.sourcecol = -1
+        # self.sinkcol will be assigned later
         
     def getStartPoint(self):
         objsource = self.source
-        portsource = objsource.getWireSourcePos(self.wire)
+        portsource = objsource.getPortSourcePos(self.sourcePort)
         return (objsource.x + portsource[0], objsource.y + portsource[1]) 
     
     def getEndPoint(self):
         objsink = self.sink
-        portsink = objsink.getWireSinkPos(self.wire)
+        portsink = objsink.getPortSinkPos(self.sinkPort)
         return (objsink.x + portsink[0], objsink.y + portsink[1]) 
     
     def setPath(self, x, y):
         self.x = x
         self.y = y
         
-    def draw(self, canvas):
+    def draw(self, canvas, debug=False):
         if (self.x == None):
             return
         
         if (self.routed):
             pass
         else:
             canvas.setForecolor('red')
```

### Comparing `py4hw-0.0.9/py4hw/simulation.py` & `py4hw-2024.1/py4hw/simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             Hardware system to simulate.
 
         Returns
         -------
         None.
 
         """
+        self.total_clks = 0
+        
         if sys.simulator != None:
             return
 
         self.sys = sys;
 
         
         self.topologicalSort()
@@ -94,16 +96,23 @@
 
             if (leaf.isPropagatable()):
                 self.propagatables.append(leaf)
                 
         # Now sort the propagatables list
         anyChange = True 
         
+        loopcount = 0
+        
         while (anyChange):
+            loopcount += 1
             anyChange = False
+            
+            if (loopcount > 1000):
+                raise Exception('Excessive loop count in topological count')
+                
             for i in range(len(self.propagatables)):
                 leaf = self.propagatables[i]
                 pos = self.findFirstDependentPosition(leaf)
                 
                 if (pos >= 0 and pos < i):
                     # exchange position, put dependent last
                     first = self.propagatables[pos]
@@ -174,15 +183,20 @@
             Number of clock cycles.
 
         Returns
         -------
         None.
 
         """
+        self.do_run = True
         for i in range(cycles):
+            if not(self.do_run):
+                # simulation was cancelled by stop
+                return
+            
             self._clk_cycle();
             
             
     def _clk_cycle(self):
         """
         Advance one clock cycle
 
@@ -200,15 +214,19 @@
             
         Wire.settleAll()
                 
         for obj in self.propagatables:
             obj.propagate();
             
         self._notifyListeners()
-            
+        self.total_clks += 1
+
+    def stop(self):
+        self.do_run = False
+           
     def addListener(self, listener):
         self.listeners.append(listener)
         
     def _notifyListeners(self):
         for listener in self.listeners:
             listener.simulatorUpdated()
```

### Comparing `py4hw-0.0.9/py4hw.egg-info/PKG-INFO` & `py4hw-2024.1/py4hw.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: py4hw
-Version: 0.0.9
+Version: 2024.1
 Summary: py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.
 Home-page: https://github.com/davidcastells/py4hw
 Author: David Castells-Rufas
 Author-email: david.castells@uab.cat
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nbwavedrom==0.2.0
+Requires-Dist: ipywidgets
+Requires-Dist: matplotlib
+Requires-Dist: deprecated
+Requires-Dist: scipy
+Requires-Dist: pytest
+Requires-Dist: edalize
+Requires-Dist: setuptools
 
 # py4hw
 
 [![PyPI version](https://badge.fury.io/py/py4hw.svg)](https://badge.fury.io/py/py4hw)
 [![Join the chat at https://gitter.im/davidcastells/py4hw](https://badges.gitter.im/davidcastells/py4hw.svg)](https://gitter.im/davidcastells/py4hw?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 py4hw is an HDL library based on python to create digital circuits (mainly) following a structural design methodology.
```

### Comparing `py4hw-0.0.9/py4hw.egg-info/SOURCES.txt` & `py4hw-2024.1/py4hw.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
+requires.txt
 setup.cfg
 setup.py
 py4hw/__init__.py
 py4hw/base.py
+py4hw/code_generation.py
 py4hw/debug.py
 py4hw/gui.py
 py4hw/helper.py
 py4hw/rtl_generation.py
 py4hw/schematic.py
 py4hw/schematic_symbols.py
 py4hw/simulation.py
 py4hw.egg-info/PKG-INFO
 py4hw.egg-info/SOURCES.txt
 py4hw.egg-info/dependency_links.txt
 py4hw.egg-info/requires.txt
 py4hw.egg-info/top_level.txt
 py4hw/logic/__init__.py
 py4hw/logic/arithmetic.py
+py4hw/logic/arithmetic_fp.py
+py4hw/logic/arithmetic_fxp.py
 py4hw/logic/bitwise.py
 py4hw/logic/clock.py
 py4hw/logic/relational.py
 py4hw/logic/simulation.py
-py4hw/logic/storage.py
+py4hw/logic/storage.py
+py4hw/transpilation/__init__.py
+py4hw/transpilation/ast2xml.py
+py4hw/transpilation/astutils.py
+py4hw/transpilation/python2cflexhdl_transpilation.py
+py4hw/transpilation/python2structural.py
+py4hw/transpilation/python2verilog_transpilation.py
```

### Comparing `py4hw-0.0.9/setup.py` & `py4hw-2024.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
                          
 setup(
     name='py4hw',
-    version='0.0.9',
+    version='2024.1',
     author='David Castells-Rufas',
     author_email='david.castells@uab.cat',
     description='py4hw is a library to model, and simulate digital logic circuits. It promotes the use of structural design style to build hardware and it is highly influenced by the ideas behind JHDL.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/davidcastells/py4hw',
-    install_requires=open('requirements.txt').readlines(),
-    tests_require=open('requirements.txt').readlines(),
+    install_requires=open('requires.txt').readlines(),
+    tests_require=open('requires.txt').readlines(),
     packages=find_packages(exclude=['riscv'])
-)
+)
```

