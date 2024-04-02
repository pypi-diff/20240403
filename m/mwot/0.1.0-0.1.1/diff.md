# Comparing `tmp/mwot-0.1.0.tar.gz` & `tmp/mwot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwot-0.1.0.tar", last modified: Thu Aug 25 23:12:22 2022, max compression
+gzip compressed data, was "mwot-0.1.1.tar", last modified: Tue Apr  2 22:12:41 2024, max compression
```

## Comparing `mwot-0.1.0.tar` & `mwot-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/
--rw-rw-r--   0 gram      (1000) gram      (1000)     4117 2022-08-25 23:12:22.571980 mwot-0.1.0/PKG-INFO
--rw-rw-r--   0 gram      (1000) gram      (1000)     3297 2022-08-01 15:21:10.000000 mwot-0.1.0/README.md
--rw-rw-r--   0 gram      (1000) gram      (1000)     1211 2021-05-06 04:30:47.000000 mwot-0.1.0/UNLICENSE
--rw-rw-r--   0 gram      (1000) gram      (1000)       81 2022-07-30 23:33:41.000000 mwot-0.1.0/pyproject.toml
--rw-rw-r--   0 gram      (1000) gram      (1000)      984 2022-08-25 23:12:22.571980 mwot-0.1.0/setup.cfg
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot/
--rw-rw-r--   0 gram      (1000) gram      (1000)     1108 2022-08-25 23:09:37.000000 mwot-0.1.0/src/mwot/__init__.py
--rw-rw-r--   0 gram      (1000) gram      (1000)       81 2022-08-12 20:57:22.000000 mwot-0.1.0/src/mwot/__main__.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot/binary/
--rw-rw-r--   0 gram      (1000) gram      (1000)      664 2022-07-05 11:54:04.000000 mwot-0.1.0/src/mwot/binary/__init__.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot/brainfuck/
--rw-rw-r--   0 gram      (1000) gram      (1000)     1114 2022-07-05 11:53:57.000000 mwot-0.1.0/src/mwot/brainfuck/__init__.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     3553 2022-07-30 17:36:38.000000 mwot-0.1.0/src/mwot/brainfuck/interpreter.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot/cli/
--rw-rw-r--   0 gram      (1000) gram      (1000)      721 2022-08-12 20:57:36.000000 mwot-0.1.0/src/mwot/cli/__init__.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     4598 2022-07-30 22:52:02.000000 mwot-0.1.0/src/mwot/cli/actions.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     2119 2022-08-24 23:26:29.000000 mwot-0.1.0/src/mwot/cli/argtypes.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     6577 2022-08-24 23:26:32.000000 mwot-0.1.0/src/mwot/cli/parsing.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      804 2022-01-11 00:54:28.000000 mwot-0.1.0/src/mwot/cli/sources.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      715 2022-07-30 22:52:02.000000 mwot-0.1.0/src/mwot/compiler.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot/decompilers/
--rw-rw-r--   0 gram      (1000) gram      (1000)      108 2021-10-17 19:35:09.000000 mwot-0.1.0/src/mwot/decompilers/__init__.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      311 2022-01-11 00:54:28.000000 mwot-0.1.0/src/mwot/decompilers/basic.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      798 2022-03-19 19:29:35.000000 mwot-0.1.0/src/mwot/decompilers/common.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      646 2022-03-19 19:29:35.000000 mwot-0.1.0/src/mwot/decompilers/guide.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      596 2022-01-11 00:54:28.000000 mwot-0.1.0/src/mwot/decompilers/rand.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     1594 2022-07-04 20:56:56.000000 mwot-0.1.0/src/mwot/join.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     3521 2022-07-30 22:52:02.000000 mwot-0.1.0/src/mwot/stypes.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     1555 2022-07-30 22:52:02.000000 mwot-0.1.0/src/mwot/util.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2022-08-25 23:12:22.571980 mwot-0.1.0/src/mwot.egg-info/
--rw-rw-r--   0 gram      (1000) gram      (1000)     4117 2022-08-25 23:12:22.000000 mwot-0.1.0/src/mwot.egg-info/PKG-INFO
--rw-rw-r--   0 gram      (1000) gram      (1000)      691 2022-08-25 23:12:22.000000 mwot-0.1.0/src/mwot.egg-info/SOURCES.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)        1 2022-08-25 23:12:22.000000 mwot-0.1.0/src/mwot.egg-info/dependency_links.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)       39 2022-08-25 23:12:22.000000 mwot-0.1.0/src/mwot.egg-info/entry_points.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)        5 2022-08-25 23:12:22.000000 mwot-0.1.0/src/mwot.egg-info/top_level.txt
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/
+-rw-r--r--   0 gram      (1000) gram      (1000)     4117 2024-04-02 22:12:41.738950 mwot-0.1.1/PKG-INFO
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3297 2022-12-29 20:53:28.000000 mwot-0.1.1/README.md
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1211 2021-05-06 04:30:47.000000 mwot-0.1.1/UNLICENSE
+-rw-rw-r--   0 gram      (1000) gram      (1000)       81 2022-07-30 23:33:41.000000 mwot-0.1.1/pyproject.toml
+-rw-rw-r--   0 gram      (1000) gram      (1000)      984 2024-04-02 22:12:41.738950 mwot-0.1.1/setup.cfg
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot/
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1108 2024-04-02 21:54:48.000000 mwot-0.1.1/src/mwot/__init__.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)       81 2022-08-12 20:57:22.000000 mwot-0.1.1/src/mwot/__main__.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot/binary/
+-rw-rw-r--   0 gram      (1000) gram      (1000)      664 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/binary/__init__.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot/brainfuck/
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1114 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/brainfuck/__init__.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     9711 2024-04-02 21:54:48.000000 mwot-0.1.1/src/mwot/brainfuck/interpreter.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot/cli/
+-rw-rw-r--   0 gram      (1000) gram      (1000)      721 2022-08-12 20:57:36.000000 mwot-0.1.1/src/mwot/cli/__init__.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     4598 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/cli/actions.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     2119 2022-08-24 23:26:29.000000 mwot-0.1.1/src/mwot/cli/argtypes.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     6611 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/cli/parsing.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      804 2024-04-02 21:27:06.000000 mwot-0.1.1/src/mwot/cli/sources.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      715 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/compiler.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot/decompilers/
+-rw-rw-r--   0 gram      (1000) gram      (1000)      108 2021-10-17 19:35:09.000000 mwot-0.1.1/src/mwot/decompilers/__init__.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      311 2022-01-11 00:54:28.000000 mwot-0.1.1/src/mwot/decompilers/basic.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      798 2022-03-19 19:29:35.000000 mwot-0.1.1/src/mwot/decompilers/common.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      646 2022-03-19 19:29:35.000000 mwot-0.1.1/src/mwot/decompilers/guide.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      596 2022-01-11 00:54:28.000000 mwot-0.1.1/src/mwot/decompilers/rand.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1594 2022-07-04 20:56:56.000000 mwot-0.1.1/src/mwot/join.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3779 2024-04-01 18:24:37.000000 mwot-0.1.1/src/mwot/stypes.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3376 2024-04-02 20:18:40.000000 mwot-0.1.1/src/mwot/util.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-02 22:12:41.738950 mwot-0.1.1/src/mwot.egg-info/
+-rw-r--r--   0 gram      (1000) gram      (1000)     4117 2024-04-02 22:12:41.000000 mwot-0.1.1/src/mwot.egg-info/PKG-INFO
+-rw-rw-r--   0 gram      (1000) gram      (1000)      691 2024-04-02 22:12:41.000000 mwot-0.1.1/src/mwot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)        1 2024-04-02 22:12:41.000000 mwot-0.1.1/src/mwot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)       39 2024-04-02 22:12:41.000000 mwot-0.1.1/src/mwot.egg-info/entry_points.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)        5 2024-04-02 22:12:41.000000 mwot-0.1.1/src/mwot.egg-info/top_level.txt
```

### Comparing `mwot-0.1.0/PKG-INFO` & `mwot-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constrained writing as an encoding
 Home-page: https://codeberg.org/gramkraxor/mwot
 Author: Gramkraxor
 Author-email: gram@krax.dev
 License: Unlicense
 Keywords: esolang,esoteric language,brainfuck
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `mwot-0.1.0/README.md` & `mwot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/UNLICENSE` & `mwot-0.1.1/UNLICENSE`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/setup.cfg` & `mwot-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/__init__.py` & `mwot-0.1.1/src/mwot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'decomp_basic',
     'decomp_guide',
     'decomp_rand',
     'decompilers',
     'run_bf',
     'run_bf_mwot',
 ]
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from . import binary
 from . import brainfuck
 from . import cli
 from . import decompilers
 from .compiler import bits_from_mwot
 from .join import joinable
