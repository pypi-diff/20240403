# Comparing `tmp/ftb-snbt-lib-0.1.2.tar.gz` & `tmp/ftb-snbt-lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb-snbt-lib-0.1.2.tar", last modified: Sun Mar 31 09:55:15 2024, max compression
+gzip compressed data, was "ftb-snbt-lib-0.1.3.tar", last modified: Wed Apr  3 05:12:15 2024, max compression
```

## Comparing `ftb-snbt-lib-0.1.2.tar` & `ftb-snbt-lib-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:55:15.952414 ftb-snbt-lib-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-31 09:55:15.948414 ftb-snbt-lib-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:55:15.948414 ftb-snbt-lib-0.1.2/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:55:15.948414 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:55:15.948414 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-31 09:55:15.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-31 09:55:15.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:55:15.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 09:55:15.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 09:55:15.000000 ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:55:15.952414 ftb-snbt-lib-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-31 09:55:11.000000 ftb-snbt-lib-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/setup.py
```

### Comparing `ftb-snbt-lib-0.1.2/LICENSE` & `ftb-snbt-lib-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/PKG-INFO` & `ftb-snbt-lib-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -100,14 +100,15 @@
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
+| Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
```

### Comparing `ftb-snbt-lib-0.1.2/README.md` & `ftb-snbt-lib-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
+| Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
```

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/parse.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     p[0] = (p[1], p[3])
 
 def p_value(p):
     """value : compound
                 | list
                 | BOOL
                 | BYTE
+                | SHORT
                 | DOUBLE
                 | LONG
                 | INTEGER
                 | STRING"""
     p[0] = p[1]
 
 def p_list(p):
```

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/parsetab.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/parsetab.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,50 +2,51 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET STRINGsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | BOOL\n                | BYTE\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETvalues : values value\n              | values COMMA value\n              | value'
+_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET SHORT STRINGsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | BOOL\n                | BYTE\n                | SHORT\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETvalues : values value\n              | values COMMA value\n              | value'
     