```

### Comparing `mwot-0.1.0/src/mwot/brainfuck/__init__.py` & `mwot-0.1.1/src/mwot/brainfuck/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     for chunk in chunk_bits(bits, chunk_size=3):
         yield cmdmap[chunk]
 
 
 @joinable()
 def to_bits(chars):
     """Convert brainfuck to MWOT bits."""
-    stype, chars = stypes.probe(chars, default=stypes.Bytes)
-    if stype is not stypes.Bytes:
+    stype, chars = stypes.probe(chars, default=stypes.BYTES)
+    if stype is not stypes.BYTES:
         raise TypeError('chars must be bytes')
     for cmd in chars:
         yield from chunkmap.get(cmd, ())
 
 
 from . import interpreter
```

### Comparing `mwot-0.1.0/src/mwot/cli/__init__.py` & `mwot-0.1.1/src/mwot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/cli/actions.py` & `mwot-0.1.1/src/mwot/cli/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,26 +68,26 @@
         output = self.transpile(source.read())
         with self.open_outfile() as f:
             self.write(f, output)
 
     def write(self, f, output):
         if self.args.shebang_out and self.args.format == 'brainfuck':
             f.write(self.bf_shebang)
-        if self.stype_out is stypes.Bytes:
+        if self.stype_out is stypes.BYTES:
             for chunk in chunks(output, 80):
                 f.write(bytes(chunk))
         else:
             for i in output:
                 f.write(i)
 
 
 class Compile(TranspilerAction):
 
-    stype_in = stypes.Text
-    stype_out = stypes.Bytes
+    stype_in = stypes.TEXT
+    stype_out = stypes.BYTES
     bf_shebang = b'#!/usr/bin/env -S mwot -xb\n'
 
     def transpile(self, source_code):
         return self.format.from_bits(bits_from_mwot(source_code))
 
     def write(self, f, output):
         if self.args.executable_out:
@@ -95,16 +95,16 @@
         super().write(f, output)
         if self.args.format == 'brainfuck':
             f.write(b'\n')
 
 
 class Decompile(TranspilerAction):
 
-    stype_in = stypes.Bytes
-    stype_out = stypes.Text
+    stype_in = stypes.BYTES
+    stype_out = stypes.TEXT
     bf_shebang = '#!/usr/bin/env -S mwot -ib\n'
     keywords = ('width', 'vocab', 'cols')
 
     def transpile(self, source_code):
         decomp = getattr(decompilers, self.args.decompiler).decomp
         if self.args.shebang_in and self.args.format == 'brainfuck':
             source_code = deshebang(source_code, self.stype_in)
@@ -114,43 +114,43 @@
         if self.args.executable_out and self.args.format == 'brainfuck':
             chmod_x(f)
         super().write(f, output)
 
 
 class InterpreterAction(Action):
 
-    stype_out = stypes.Bytes
+    stype_out = stypes.BYTES
 
     def get_input(self):
         """Retrieve the correct interpreter input source."""
         if self.args.input is not None:
             return StringSource(self.args.input.encode())
         if self.args.infile != '-':