-_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,3,3,-18,-21,-17,-19,3,-20,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,25,27,29,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-8,-18,-17,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,25,27,29,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-8,-18,-17,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,],[8,8,-3,-6,-2,-4,8,23,23,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,23,-8,23,-18,-21,-17,-19,23,-20,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,25,26,27,28,29,30,32,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-8,31,-18,-21,-17,-19,-20,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,26,27,28,29,30,32,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,27,29,-18,-21,-17,-19,-20,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,18,18,-9,-10,-11,-12,-13,-14,-15,-16,18,18,-18,-21,-17,-19,18,-20,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,19,19,-18,-21,-17,-19,19,-20,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,20,20,-18,-21,-17,-19,20,-20,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,21,21,-18,-21,-17,-19,21,-20,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,22,22,-18,-21,-17,-19,22,-20,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,32,],[-3,-2,24,24,-9,-10,-11,-12,-13,-14,-15,-16,24,24,-18,-21,-17,-19,24,-20,]),'COLON':([7,8,],[12,13,]),}
+_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,-17,3,3,-19,-22,-18,-20,3,-21,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,26,28,30,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-8,-19,-18,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,24,26,28,30,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-8,-19,-18,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,],[8,8,-3,-6,-2,-4,8,24,24,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,24,-8,24,-19,-22,-18,-20,24,-21,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,33,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-8,32,-19,-22,-18,-20,-21,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,33,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,-17,28,30,-19,-22,-18,-20,-21,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,18,18,-9,-10,-11,-12,-13,-14,-15,-16,-17,18,18,-19,-22,-18,-20,18,-21,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,-17,19,19,-19,-22,-18,-20,19,-21,]),'SHORT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,-17,20,20,-19,-22,-18,-20,20,-21,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,-17,21,21,-19,-22,-18,-20,21,-21,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,-17,22,22,-19,-22,-18,-20,22,-21,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,23,23,-9,-10,-11,-12,-13,-14,-15,-16,-17,23,23,-19,-22,-18,-20,23,-21,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,27,28,29,30,31,32,33,],[-3,-2,25,25,-9,-10,-11,-12,-13,-14,-15,-16,-17,25,25,-19,-22,-18,-20,25,-21,]),'COLON':([7,8,],[12,13,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'snbt':([0,],[1,]),'compound':([0,12,13,24,26,31,],[2,16,16,16,16,16,]),'key_value_pairs':([3,],[4,]),'key_value_pair':([3,4,11,],[6,10,14,]),'value':([12,13,24,26,31,],[15,25,28,30,32,]),'list':([12,13,24,26,31,],[17,17,17,17,17,]),'values':([24,],[26,]),}
+_lr_goto_items = {'snbt':([0,],[1,]),'compound':([0,12,13,25,27,32,],[2,16,16,16,16,16,]),'key_value_pairs':([3,],[4,]),'key_value_pair':([3,4,11,],[6,10,14,]),'value':([12,13,25,27,32,],[15,26,29,31,33,]),'list':([12,13,25,27,32,],[17,17,17,17,17,]),'values':([25,],[27,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> snbt","S'",1,None,None,None),
-  ('snbt -> compound','snbt',1,'p_snbt','parse.py',6),
-  ('compound -> LBRACE key_value_pairs RBRACE','compound',3,'p_compound','parse.py',10),
-  ('compound -> LBRACE RBRACE','compound',2,'p_compound','parse.py',11),
-  ('key_value_pairs -> key_value_pairs key_value_pair','key_value_pairs',2,'p_key_value_pairs','parse.py',18),
-  ('key_value_pairs -> key_value_pairs COMMA key_value_pair','key_value_pairs',3,'p_key_value_pairs','parse.py',19),
-  ('key_value_pairs -> key_value_pair','key_value_pairs',1,'p_key_value_pairs','parse.py',20),
-  ('key_value_pair -> NAME COLON value','key_value_pair',3,'p_key_value_pair','parse.py',29),
-  ('key_value_pair -> STRING COLON value','key_value_pair',3,'p_key_value_pair','parse.py',30),
-  ('value -> compound','value',1,'p_value','parse.py',34),
-  ('value -> list','value',1,'p_value','parse.py',35),
-  ('value -> BOOL','value',1,'p_value','parse.py',36),
-  ('value -> BYTE','value',1,'p_value','parse.py',37),
-  ('value -> DOUBLE','value',1,'p_value','parse.py',38),
-  ('value -> LONG','value',1,'p_value','parse.py',39),
-  ('value -> INTEGER','value',1,'p_value','parse.py',40),
-  ('value -> STRING','value',1,'p_value','parse.py',41),
-  ('list -> LBRACKET values RBRACKET','list',3,'p_list','parse.py',45),
-  ('list -> LBRACKET RBRACKET','list',2,'p_list','parse.py',46),
-  ('values -> values value','values',2,'p_values','parse.py',53),
-  ('values -> values COMMA value','values',3,'p_values','parse.py',54),
-  ('values -> value','values',1,'p_values','parse.py',55),
+  ('snbt -> compound','snbt',1,'p_snbt','parse.py',8),
+  ('compound -> LBRACE key_value_pairs RBRACE','compound',3,'p_compound','parse.py',12),
+  ('compound -> LBRACE RBRACE','compound',2,'p_compound','parse.py',13),
+  ('key_value_pairs -> key_value_pairs key_value_pair','key_value_pairs',2,'p_key_value_pairs','parse.py',20),
+  ('key_value_pairs -> key_value_pairs COMMA key_value_pair','key_value_pairs',3,'p_key_value_pairs','parse.py',21),
+  ('key_value_pairs -> key_value_pair','key_value_pairs',1,'p_key_value_pairs','parse.py',22),
+  ('key_value_pair -> NAME COLON value','key_value_pair',3,'p_key_value_pair','parse.py',31),
+  ('key_value_pair -> STRING COLON value','key_value_pair',3,'p_key_value_pair','parse.py',32),
+  ('value -> compound','value',1,'p_value','parse.py',36),
+  ('value -> list','value',1,'p_value','parse.py',37),
+  ('value -> BOOL','value',1,'p_value','parse.py',38),
+  ('value -> BYTE','value',1,'p_value','parse.py',39),
+  ('value -> SHORT','value',1,'p_value','parse.py',40),
+  ('value -> DOUBLE','value',1,'p_value','parse.py',41),
+  ('value -> LONG','value',1,'p_value','parse.py',42),
+  ('value -> INTEGER','value',1,'p_value','parse.py',43),
+  ('value -> STRING','value',1,'p_value','parse.py',44),
+  ('list -> LBRACKET values RBRACKET','list',3,'p_list','parse.py',48),
+  ('list -> LBRACKET RBRACKET','list',2,'p_list','parse.py',49),
+  ('values -> values value','values',2,'p_values','parse.py',56),
+  ('values -> values COMMA value','values',3,'p_values','parse.py',57),
+  ('values -> value','values',1,'p_values','parse.py',58),
 ]
```

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/cpp.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/ctokens.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/lex.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/yacc.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/ply/ygen.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/tag.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Integer", "Long", "Double", "Bool", "String", "List", "Compound"]
+__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Short", "Integer", "Long", "Double", "Bool", "String", "List", "Compound"]
 
 class InvalidTypeError(ValueError):
     def __init__(self, item, cls):
         self.item = item
         self.cls = cls
         super().__init__(f"{self.item!r} is not a valid type for the items of {cls.__name__}.\nThis error is likely caused by a type mismatch in a list.")
 
@@ -40,14 +40,19 @@
         return self
 
 class Byte(NumericInteger):
     __slots__ = ()
     size = 1
     suffix = "b"
 
+class Short(NumericInteger):
+    __slots__ = ()
+    size = 2
+    suffix = "s"
+
 class Integer(NumericInteger):
     __slots__ = ()
     size = 4
 
 class Long(NumericInteger):
     __slots__ = ()
     size = 8
```

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/token.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 tokens = (
     "LBRACE",
     "RBRACE",
     "LBRACKET",
     "RBRACKET",
     "BOOL",
     "BYTE",
+    "SHORT",
     "DOUBLE",
     "LONG",
     "INTEGER",
     "STRING",
     "NAME",
     "COLON",
     "COMMA",
@@ -49,14 +50,19 @@
     return t
 
 def t_BYTE(t):
     r'\-?[0-9]+b'
     t.value = Byte(t.value[:-1])
     return t
 
+def t_SHORT(t):
+    r'\-?[0-9]+s'
+    t.value = Short(t.value[:-1])
+    return t
+
 def t_DOUBLE(t):
     r'\-?[0-9]+\.[0-9]+d'
     t.value = Double(t.value[:-1])
     return t
 
 def t_LONG(t):
     r'\-?[0-9]+L'
```

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib/write.py` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib/write.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.2/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -100,14 +100,15 @@
 >>> json.dump(another_snbt, open("tests/test.json", "w", encoding="utf-8"), indent=4, ensure_ascii=False)
 ```
 
 ## Data Types
 | Type | Description | Format | Example |
 | - | - | - | - |
 | Byte | A signed 8-bit integer.<br>Range: ``-128`` ~ ``127`` | ``<number>b`` | ``12b``, ``-35b`` |
+| Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
```

### Comparing `ftb-snbt-lib-0.1.2/pyproject.toml` & `ftb-snbt-lib-0.1.3/pyproject.toml`

 * *Files identical despite different names*