-            return Source(self.args.infile, stypes.Bytes)
+            return Source(self.args.infile, stypes.BYTES)
         if self.args.source is None and self.args.srcfile == '-':
             return StringSource(b'')
-        return Source('-', stypes.Bytes)
+        return Source('-', stypes.BYTES)
 
     def run(self):
         source_code = self.get_source().read()
         with self.get_input().open() as infile, self.open_outfile() as outfile:
             self.kwargs['infile'] = infile
             self.kwargs['outfile'] = outfile
             self.execute(source_code)
 
 
 class Interpret(InterpreterAction):
 
-    stype_in = stypes.Text
+    stype_in = stypes.TEXT
     keywords = ('cellsize', 'eof', 'totalcells', 'wraparound')
 
     def execute(self, source_code):
         self.format.interpreter.run_mwot(source_code, **self.kwargs)
 
 
 class Execute(InterpreterAction):
 
-    stype_in = stypes.Bytes
+    stype_in = stypes.BYTES
     keywords = ('shebang_in', 'cellsize', 'eof', 'totalcells', 'wraparound')
 
     def execute(self, source_code):
         self.format.interpreter.run(source_code, **self.kwargs)
```

### Comparing `mwot-0.1.0/src/mwot/cli/argtypes.py` & `mwot-0.1.1/src/mwot/cli/argtypes.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/cli/parsing.py` & `mwot-0.1.1/src/mwot/cli/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     parser = argparse.ArgumentParser(
         prog='mwot',
         usage=argparse.SUPPRESS,
         description=description,
         epilog=epilog,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         add_help=False,
+        allow_abbrev=False,
     )
 
     main_opts = parser.add_argument_group(
         'Main options')
     trans_opts = parser.add_argument_group(
         'Transpilation (-{c|d}) options')
     decomp_opts = parser.add_argument_group(
@@ -99,15 +100,15 @@
     src_mx_opts.add_argument(
         'srcfile',
         metavar='SRCFILE',
         nargs='?',
         help="source file (absent or '-' for stdin)",
     )
     src_mx_opts.add_argument(
-        '--source',
+        '-e', '--source',
         dest='source',
         metavar='SOURCE',
         help="take source code as an argument; don't accept SRCFILE",
     )
     main_opts.add_argument(
         '-o', '--output-file',
         dest='outfile',
```

### Comparing `mwot-0.1.0/src/mwot/cli/sources.py` & `mwot-0.1.1/src/mwot/cli/sources.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/compiler.py` & `mwot-0.1.1/src/mwot/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 @joinable()
 def bits_from_mwot(mwot):
     """Yield MWOT bits from MWOT source.
 
     Yields the even/oddness of the letter count of each
     whitespace-separated word, ignoring words with 0 letters.
     """
-    stype, mwot = stypes.probe(mwot, default=stypes.Text)
-    if stype is not stypes.Text:
+    stype, mwot = stypes.probe(mwot, default=stypes.TEXT)
+    if stype is not stypes.TEXT:
         raise TypeError('mwot must be text')
     for word in split(deshebang(mwot, stype)):
         length = letter_count(word)
         if length:
             yield length & 1
```

### Comparing `mwot-0.1.0/src/mwot/decompilers/common.py` & `mwot-0.1.1/src/mwot/decompilers/common.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/decompilers/guide.py` & `mwot-0.1.1/src/mwot/decompilers/guide.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/decompilers/rand.py` & `mwot-0.1.1/src/mwot/decompilers/rand.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot/join.py` & `mwot-0.1.1/src/mwot/join.py`

 * *Files identical despite different names*

### Comparing `mwot-0.1.0/src/mwot.egg-info/PKG-INFO` & `mwot-0.1.1/src/mwot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constrained writing as an encoding
 Home-page: https://codeberg.org/gramkraxor/mwot
 Author: Gramkraxor
 Author-email: gram@krax.dev
 License: Unlicense
 Keywords: esolang,esoteric language,brainfuck
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `mwot-0.1.0/src/mwot.egg-info/SOURCES.txt` & `mwot-0.1.1/src/mwot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

