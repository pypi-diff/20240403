# Comparing `tmp/pyhtml_enhanced-2.0.0.tar.gz` & `tmp/pyhtml_enhanced-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml_enhanced-2.0.0.tar", max compression
+gzip compressed data, was "pyhtml_enhanced-2.0.1.tar", max compression
```

## Comparing `pyhtml_enhanced-2.0.0.tar` & `pyhtml_enhanced-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1090 2024-02-10 07:30:41.220032 pyhtml_enhanced-2.0.0/LICENSE.md
--rw-r--r--   0        0        0    14277 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/LICENSE_DOCS.md
--rw-r--r--   0        0        0     6153 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/README.md
--rw-r--r--   0        0        0     8980 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__init__.py
--rw-r--r--   0        0        0     5080 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__tag_base.py
--rw-r--r--   0        0        0     2944 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__tags/__init__.py
--rw-r--r--   0        0        0   205297 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__tags/generated.py
--rw-r--r--   0        0        0    16608 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__tags/input.py
--rw-r--r--   0        0        0      441 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__tags/renames.py
--rw-r--r--   0        0        0     1231 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__types.py
--rw-r--r--   0        0        0     3898 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/__util.py
--rw-r--r--   0        0        0        0 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyhtml/py.typed
--rw-r--r--   0        0        0     1907 2024-02-10 07:30:41.224032 pyhtml_enhanced-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7384 1970-01-01 00:00:00.000000 pyhtml_enhanced-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0    14277 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/LICENSE_DOCS.md
+-rw-r--r--   0        0        0     6407 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/README.md
+-rw-r--r--   0        0        0     9284 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__init__.py
+-rw-r--r--   0        0        0     4565 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tag_base.py
+-rw-r--r--   0        0        0     3111 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/comment.py
+-rw-r--r--   0        0        0     1543 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/dangerous_raw_html.py
+-rw-r--r--   0        0        0   205360 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/generated.py
+-rw-r--r--   0        0        0    16608 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/input.py
+-rw-r--r--   0        0        0      441 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/renames.py
+-rw-r--r--   0        0        0     1231 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__types.py
+-rw-r--r--   0        0        0     4055 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__util.py
+-rw-r--r--   0        0        0        0 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/py.typed
+-rw-r--r--   0        0        0     1907 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 pyhtml_enhanced-2.0.1/PKG-INFO
```

### Comparing `pyhtml_enhanced-2.0.0/LICENSE.md` & `pyhtml_enhanced-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.0/LICENSE_DOCS.md` & `pyhtml_enhanced-2.0.1/LICENSE_DOCS.md`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.0/README.md` & `pyhtml_enhanced-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -216,23 +216,30 @@
 
 ## Credits
 
 ### [Cenkalti/PyHTML](https://github.com/cenkalti/pyhtml)
 
 Cenk Altı's work was used as a source of inspiration and reference. Although
 all the code in `pyhtml-enhanced` was written by me, I want to thank them for
-the significant help their hard work provided while creating this project.
+the significant help their hard work provided while creating this project,
+going as far as to give design advice on request.
 
 ### [MDN Web Docs](https://developer.mozilla.org/en-US/)
 
 Almost all of the documentation was gathered from the MDN Web Docs. It's super
 neat that all their documentation is open (licensed as
 [CC-BY-SA-2.5](https://creativecommons.org/licenses/by-sa/2.5/) if you're
 interested).
 
+### COMP1010 students and staff
+
+COMP1010's students and staff members have uncovered and helped to resolve many
+bugs, and have suggested many improvements. I'd like to thank them for all of
+their help!
+
 ## License
 
 ### Source code
 
 Copyright (c) 2023 Miguel Guthridge, COMP1010 UNSW
 
 Source code for the library is open source, using the
```

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__init__.py` & `pyhtml_enhanced-2.0.1/pyhtml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,23 +217,30 @@
 
 ## Credits
 
 ### [Cenkalti/PyHTML](https://github.com/cenkalti/pyhtml)
 
 Cenk Altı's work was used as a source of inspiration and reference. Although
 all the code in `pyhtml-enhanced` was written by me, I want to thank them for
-the significant help their hard work provided while creating this project.
+the significant help their hard work provided while creating this project,
+going as far as to give design advice on request.
 
 ### [MDN Web Docs](https://developer.mozilla.org/en-US/)
 
 Almost all of the documentation was gathered from the MDN Web Docs. It's super
 neat that all their documentation is open (licensed as
 [CC-BY-SA-2.5](https://creativecommons.org/licenses/by-sa/2.5/) if you're
 interested).
 
+### COMP1010 students and staff
+
+COMP1010's students and staff members have uncovered and helped to resolve many
+bugs, and have suggested many improvements. I'd like to thank them for all of
+their help!
+
 ## License
 
 ### Source code
 
 Copyright (c) 2023 Miguel Guthridge, COMP1010 UNSW
 
 Source code for the library is open source, using the
@@ -245,20 +252,21 @@
 Documentation is copied from MDN Web Docs, and is license under
 [CC-BY-SA-2.5](https://creativecommons.org/licenses/by-sa/2.5/). A copy of the
 license text is available in [LICENSE_DOCS.md](https://github.com/COMP1010UNSW/pyhtml-enhanced/blob/main/LICENSE_DOCS.md)
 
 """
 # Disable Flake8, since it really doesn't like our docstring above
 # flake8: noqa
-from .__tag_base import Tag, Comment
+from .__tag_base import Tag
 
 from .__tags import input_, object_
 
 __all__ = [
     'Tag',
+    'DangerousRawHtml',
     'Comment',
     'input_',
     'object_',
     'html',
     'base',
     'head',
     'link',
@@ -371,14 +379,16 @@
     'summary',
     'slot',
     'template',
 ]
 
 
 from .__tags import (
+    DangerousRawHtml,
+    Comment,
     html,
     base,
     head,
     link,
     meta,
     style,
     title,
```

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__tag_base.py` & `pyhtml_enhanced-2.0.1/pyhtml/__tag_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,25 @@
         attributes.
 
         This is overridden by child classes to return a dictionary of default
         attributes that are applied to the class.
         """
         return {}
 
+    def _escape_children(self) -> bool:
+        """
+        Returns whether the contents of the element should be escaped, or
+        rendered plainly.
+
+        By default, all string content should be escaped to prevent security
+        vulnerabilities such as XSS, but this is disabled for certain tags such
+        as <script>.
+        """
+        return True
+
     def _render(self) -> list[str]:
         """
         Renders tag and its children to a list of strings where each string is
         a single line of output
         """
         attributes = util.filter_attributes(util.dict_union(
             self._get_default_attributes(self.attributes),
@@ -93,15 +104,17 @@
 
         if not len(self.children):
             opening += f"</{self._get_tag_name()}>"
             return [opening]
         else:
             out = [opening]
             # Children
-            out.extend(util.render_children(self.children))
+            out.extend(
+                util.render_children(self.children, self._escape_children())
+            )
             # Closing tag
             out.append(f"</{self._get_tag_name()}>")
 
             return out
 
     def render(self) -> str:
         """
@@ -112,54 +125,14 @@
     def __str__(self) -> str:
         return self.render()
 
     def __repr__(self) -> str:
         return self.render()
 
 
-class Comment(Tag):
-    """
-    An HTML comment.
-
-    Renders as:
-
-    ```html
-    <!-- [comment text] -->
-    ```
-
-    Note that this does not render as a `<comment>` tag
-    """
-    def __init__(self, text: str) -> None:
-        self.comment_data = text
-        super().__init__()
-
-    def __call__(self):
-        raise TypeError('Comment tags are not callable')
-
-    def _get_tag_name(self) -> str:
-        # Ignore coverage since this is only implemented to satisfy inheritance
-        # and is never used since we override _render
-        return '!--'  # pragma: no cover
-
-    def _render(self) -> list[str]:
-        """
-        Override of render, to render comments
-        """
-
-        return [
-            '<!--',
-            *util.increase_indent(
-                util.escape_string(self.comment_data).splitlines(),
-                # FIXME: Yucky magic number
-                2,
-            ),
-            '-->'
-        ]
-
-
 class SelfClosingTag(Tag):
     """
     Self-closing tags don't contain child elements
     """
     def __init__(self, **attributes: AttributeType) -> None:
         # Self-closing tags don't allow children
         super().__init__(**attributes)
```

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__tags/__init__.py` & `pyhtml_enhanced-2.0.1/pyhtml/__tags/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 # PyHTML Enhanced / Tags
 
 Definitions for tags
 """
 # Re-export renamed versions of tags
 from .renames import input_, object_
 from .input import input
+from .dangerous_raw_html import DangerousRawHtml
+from .comment import Comment
 
 # Copy this into pyhtml/__tags/__init__.py
 __all__ = [
     # This one is generated by hand
     'input',
+    # These are extra features of PyHTML enhanced
+    'DangerousRawHtml',
+    'Comment',
     # These two are renamed
     'input_',
     'object_',
     # These are generated
     'html',
     'base',
     'head',
```

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__tags/generated.py` & `pyhtml_enhanced-2.0.1/pyhtml/__tags/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -9406,3427 +9406,3430 @@
 00024bd0: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
 00024be0: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
 00024bf0: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
 00024c00: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
 00024c10: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
 00024c20: 7475 726e 207b 2774 7970 6527 3a20 2774  turn {'type': 't
 00024c30: 6578 742f 6a61 7661 7363 7269 7074 277d  ext/javascript'}
-00024c40: 0a0a 0a63 6c61 7373 2064 656c 5f28 5461  ...class del_(Ta
-00024c50: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
-00024c60: 5265 7072 6573 656e 7473 2061 2072 616e  Represents a ran
-00024c70: 6765 206f 6620 7465 7874 2074 6861 7420  ge of text that 
-00024c80: 6861 7320 6265 656e 2064 656c 6574 6564  has been deleted
-00024c90: 2066 726f 6d20 6120 646f 6375 6d65 6e74   from a document
-00024ca0: 2e20 5468 6973 2063 616e 2062 6520 7573  . This can be us
-00024cb0: 6564 2077 6865 6e20 7265 6e64 6572 696e  ed when renderin
-00024cc0: 6720 2274 7261 636b 2063 6861 6e67 6573  g "track changes
-00024cd0: 2220 6f72 2073 6f75 7263 6520 636f 6465  " or source code
-00024ce0: 2064 6966 6620 696e 666f 726d 6174 696f   diff informatio
-00024cf0: 6e2c 2066 6f72 2065 7861 6d70 6c65 2e20  n, for example. 
-00024d00: 5468 6520 603c 696e 733e 6020 656c 656d  The `<ins>` elem
-00024d10: 656e 7420 6361 6e20 6265 2075 7365 6420  ent can be used 
-00024d20: 666f 7220 7468 6520 6f70 706f 7369 7465  for the opposite
-00024d30: 2070 7572 706f 7365 3a20 746f 2069 6e64   purpose: to ind
-00024d40: 6963 6174 6520 7465 7874 2074 6861 7420  icate text that 
-00024d50: 6861 7320 6265 656e 2061 6464 6564 2074  has been added t
-00024d60: 6f20 7468 6520 646f 6375 6d65 6e74 2e0a  o the document..
-00024d70: 0a20 2020 200a 0a20 2020 205b 5669 6577  .    ..    [View
-00024d80: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-00024d90: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-00024da0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-00024db0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-00024dc0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f64  b/HTML/Element/d
-00024dd0: 656c 290a 2020 2020 2222 220a 2020 2020  el).    """.    
-00024de0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00024df0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00024e00: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-00024e10: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-00024e20: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00024e30: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-00024e40: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-00024e50: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00024e60: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00024e70: 7072 6573 656e 7473 2061 2072 616e 6765  presents a range
-00024e80: 206f 6620 7465 7874 2074 6861 7420 6861   of text that ha
-00024e90: 7320 6265 656e 2064 656c 6574 6564 2066  s been deleted f
-00024ea0: 726f 6d20 6120 646f 6375 6d65 6e74 2e20  rom a document. 
-00024eb0: 5468 6973 2063 616e 2062 6520 7573 6564  This can be used
-00024ec0: 2077 6865 6e20 7265 6e64 6572 696e 6720   when rendering 
-00024ed0: 2274 7261 636b 2063 6861 6e67 6573 2220  "track changes" 
-00024ee0: 6f72 2073 6f75 7263 6520 636f 6465 2064  or source code d
-00024ef0: 6966 6620 696e 666f 726d 6174 696f 6e2c  iff information,
-00024f00: 2066 6f72 2065 7861 6d70 6c65 2e20 5468   for example. Th
-00024f10: 6520 603c 696e 733e 6020 656c 656d 656e  e `<ins>` elemen
-00024f20: 7420 6361 6e20 6265 2075 7365 6420 666f  t can be used fo
-00024f30: 7220 7468 6520 6f70 706f 7369 7465 2070  r the opposite p
-00024f40: 7572 706f 7365 3a20 746f 2069 6e64 6963  urpose: to indic
-00024f50: 6174 6520 7465 7874 2074 6861 7420 6861  ate text that ha
-00024f60: 7320 6265 656e 2061 6464 6564 2074 6f20  s been added to 
-00024f70: 7468 6520 646f 6375 6d65 6e74 2e0a 0a20  the document... 
-00024f80: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-00024f90: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-00024fa0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00024fb0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-00024fc0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-00024fd0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-00024fe0: 6d65 6e74 2f64 656c 290a 2020 2020 2020  ment/del).      
-00024ff0: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
-00025000: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
-00025010: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00025020: 2020 207d 0a20 2020 2020 2020 2073 7570     }.        sup
-00025030: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a63  er().__init__(*c
-00025040: 6869 6c64 7265 6e2c 202a 2a61 7474 7269  hildren, **attri
-00025050: 6275 7465 7329 0a0a 2020 2020 6465 6620  butes)..    def 
-00025060: 5f5f 6361 6c6c 5f5f 2820 2023 2074 7970  __call__(  # typ
-00025070: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-00025080: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00025090: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
-000250a0: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
-000250b0: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
-000250c0: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
-000250d0: 6554 7970 652c 0a20 2020 2029 3a0a 2020  eType,.    ):.  
-000250e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000250f0: 2020 5265 7072 6573 656e 7473 2061 2072    Represents a r
-00025100: 616e 6765 206f 6620 7465 7874 2074 6861  ange of text tha
-00025110: 7420 6861 7320 6265 656e 2064 656c 6574  t has been delet
-00025120: 6564 2066 726f 6d20 6120 646f 6375 6d65  ed from a docume
-00025130: 6e74 2e20 5468 6973 2063 616e 2062 6520  nt. This can be 
-00025140: 7573 6564 2077 6865 6e20 7265 6e64 6572  used when render
-00025150: 696e 6720 2274 7261 636b 2063 6861 6e67  ing "track chang
-00025160: 6573 2220 6f72 2073 6f75 7263 6520 636f  es" or source co
-00025170: 6465 2064 6966 6620 696e 666f 726d 6174  de diff informat
-00025180: 696f 6e2c 2066 6f72 2065 7861 6d70 6c65  ion, for example
-00025190: 2e20 5468 6520 603c 696e 733e 6020 656c  . The `<ins>` el
-000251a0: 656d 656e 7420 6361 6e20 6265 2075 7365  ement can be use
-000251b0: 6420 666f 7220 7468 6520 6f70 706f 7369  d for the opposi
-000251c0: 7465 2070 7572 706f 7365 3a20 746f 2069  te purpose: to i
-000251d0: 6e64 6963 6174 6520 7465 7874 2074 6861  ndicate text tha
-000251e0: 7420 6861 7320 6265 656e 2061 6464 6564  t has been added
-000251f0: 2074 6f20 7468 6520 646f 6375 6d65 6e74   to the document
-00025200: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
-00025210: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
-00025220: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00025230: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00025240: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-00025250: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-00025260: 2f45 6c65 6d65 6e74 2f64 656c 290a 2020  /Element/del).  
-00025270: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00025280: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-00025290: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-000252a0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000252b0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-000252c0: 5f5f 6361 6c6c 5f5f 282a 6368 696c 6472  __call__(*childr
-000252d0: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
-000252e0: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-000252f0: 6465 6661 756c 745f 6174 7472 6962 7574  default_attribut
-00025300: 6573 2873 656c 662c 2067 6976 656e 3a20  es(self, given: 
-00025310: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
-00025320: 7574 6554 7970 655d 2920 2d3e 2064 6963  uteType]) -> dic
-00025330: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
-00025340: 5479 7065 5d3a 0a20 2020 2020 2020 2072  Type]:.        r
-00025350: 6574 7572 6e20 7b7d 0a0a 0a63 6c61 7373  eturn {}...class
-00025360: 2069 6e73 2854 6167 293a 0a20 2020 2022   ins(Tag):.    "
-00025370: 2222 0a20 2020 2052 6570 7265 7365 6e74  "".    Represent
-00025380: 7320 6120 7261 6e67 6520 6f66 2074 6578  s a range of tex
-00025390: 7420 7468 6174 2068 6173 2062 6565 6e20  t that has been 
-000253a0: 6164 6465 6420 746f 2061 2064 6f63 756d  added to a docum
-000253b0: 656e 742e 2059 6f75 2063 616e 2075 7365  ent. You can use
-000253c0: 2074 6865 2060 3c64 656c 3e60 2065 6c65   the `<del>` ele
-000253d0: 6d65 6e74 2074 6f20 7369 6d69 6c61 726c  ment to similarl
-000253e0: 7920 7265 7072 6573 656e 7420 6120 7261  y represent a ra
-000253f0: 6e67 6520 6f66 2074 6578 7420 7468 6174  nge of text that
-00025400: 2068 6173 2062 6565 6e20 6465 6c65 7465   has been delete
-00025410: 6420 6672 6f6d 2074 6865 2064 6f63 756d  d from the docum
-00025420: 656e 742e 0a0a 2020 2020 0a0a 2020 2020  ent...    ..    
-00025430: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
-00025440: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00025450: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00025460: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-00025470: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-00025480: 656e 742f 696e 7329 0a20 2020 2022 2222  ent/ins).    """
-00025490: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000254a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000254b0: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-000254c0: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-000254d0: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-000254e0: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-000254f0: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-00025500: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-00025510: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00025520: 2020 2052 6570 7265 7365 6e74 7320 6120     Represents a 
-00025530: 7261 6e67 6520 6f66 2074 6578 7420 7468  range of text th
-00025540: 6174 2068 6173 2062 6565 6e20 6164 6465  at has been adde
-00025550: 6420 746f 2061 2064 6f63 756d 656e 742e  d to a document.
-00025560: 2059 6f75 2063 616e 2075 7365 2074 6865   You can use the
-00025570: 2060 3c64 656c 3e60 2065 6c65 6d65 6e74   `<del>` element
-00025580: 2074 6f20 7369 6d69 6c61 726c 7920 7265   to similarly re
-00025590: 7072 6573 656e 7420 6120 7261 6e67 6520  present a range 
-000255a0: 6f66 2074 6578 7420 7468 6174 2068 6173  of text that has
-000255b0: 2062 6565 6e20 6465 6c65 7465 6420 6672   been deleted fr
-000255c0: 6f6d 2074 6865 2064 6f63 756d 656e 742e  om the document.
-000255d0: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
-000255e0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-000255f0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00025600: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-00025610: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-00025620: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-00025630: 456c 656d 656e 742f 696e 7329 0a20 2020  Element/ins).   
-00025640: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00025650: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-00025660: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00025670: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00025680: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00025690: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
-000256a0: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
-000256b0: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
-000256c0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-000256d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000256e0: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-000256f0: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-00025700: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-00025710: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-00025720: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
-00025730: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00025740: 2020 2020 2052 6570 7265 7365 6e74 7320       Represents 
-00025750: 6120 7261 6e67 6520 6f66 2074 6578 7420  a range of text 
-00025760: 7468 6174 2068 6173 2062 6565 6e20 6164  that has been ad
-00025770: 6465 6420 746f 2061 2064 6f63 756d 656e  ded to a documen
-00025780: 742e 2059 6f75 2063 616e 2075 7365 2074  t. You can use t
-00025790: 6865 2060 3c64 656c 3e60 2065 6c65 6d65  he `<del>` eleme
-000257a0: 6e74 2074 6f20 7369 6d69 6c61 726c 7920  nt to similarly 
-000257b0: 7265 7072 6573 656e 7420 6120 7261 6e67  represent a rang
-000257c0: 6520 6f66 2074 6578 7420 7468 6174 2068  e of text that h
-000257d0: 6173 2062 6565 6e20 6465 6c65 7465 6420  as been deleted 
-000257e0: 6672 6f6d 2074 6865 2064 6f63 756d 656e  from the documen
-000257f0: 742e 0a0a 2020 2020 2020 2020 0a0a 2020  t...        ..  
-00025800: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
-00025810: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00025820: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00025830: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00025840: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00025850: 4c2f 456c 656d 656e 742f 696e 7329 0a20  L/Element/ins). 
-00025860: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00025870: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
-00025880: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
-00025890: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000258a0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-000258b0: 2e5f 5f63 616c 6c5f 5f28 2a63 6869 6c64  .__call__(*child
-000258c0: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
-000258d0: 7329 0a0a 2020 2020 6465 6620 5f67 6574  s)..    def _get
-000258e0: 5f64 6566 6175 6c74 5f61 7474 7269 6275  _default_attribu
-000258f0: 7465 7328 7365 6c66 2c20 6769 7665 6e3a  tes(self, given:
-00025900: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
-00025910: 6275 7465 5479 7065 5d29 202d 3e20 6469  buteType]) -> di
-00025920: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
-00025930: 6554 7970 655d 3a0a 2020 2020 2020 2020  eType]:.        
-00025940: 7265 7475 726e 207b 7d0a 0a0a 636c 6173  return {}...clas
-00025950: 7320 6361 7074 696f 6e28 5461 6729 3a0a  s caption(Tag):.
-00025960: 2020 2020 2222 220a 2020 2020 5370 6563      """.    Spec
-00025970: 6966 6965 7320 7468 6520 6361 7074 696f  ifies the captio
-00025980: 6e20 286f 7220 7469 746c 6529 206f 6620  n (or title) of 
-00025990: 6120 7461 626c 652e 0a0a 2020 2020 0a0a  a table...    ..
-000259a0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-000259b0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000259c0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-000259d0: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-000259e0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-000259f0: 456c 656d 656e 742f 6361 7074 696f 6e29  Element/caption)
-00025a00: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
-00025a10: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00025a20: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00025a30: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
-00025a40: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
-00025a50: 2020 0a20 2020 2020 2020 202a 2a61 7474    .        **att
-00025a60: 7269 6275 7465 733a 2041 7474 7269 6275  ributes: Attribu
-00025a70: 7465 5479 7065 2c0a 2020 2020 2920 2d3e  teType,.    ) ->
-00025a80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00025a90: 2222 0a20 2020 2020 2020 2053 7065 6369  "".        Speci
-00025aa0: 6669 6573 2074 6865 2063 6170 7469 6f6e  fies the caption
-00025ab0: 2028 6f72 2074 6974 6c65 2920 6f66 2061   (or title) of a
-00025ac0: 2074 6162 6c65 2e0a 0a20 2020 2020 2020   table...       
-00025ad0: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-00025ae0: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-00025af0: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-00025b00: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-00025b10: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-00025b20: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f63  b/HTML/Element/c
-00025b30: 6170 7469 6f6e 290a 2020 2020 2020 2020  aption).        
-00025b40: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
-00025b50: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
-00025b60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00025b70: 207d 0a20 2020 2020 2020 2073 7570 6572   }.        super
-00025b80: 2829 2e5f 5f69 6e69 745f 5f28 2a63 6869  ().__init__(*chi
-00025b90: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
-00025ba0: 7465 7329 0a0a 2020 2020 6465 6620 5f5f  tes)..    def __
-00025bb0: 6361 6c6c 5f5f 2820 2023 2074 7970 653a  call__(  # type:
-00025bc0: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
-00025bd0: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
-00025be0: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
-00025bf0: 6e54 7970 652c 0a20 2020 2020 2020 200a  nType,.        .
-00025c00: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
-00025c10: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
-00025c20: 7970 652c 0a20 2020 2029 3a0a 2020 2020  ype,.    ):.    
-00025c30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00025c40: 5370 6563 6966 6965 7320 7468 6520 6361  Specifies the ca
-00025c50: 7074 696f 6e20 286f 7220 7469 746c 6529  ption (or title)
-00025c60: 206f 6620 6120 7461 626c 652e 0a0a 2020   of a table...  
-00025c70: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
-00025c80: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
-00025c90: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00025ca0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00025cb0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-00025cc0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-00025cd0: 656e 742f 6361 7074 696f 6e29 0a20 2020  ent/caption).   
-00025ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00025cf0: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-00025d00: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00025d10: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00025d20: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
-00025d30: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
-00025d40: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
-00025d50: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
-00025d60: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
-00025d70: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
-00025d80: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
-00025d90: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
-00025da0: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
-00025db0: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
-00025dc0: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
-00025dd0: 636f 6c28 5461 6729 3a0a 2020 2020 2222  col(Tag):.    ""
-00025de0: 220a 2020 2020 4465 6669 6e65 7320 6f6e  ".    Defines on
-00025df0: 6520 6f72 206d 6f72 6520 636f 6c75 6d6e  e or more column
-00025e00: 7320 696e 2061 2063 6f6c 756d 6e20 6772  s in a column gr
-00025e10: 6f75 7020 7265 7072 6573 656e 7465 6420  oup represented 
-00025e20: 6279 2069 7473 2069 6d70 6c69 6369 7420  by its implicit 
-00025e30: 6f72 2065 7870 6c69 6369 7420 7061 7265  or explicit pare
-00025e40: 6e74 205b 603c 636f 6c67 726f 7570 3e60  nt [`<colgroup>`
-00025e50: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00025e60: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-00025e70: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-00025e80: 544d 4c2f 456c 656d 656e 742f 636f 6c67  TML/Element/colg
-00025e90: 726f 7570 2920 656c 656d 656e 742e 2054  roup) element. T
-00025ea0: 6865 2060 3c63 6f6c 3e60 2065 6c65 6d65  he `<col>` eleme
-00025eb0: 6e74 2069 7320 6f6e 6c79 2076 616c 6964  nt is only valid
-00025ec0: 2061 7320 6120 6368 696c 6420 6f66 2061   as a child of a
-00025ed0: 205b 603c 636f 6c67 726f 7570 3e60 5d28   [`<colgroup>`](
-00025ee0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00025ef0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00025f00: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00025f10: 4c2f 456c 656d 656e 742f 636f 6c67 726f  L/Element/colgro
-00025f20: 7570 2920 656c 656d 656e 7420 7468 6174  up) element that
-00025f30: 2068 6173 206e 6f20 5b60 7370 616e 605d   has no [`span`]
-00025f40: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-00025f50: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00025f60: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00025f70: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 6772  ML/Element/colgr
-00025f80: 6f75 7023 7370 616e 2920 6174 7472 6962  oup#span) attrib
-00025f90: 7574 6520 6465 6669 6e65 642e 0a0a 2020  ute defined...  
-00025fa0: 2020 0a0a 2020 2020 5b56 6965 7720 6675    ..    [View fu
-00025fb0: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
-00025fc0: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00025fd0: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-00025fe0: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-00025ff0: 544d 4c2f 456c 656d 656e 742f 636f 6c29  TML/Element/col)
-00026000: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
-00026010: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00026020: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00026030: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
-00026040: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
-00026050: 2020 0a20 2020 2020 2020 202a 2a61 7474    .        **att
-00026060: 7269 6275 7465 733a 2041 7474 7269 6275  ributes: Attribu
-00026070: 7465 5479 7065 2c0a 2020 2020 2920 2d3e  teType,.    ) ->
-00026080: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00026090: 2222 0a20 2020 2020 2020 2044 6566 696e  "".        Defin
-000260a0: 6573 206f 6e65 206f 7220 6d6f 7265 2063  es one or more c
-000260b0: 6f6c 756d 6e73 2069 6e20 6120 636f 6c75  olumns in a colu
-000260c0: 6d6e 2067 726f 7570 2072 6570 7265 7365  mn group represe
-000260d0: 6e74 6564 2062 7920 6974 7320 696d 706c  nted by its impl
-000260e0: 6963 6974 206f 7220 6578 706c 6963 6974  icit or explicit
-000260f0: 2070 6172 656e 7420 5b60 3c63 6f6c 6772   parent [`<colgr
-00026100: 6f75 703e 605d 2868 7474 7073 3a2f 2f64  oup>`](https://d
-00026110: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-00026120: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-00026130: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00026140: 2f63 6f6c 6772 6f75 7029 2065 6c65 6d65  /colgroup) eleme
-00026150: 6e74 2e20 5468 6520 603c 636f 6c3e 6020  nt. The `<col>` 
-00026160: 656c 656d 656e 7420 6973 206f 6e6c 7920  element is only 
-00026170: 7661 6c69 6420 6173 2061 2063 6869 6c64  valid as a child
-00026180: 206f 6620 6120 5b60 3c63 6f6c 6772 6f75   of a [`<colgrou
-00026190: 703e 605d 2868 7474 7073 3a2f 2f64 6576  p>`](https://dev
-000261a0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-000261b0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-000261c0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f63  b/HTML/Element/c
-000261d0: 6f6c 6772 6f75 7029 2065 6c65 6d65 6e74  olgroup) element
-000261e0: 2074 6861 7420 6861 7320 6e6f 205b 6073   that has no [`s
-000261f0: 7061 6e60 5d28 6874 7470 733a 2f2f 6465  pan`](https://de
-00026200: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-00026210: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-00026220: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-00026230: 636f 6c67 726f 7570 2373 7061 6e29 2061  colgroup#span) a
-00026240: 7474 7269 6275 7465 2064 6566 696e 6564  ttribute defined
-00026250: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
-00026260: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
-00026270: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00026280: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00026290: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-000262a0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-000262b0: 2f45 6c65 6d65 6e74 2f63 6f6c 290a 2020  /Element/col).  
-000262c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000262d0: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-000262e0: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-000262f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00026300: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00026310: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
-00026320: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
-00026330: 6465 6620 5f5f 6361 6c6c 5f5f 2820 2023  def __call__(  #
-00026340: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-00026350: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00026360: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-00026370: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-00026380: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00026390: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-000263a0: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-000263b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000263c0: 2020 2020 2020 4465 6669 6e65 7320 6f6e        Defines on
-000263d0: 6520 6f72 206d 6f72 6520 636f 6c75 6d6e  e or more column
-000263e0: 7320 696e 2061 2063 6f6c 756d 6e20 6772  s in a column gr
-000263f0: 6f75 7020 7265 7072 6573 656e 7465 6420  oup represented 
-00026400: 6279 2069 7473 2069 6d70 6c69 6369 7420  by its implicit 
-00026410: 6f72 2065 7870 6c69 6369 7420 7061 7265  or explicit pare
-00026420: 6e74 205b 603c 636f 6c67 726f 7570 3e60  nt [`<colgroup>`
-00026430: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00026440: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-00026450: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-00026460: 544d 4c2f 456c 656d 656e 742f 636f 6c67  TML/Element/colg
-00026470: 726f 7570 2920 656c 656d 656e 742e 2054  roup) element. T
-00026480: 6865 2060 3c63 6f6c 3e60 2065 6c65 6d65  he `<col>` eleme
-00026490: 6e74 2069 7320 6f6e 6c79 2076 616c 6964  nt is only valid
-000264a0: 2061 7320 6120 6368 696c 6420 6f66 2061   as a child of a
-000264b0: 205b 603c 636f 6c67 726f 7570 3e60 5d28   [`<colgroup>`](
-000264c0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-000264d0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-000264e0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-000264f0: 4c2f 456c 656d 656e 742f 636f 6c67 726f  L/Element/colgro
-00026500: 7570 2920 656c 656d 656e 7420 7468 6174  up) element that
-00026510: 2068 6173 206e 6f20 5b60 7370 616e 605d   has no [`span`]
-00026520: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-00026530: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00026540: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00026550: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 6772  ML/Element/colgr
-00026560: 6f75 7023 7370 616e 2920 6174 7472 6962  oup#span) attrib
-00026570: 7574 6520 6465 6669 6e65 642e 0a0a 2020  ute defined...  
-00026580: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
-00026590: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
-000265a0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-000265b0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-000265c0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-000265d0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-000265e0: 656e 742f 636f 6c29 0a20 2020 2020 2020  ent/col).       
-000265f0: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-00026600: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-00026610: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00026620: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
-00026630: 726e 2073 7570 6572 2829 2e5f 5f63 616c  rn super().__cal
-00026640: 6c5f 5f28 2a63 6869 6c64 7265 6e2c 202a  l__(*children, *
-00026650: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-00026660: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
-00026670: 6c74 5f61 7474 7269 6275 7465 7328 7365  lt_attributes(se
-00026680: 6c66 2c20 6769 7665 6e3a 2064 6963 745b  lf, given: dict[
-00026690: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
-000266a0: 7065 5d29 202d 3e20 6469 6374 5b73 7472  pe]) -> dict[str
-000266b0: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-000266c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000266d0: 207b 7d0a 0a0a 636c 6173 7320 636f 6c67   {}...class colg
-000266e0: 726f 7570 2854 6167 293a 0a20 2020 2022  roup(Tag):.    "
-000266f0: 2222 0a20 2020 2044 6566 696e 6573 2061  "".    Defines a
-00026700: 2067 726f 7570 206f 6620 636f 6c75 6d6e   group of column
-00026710: 7320 7769 7468 696e 2061 2074 6162 6c65  s within a table
-00026720: 2e0a 0a20 2020 200a 0a20 2020 205b 5669  ...    ..    [Vi
-00026730: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-00026740: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00026750: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-00026760: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-00026770: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00026780: 2f63 6f6c 6772 6f75 7029 0a20 2020 2022  /colgroup).    "
-00026790: 2222 0a20 2020 2064 6566 205f 5f69 6e69  "".    def __ini
-000267a0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000267b0: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
-000267c0: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
-000267d0: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
-000267e0: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
-000267f0: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
-00026800: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00026810: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00026820: 2020 2020 2044 6566 696e 6573 2061 2067       Defines a g
-00026830: 726f 7570 206f 6620 636f 6c75 6d6e 7320  roup of columns 
-00026840: 7769 7468 696e 2061 2074 6162 6c65 2e0a  within a table..
-00026850: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
-00026860: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
-00026870: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00026880: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-00026890: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-000268a0: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-000268b0: 6c65 6d65 6e74 2f63 6f6c 6772 6f75 7029  lement/colgroup)
-000268c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000268d0: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
-000268e0: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
-000268f0: 200a 2020 2020 2020 2020 7d0a 2020 2020   .        }.    
-00026900: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00026910: 6974 5f5f 282a 6368 696c 6472 656e 2c20  it__(*children, 
-00026920: 2a2a 6174 7472 6962 7574 6573 290a 0a20  **attributes).. 
-00026930: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00026940: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00026950: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00026960: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-00026970: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-00026980: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00026990: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
-000269a0: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
-000269b0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000269c0: 0a20 2020 2020 2020 2044 6566 696e 6573  .        Defines
-000269d0: 2061 2067 726f 7570 206f 6620 636f 6c75   a group of colu
-000269e0: 6d6e 7320 7769 7468 696e 2061 2074 6162  mns within a tab
-000269f0: 6c65 2e0a 0a20 2020 2020 2020 200a 0a20  le...        .. 
-00026a00: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
-00026a10: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-00026a20: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-00026a30: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00026a40: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00026a50: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 6772  ML/Element/colgr
-00026a60: 6f75 7029 0a20 2020 2020 2020 2022 2222  oup).        """
-00026a70: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
-00026a80: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
-00026a90: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
-00026aa0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00026ab0: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-00026ac0: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
-00026ad0: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
-00026ae0: 6620 5f67 6574 5f64 6566 6175 6c74 5f61  f _get_default_a
-00026af0: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
-00026b00: 6769 7665 6e3a 2064 6963 745b 7374 722c  given: dict[str,
-00026b10: 2041 7474 7269 6275 7465 5479 7065 5d29   AttributeType])
-00026b20: 202d 3e20 6469 6374 5b73 7472 2c20 4174   -> dict[str, At
-00026b30: 7472 6962 7574 6554 7970 655d 3a0a 2020  tributeType]:.  
-00026b40: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
-00026b50: 0a0a 636c 6173 7320 7461 626c 6528 5461  ..class table(Ta
-00026b60: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
-00026b70: 5265 7072 6573 656e 7473 2074 6162 756c  Represents tabul
-00026b80: 6172 2064 6174 61e2 8094 7468 6174 2069  ar data...that i
-00026b90: 732c 2069 6e66 6f72 6d61 7469 6f6e 2070  s, information p
-00026ba0: 7265 7365 6e74 6564 2069 6e20 6120 7477  resented in a tw
-00026bb0: 6f2d 6469 6d65 6e73 696f 6e61 6c20 7461  o-dimensional ta
-00026bc0: 626c 6520 636f 6d70 7269 7365 6420 6f66  ble comprised of
-00026bd0: 2072 6f77 7320 616e 6420 636f 6c75 6d6e   rows and column
-00026be0: 7320 6f66 2063 656c 6c73 2063 6f6e 7461  s of cells conta
-00026bf0: 696e 696e 6720 6461 7461 2e0a 0a20 2020  ining data...   
-00026c00: 200a 0a20 2020 205b 5669 6577 2066 756c   ..    [View ful
-00026c10: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-00026c20: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-00026c30: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00026c40: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00026c50: 4d4c 2f45 6c65 6d65 6e74 2f74 6162 6c65  ML/Element/table
-00026c60: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
-00026c70: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00026c80: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00026c90: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
-00026ca0: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
-00026cb0: 2020 200a 2020 2020 2020 2020 6964 3a20     .        id: 
-00026cc0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00026cd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 5f63  None,.        _c
-00026ce0: 6c61 7373 3a20 4f70 7469 6f6e 616c 5b73  lass: Optional[s
-00026cf0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00026d00: 2020 2020 7374 796c 653a 204f 7074 696f      style: Optio
-00026d10: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00026d20: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
-00026d30: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
-00026d40: 5479 7065 2c0a 2020 2020 2920 2d3e 204e  Type,.    ) -> N
-00026d50: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00026d60: 0a20 2020 2020 2020 2052 6570 7265 7365  .        Represe
-00026d70: 6e74 7320 7461 6275 6c61 7220 6461 7461  nts tabular data
-00026d80: e280 9474 6861 7420 6973 2c20 696e 666f  ...that is, info
-00026d90: 726d 6174 696f 6e20 7072 6573 656e 7465  rmation presente
-00026da0: 6420 696e 2061 2074 776f 2d64 696d 656e  d in a two-dimen
-00026db0: 7369 6f6e 616c 2074 6162 6c65 2063 6f6d  sional table com
-00026dc0: 7072 6973 6564 206f 6620 726f 7773 2061  prised of rows a
-00026dd0: 6e64 2063 6f6c 756d 6e73 206f 6620 6365  nd columns of ce
-00026de0: 6c6c 7320 636f 6e74 6169 6e69 6e67 2064  lls containing d
-00026df0: 6174 612e 0a0a 2020 2020 2020 2020 0a0a  ata...        ..
-00026e00: 2020 2020 2020 2020 5b56 6965 7720 6675          [View fu
-00026e10: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
-00026e20: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00026e30: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-00026e40: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-00026e50: 544d 4c2f 456c 656d 656e 742f 7461 626c  TML/Element/tabl
-00026e60: 6529 0a20 2020 2020 2020 2022 2222 0a20  e).        """. 
-00026e70: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
-00026e80: 7320 7c3d 207b 0a20 2020 2020 2020 2020  s |= {.         
-00026e90: 2020 2027 5f63 6c61 7373 273a 205f 636c     '_class': _cl
-00026ea0: 6173 732c 0a20 2020 2020 2020 2020 2020  ass,.           
-00026eb0: 2027 6964 273a 2069 642c 0a20 2020 2020   'id': id,.     
-00026ec0: 2020 2020 2020 2027 7374 796c 6527 3a20         'style': 
-00026ed0: 7374 796c 652c 0a20 2020 2020 2020 2020  style,.         
-00026ee0: 2020 200a 2020 2020 2020 2020 7d0a 2020     .        }.  
-00026ef0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00026f00: 696e 6974 5f5f 282a 6368 696c 6472 656e  init__(*children
-00026f10: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
-00026f20: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-00026f30: 5f28 2020 2320 7479 7065 3a20 6967 6e6f  _(  # type: igno
-00026f40: 7265 0a20 2020 2020 2020 2073 656c 662c  re.        self,
-00026f50: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-00026f60: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-00026f70: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-00026f80: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
-00026f90: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00026fa0: 2020 2020 205f 636c 6173 733a 204f 7074       _class: Opt
-00026fb0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00026fc0: 652c 0a20 2020 2020 2020 2073 7479 6c65  e,.        style
-00026fd0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00026fe0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00026ff0: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
-00027000: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
-00027010: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-00027020: 2020 2020 2020 2020 5265 7072 6573 656e          Represen
-00027030: 7473 2074 6162 756c 6172 2064 6174 61e2  ts tabular data.
-00027040: 8094 7468 6174 2069 732c 2069 6e66 6f72  ..that is, infor
-00027050: 6d61 7469 6f6e 2070 7265 7365 6e74 6564  mation presented
-00027060: 2069 6e20 6120 7477 6f2d 6469 6d65 6e73   in a two-dimens
-00027070: 696f 6e61 6c20 7461 626c 6520 636f 6d70  ional table comp
-00027080: 7269 7365 6420 6f66 2072 6f77 7320 616e  rised of rows an
-00027090: 6420 636f 6c75 6d6e 7320 6f66 2063 656c  d columns of cel
-000270a0: 6c73 2063 6f6e 7461 696e 696e 6720 6461  ls containing da
-000270b0: 7461 2e0a 0a20 2020 2020 2020 200a 0a20  ta...        .. 
-000270c0: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
-000270d0: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-000270e0: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-000270f0: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00027100: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00027110: 4d4c 2f45 6c65 6d65 6e74 2f74 6162 6c65  ML/Element/table
-00027120: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00027130: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
-00027140: 207c 3d20 7b0a 2020 2020 2020 2020 2020   |= {.          
-00027150: 2020 275f 636c 6173 7327 3a20 5f63 6c61    '_class': _cla
-00027160: 7373 2c0a 2020 2020 2020 2020 2020 2020  ss,.            
-00027170: 2769 6427 3a20 6964 2c0a 2020 2020 2020  'id': id,.      
-00027180: 2020 2020 2020 2773 7479 6c65 273a 2073        'style': s
-00027190: 7479 6c65 2c0a 2020 2020 2020 2020 2020  tyle,.          
-000271a0: 2020 0a20 2020 2020 2020 207d 0a20 2020    .        }.   
-000271b0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000271c0: 7228 292e 5f5f 6361 6c6c 5f5f 282a 6368  r().__call__(*ch
-000271d0: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
-000271e0: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
-000271f0: 6765 745f 6465 6661 756c 745f 6174 7472  get_default_attr
-00027200: 6962 7574 6573 2873 656c 662c 2067 6976  ibutes(self, giv
-00027210: 656e 3a20 6469 6374 5b73 7472 2c20 4174  en: dict[str, At
-00027220: 7472 6962 7574 6554 7970 655d 2920 2d3e  tributeType]) ->
-00027230: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
-00027240: 6275 7465 5479 7065 5d3a 0a20 2020 2020  buteType]:.     
-00027250: 2020 2072 6574 7572 6e20 7b7d 0a0a 0a63     return {}...c
-00027260: 6c61 7373 2074 626f 6479 2854 6167 293a  lass tbody(Tag):
-00027270: 0a20 2020 2022 2222 0a20 2020 2045 6e63  .    """.    Enc
-00027280: 6170 7375 6c61 7465 7320 6120 7365 7420  apsulates a set 
-00027290: 6f66 2074 6162 6c65 2072 6f77 7320 285b  of table rows ([
-000272a0: 603c 7472 3e60 5d28 6874 7470 733a 2f2f  `<tr>`](https://
-000272b0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-000272c0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-000272d0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-000272e0: 742f 7472 2920 656c 656d 656e 7473 292c  t/tr) elements),
-000272f0: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
-00027300: 2074 6865 7920 636f 6d70 7269 7365 2074   they comprise t
-00027310: 6865 2062 6f64 7920 6f66 2061 2074 6162  he body of a tab
-00027320: 6c65 2773 2028 6d61 696e 2920 6461 7461  le's (main) data
-00027330: 2e0a 0a20 2020 200a 0a20 2020 205b 5669  ...    ..    [Vi
-00027340: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-00027350: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00027360: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-00027370: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-00027380: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00027390: 2f74 626f 6479 290a 2020 2020 2222 220a  /tbody).    """.
-000273a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000273b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000273c0: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
-000273d0: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
-000273e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000273f0: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
-00027400: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
-00027410: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
-00027420: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00027430: 2020 456e 6361 7073 756c 6174 6573 2061    Encapsulates a
-00027440: 2073 6574 206f 6620 7461 626c 6520 726f   set of table ro
-00027450: 7773 2028 5b60 3c74 723e 605d 2868 7474  ws ([`<tr>`](htt
-00027460: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-00027470: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-00027480: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-00027490: 6c65 6d65 6e74 2f74 7229 2065 6c65 6d65  lement/tr) eleme
-000274a0: 6e74 7329 2c20 696e 6469 6361 7469 6e67  nts), indicating
-000274b0: 2074 6861 7420 7468 6579 2063 6f6d 7072   that they compr
-000274c0: 6973 6520 7468 6520 626f 6479 206f 6620  ise the body of 
-000274d0: 6120 7461 626c 6527 7320 286d 6169 6e29  a table's (main)
-000274e0: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
-000274f0: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
-00027500: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
-00027510: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
-00027520: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
-00027530: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
-00027540: 2f48 544d 4c2f 456c 656d 656e 742f 7462  /HTML/Element/tb
-00027550: 6f64 7929 0a20 2020 2020 2020 2022 2222  ody).        """
-00027560: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
-00027570: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
-00027580: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
-00027590: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-000275a0: 5f5f 696e 6974 5f5f 282a 6368 696c 6472  __init__(*childr
-000275b0: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
-000275c0: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
-000275d0: 6c5f 5f28 2020 2320 7479 7065 3a20 6967  l__(  # type: ig
-000275e0: 6e6f 7265 0a20 2020 2020 2020 2073 656c  nore.        sel
-000275f0: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
-00027600: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
-00027610: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
-00027620: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
-00027630: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
-00027640: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00027650: 2022 2222 0a20 2020 2020 2020 2045 6e63   """.        Enc
-00027660: 6170 7375 6c61 7465 7320 6120 7365 7420  apsulates a set 
-00027670: 6f66 2074 6162 6c65 2072 6f77 7320 285b  of table rows ([
-00027680: 603c 7472 3e60 5d28 6874 7470 733a 2f2f  `<tr>`](https://
-00027690: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-000276a0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-000276b0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-000276c0: 742f 7472 2920 656c 656d 656e 7473 292c  t/tr) elements),
-000276d0: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
-000276e0: 2074 6865 7920 636f 6d70 7269 7365 2074   they comprise t
-000276f0: 6865 2062 6f64 7920 6f66 2061 2074 6162  he body of a tab
-00027700: 6c65 2773 2028 6d61 696e 2920 6461 7461  le's (main) data
-00027710: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
-00027720: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
-00027730: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00027740: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00027750: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-00027760: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-00027770: 2f45 6c65 6d65 6e74 2f74 626f 6479 290a  /Element/tbody).
-00027780: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00027790: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
-000277a0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000277b0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-000277c0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-000277d0: 292e 5f5f 6361 6c6c 5f5f 282a 6368 696c  ).__call__(*chil
-000277e0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
-000277f0: 6573 290a 0a20 2020 2064 6566 205f 6765  es)..    def _ge
-00027800: 745f 6465 6661 756c 745f 6174 7472 6962  t_default_attrib
-00027810: 7574 6573 2873 656c 662c 2067 6976 656e  utes(self, given
-00027820: 3a20 6469 6374 5b73 7472 2c20 4174 7472  : dict[str, Attr
-00027830: 6962 7574 6554 7970 655d 2920 2d3e 2064  ibuteType]) -> d
-00027840: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
-00027850: 7465 5479 7065 5d3a 0a20 2020 2020 2020  teType]:.       
-00027860: 2072 6574 7572 6e20 7b7d 0a0a 0a63 6c61   return {}...cla
-00027870: 7373 2074 6428 5461 6729 3a0a 2020 2020  ss td(Tag):.    
-00027880: 2222 220a 2020 2020 4120 6368 696c 6420  """.    A child 
-00027890: 6f66 2074 6865 205b 603c 7472 3e60 5d28  of the [`<tr>`](
-000278a0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-000278b0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-000278c0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-000278d0: 4c2f 456c 656d 656e 742f 7472 2920 656c  L/Element/tr) el
-000278e0: 656d 656e 742c 2069 7420 6465 6669 6e65  ement, it define
-000278f0: 7320 6120 6365 6c6c 206f 6620 6120 7461  s a cell of a ta
-00027900: 626c 6520 7468 6174 2063 6f6e 7461 696e  ble that contain
-00027910: 7320 6461 7461 2e0a 0a20 2020 202a 2060  s data...    * `
-00027920: 636f 6c73 7061 6e60 3a20 5468 6520 6e75  colspan`: The nu
-00027930: 6d62 6572 206f 6620 636f 6c75 6d6e 7320  mber of columns 
-00027940: 696e 2074 6865 2074 6162 6c65 2074 6861  in the table tha
-00027950: 7420 7468 6973 2063 656c 6c20 7370 616e  t this cell span
-00027960: 732e 0a20 2020 202a 2060 726f 7773 7061  s..    * `rowspa
-00027970: 6e60 3a20 5468 6520 6e75 6d62 6572 206f  n`: The number o
-00027980: 6620 726f 7773 2069 6e20 7468 6520 7461  f rows in the ta
-00027990: 626c 6520 7468 6174 2074 6869 7320 6365  ble that this ce
-000279a0: 6c6c 2073 7061 6e73 2e0a 0a20 2020 205b  ll spans...    [
-000279b0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-000279c0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-000279d0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-000279e0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-000279f0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-00027a00: 6e74 2f74 6429 0a20 2020 2022 2222 0a20  nt/td).    """. 
-00027a10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00027a20: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00027a30: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-00027a40: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-00027a50: 2020 2020 2020 2020 636f 6c73 7061 6e3a          colspan:
-00027a60: 2041 7474 7269 6275 7465 5479 7065 203d   AttributeType =
-00027a70: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-00027a80: 6f77 7370 616e 3a20 4174 7472 6962 7574  owspan: Attribut
-00027a90: 6554 7970 6520 3d20 4e6f 6e65 2c0a 2020  eType = None,.  
-00027aa0: 2020 2020 2020 6964 3a20 4f70 7469 6f6e        id: Option
-00027ab0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00027ac0: 2020 2020 2020 2020 5f63 6c61 7373 3a20          _class: 
-00027ad0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00027ae0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00027af0: 796c 653a 204f 7074 696f 6e61 6c5b 7374  yle: Optional[st
-00027b00: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00027b10: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-00027b20: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-00027b30: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-00027b40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00027b50: 2020 2041 2063 6869 6c64 206f 6620 7468     A child of th
-00027b60: 6520 5b60 3c74 723e 605d 2868 7474 7073  e [`<tr>`](https
-00027b70: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-00027b80: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-00027b90: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-00027ba0: 6d65 6e74 2f74 7229 2065 6c65 6d65 6e74  ment/tr) element
-00027bb0: 2c20 6974 2064 6566 696e 6573 2061 2063  , it defines a c
-00027bc0: 656c 6c20 6f66 2061 2074 6162 6c65 2074  ell of a table t
-00027bd0: 6861 7420 636f 6e74 6169 6e73 2064 6174  hat contains dat
-00027be0: 612e 0a0a 2020 2020 2020 2020 2a20 6063  a...        * `c
-00027bf0: 6f6c 7370 616e 603a 2054 6865 206e 756d  olspan`: The num
-00027c00: 6265 7220 6f66 2063 6f6c 756d 6e73 2069  ber of columns i
-00027c10: 6e20 7468 6520 7461 626c 6520 7468 6174  n the table that
-00027c20: 2074 6869 7320 6365 6c6c 2073 7061 6e73   this cell spans
-00027c30: 2e0a 2020 2020 2020 2020 2a20 6072 6f77  ..        * `row
-00027c40: 7370 616e 603a 2054 6865 206e 756d 6265  span`: The numbe
-00027c50: 7220 6f66 2072 6f77 7320 696e 2074 6865  r of rows in the
-00027c60: 2074 6162 6c65 2074 6861 7420 7468 6973   table that this
-00027c70: 2063 656c 6c20 7370 616e 732e 0a0a 2020   cell spans...  
-00027c80: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
-00027c90: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00027ca0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00027cb0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00027cc0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00027cd0: 4c2f 456c 656d 656e 742f 7464 290a 2020  L/Element/td).  
-00027ce0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00027cf0: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-00027d00: 7b0a 2020 2020 2020 2020 2020 2020 275f  {.            '_
-00027d10: 636c 6173 7327 3a20 5f63 6c61 7373 2c0a  class': _class,.
-00027d20: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
-00027d30: 3a20 6964 2c0a 2020 2020 2020 2020 2020  : id,.          
-00027d40: 2020 2773 7479 6c65 273a 2073 7479 6c65    'style': style
-00027d50: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
-00027d60: 6f6c 7370 616e 273a 2063 6f6c 7370 616e  olspan': colspan
-00027d70: 2c0a 2020 2020 2020 2020 2020 2020 2772  ,.            'r
-00027d80: 6f77 7370 616e 273a 2072 6f77 7370 616e  owspan': rowspan
-00027d90: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-00027da0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00027db0: 6974 5f5f 282a 6368 696c 6472 656e 2c20  it__(*children, 
-00027dc0: 2a2a 6174 7472 6962 7574 6573 290a 0a20  **attributes).. 
-00027dd0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00027de0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00027df0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00027e00: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-00027e10: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-00027e20: 2020 2020 2020 2020 636f 6c73 7061 6e3a          colspan:
-00027e30: 2041 7474 7269 6275 7465 5479 7065 203d   AttributeType =
-00027e40: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-00027e50: 6f77 7370 616e 3a20 4174 7472 6962 7574  owspan: Attribut
-00027e60: 6554 7970 6520 3d20 4e6f 6e65 2c0a 2020  eType = None,.  
-00027e70: 2020 2020 2020 6964 3a20 4f70 7469 6f6e        id: Option
-00027e80: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00027e90: 2020 2020 2020 2020 5f63 6c61 7373 3a20          _class: 
-00027ea0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00027eb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00027ec0: 796c 653a 204f 7074 696f 6e61 6c5b 7374  yle: Optional[st
-00027ed0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00027ee0: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-00027ef0: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-00027f00: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00027f10: 2222 0a20 2020 2020 2020 2041 2063 6869  "".        A chi
-00027f20: 6c64 206f 6620 7468 6520 5b60 3c74 723e  ld of the [`<tr>
-00027f30: 605d 2868 7474 7073 3a2f 2f64 6576 656c  `](https://devel
-00027f40: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-00027f50: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-00027f60: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 7229  HTML/Element/tr)
-00027f70: 2065 6c65 6d65 6e74 2c20 6974 2064 6566   element, it def
-00027f80: 696e 6573 2061 2063 656c 6c20 6f66 2061  ines a cell of a
-00027f90: 2074 6162 6c65 2074 6861 7420 636f 6e74   table that cont
-00027fa0: 6169 6e73 2064 6174 612e 0a0a 2020 2020  ains data...    
-00027fb0: 2020 2020 2a20 6063 6f6c 7370 616e 603a      * `colspan`:
-00027fc0: 2054 6865 206e 756d 6265 7220 6f66 2063   The number of c
-00027fd0: 6f6c 756d 6e73 2069 6e20 7468 6520 7461  olumns in the ta
-00027fe0: 626c 6520 7468 6174 2074 6869 7320 6365  ble that this ce
-00027ff0: 6c6c 2073 7061 6e73 2e0a 2020 2020 2020  ll spans..      
-00028000: 2020 2a20 6072 6f77 7370 616e 603a 2054    * `rowspan`: T
-00028010: 6865 206e 756d 6265 7220 6f66 2072 6f77  he number of row
-00028020: 7320 696e 2074 6865 2074 6162 6c65 2074  s in the table t
-00028030: 6861 7420 7468 6973 2063 656c 6c20 7370  hat this cell sp
-00028040: 616e 732e 0a0a 2020 2020 2020 2020 5b56  ans...        [V
-00028050: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
-00028060: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-00028070: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-00028080: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-00028090: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-000280a0: 742f 7464 290a 2020 2020 2020 2020 2222  t/td).        ""
-000280b0: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-000280c0: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-000280d0: 2020 2020 2020 275f 636c 6173 7327 3a20        '_class': 
-000280e0: 5f63 6c61 7373 2c0a 2020 2020 2020 2020  _class,.        
-000280f0: 2020 2020 2769 6427 3a20 6964 2c0a 2020      'id': id,.  
-00028100: 2020 2020 2020 2020 2020 2773 7479 6c65            'style
-00028110: 273a 2073 7479 6c65 2c0a 2020 2020 2020  ': style,.      
-00028120: 2020 2020 2020 2763 6f6c 7370 616e 273a        'colspan':
-00028130: 2063 6f6c 7370 616e 2c0a 2020 2020 2020   colspan,.      
-00028140: 2020 2020 2020 2772 6f77 7370 616e 273a        'rowspan':
-00028150: 2072 6f77 7370 616e 2c0a 2020 2020 2020   rowspan,.      
-00028160: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
-00028170: 726e 2073 7570 6572 2829 2e5f 5f63 616c  rn super().__cal
-00028180: 6c5f 5f28 2a63 6869 6c64 7265 6e2c 202a  l__(*children, *
-00028190: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-000281a0: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
-000281b0: 6c74 5f61 7474 7269 6275 7465 7328 7365  lt_attributes(se
-000281c0: 6c66 2c20 6769 7665 6e3a 2064 6963 745b  lf, given: dict[
-000281d0: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
-000281e0: 7065 5d29 202d 3e20 6469 6374 5b73 7472  pe]) -> dict[str
-000281f0: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-00028200: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00028210: 207b 2763 6f6c 7370 616e 273a 204e 6f6e   {'colspan': Non
-00028220: 652c 2027 726f 7773 7061 6e27 3a20 4e6f  e, 'rowspan': No
-00028230: 6e65 7d0a 0a0a 636c 6173 7320 7466 6f6f  ne}...class tfoo
-00028240: 7428 5461 6729 3a0a 2020 2020 2222 220a  t(Tag):.    """.
-00028250: 2020 2020 456e 6361 7073 756c 6174 6573      Encapsulates
-00028260: 2061 2073 6574 206f 6620 7461 626c 6520   a set of table 
-00028270: 726f 7773 2028 5b60 3c74 723e 605d 2868  rows ([`<tr>`](h
-00028280: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00028290: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-000282a0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-000282b0: 2f45 6c65 6d65 6e74 2f74 7229 2065 6c65  /Element/tr) ele
-000282c0: 6d65 6e74 7329 2c20 696e 6469 6361 7469  ments), indicati
-000282d0: 6e67 2074 6861 7420 7468 6579 2063 6f6d  ng that they com
-000282e0: 7072 6973 6520 7468 6520 666f 6f74 206f  prise the foot o
-000282f0: 6620 6120 7461 626c 6520 7769 7468 2069  f a table with i
-00028300: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00028310: 2074 6865 2074 6162 6c65 2773 2063 6f6c   the table's col
-00028320: 756d 6e73 2e20 5468 6973 2069 7320 7573  umns. This is us
-00028330: 7561 6c6c 7920 6120 7375 6d6d 6172 7920  ually a summary 
-00028340: 6f66 2074 6865 2063 6f6c 756d 6e73 2c20  of the columns, 
-00028350: 652e 672e 2c20 6120 7375 6d20 6f66 2074  e.g., a sum of t
-00028360: 6865 2067 6976 656e 206e 756d 6265 7273  he given numbers
-00028370: 2069 6e20 6120 636f 6c75 6d6e 2e0a 0a20   in a column... 
-00028380: 2020 200a 0a20 2020 205b 5669 6577 2066     ..    [View f
-00028390: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
-000283a0: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
-000283b0: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-000283c0: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-000283d0: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 666f  HTML/Element/tfo
-000283e0: 6f74 290a 2020 2020 2222 220a 2020 2020  ot).    """.    
-000283f0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00028400: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00028410: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-00028420: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-00028430: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00028440: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-00028450: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-00028460: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00028470: 2020 2222 220a 2020 2020 2020 2020 456e    """.        En
-00028480: 6361 7073 756c 6174 6573 2061 2073 6574  capsulates a set
-00028490: 206f 6620 7461 626c 6520 726f 7773 2028   of table rows (
-000284a0: 5b60 3c74 723e 605d 2868 7474 7073 3a2f  [`<tr>`](https:/
-000284b0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-000284c0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-000284d0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-000284e0: 6e74 2f74 7229 2065 6c65 6d65 6e74 7329  nt/tr) elements)
-000284f0: 2c20 696e 6469 6361 7469 6e67 2074 6861  , indicating tha
-00028500: 7420 7468 6579 2063 6f6d 7072 6973 6520  t they comprise 
-00028510: 7468 6520 666f 6f74 206f 6620 6120 7461  the foot of a ta
-00028520: 626c 6520 7769 7468 2069 6e66 6f72 6d61  ble with informa
-00028530: 7469 6f6e 2061 626f 7574 2074 6865 2074  tion about the t
-00028540: 6162 6c65 2773 2063 6f6c 756d 6e73 2e20  able's columns. 
-00028550: 5468 6973 2069 7320 7573 7561 6c6c 7920  This is usually 
-00028560: 6120 7375 6d6d 6172 7920 6f66 2074 6865  a summary of the
-00028570: 2063 6f6c 756d 6e73 2c20 652e 672e 2c20   columns, e.g., 
-00028580: 6120 7375 6d20 6f66 2074 6865 2067 6976  a sum of the giv
-00028590: 656e 206e 756d 6265 7273 2069 6e20 6120  en numbers in a 
-000285a0: 636f 6c75 6d6e 2e0a 0a20 2020 2020 2020  column...       
-000285b0: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-000285c0: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-000285d0: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-000285e0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-000285f0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-00028600: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f74  b/HTML/Element/t
-00028610: 666f 6f74 290a 2020 2020 2020 2020 2222  foot).        ""
-00028620: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-00028630: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-00028640: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
-00028650: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00028660: 2e5f 5f69 6e69 745f 5f28 2a63 6869 6c64  .__init__(*child
-00028670: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
-00028680: 7329 0a0a 2020 2020 6465 6620 5f5f 6361  s)..    def __ca
-00028690: 6c6c 5f5f 2820 2023 2074 7970 653a 2069  ll__(  # type: i
-000286a0: 676e 6f72 650a 2020 2020 2020 2020 7365  gnore.        se
-000286b0: 6c66 2c0a 2020 2020 2020 2020 2a63 6869  lf,.        *chi
-000286c0: 6c64 7265 6e3a 2043 6869 6c64 7265 6e54  ldren: ChildrenT
-000286d0: 7970 652c 0a20 2020 2020 2020 200a 2020  ype,.        .  
-000286e0: 2020 2020 2020 2a2a 6174 7472 6962 7574        **attribut
-000286f0: 6573 3a20 4174 7472 6962 7574 6554 7970  es: AttributeTyp
-00028700: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00028710: 2020 2222 220a 2020 2020 2020 2020 456e    """.        En
-00028720: 6361 7073 756c 6174 6573 2061 2073 6574  capsulates a set
-00028730: 206f 6620 7461 626c 6520 726f 7773 2028   of table rows (
-00028740: 5b60 3c74 723e 605d 2868 7474 7073 3a2f  [`<tr>`](https:/
-00028750: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-00028760: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-00028770: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-00028780: 6e74 2f74 7229 2065 6c65 6d65 6e74 7329  nt/tr) elements)
-00028790: 2c20 696e 6469 6361 7469 6e67 2074 6861  , indicating tha
-000287a0: 7420 7468 6579 2063 6f6d 7072 6973 6520  t they comprise 
-000287b0: 7468 6520 666f 6f74 206f 6620 6120 7461  the foot of a ta
-000287c0: 626c 6520 7769 7468 2069 6e66 6f72 6d61  ble with informa
-000287d0: 7469 6f6e 2061 626f 7574 2074 6865 2074  tion about the t
-000287e0: 6162 6c65 2773 2063 6f6c 756d 6e73 2e20  able's columns. 
-000287f0: 5468 6973 2069 7320 7573 7561 6c6c 7920  This is usually 
-00028800: 6120 7375 6d6d 6172 7920 6f66 2074 6865  a summary of the
-00028810: 2063 6f6c 756d 6e73 2c20 652e 672e 2c20   columns, e.g., 
-00028820: 6120 7375 6d20 6f66 2074 6865 2067 6976  a sum of the giv
-00028830: 656e 206e 756d 6265 7273 2069 6e20 6120  en numbers in a 
-00028840: 636f 6c75 6d6e 2e0a 0a20 2020 2020 2020  column...       
-00028850: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-00028860: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-00028870: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-00028880: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-00028890: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-000288a0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f74  b/HTML/Element/t
-000288b0: 666f 6f74 290a 2020 2020 2020 2020 2222  foot).        ""
-000288c0: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-000288d0: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-000288e0: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
-000288f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00028900: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
-00028910: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
-00028920: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
-00028930: 6566 205f 6765 745f 6465 6661 756c 745f  ef _get_default_
-00028940: 6174 7472 6962 7574 6573 2873 656c 662c  attributes(self,
-00028950: 2067 6976 656e 3a20 6469 6374 5b73 7472   given: dict[str
-00028960: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-00028970: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
-00028980: 7474 7269 6275 7465 5479 7065 5d3a 0a20  ttributeType]:. 
-00028990: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
-000289a0: 0a0a 0a63 6c61 7373 2074 6828 5461 6729  ...class th(Tag)
-000289b0: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-000289c0: 6368 696c 6420 6f66 2074 6865 205b 603c  child of the [`<
-000289d0: 7472 3e60 5d28 6874 7470 733a 2f2f 6465  tr>`](https://de
-000289e0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-000289f0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-00028a00: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-00028a10: 7472 2920 656c 656d 656e 742c 2069 7420  tr) element, it 
-00028a20: 6465 6669 6e65 7320 6120 6365 6c6c 2061  defines a cell a
-00028a30: 7320 7468 6520 6865 6164 6572 206f 6620  s the header of 
-00028a40: 6120 6772 6f75 7020 6f66 2074 6162 6c65  a group of table
-00028a50: 2063 656c 6c73 2e20 5468 6520 6e61 7475   cells. The natu
-00028a60: 7265 206f 6620 7468 6973 2067 726f 7570  re of this group
-00028a70: 2063 616e 2062 6520 6578 706c 6963 6974   can be explicit
-00028a80: 6c79 2064 6566 696e 6564 2062 7920 7468  ly defined by th
-00028a90: 6520 5b60 7363 6f70 6560 5d28 6874 7470  e [`scope`](http
-00028aa0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-00028ab0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-00028ac0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-00028ad0: 656d 656e 742f 7468 2373 636f 7065 2920  ement/th#scope) 
-00028ae0: 616e 6420 5b60 6865 6164 6572 7360 5d28  and [`headers`](
-00028af0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00028b00: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00028b10: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00028b20: 4c2f 456c 656d 656e 742f 7468 2368 6561  L/Element/th#hea
-00028b30: 6465 7273 2920 6174 7472 6962 7574 6573  ders) attributes
-00028b40: 2e0a 0a20 2020 202a 2060 7363 6f70 6560  ...    * `scope`
-00028b50: 3a20 5468 6520 6172 6561 206f 6620 7468  : The area of th
-00028b60: 6520 7461 626c 6520 7468 6174 2074 6869  e table that thi
-00028b70: 7320 6865 6164 696e 6720 6170 706c 6965  s heading applie
-00028b80: 7320 746f 2e20 416c 6c6f 7765 6420 7661  s to. Allowed va
-00028b90: 6c75 6573 3a20 6022 636f 6c22 602c 2060  lues: `"col"`, `
-00028ba0: 2272 6f77 2260 2c20 6022 636f 6c67 726f  "row"`, `"colgro
-00028bb0: 7570 2260 2c20 6022 726f 7767 726f 7570  up"`, `"rowgroup
-00028bc0: 2260 0a20 2020 202a 2060 636f 6c73 7061  "`.    * `colspa
-00028bd0: 6e60 3a20 5468 6520 6e75 6d62 6572 206f  n`: The number o
-00028be0: 6620 636f 6c75 6d6e 7320 696e 2074 6865  f columns in the
-00028bf0: 2074 6162 6c65 2074 6861 7420 7468 6973   table that this
-00028c00: 2068 6561 6469 6e67 2073 7061 6e73 2e0a   heading spans..
-00028c10: 2020 2020 2a20 6072 6f77 7370 616e 603a      * `rowspan`:
-00028c20: 2054 6865 206e 756d 6265 7220 6f66 2072   The number of r
-00028c30: 6f77 7320 696e 2074 6865 2074 6162 6c65  ows in the table
-00028c40: 2074 6861 7420 7468 6973 2068 6561 6469   that this headi
-00028c50: 6e67 2073 7061 6e73 2e0a 0a20 2020 205b  ng spans...    [
-00028c60: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-00028c70: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00028c80: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-00028c90: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-00028ca0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-00028cb0: 6e74 2f74 6829 0a20 2020 2022 2222 0a20  nt/th).    """. 
-00028cc0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00028cd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00028ce0: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-00028cf0: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-00028d00: 2020 2020 2020 2020 7363 6f70 653a 2041          scope: A
-00028d10: 7474 7269 6275 7465 5479 7065 203d 204e  ttributeType = N
-00028d20: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
-00028d30: 7370 616e 3a20 4174 7472 6962 7574 6554  span: AttributeT
-00028d40: 7970 6520 3d20 4e6f 6e65 2c0a 2020 2020  ype = None,.    
-00028d50: 2020 2020 726f 7773 7061 6e3a 2041 7474      rowspan: Att
-00028d60: 7269 6275 7465 5479 7065 203d 204e 6f6e  ributeType = Non
-00028d70: 652c 0a20 2020 2020 2020 2069 643a 204f  e,.        id: O
-00028d80: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00028d90: 6f6e 652c 0a20 2020 2020 2020 205f 636c  one,.        _cl
-00028da0: 6173 733a 204f 7074 696f 6e61 6c5b 7374  ass: Optional[st
-00028db0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00028dc0: 2020 2073 7479 6c65 3a20 4f70 7469 6f6e     style: Option
-00028dd0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00028de0: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
-00028df0: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
-00028e00: 7970 652c 0a20 2020 2029 202d 3e20 4e6f  ype,.    ) -> No
-00028e10: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00028e20: 2020 2020 2020 2020 4120 6368 696c 6420          A child 
-00028e30: 6f66 2074 6865 205b 603c 7472 3e60 5d28  of the [`<tr>`](
-00028e40: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00028e50: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00028e60: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00028e70: 4c2f 456c 656d 656e 742f 7472 2920 656c  L/Element/tr) el
-00028e80: 656d 656e 742c 2069 7420 6465 6669 6e65  ement, it define
-00028e90: 7320 6120 6365 6c6c 2061 7320 7468 6520  s a cell as the 
-00028ea0: 6865 6164 6572 206f 6620 6120 6772 6f75  header of a grou
-00028eb0: 7020 6f66 2074 6162 6c65 2063 656c 6c73  p of table cells
-00028ec0: 2e20 5468 6520 6e61 7475 7265 206f 6620  . The nature of 
-00028ed0: 7468 6973 2067 726f 7570 2063 616e 2062  this group can b
-00028ee0: 6520 6578 706c 6963 6974 6c79 2064 6566  e explicitly def
-00028ef0: 696e 6564 2062 7920 7468 6520 5b60 7363  ined by the [`sc
-00028f00: 6f70 6560 5d28 6874 7470 733a 2f2f 6465  ope`](https://de
-00028f10: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-00028f20: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-00028f30: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-00028f40: 7468 2373 636f 7065 2920 616e 6420 5b60  th#scope) and [`
-00028f50: 6865 6164 6572 7360 5d28 6874 7470 733a  headers`](https:
-00028f60: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00028f70: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-00028f80: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-00028f90: 656e 742f 7468 2368 6561 6465 7273 2920  ent/th#headers) 
-00028fa0: 6174 7472 6962 7574 6573 2e0a 0a20 2020  attributes...   
-00028fb0: 2020 2020 202a 2060 7363 6f70 6560 3a20       * `scope`: 
-00028fc0: 5468 6520 6172 6561 206f 6620 7468 6520  The area of the 
-00028fd0: 7461 626c 6520 7468 6174 2074 6869 7320  table that this 
-00028fe0: 6865 6164 696e 6720 6170 706c 6965 7320  heading applies 
-00028ff0: 746f 2e20 416c 6c6f 7765 6420 7661 6c75  to. Allowed valu
-00029000: 6573 3a20 6022 636f 6c22 602c 2060 2272  es: `"col"`, `"r
-00029010: 6f77 2260 2c20 6022 636f 6c67 726f 7570  ow"`, `"colgroup
-00029020: 2260 2c20 6022 726f 7767 726f 7570 2260  "`, `"rowgroup"`
-00029030: 0a20 2020 2020 2020 202a 2060 636f 6c73  .        * `cols
-00029040: 7061 6e60 3a20 5468 6520 6e75 6d62 6572  pan`: The number
-00029050: 206f 6620 636f 6c75 6d6e 7320 696e 2074   of columns in t
-00029060: 6865 2074 6162 6c65 2074 6861 7420 7468  he table that th
-00029070: 6973 2068 6561 6469 6e67 2073 7061 6e73  is heading spans
-00029080: 2e0a 2020 2020 2020 2020 2a20 6072 6f77  ..        * `row
-00029090: 7370 616e 603a 2054 6865 206e 756d 6265  span`: The numbe
-000290a0: 7220 6f66 2072 6f77 7320 696e 2074 6865  r of rows in the
-000290b0: 2074 6162 6c65 2074 6861 7420 7468 6973   table that this
-000290c0: 2068 6561 6469 6e67 2073 7061 6e73 2e0a   heading spans..
-000290d0: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
-000290e0: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
-000290f0: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
-00029100: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-00029110: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-00029120: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 6829  HTML/Element/th)
-00029130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00029140: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
-00029150: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
-00029160: 2027 5f63 6c61 7373 273a 205f 636c 6173   '_class': _clas
-00029170: 732c 0a20 2020 2020 2020 2020 2020 2027  s,.            '
-00029180: 6964 273a 2069 642c 0a20 2020 2020 2020  id': id,.       
-00029190: 2020 2020 2027 7374 796c 6527 3a20 7374       'style': st
-000291a0: 796c 652c 0a20 2020 2020 2020 2020 2020  yle,.           
-000291b0: 2027 7363 6f70 6527 3a20 7363 6f70 652c   'scope': scope,
-000291c0: 0a20 2020 2020 2020 2020 2020 2027 636f  .            'co
-000291d0: 6c73 7061 6e27 3a20 636f 6c73 7061 6e2c  lspan': colspan,
-000291e0: 0a20 2020 2020 2020 2020 2020 2027 726f  .            'ro
-000291f0: 7773 7061 6e27 3a20 726f 7773 7061 6e2c  wspan': rowspan,
-00029200: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00029210: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00029220: 745f 5f28 2a63 6869 6c64 7265 6e2c 202a  t__(*children, *
-00029230: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-00029240: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2820    def __call__( 
-00029250: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
-00029260: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00029270: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
-00029280: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
-00029290: 2020 2020 2020 2073 636f 7065 3a20 4174         scope: At
-000292a0: 7472 6962 7574 6554 7970 6520 3d20 4e6f  tributeType = No
-000292b0: 6e65 2c0a 2020 2020 2020 2020 636f 6c73  ne,.        cols
-000292c0: 7061 6e3a 2041 7474 7269 6275 7465 5479  pan: AttributeTy
-000292d0: 7065 203d 204e 6f6e 652c 0a20 2020 2020  pe = None,.     
-000292e0: 2020 2072 6f77 7370 616e 3a20 4174 7472     rowspan: Attr
-000292f0: 6962 7574 6554 7970 6520 3d20 4e6f 6e65  ibuteType = None
-00029300: 2c0a 2020 2020 2020 2020 6964 3a20 4f70  ,.        id: Op
-00029310: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00029320: 6e65 2c0a 2020 2020 2020 2020 5f63 6c61  ne,.        _cla
-00029330: 7373 3a20 4f70 7469 6f6e 616c 5b73 7472  ss: Optional[str
-00029340: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00029350: 2020 7374 796c 653a 204f 7074 696f 6e61    style: Optiona
-00029360: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00029370: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
-00029380: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
-00029390: 7065 2c0a 2020 2020 293a 0a20 2020 2020  pe,.    ):.     
-000293a0: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
-000293b0: 2063 6869 6c64 206f 6620 7468 6520 5b60   child of the [`
-000293c0: 3c74 723e 605d 2868 7474 7073 3a2f 2f64  <tr>`](https://d
-000293d0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-000293e0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-000293f0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00029400: 2f74 7229 2065 6c65 6d65 6e74 2c20 6974  /tr) element, it
-00029410: 2064 6566 696e 6573 2061 2063 656c 6c20   defines a cell 
-00029420: 6173 2074 6865 2068 6561 6465 7220 6f66  as the header of
-00029430: 2061 2067 726f 7570 206f 6620 7461 626c   a group of tabl
-00029440: 6520 6365 6c6c 732e 2054 6865 206e 6174  e cells. The nat
-00029450: 7572 6520 6f66 2074 6869 7320 6772 6f75  ure of this grou
-00029460: 7020 6361 6e20 6265 2065 7870 6c69 6369  p can be explici
-00029470: 746c 7920 6465 6669 6e65 6420 6279 2074  tly defined by t
-00029480: 6865 205b 6073 636f 7065 605d 2868 7474  he [`scope`](htt
-00029490: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-000294a0: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-000294b0: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-000294c0: 6c65 6d65 6e74 2f74 6823 7363 6f70 6529  lement/th#scope)
-000294d0: 2061 6e64 205b 6068 6561 6465 7273 605d   and [`headers`]
-000294e0: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-000294f0: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-00029500: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-00029510: 4d4c 2f45 6c65 6d65 6e74 2f74 6823 6865  ML/Element/th#he
-00029520: 6164 6572 7329 2061 7474 7269 6275 7465  aders) attribute
-00029530: 732e 0a0a 2020 2020 2020 2020 2a20 6073  s...        * `s
-00029540: 636f 7065 603a 2054 6865 2061 7265 6120  cope`: The area 
-00029550: 6f66 2074 6865 2074 6162 6c65 2074 6861  of the table tha
-00029560: 7420 7468 6973 2068 6561 6469 6e67 2061  t this heading a
-00029570: 7070 6c69 6573 2074 6f2e 2041 6c6c 6f77  pplies to. Allow
-00029580: 6564 2076 616c 7565 733a 2060 2263 6f6c  ed values: `"col
-00029590: 2260 2c20 6022 726f 7722 602c 2060 2263  "`, `"row"`, `"c
-000295a0: 6f6c 6772 6f75 7022 602c 2060 2272 6f77  olgroup"`, `"row
-000295b0: 6772 6f75 7022 600a 2020 2020 2020 2020  group"`.        
-000295c0: 2a20 6063 6f6c 7370 616e 603a 2054 6865  * `colspan`: The
-000295d0: 206e 756d 6265 7220 6f66 2063 6f6c 756d   number of colum
-000295e0: 6e73 2069 6e20 7468 6520 7461 626c 6520  ns in the table 
-000295f0: 7468 6174 2074 6869 7320 6865 6164 696e  that this headin
-00029600: 6720 7370 616e 732e 0a20 2020 2020 2020  g spans..       
-00029610: 202a 2060 726f 7773 7061 6e60 3a20 5468   * `rowspan`: Th
-00029620: 6520 6e75 6d62 6572 206f 6620 726f 7773  e number of rows
-00029630: 2069 6e20 7468 6520 7461 626c 6520 7468   in the table th
-00029640: 6174 2074 6869 7320 6865 6164 696e 6720  at this heading 
-00029650: 7370 616e 732e 0a0a 2020 2020 2020 2020  spans...        
-00029660: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
-00029670: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00029680: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00029690: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-000296a0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-000296b0: 656e 742f 7468 290a 2020 2020 2020 2020  ent/th).        
-000296c0: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
-000296d0: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
-000296e0: 2020 2020 2020 2020 275f 636c 6173 7327          '_class'
-000296f0: 3a20 5f63 6c61 7373 2c0a 2020 2020 2020  : _class,.      
-00029700: 2020 2020 2020 2769 6427 3a20 6964 2c0a        'id': id,.
-00029710: 2020 2020 2020 2020 2020 2020 2773 7479              'sty
-00029720: 6c65 273a 2073 7479 6c65 2c0a 2020 2020  le': style,.    
-00029730: 2020 2020 2020 2020 2773 636f 7065 273a          'scope':
-00029740: 2073 636f 7065 2c0a 2020 2020 2020 2020   scope,.        
-00029750: 2020 2020 2763 6f6c 7370 616e 273a 2063      'colspan': c
-00029760: 6f6c 7370 616e 2c0a 2020 2020 2020 2020  olspan,.        
-00029770: 2020 2020 2772 6f77 7370 616e 273a 2072      'rowspan': r
-00029780: 6f77 7370 616e 2c0a 2020 2020 2020 2020  owspan,.        
-00029790: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
-000297a0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
-000297b0: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
-000297c0: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
-000297d0: 6465 6620 5f67 6574 5f64 6566 6175 6c74  def _get_default
-000297e0: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
-000297f0: 2c20 6769 7665 6e3a 2064 6963 745b 7374  , given: dict[st
-00029800: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
-00029810: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
-00029820: 4174 7472 6962 7574 6554 7970 655d 3a0a  AttributeType]:.
-00029830: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00029840: 2773 636f 7065 273a 204e 6f6e 652c 2027  'scope': None, '
-00029850: 636f 6c73 7061 6e27 3a20 4e6f 6e65 2c20  colspan': None, 
-00029860: 2772 6f77 7370 616e 273a 204e 6f6e 657d  'rowspan': None}
-00029870: 0a0a 0a63 6c61 7373 2074 6865 6164 2854  ...class thead(T
-00029880: 6167 293a 0a20 2020 2022 2222 0a20 2020  ag):.    """.   
-00029890: 2045 6e63 6170 7375 6c61 7465 7320 6120   Encapsulates a 
-000298a0: 7365 7420 6f66 2074 6162 6c65 2072 6f77  set of table row
-000298b0: 7320 285b 603c 7472 3e60 5d28 6874 7470  s ([`<tr>`](http
-000298c0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-000298d0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-000298e0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-000298f0: 656d 656e 742f 7472 2920 656c 656d 656e  ement/tr) elemen
-00029900: 7473 292c 2069 6e64 6963 6174 696e 6720  ts), indicating 
-00029910: 7468 6174 2074 6865 7920 636f 6d70 7269  that they compri
-00029920: 7365 2074 6865 2068 6561 6420 6f66 2061  se the head of a
-00029930: 2074 6162 6c65 2077 6974 6820 696e 666f   table with info
-00029940: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
-00029950: 6520 7461 626c 6527 7320 636f 6c75 6d6e  e table's column
-00029960: 732e 2054 6869 7320 6973 2075 7375 616c  s. This is usual
-00029970: 6c79 2069 6e20 7468 6520 666f 726d 206f  ly in the form o
-00029980: 6620 636f 6c75 6d6e 2068 6561 6465 7273  f column headers
-00029990: 2028 5b60 3c74 683e 605d 2868 7474 7073   ([`<th>`](https
-000299a0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-000299b0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-000299c0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-000299d0: 6d65 6e74 2f74 6829 2065 6c65 6d65 6e74  ment/th) element
-000299e0: 7329 2e0a 0a20 2020 200a 0a20 2020 205b  s)...    ..    [
-000299f0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-00029a00: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00029a10: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-00029a20: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-00029a30: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-00029a40: 6e74 2f74 6865 6164 290a 2020 2020 2222  nt/thead).    ""
-00029a50: 220a 2020 2020 6465 6620 5f5f 696e 6974  ".    def __init
-00029a60: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00029a70: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
-00029a80: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
-00029a90: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
-00029aa0: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
-00029ab0: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
-00029ac0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-00029ad0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00029ae0: 2020 2020 456e 6361 7073 756c 6174 6573      Encapsulates
-00029af0: 2061 2073 6574 206f 6620 7461 626c 6520   a set of table 
-00029b00: 726f 7773 2028 5b60 3c74 723e 605d 2868  rows ([`<tr>`](h
-00029b10: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00029b20: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-00029b30: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-00029b40: 2f45 6c65 6d65 6e74 2f74 7229 2065 6c65  /Element/tr) ele
-00029b50: 6d65 6e74 7329 2c20 696e 6469 6361 7469  ments), indicati
-00029b60: 6e67 2074 6861 7420 7468 6579 2063 6f6d  ng that they com
-00029b70: 7072 6973 6520 7468 6520 6865 6164 206f  prise the head o
-00029b80: 6620 6120 7461 626c 6520 7769 7468 2069  f a table with i
-00029b90: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00029ba0: 2074 6865 2074 6162 6c65 2773 2063 6f6c   the table's col
-00029bb0: 756d 6e73 2e20 5468 6973 2069 7320 7573  umns. This is us
-00029bc0: 7561 6c6c 7920 696e 2074 6865 2066 6f72  ually in the for
-00029bd0: 6d20 6f66 2063 6f6c 756d 6e20 6865 6164  m of column head
-00029be0: 6572 7320 285b 603c 7468 3e60 5d28 6874  ers ([`<th>`](ht
-00029bf0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-00029c00: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-00029c10: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-00029c20: 456c 656d 656e 742f 7468 2920 656c 656d  Element/th) elem
-00029c30: 656e 7473 292e 0a0a 2020 2020 2020 2020  ents)...        
-00029c40: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
-00029c50: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
-00029c60: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
-00029c70: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
-00029c80: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
-00029c90: 2f48 544d 4c2f 456c 656d 656e 742f 7468  /HTML/Element/th
-00029ca0: 6561 6429 0a20 2020 2020 2020 2022 2222  ead).        """
-00029cb0: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
-00029cc0: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
-00029cd0: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
-00029ce0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00029cf0: 5f5f 696e 6974 5f5f 282a 6368 696c 6472  __init__(*childr
-00029d00: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
-00029d10: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
-00029d20: 6c5f 5f28 2020 2320 7479 7065 3a20 6967  l__(  # type: ig
-00029d30: 6e6f 7265 0a20 2020 2020 2020 2073 656c  nore.        sel
-00029d40: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
-00029d50: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
-00029d60: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
-00029d70: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
-00029d80: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
-00029d90: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00029da0: 2022 2222 0a20 2020 2020 2020 2045 6e63   """.        Enc
-00029db0: 6170 7375 6c61 7465 7320 6120 7365 7420  apsulates a set 
-00029dc0: 6f66 2074 6162 6c65 2072 6f77 7320 285b  of table rows ([
-00029dd0: 603c 7472 3e60 5d28 6874 7470 733a 2f2f  `<tr>`](https://
-00029de0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-00029df0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-00029e00: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-00029e10: 742f 7472 2920 656c 656d 656e 7473 292c  t/tr) elements),
-00029e20: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
-00029e30: 2074 6865 7920 636f 6d70 7269 7365 2074   they comprise t
-00029e40: 6865 2068 6561 6420 6f66 2061 2074 6162  he head of a tab
-00029e50: 6c65 2077 6974 6820 696e 666f 726d 6174  le with informat
-00029e60: 696f 6e20 6162 6f75 7420 7468 6520 7461  ion about the ta
-00029e70: 626c 6527 7320 636f 6c75 6d6e 732e 2054  ble's columns. T
-00029e80: 6869 7320 6973 2075 7375 616c 6c79 2069  his is usually i
-00029e90: 6e20 7468 6520 666f 726d 206f 6620 636f  n the form of co
-00029ea0: 6c75 6d6e 2068 6561 6465 7273 2028 5b60  lumn headers ([`
-00029eb0: 3c74 683e 605d 2868 7474 7073 3a2f 2f64  <th>`](https://d
-00029ec0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-00029ed0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-00029ee0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00029ef0: 2f74 6829 2065 6c65 6d65 6e74 7329 2e0a  /th) elements)..
-00029f00: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
-00029f10: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
-00029f20: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00029f30: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-00029f40: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-00029f50: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-00029f60: 6c65 6d65 6e74 2f74 6865 6164 290a 2020  lement/thead).  
-00029f70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00029f80: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-00029f90: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-00029fa0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00029fb0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00029fc0: 5f5f 6361 6c6c 5f5f 282a 6368 696c 6472  __call__(*childr
-00029fd0: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
-00029fe0: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-00029ff0: 6465 6661 756c 745f 6174 7472 6962 7574  default_attribut
-0002a000: 6573 2873 656c 662c 2067 6976 656e 3a20  es(self, given: 
-0002a010: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
-0002a020: 7574 6554 7970 655d 2920 2d3e 2064 6963  uteType]) -> dic
-0002a030: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
-0002a040: 5479 7065 5d3a 0a20 2020 2020 2020 2072  Type]:.        r
-0002a050: 6574 7572 6e20 7b7d 0a0a 0a63 6c61 7373  eturn {}...class
-0002a060: 2074 7228 5461 6729 3a0a 2020 2020 2222   tr(Tag):.    ""
-0002a070: 220a 2020 2020 4465 6669 6e65 7320 6120  ".    Defines a 
-0002a080: 726f 7720 6f66 2063 656c 6c73 2069 6e20  row of cells in 
-0002a090: 6120 7461 626c 652e 2054 6865 2072 6f77  a table. The row
-0002a0a0: 2773 2063 656c 6c73 2063 616e 2074 6865  's cells can the
-0002a0b0: 6e20 6265 2065 7374 6162 6c69 7368 6564  n be established
-0002a0c0: 2075 7369 6e67 2061 206d 6978 206f 6620   using a mix of 
-0002a0d0: 5b60 3c74 643e 605d 2868 7474 7073 3a2f  [`<td>`](https:/
-0002a0e0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002a0f0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002a100: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002a110: 6e74 2f74 6429 2028 6461 7461 2063 656c  nt/td) (data cel
-0002a120: 6c29 2061 6e64 205b 603c 7468 3e60 5d28  l) and [`<th>`](
-0002a130: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-0002a140: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-0002a150: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-0002a160: 4c2f 456c 656d 656e 742f 7468 2920 2868  L/Element/th) (h
-0002a170: 6561 6465 7220 6365 6c6c 2920 656c 656d  eader cell) elem
-0002a180: 656e 7473 2e0a 0a20 2020 200a 0a20 2020  ents...    ..   
-0002a190: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-0002a1a0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-0002a1b0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002a1c0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002a1d0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002a1e0: 6d65 6e74 2f74 7229 0a20 2020 2022 2222  ment/tr).    """
-0002a1f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002a200: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0002a210: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-0002a220: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-0002a230: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-0002a240: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-0002a250: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-0002a260: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-0002a270: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002a280: 2020 2044 6566 696e 6573 2061 2072 6f77     Defines a row
-0002a290: 206f 6620 6365 6c6c 7320 696e 2061 2074   of cells in a t
-0002a2a0: 6162 6c65 2e20 5468 6520 726f 7727 7320  able. The row's 
-0002a2b0: 6365 6c6c 7320 6361 6e20 7468 656e 2062  cells can then b
-0002a2c0: 6520 6573 7461 626c 6973 6865 6420 7573  e established us
-0002a2d0: 696e 6720 6120 6d69 7820 6f66 205b 603c  ing a mix of [`<
-0002a2e0: 7464 3e60 5d28 6874 7470 733a 2f2f 6465  td>`](https://de
-0002a2f0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-0002a300: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-0002a310: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-0002a320: 7464 2920 2864 6174 6120 6365 6c6c 2920  td) (data cell) 
-0002a330: 616e 6420 5b60 3c74 683e 605d 2868 7474  and [`<th>`](htt
-0002a340: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-0002a350: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-0002a360: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-0002a370: 6c65 6d65 6e74 2f74 6829 2028 6865 6164  lement/th) (head
-0002a380: 6572 2063 656c 6c29 2065 6c65 6d65 6e74  er cell) element
-0002a390: 732e 0a0a 2020 2020 2020 2020 0a0a 2020  s...        ..  
-0002a3a0: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
-0002a3b0: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-0002a3c0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-0002a3d0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-0002a3e0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-0002a3f0: 4c2f 456c 656d 656e 742f 7472 290a 2020  L/Element/tr).  
-0002a400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0002a410: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-0002a420: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-0002a430: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0002a440: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-0002a450: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
-0002a460: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
-0002a470: 6465 6620 5f5f 6361 6c6c 5f5f 2820 2023  def __call__(  #
-0002a480: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-0002a490: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0002a4a0: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-0002a4b0: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-0002a4c0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-0002a4d0: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-0002a4e0: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-0002a4f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0002a500: 2020 2020 2020 4465 6669 6e65 7320 6120        Defines a 
-0002a510: 726f 7720 6f66 2063 656c 6c73 2069 6e20  row of cells in 
-0002a520: 6120 7461 626c 652e 2054 6865 2072 6f77  a table. The row
-0002a530: 2773 2063 656c 6c73 2063 616e 2074 6865  's cells can the
-0002a540: 6e20 6265 2065 7374 6162 6c69 7368 6564  n be established
-0002a550: 2075 7369 6e67 2061 206d 6978 206f 6620   using a mix of 
-0002a560: 5b60 3c74 643e 605d 2868 7474 7073 3a2f  [`<td>`](https:/
-0002a570: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002a580: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002a590: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002a5a0: 6e74 2f74 6429 2028 6461 7461 2063 656c  nt/td) (data cel
-0002a5b0: 6c29 2061 6e64 205b 603c 7468 3e60 5d28  l) and [`<th>`](
-0002a5c0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-0002a5d0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-0002a5e0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-0002a5f0: 4c2f 456c 656d 656e 742f 7468 2920 2868  L/Element/th) (h
-0002a600: 6561 6465 7220 6365 6c6c 2920 656c 656d  eader cell) elem
-0002a610: 656e 7473 2e0a 0a20 2020 2020 2020 200a  ents...        .
-0002a620: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
-0002a630: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
-0002a640: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
-0002a650: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-0002a660: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-0002a670: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 7229  HTML/Element/tr)
-0002a680: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002a690: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
-0002a6a0: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
-0002a6b0: 200a 2020 2020 2020 2020 7d0a 2020 2020   .        }.    
-0002a6c0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-0002a6d0: 2829 2e5f 5f63 616c 6c5f 5f28 2a63 6869  ().__call__(*chi
-0002a6e0: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
-0002a6f0: 7465 7329 0a0a 2020 2020 6465 6620 5f67  tes)..    def _g
-0002a700: 6574 5f64 6566 6175 6c74 5f61 7474 7269  et_default_attri
-0002a710: 6275 7465 7328 7365 6c66 2c20 6769 7665  butes(self, give
-0002a720: 6e3a 2064 6963 745b 7374 722c 2041 7474  n: dict[str, Att
-0002a730: 7269 6275 7465 5479 7065 5d29 202d 3e20  ributeType]) -> 
-0002a740: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
-0002a750: 7574 6554 7970 655d 3a0a 2020 2020 2020  uteType]:.      
-0002a760: 2020 7265 7475 726e 207b 7d0a 0a0a 636c    return {}...cl
-0002a770: 6173 7320 6275 7474 6f6e 2854 6167 293a  ass button(Tag):
-0002a780: 0a20 2020 2022 2222 0a20 2020 2041 6e20  .    """.    An 
-0002a790: 696e 7465 7261 6374 6976 6520 656c 656d  interactive elem
-0002a7a0: 656e 7420 6163 7469 7661 7465 6420 6279  ent activated by
-0002a7b0: 2061 2075 7365 7220 7769 7468 2061 206d   a user with a m
-0002a7c0: 6f75 7365 2c20 6b65 7962 6f61 7264 2c20  ouse, keyboard, 
-0002a7d0: 6669 6e67 6572 2c20 766f 6963 6520 636f  finger, voice co
-0002a7e0: 6d6d 616e 642c 206f 7220 6f74 6865 7220  mmand, or other 
-0002a7f0: 6173 7369 7374 6976 6520 7465 6368 6e6f  assistive techno
-0002a800: 6c6f 6779 2e20 4f6e 6365 2061 6374 6976  logy. Once activ
-0002a810: 6174 6564 2c20 6974 2070 6572 666f 726d  ated, it perform
-0002a820: 7320 616e 2061 6374 696f 6e2c 2073 7563  s an action, suc
-0002a830: 6820 6173 2073 7562 6d69 7474 696e 6720  h as submitting 
-0002a840: 6120 5b66 6f72 6d5d 282f 656e 2d55 532f  a [form](/en-US/
-0002a850: 646f 6373 2f4c 6561 726e 2f46 6f72 6d73  docs/Learn/Forms
-0002a860: 2920 6f72 206f 7065 6e69 6e67 2061 2064  ) or opening a d
-0002a870: 6961 6c6f 672e 0a0a 2020 2020 2a20 6066  ialog...    * `f
-0002a880: 6f72 6d6d 6574 686f 6460 3a20 5468 6520  ormmethod`: The 
-0002a890: 4854 5450 2072 6571 7565 7374 206d 6574  HTTP request met
-0002a8a0: 686f 6420 746f 2075 7365 206f 6e20 636c  hod to use on cl
-0002a8b0: 6963 6b2e 2047 656e 6572 616c 6c79 2c20  ick. Generally, 
-0002a8c0: 6974 2069 7320 7072 6566 6572 7265 6420  it is preferred 
-0002a8d0: 746f 2073 6574 2074 6865 2060 6d65 7468  to set the `meth
-0002a8e0: 6f64 6020 6174 7472 6962 7574 6520 6f6e  od` attribute on
-0002a8f0: 2074 6865 2060 3c66 6f72 6d3e 6020 656c   the `<form>` el
-0002a900: 656d 656e 7420 696e 7374 6561 6420 6f66  ement instead of
-0002a910: 2074 6869 732e 0a20 2020 202a 2060 666f   this..    * `fo
-0002a920: 726d 6163 7469 6f6e 603a 2054 6865 2055  rmaction`: The U
-0002a930: 524c 2074 6f20 7265 7175 6573 7420 746f  RL to request to
-0002a940: 206f 6e20 636c 6963 6b2e 2047 656e 6572   on click. Gener
-0002a950: 616c 6c79 2c20 6974 2069 7320 7072 6566  ally, it is pref
-0002a960: 6572 7265 6420 746f 2073 6574 2074 6865  erred to set the
-0002a970: 2060 6163 7469 6f6e 6020 6174 7472 6962   `action` attrib
-0002a980: 7574 6520 6f6e 2074 6865 2060 3c66 6f72  ute on the `<for
-0002a990: 6d3e 6020 656c 656d 656e 7420 696e 7374  m>` element inst
-0002a9a0: 6561 6420 6f66 2074 6869 732e 0a0a 2020  ead of this...  
-0002a9b0: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-0002a9c0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-0002a9d0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-0002a9e0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-0002a9f0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-0002aa00: 656d 656e 742f 6275 7474 6f6e 290a 2020  ement/button).  
-0002aa10: 2020 2222 220a 2020 2020 6465 6620 5f5f    """.    def __
-0002aa20: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0002aa30: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
-0002aa40: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
-0002aa50: 6e54 7970 652c 0a20 2020 2020 2020 2066  nType,.        f
-0002aa60: 6f72 6d6d 6574 686f 643a 2041 7474 7269  ormmethod: Attri
-0002aa70: 6275 7465 5479 7065 203d 204e 6f6e 652c  buteType = None,
-0002aa80: 0a20 2020 2020 2020 2066 6f72 6d61 6374  .        formact
-0002aa90: 696f 6e3a 2041 7474 7269 6275 7465 5479  ion: AttributeTy
-0002aaa0: 7065 203d 204e 6f6e 652c 0a20 2020 2020  pe = None,.     
-0002aab0: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
-0002aac0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0002aad0: 2020 2020 205f 636c 6173 733a 204f 7074       _class: Opt
-0002aae0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0002aaf0: 652c 0a20 2020 2020 2020 2073 7479 6c65  e,.        style
-0002ab00: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0002ab10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002ab20: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
-0002ab30: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
-0002ab40: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-0002ab50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002ab60: 416e 2069 6e74 6572 6163 7469 7665 2065  An interactive e
-0002ab70: 6c65 6d65 6e74 2061 6374 6976 6174 6564  lement activated
-0002ab80: 2062 7920 6120 7573 6572 2077 6974 6820   by a user with 
-0002ab90: 6120 6d6f 7573 652c 206b 6579 626f 6172  a mouse, keyboar
-0002aba0: 642c 2066 696e 6765 722c 2076 6f69 6365  d, finger, voice
-0002abb0: 2063 6f6d 6d61 6e64 2c20 6f72 206f 7468   command, or oth
-0002abc0: 6572 2061 7373 6973 7469 7665 2074 6563  er assistive tec
-0002abd0: 686e 6f6c 6f67 792e 204f 6e63 6520 6163  hnology. Once ac
-0002abe0: 7469 7661 7465 642c 2069 7420 7065 7266  tivated, it perf
-0002abf0: 6f72 6d73 2061 6e20 6163 7469 6f6e 2c20  orms an action, 
-0002ac00: 7375 6368 2061 7320 7375 626d 6974 7469  such as submitti
-0002ac10: 6e67 2061 205b 666f 726d 5d28 2f65 6e2d  ng a [form](/en-
-0002ac20: 5553 2f64 6f63 732f 4c65 6172 6e2f 466f  US/docs/Learn/Fo
-0002ac30: 726d 7329 206f 7220 6f70 656e 696e 6720  rms) or opening 
-0002ac40: 6120 6469 616c 6f67 2e0a 0a20 2020 2020  a dialog...     
-0002ac50: 2020 202a 2060 666f 726d 6d65 7468 6f64     * `formmethod
-0002ac60: 603a 2054 6865 2048 5454 5020 7265 7175  `: The HTTP requ
-0002ac70: 6573 7420 6d65 7468 6f64 2074 6f20 7573  est method to us
-0002ac80: 6520 6f6e 2063 6c69 636b 2e20 4765 6e65  e on click. Gene
-0002ac90: 7261 6c6c 792c 2069 7420 6973 2070 7265  rally, it is pre
-0002aca0: 6665 7272 6564 2074 6f20 7365 7420 7468  ferred to set th
-0002acb0: 6520 606d 6574 686f 6460 2061 7474 7269  e `method` attri
-0002acc0: 6275 7465 206f 6e20 7468 6520 603c 666f  bute on the `<fo
-0002acd0: 726d 3e60 2065 6c65 6d65 6e74 2069 6e73  rm>` element ins
-0002ace0: 7465 6164 206f 6620 7468 6973 2e0a 2020  tead of this..  
-0002acf0: 2020 2020 2020 2a20 6066 6f72 6d61 6374        * `formact
-0002ad00: 696f 6e60 3a20 5468 6520 5552 4c20 746f  ion`: The URL to
-0002ad10: 2072 6571 7565 7374 2074 6f20 6f6e 2063   request to on c
-0002ad20: 6c69 636b 2e20 4765 6e65 7261 6c6c 792c  lick. Generally,
-0002ad30: 2069 7420 6973 2070 7265 6665 7272 6564   it is preferred
-0002ad40: 2074 6f20 7365 7420 7468 6520 6061 6374   to set the `act
-0002ad50: 696f 6e60 2061 7474 7269 6275 7465 206f  ion` attribute o
-0002ad60: 6e20 7468 6520 603c 666f 726d 3e60 2065  n the `<form>` e
-0002ad70: 6c65 6d65 6e74 2069 6e73 7465 6164 206f  lement instead o
-0002ad80: 6620 7468 6973 2e0a 0a20 2020 2020 2020  f this...       
-0002ad90: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-0002ada0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-0002adb0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002adc0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002add0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002ade0: 6d65 6e74 2f62 7574 746f 6e29 0a20 2020  ment/button).   
-0002adf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002ae00: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002ae10: 0a20 2020 2020 2020 2020 2020 2027 5f63  .            '_c
-0002ae20: 6c61 7373 273a 205f 636c 6173 732c 0a20  lass': _class,. 
-0002ae30: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
-0002ae40: 2069 642c 0a20 2020 2020 2020 2020 2020   id,.           
-0002ae50: 2027 7374 796c 6527 3a20 7374 796c 652c   'style': style,
-0002ae60: 0a20 2020 2020 2020 2020 2020 2027 666f  .            'fo
-0002ae70: 726d 6d65 7468 6f64 273a 2066 6f72 6d6d  rmmethod': formm
-0002ae80: 6574 686f 642c 0a20 2020 2020 2020 2020  ethod,.         
-0002ae90: 2020 2027 666f 726d 6163 7469 6f6e 273a     'formaction':
-0002aea0: 2066 6f72 6d61 6374 696f 6e2c 0a20 2020   formaction,.   
-0002aeb0: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
-0002aec0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-0002aed0: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
-0002aee0: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
-0002aef0: 6620 5f5f 6361 6c6c 5f5f 2820 2023 2074  f __call__(  # t
-0002af00: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0002af10: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002af20: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
-0002af30: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
-0002af40: 2020 2066 6f72 6d6d 6574 686f 643a 2041     formmethod: A
-0002af50: 7474 7269 6275 7465 5479 7065 203d 204e  ttributeType = N
-0002af60: 6f6e 652c 0a20 2020 2020 2020 2066 6f72  one,.        for
-0002af70: 6d61 6374 696f 6e3a 2041 7474 7269 6275  maction: Attribu
-0002af80: 7465 5479 7065 203d 204e 6f6e 652c 0a20  teType = None,. 
-0002af90: 2020 2020 2020 2069 643a 204f 7074 696f         id: Optio
-0002afa0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0002afb0: 0a20 2020 2020 2020 205f 636c 6173 733a  .        _class:
-0002afc0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0002afd0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0002afe0: 7479 6c65 3a20 4f70 7469 6f6e 616c 5b73  tyle: Optional[s
-0002aff0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0002b000: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
-0002b010: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
-0002b020: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0002b030: 2222 220a 2020 2020 2020 2020 416e 2069  """.        An i
-0002b040: 6e74 6572 6163 7469 7665 2065 6c65 6d65  nteractive eleme
-0002b050: 6e74 2061 6374 6976 6174 6564 2062 7920  nt activated by 
-0002b060: 6120 7573 6572 2077 6974 6820 6120 6d6f  a user with a mo
-0002b070: 7573 652c 206b 6579 626f 6172 642c 2066  use, keyboard, f
-0002b080: 696e 6765 722c 2076 6f69 6365 2063 6f6d  inger, voice com
-0002b090: 6d61 6e64 2c20 6f72 206f 7468 6572 2061  mand, or other a
-0002b0a0: 7373 6973 7469 7665 2074 6563 686e 6f6c  ssistive technol
-0002b0b0: 6f67 792e 204f 6e63 6520 6163 7469 7661  ogy. Once activa
-0002b0c0: 7465 642c 2069 7420 7065 7266 6f72 6d73  ted, it performs
-0002b0d0: 2061 6e20 6163 7469 6f6e 2c20 7375 6368   an action, such
-0002b0e0: 2061 7320 7375 626d 6974 7469 6e67 2061   as submitting a
-0002b0f0: 205b 666f 726d 5d28 2f65 6e2d 5553 2f64   [form](/en-US/d
-0002b100: 6f63 732f 4c65 6172 6e2f 466f 726d 7329  ocs/Learn/Forms)
-0002b110: 206f 7220 6f70 656e 696e 6720 6120 6469   or opening a di
-0002b120: 616c 6f67 2e0a 0a20 2020 2020 2020 202a  alog...        *
-0002b130: 2060 666f 726d 6d65 7468 6f64 603a 2054   `formmethod`: T
-0002b140: 6865 2048 5454 5020 7265 7175 6573 7420  he HTTP request 
-0002b150: 6d65 7468 6f64 2074 6f20 7573 6520 6f6e  method to use on
-0002b160: 2063 6c69 636b 2e20 4765 6e65 7261 6c6c   click. Generall
-0002b170: 792c 2069 7420 6973 2070 7265 6665 7272  y, it is preferr
-0002b180: 6564 2074 6f20 7365 7420 7468 6520 606d  ed to set the `m
-0002b190: 6574 686f 6460 2061 7474 7269 6275 7465  ethod` attribute
-0002b1a0: 206f 6e20 7468 6520 603c 666f 726d 3e60   on the `<form>`
-0002b1b0: 2065 6c65 6d65 6e74 2069 6e73 7465 6164   element instead
-0002b1c0: 206f 6620 7468 6973 2e0a 2020 2020 2020   of this..      
-0002b1d0: 2020 2a20 6066 6f72 6d61 6374 696f 6e60    * `formaction`
-0002b1e0: 3a20 5468 6520 5552 4c20 746f 2072 6571  : The URL to req
-0002b1f0: 7565 7374 2074 6f20 6f6e 2063 6c69 636b  uest to on click
-0002b200: 2e20 4765 6e65 7261 6c6c 792c 2069 7420  . Generally, it 
-0002b210: 6973 2070 7265 6665 7272 6564 2074 6f20  is preferred to 
-0002b220: 7365 7420 7468 6520 6061 6374 696f 6e60  set the `action`
-0002b230: 2061 7474 7269 6275 7465 206f 6e20 7468   attribute on th
-0002b240: 6520 603c 666f 726d 3e60 2065 6c65 6d65  e `<form>` eleme
-0002b250: 6e74 2069 6e73 7465 6164 206f 6620 7468  nt instead of th
-0002b260: 6973 2e0a 0a20 2020 2020 2020 205b 5669  is...        [Vi
-0002b270: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-0002b280: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-0002b290: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002b2a0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002b2b0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002b2c0: 2f62 7574 746f 6e29 0a20 2020 2020 2020  /button).       
-0002b2d0: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-0002b2e0: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-0002b2f0: 2020 2020 2020 2020 2027 5f63 6c61 7373           '_class
-0002b300: 273a 205f 636c 6173 732c 0a20 2020 2020  ': _class,.     
-0002b310: 2020 2020 2020 2027 6964 273a 2069 642c         'id': id,
-0002b320: 0a20 2020 2020 2020 2020 2020 2027 7374  .            'st
-0002b330: 796c 6527 3a20 7374 796c 652c 0a20 2020  yle': style,.   
-0002b340: 2020 2020 2020 2020 2027 666f 726d 6d65           'formme
-0002b350: 7468 6f64 273a 2066 6f72 6d6d 6574 686f  thod': formmetho
-0002b360: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
-0002b370: 666f 726d 6163 7469 6f6e 273a 2066 6f72  formaction': for
-0002b380: 6d61 6374 696f 6e2c 0a20 2020 2020 2020  maction,.       
-0002b390: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
-0002b3a0: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
-0002b3b0: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
-0002b3c0: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
-0002b3d0: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
-0002b3e0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
-0002b3f0: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
-0002b400: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
-0002b410: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
-0002b420: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
-0002b430: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002b440: 7b27 666f 726d 6d65 7468 6f64 273a 204e  {'formmethod': N
-0002b450: 6f6e 652c 2027 666f 726d 6163 7469 6f6e  one, 'formaction
-0002b460: 273a 204e 6f6e 657d 0a0a 0a63 6c61 7373  ': None}...class
-0002b470: 2064 6174 616c 6973 7428 5461 6729 3a0a   datalist(Tag):.
-0002b480: 2020 2020 2222 220a 2020 2020 436f 6e74      """.    Cont
-0002b490: 6169 6e73 2061 2073 6574 206f 6620 5b60  ains a set of [`
-0002b4a0: 3c6f 7074 696f 6e3e 605d 2868 7474 7073  <option>`](https
-0002b4b0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002b4c0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002b4d0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002b4e0: 6d65 6e74 2f6f 7074 696f 6e29 2065 6c65  ment/option) ele
-0002b4f0: 6d65 6e74 7320 7468 6174 2072 6570 7265  ments that repre
-0002b500: 7365 6e74 2074 6865 2070 6572 6d69 7373  sent the permiss
-0002b510: 6962 6c65 206f 7220 7265 636f 6d6d 656e  ible or recommen
-0002b520: 6465 6420 6f70 7469 6f6e 7320 6176 6169  ded options avai
-0002b530: 6c61 626c 6520 746f 2063 686f 6f73 6520  lable to choose 
-0002b540: 6672 6f6d 2077 6974 6869 6e20 6f74 6865  from within othe
-0002b550: 7220 636f 6e74 726f 6c73 2e0a 0a20 2020  r controls...   
-0002b560: 200a 0a20 2020 205b 5669 6577 2066 756c   ..    [View ful
-0002b570: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-0002b580: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002b590: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002b5a0: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002b5b0: 4d4c 2f45 6c65 6d65 6e74 2f64 6174 616c  ML/Element/datal
-0002b5c0: 6973 7429 0a20 2020 2022 2222 0a20 2020  ist).    """.   
-0002b5d0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0002b5e0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002b5f0: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
-0002b600: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
-0002b610: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-0002b620: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
-0002b630: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
-0002b640: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0002b650: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0002b660: 6f6e 7461 696e 7320 6120 7365 7420 6f66  ontains a set of
-0002b670: 205b 603c 6f70 7469 6f6e 3e60 5d28 6874   [`<option>`](ht
-0002b680: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-0002b690: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-0002b6a0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-0002b6b0: 456c 656d 656e 742f 6f70 7469 6f6e 2920  Element/option) 
-0002b6c0: 656c 656d 656e 7473 2074 6861 7420 7265  elements that re
-0002b6d0: 7072 6573 656e 7420 7468 6520 7065 726d  present the perm
-0002b6e0: 6973 7369 626c 6520 6f72 2072 6563 6f6d  issible or recom
-0002b6f0: 6d65 6e64 6564 206f 7074 696f 6e73 2061  mended options a
-0002b700: 7661 696c 6162 6c65 2074 6f20 6368 6f6f  vailable to choo
-0002b710: 7365 2066 726f 6d20 7769 7468 696e 206f  se from within o
-0002b720: 7468 6572 2063 6f6e 7472 6f6c 732e 0a0a  ther controls...
-0002b730: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-0002b740: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-0002b750: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-0002b760: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-0002b770: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-0002b780: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-0002b790: 656d 656e 742f 6461 7461 6c69 7374 290a  ement/datalist).
-0002b7a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0002b7b0: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
-0002b7c0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0002b7d0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-0002b7e0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0002b7f0: 745f 5f28 2a63 6869 6c64 7265 6e2c 202a  t__(*children, *
-0002b800: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-0002b810: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2820    def __call__( 
-0002b820: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
-0002b830: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0002b840: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
-0002b850: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
-0002b860: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0002b870: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
-0002b880: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
-0002b890: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-0002b8a0: 2020 2020 2020 2020 436f 6e74 6169 6e73          Contains
-0002b8b0: 2061 2073 6574 206f 6620 5b60 3c6f 7074   a set of [`<opt
-0002b8c0: 696f 6e3e 605d 2868 7474 7073 3a2f 2f64  ion>`](https://d
-0002b8d0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002b8e0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002b8f0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002b900: 2f6f 7074 696f 6e29 2065 6c65 6d65 6e74  /option) element
-0002b910: 7320 7468 6174 2072 6570 7265 7365 6e74  s that represent
-0002b920: 2074 6865 2070 6572 6d69 7373 6962 6c65   the permissible
-0002b930: 206f 7220 7265 636f 6d6d 656e 6465 6420   or recommended 
-0002b940: 6f70 7469 6f6e 7320 6176 6169 6c61 626c  options availabl
-0002b950: 6520 746f 2063 686f 6f73 6520 6672 6f6d  e to choose from
-0002b960: 2077 6974 6869 6e20 6f74 6865 7220 636f   within other co
-0002b970: 6e74 726f 6c73 2e0a 0a20 2020 2020 2020  ntrols...       
-0002b980: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-0002b990: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-0002b9a0: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-0002b9b0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002b9c0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002b9d0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f64  b/HTML/Element/d
-0002b9e0: 6174 616c 6973 7429 0a20 2020 2020 2020  atalist).       
-0002b9f0: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-0002ba00: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-0002ba10: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0002ba20: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
-0002ba30: 726e 2073 7570 6572 2829 2e5f 5f63 616c  rn super().__cal
-0002ba40: 6c5f 5f28 2a63 6869 6c64 7265 6e2c 202a  l__(*children, *
-0002ba50: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-0002ba60: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
-0002ba70: 6c74 5f61 7474 7269 6275 7465 7328 7365  lt_attributes(se
-0002ba80: 6c66 2c20 6769 7665 6e3a 2064 6963 745b  lf, given: dict[
-0002ba90: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
-0002baa0: 7065 5d29 202d 3e20 6469 6374 5b73 7472  pe]) -> dict[str
-0002bab0: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-0002bac0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0002bad0: 207b 7d0a 0a0a 636c 6173 7320 6669 656c   {}...class fiel
-0002bae0: 6473 6574 2854 6167 293a 0a20 2020 2022  dset(Tag):.    "
-0002baf0: 2222 0a20 2020 2055 7365 6420 746f 2067  "".    Used to g
-0002bb00: 726f 7570 2073 6576 6572 616c 2063 6f6e  roup several con
-0002bb10: 7472 6f6c 7320 6173 2077 656c 6c20 6173  trols as well as
-0002bb20: 206c 6162 656c 7320 285b 603c 6c61 6265   labels ([`<labe
-0002bb30: 6c3e 605d 2868 7474 7073 3a2f 2f64 6576  l>`](https://dev
-0002bb40: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002bb50: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002bb60: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f6c  b/HTML/Element/l
-0002bb70: 6162 656c 2929 2077 6974 6869 6e20 6120  abel)) within a 
-0002bb80: 7765 6220 666f 726d 2e0a 0a20 2020 200a  web form...    .
-0002bb90: 0a20 2020 205b 5669 6577 2066 756c 6c20  .    [View full 
-0002bba0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-0002bbb0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-0002bbc0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-0002bbd0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-0002bbe0: 2f45 6c65 6d65 6e74 2f66 6965 6c64 7365  /Element/fieldse
-0002bbf0: 7429 0a20 2020 2022 2222 0a20 2020 2064  t).    """.    d
-0002bc00: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002bc10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002bc20: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-0002bc30: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-0002bc40: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-0002bc50: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-0002bc60: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
-0002bc70: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0002bc80: 2022 2222 0a20 2020 2020 2020 2055 7365   """.        Use
-0002bc90: 6420 746f 2067 726f 7570 2073 6576 6572  d to group sever
-0002bca0: 616c 2063 6f6e 7472 6f6c 7320 6173 2077  al controls as w
-0002bcb0: 656c 6c20 6173 206c 6162 656c 7320 285b  ell as labels ([
-0002bcc0: 603c 6c61 6265 6c3e 605d 2868 7474 7073  `<label>`](https
-0002bcd0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002bce0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002bcf0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002bd00: 6d65 6e74 2f6c 6162 656c 2929 2077 6974  ment/label)) wit
-0002bd10: 6869 6e20 6120 7765 6220 666f 726d 2e0a  hin a web form..
-0002bd20: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
-0002bd30: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
-0002bd40: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-0002bd50: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-0002bd60: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-0002bd70: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-0002bd80: 6c65 6d65 6e74 2f66 6965 6c64 7365 7429  lement/fieldset)
-0002bd90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002bda0: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
-0002bdb0: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
-0002bdc0: 200a 2020 2020 2020 2020 7d0a 2020 2020   .        }.    
-0002bdd0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0002bde0: 6974 5f5f 282a 6368 696c 6472 656e 2c20  it__(*children, 
-0002bdf0: 2a2a 6174 7472 6962 7574 6573 290a 0a20  **attributes).. 
-0002be00: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-0002be10: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0002be20: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002be30: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-0002be40: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-0002be50: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002be60: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
-0002be70: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
-0002be80: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0002be90: 0a20 2020 2020 2020 2055 7365 6420 746f  .        Used to
-0002bea0: 2067 726f 7570 2073 6576 6572 616c 2063   group several c
-0002beb0: 6f6e 7472 6f6c 7320 6173 2077 656c 6c20  ontrols as well 
-0002bec0: 6173 206c 6162 656c 7320 285b 603c 6c61  as labels ([`<la
-0002bed0: 6265 6c3e 605d 2868 7474 7073 3a2f 2f64  bel>`](https://d
-0002bee0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002bef0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002bf00: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002bf10: 2f6c 6162 656c 2929 2077 6974 6869 6e20  /label)) within 
-0002bf20: 6120 7765 6220 666f 726d 2e0a 0a20 2020  a web form...   
-0002bf30: 2020 2020 200a 0a20 2020 2020 2020 205b       ..        [
-0002bf40: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-0002bf50: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-0002bf60: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002bf70: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002bf80: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002bf90: 6e74 2f66 6965 6c64 7365 7429 0a20 2020  nt/fieldset).   
-0002bfa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002bfb0: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002bfc0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-0002bfd0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0002bfe0: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
-0002bff0: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
-0002c000: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
-0002c010: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
-0002c020: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
-0002c030: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
-0002c040: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
-0002c050: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
-0002c060: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
-0002c070: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
-0002c080: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
-0002c090: 666f 726d 2854 6167 293a 0a20 2020 2022  form(Tag):.    "
-0002c0a0: 2222 0a20 2020 2052 6570 7265 7365 6e74  "".    Represent
-0002c0b0: 7320 6120 646f 6375 6d65 6e74 2073 6563  s a document sec
-0002c0c0: 7469 6f6e 2063 6f6e 7461 696e 696e 6720  tion containing 
-0002c0d0: 696e 7465 7261 6374 6976 6520 636f 6e74  interactive cont
-0002c0e0: 726f 6c73 2066 6f72 2073 7562 6d69 7474  rols for submitt
-0002c0f0: 696e 6720 696e 666f 726d 6174 696f 6e2e  ing information.
-0002c100: 0a0a 2020 2020 2a20 606d 6574 686f 6460  ..    * `method`
-0002c110: 3a20 5468 6520 4854 5450 2072 6571 7565  : The HTTP reque
-0002c120: 7374 206d 6574 686f 6420 746f 2075 7365  st method to use
-0002c130: 2077 6865 6e20 7375 626d 6974 7469 6e67   when submitting
-0002c140: 2074 6869 7320 666f 726d 2e20 496e 2061   this form. In a
-0002c150: 6c6d 6f73 7420 616c 6c20 6361 7365 732c  lmost all cases,
-0002c160: 2079 6f75 276c 6c20 7761 6e74 2074 6869   you'll want thi
-0002c170: 7320 746f 2062 6520 504f 5354 2e20 2864  s to be POST. (d
-0002c180: 6566 6175 6c74 7320 746f 2060 2770 6f73  efaults to `'pos
-0002c190: 7427 6029 0a20 2020 202a 2060 6163 7469  t'`).    * `acti
-0002c1a0: 6f6e 603a 2054 6865 2055 524c 2074 6f20  on`: The URL to 
-0002c1b0: 7265 7175 6573 7420 746f 2077 6865 6e20  request to when 
-0002c1c0: 7375 626d 6974 7469 6e67 2074 6869 7320  submitting this 
-0002c1d0: 666f 726d 2e20 4279 2064 6566 6175 6c74  form. By default
-0002c1e0: 2c20 7265 7175 6573 7473 2077 696c 6c20  , requests will 
-0002c1f0: 6265 2073 656e 7420 746f 2074 6865 2073  be sent to the s
-0002c200: 616d 6520 5552 4c20 6173 2074 6865 2063  ame URL as the c
-0002c210: 7572 7265 6e74 2070 6167 652e 0a0a 2020  urrent page...  
-0002c220: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-0002c230: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-0002c240: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-0002c250: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-0002c260: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-0002c270: 656d 656e 742f 666f 726d 290a 2020 2020  ement/form).    
-0002c280: 2222 220a 2020 2020 6465 6620 5f5f 696e  """.    def __in
-0002c290: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0002c2a0: 6c66 2c0a 2020 2020 2020 2020 2a63 6869  lf,.        *chi
-0002c2b0: 6c64 7265 6e3a 2043 6869 6c64 7265 6e54  ldren: ChildrenT
-0002c2c0: 7970 652c 0a20 2020 2020 2020 206d 6574  ype,.        met
-0002c2d0: 686f 643a 204f 7074 696f 6e61 6c5b 4c69  hod: Optional[Li
-0002c2e0: 7465 7261 6c5b 2770 6f73 7427 2c20 2767  teral['post', 'g
-0002c2f0: 6574 275d 5d20 3d20 4e6f 6e65 2c0a 2020  et']] = None,.  
-0002c300: 2020 2020 2020 6163 7469 6f6e 3a20 4174        action: At
-0002c310: 7472 6962 7574 6554 7970 6520 3d20 4e6f  tributeType = No
-0002c320: 6e65 2c0a 2020 2020 2020 2020 2a2a 6174  ne,.        **at
-0002c330: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
-0002c340: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
-0002c350: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0002c360: 2222 220a 2020 2020 2020 2020 5265 7072  """.        Repr
-0002c370: 6573 656e 7473 2061 2064 6f63 756d 656e  esents a documen
-0002c380: 7420 7365 6374 696f 6e20 636f 6e74 6169  t section contai
-0002c390: 6e69 6e67 2069 6e74 6572 6163 7469 7665  ning interactive
-0002c3a0: 2063 6f6e 7472 6f6c 7320 666f 7220 7375   controls for su
-0002c3b0: 626d 6974 7469 6e67 2069 6e66 6f72 6d61  bmitting informa
-0002c3c0: 7469 6f6e 2e0a 0a20 2020 2020 2020 202a  tion...        *
-0002c3d0: 2060 6d65 7468 6f64 603a 2054 6865 2048   `method`: The H
-0002c3e0: 5454 5020 7265 7175 6573 7420 6d65 7468  TTP request meth
-0002c3f0: 6f64 2074 6f20 7573 6520 7768 656e 2073  od to use when s
-0002c400: 7562 6d69 7474 696e 6720 7468 6973 2066  ubmitting this f
-0002c410: 6f72 6d2e 2049 6e20 616c 6d6f 7374 2061  orm. In almost a
-0002c420: 6c6c 2063 6173 6573 2c20 796f 7527 6c6c  ll cases, you'll
-0002c430: 2077 616e 7420 7468 6973 2074 6f20 6265   want this to be
-0002c440: 2050 4f53 542e 2028 6465 6661 756c 7473   POST. (defaults
-0002c450: 2074 6f20 6027 706f 7374 2760 290a 2020   to `'post'`).  
-0002c460: 2020 2020 2020 2a20 6061 6374 696f 6e60        * `action`
-0002c470: 3a20 5468 6520 5552 4c20 746f 2072 6571  : The URL to req
-0002c480: 7565 7374 2074 6f20 7768 656e 2073 7562  uest to when sub
-0002c490: 6d69 7474 696e 6720 7468 6973 2066 6f72  mitting this for
-0002c4a0: 6d2e 2042 7920 6465 6661 756c 742c 2072  m. By default, r
-0002c4b0: 6571 7565 7374 7320 7769 6c6c 2062 6520  equests will be 
-0002c4c0: 7365 6e74 2074 6f20 7468 6520 7361 6d65  sent to the same
-0002c4d0: 2055 524c 2061 7320 7468 6520 6375 7272   URL as the curr
-0002c4e0: 656e 7420 7061 6765 2e0a 0a20 2020 2020  ent page...     
-0002c4f0: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
-0002c500: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-0002c510: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-0002c520: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-0002c530: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-0002c540: 6c65 6d65 6e74 2f66 6f72 6d29 0a20 2020  lement/form).   
-0002c550: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002c560: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002c570: 0a20 2020 2020 2020 2020 2020 2027 6d65  .            'me
-0002c580: 7468 6f64 273a 206d 6574 686f 642c 0a20  thod': method,. 
-0002c590: 2020 2020 2020 2020 2020 2027 6163 7469             'acti
-0002c5a0: 6f6e 273a 2061 6374 696f 6e2c 0a20 2020  on': action,.   
-0002c5b0: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
-0002c5c0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-0002c5d0: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
-0002c5e0: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
-0002c5f0: 6620 5f5f 6361 6c6c 5f5f 2820 2023 2074  f __call__(  # t
-0002c600: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0002c610: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002c620: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
-0002c630: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
-0002c640: 2020 206d 6574 686f 643a 204f 7074 696f     method: Optio
-0002c650: 6e61 6c5b 4c69 7465 7261 6c5b 2770 6f73  nal[Literal['pos
-0002c660: 7427 2c20 2767 6574 275d 5d20 3d20 4e6f  t', 'get']] = No
-0002c670: 6e65 2c0a 2020 2020 2020 2020 6163 7469  ne,.        acti
-0002c680: 6f6e 3a20 4174 7472 6962 7574 6554 7970  on: AttributeTyp
-0002c690: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0002c6a0: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
-0002c6b0: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
-0002c6c0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0002c6d0: 220a 2020 2020 2020 2020 5265 7072 6573  ".        Repres
-0002c6e0: 656e 7473 2061 2064 6f63 756d 656e 7420  ents a document 
-0002c6f0: 7365 6374 696f 6e20 636f 6e74 6169 6e69  section containi
-0002c700: 6e67 2069 6e74 6572 6163 7469 7665 2063  ng interactive c
-0002c710: 6f6e 7472 6f6c 7320 666f 7220 7375 626d  ontrols for subm
-0002c720: 6974 7469 6e67 2069 6e66 6f72 6d61 7469  itting informati
-0002c730: 6f6e 2e0a 0a20 2020 2020 2020 202a 2060  on...        * `
-0002c740: 6d65 7468 6f64 603a 2054 6865 2048 5454  method`: The HTT
-0002c750: 5020 7265 7175 6573 7420 6d65 7468 6f64  P request method
-0002c760: 2074 6f20 7573 6520 7768 656e 2073 7562   to use when sub
-0002c770: 6d69 7474 696e 6720 7468 6973 2066 6f72  mitting this for
-0002c780: 6d2e 2049 6e20 616c 6d6f 7374 2061 6c6c  m. In almost all
-0002c790: 2063 6173 6573 2c20 796f 7527 6c6c 2077   cases, you'll w
-0002c7a0: 616e 7420 7468 6973 2074 6f20 6265 2050  ant this to be P
-0002c7b0: 4f53 542e 2028 6465 6661 756c 7473 2074  OST. (defaults t
-0002c7c0: 6f20 6027 706f 7374 2760 290a 2020 2020  o `'post'`).    
-0002c7d0: 2020 2020 2a20 6061 6374 696f 6e60 3a20      * `action`: 
-0002c7e0: 5468 6520 5552 4c20 746f 2072 6571 7565  The URL to reque
-0002c7f0: 7374 2074 6f20 7768 656e 2073 7562 6d69  st to when submi
-0002c800: 7474 696e 6720 7468 6973 2066 6f72 6d2e  tting this form.
-0002c810: 2042 7920 6465 6661 756c 742c 2072 6571   By default, req
-0002c820: 7565 7374 7320 7769 6c6c 2062 6520 7365  uests will be se
-0002c830: 6e74 2074 6f20 7468 6520 7361 6d65 2055  nt to the same U
-0002c840: 524c 2061 7320 7468 6520 6375 7272 656e  RL as the curren
-0002c850: 7420 7061 6765 2e0a 0a20 2020 2020 2020  t page...       
-0002c860: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-0002c870: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-0002c880: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002c890: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002c8a0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002c8b0: 6d65 6e74 2f66 6f72 6d29 0a20 2020 2020  ment/form).     
-0002c8c0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-0002c8d0: 7474 7269 6275 7465 7320 7c3d 207b 0a20  ttributes |= {. 
-0002c8e0: 2020 2020 2020 2020 2020 2027 6d65 7468             'meth
-0002c8f0: 6f64 273a 206d 6574 686f 642c 0a20 2020  od': method,.   
-0002c900: 2020 2020 2020 2020 2027 6163 7469 6f6e           'action
-0002c910: 273a 2061 6374 696f 6e2c 0a20 2020 2020  ': action,.     
-0002c920: 2020 207d 0a20 2020 2020 2020 2072 6574     }.        ret
-0002c930: 7572 6e20 7375 7065 7228 292e 5f5f 6361  urn super().__ca
-0002c940: 6c6c 5f5f 282a 6368 696c 6472 656e 2c20  ll__(*children, 
-0002c950: 2a2a 6174 7472 6962 7574 6573 290a 0a20  **attributes).. 
-0002c960: 2020 2064 6566 205f 6765 745f 6465 6661     def _get_defa
-0002c970: 756c 745f 6174 7472 6962 7574 6573 2873  ult_attributes(s
-0002c980: 656c 662c 2067 6976 656e 3a20 6469 6374  elf, given: dict
-0002c990: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
-0002c9a0: 7970 655d 2920 2d3e 2064 6963 745b 7374  ype]) -> dict[st
-0002c9b0: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
-0002c9c0: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-0002c9d0: 6e20 7b27 6d65 7468 6f64 273a 2027 706f  n {'method': 'po
-0002c9e0: 7374 272c 2027 6163 7469 6f6e 273a 204e  st', 'action': N
-0002c9f0: 6f6e 657d 0a0a 0a63 6c61 7373 206c 6162  one}...class lab
-0002ca00: 656c 2854 6167 293a 0a20 2020 2022 2222  el(Tag):.    """
-0002ca10: 0a20 2020 2052 6570 7265 7365 6e74 7320  .    Represents 
-0002ca20: 6120 6361 7074 696f 6e20 666f 7220 616e  a caption for an
-0002ca30: 2069 7465 6d20 696e 2061 2075 7365 7220   item in a user 
-0002ca40: 696e 7465 7266 6163 652e 0a0a 2020 2020  interface...    
-0002ca50: 2a20 6066 6f72 5f60 3a20 4944 206f 6620  * `for_`: ID of 
-0002ca60: 696e 7075 7420 6669 656c 6420 746f 2061  input field to a
-0002ca70: 7373 6f63 6961 7465 2074 6869 7320 6c61  ssociate this la
-0002ca80: 6265 6c20 7769 7468 0a0a 2020 2020 5b56  bel with..    [V
-0002ca90: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
-0002caa0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-0002cab0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-0002cac0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-0002cad0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-0002cae0: 742f 6c61 6265 6c29 0a20 2020 2022 2222  t/label).    """
-0002caf0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002cb00: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0002cb10: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-0002cb20: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-0002cb30: 2c0a 2020 2020 2020 2020 666f 725f 3a20  ,.        for_: 
-0002cb40: 4174 7472 6962 7574 6554 7970 6520 3d20  AttributeType = 
-0002cb50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2a  None,.        **
-0002cb60: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-0002cb70: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-0002cb80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0002cb90: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0002cba0: 7072 6573 656e 7473 2061 2063 6170 7469  presents a capti
-0002cbb0: 6f6e 2066 6f72 2061 6e20 6974 656d 2069  on for an item i
-0002cbc0: 6e20 6120 7573 6572 2069 6e74 6572 6661  n a user interfa
-0002cbd0: 6365 2e0a 0a20 2020 2020 2020 202a 2060  ce...        * `
-0002cbe0: 666f 725f 603a 2049 4420 6f66 2069 6e70  for_`: ID of inp
-0002cbf0: 7574 2066 6965 6c64 2074 6f20 6173 736f  ut field to asso
-0002cc00: 6369 6174 6520 7468 6973 206c 6162 656c  ciate this label
-0002cc10: 2077 6974 680a 0a20 2020 2020 2020 205b   with..        [
-0002cc20: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-0002cc30: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-0002cc40: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002cc50: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002cc60: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002cc70: 6e74 2f6c 6162 656c 290a 2020 2020 2020  nt/label).      
-0002cc80: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
-0002cc90: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
-0002cca0: 2020 2020 2020 2020 2020 2766 6f72 5f27            'for_'
-0002ccb0: 3a20 666f 725f 2c0a 2020 2020 2020 2020  : for_,.        
-0002ccc0: 7d0a 2020 2020 2020 2020 7375 7065 7228  }.        super(
-0002ccd0: 292e 5f5f 696e 6974 5f5f 282a 6368 696c  ).__init__(*chil
-0002cce0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
-0002ccf0: 6573 290a 0a20 2020 2064 6566 205f 5f63  es)..    def __c
-0002cd00: 616c 6c5f 5f28 2020 2320 7479 7065 3a20  all__(  # type: 
-0002cd10: 6967 6e6f 7265 0a20 2020 2020 2020 2073  ignore.        s
-0002cd20: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
-0002cd30: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
-0002cd40: 5479 7065 2c0a 2020 2020 2020 2020 666f  Type,.        fo
-0002cd50: 725f 3a20 4174 7472 6962 7574 6554 7970  r_: AttributeTyp
-0002cd60: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0002cd70: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
-0002cd80: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
-0002cd90: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0002cda0: 220a 2020 2020 2020 2020 5265 7072 6573  ".        Repres
-0002cdb0: 656e 7473 2061 2063 6170 7469 6f6e 2066  ents a caption f
-0002cdc0: 6f72 2061 6e20 6974 656d 2069 6e20 6120  or an item in a 
-0002cdd0: 7573 6572 2069 6e74 6572 6661 6365 2e0a  user interface..
-0002cde0: 0a20 2020 2020 2020 202a 2060 666f 725f  .        * `for_
-0002cdf0: 603a 2049 4420 6f66 2069 6e70 7574 2066  `: ID of input f
-0002ce00: 6965 6c64 2074 6f20 6173 736f 6369 6174  ield to associat
-0002ce10: 6520 7468 6973 206c 6162 656c 2077 6974  e this label wit
-0002ce20: 680a 0a20 2020 2020 2020 205b 5669 6577  h..        [View
-0002ce30: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-0002ce40: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-0002ce50: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002ce60: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002ce70: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f6c  b/HTML/Element/l
-0002ce80: 6162 656c 290a 2020 2020 2020 2020 2222  abel).        ""
-0002ce90: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-0002cea0: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-0002ceb0: 2020 2020 2020 2766 6f72 5f27 3a20 666f        'for_': fo
-0002cec0: 725f 2c0a 2020 2020 2020 2020 7d0a 2020  r_,.        }.  
-0002ced0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-0002cee0: 6572 2829 2e5f 5f63 616c 6c5f 5f28 2a63  er().__call__(*c
-0002cef0: 6869 6c64 7265 6e2c 202a 2a61 7474 7269  hildren, **attri
-0002cf00: 6275 7465 7329 0a0a 2020 2020 6465 6620  butes)..    def 
-0002cf10: 5f67 6574 5f64 6566 6175 6c74 5f61 7474  _get_default_att
-0002cf20: 7269 6275 7465 7328 7365 6c66 2c20 6769  ributes(self, gi
-0002cf30: 7665 6e3a 2064 6963 745b 7374 722c 2041  ven: dict[str, A
-0002cf40: 7474 7269 6275 7465 5479 7065 5d29 202d  ttributeType]) -
-0002cf50: 3e20 6469 6374 5b73 7472 2c20 4174 7472  > dict[str, Attr
-0002cf60: 6962 7574 6554 7970 655d 3a0a 2020 2020  ibuteType]:.    
-0002cf70: 2020 2020 7265 7475 726e 207b 2766 6f72      return {'for
-0002cf80: 5f27 3a20 4e6f 6e65 7d0a 0a0a 636c 6173  _': None}...clas
-0002cf90: 7320 6c65 6765 6e64 2854 6167 293a 0a20  s legend(Tag):. 
-0002cfa0: 2020 2022 2222 0a20 2020 2052 6570 7265     """.    Repre
-0002cfb0: 7365 6e74 7320 6120 6361 7074 696f 6e20  sents a caption 
-0002cfc0: 666f 7220 7468 6520 636f 6e74 656e 7420  for the content 
-0002cfd0: 6f66 2069 7473 2070 6172 656e 7420 5b60  of its parent [`
-0002cfe0: 3c66 6965 6c64 7365 743e 605d 2868 7474  <fieldset>`](htt
-0002cff0: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-0002d000: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-0002d010: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-0002d020: 6c65 6d65 6e74 2f66 6965 6c64 7365 7429  lement/fieldset)
-0002d030: 2e0a 0a20 2020 200a 0a20 2020 205b 5669  ...    ..    [Vi
-0002d040: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-0002d050: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-0002d060: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002d070: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002d080: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002d090: 2f6c 6567 656e 6429 0a20 2020 2022 2222  /legend).    """
-0002d0a0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002d0b0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0002d0c0: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-0002d0d0: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-0002d0e0: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-0002d0f0: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-0002d100: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-0002d110: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-0002d120: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002d130: 2020 2052 6570 7265 7365 6e74 7320 6120     Represents a 
-0002d140: 6361 7074 696f 6e20 666f 7220 7468 6520  caption for the 
-0002d150: 636f 6e74 656e 7420 6f66 2069 7473 2070  content of its p
-0002d160: 6172 656e 7420 5b60 3c66 6965 6c64 7365  arent [`<fieldse
-0002d170: 743e 605d 2868 7474 7073 3a2f 2f64 6576  t>`](https://dev
-0002d180: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002d190: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002d1a0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f66  b/HTML/Element/f
-0002d1b0: 6965 6c64 7365 7429 2e0a 0a20 2020 2020  ieldset)...     
-0002d1c0: 2020 200a 0a20 2020 2020 2020 205b 5669     ..        [Vi
-0002d1d0: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-0002d1e0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-0002d1f0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002d200: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002d210: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002d220: 2f6c 6567 656e 6429 0a20 2020 2020 2020  /legend).       
-0002d230: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-0002d240: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-0002d250: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0002d260: 2020 7d0a 2020 2020 2020 2020 7375 7065    }.        supe
-0002d270: 7228 292e 5f5f 696e 6974 5f5f 282a 6368  r().__init__(*ch
-0002d280: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
-0002d290: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
-0002d2a0: 5f63 616c 6c5f 5f28 2020 2320 7479 7065  _call__(  # type
-0002d2b0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0002d2c0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-0002d2d0: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
-0002d2e0: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
-0002d2f0: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
-0002d300: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
-0002d310: 5479 7065 2c0a 2020 2020 293a 0a20 2020  Type,.    ):.   
-0002d320: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002d330: 2052 6570 7265 7365 6e74 7320 6120 6361   Represents a ca
-0002d340: 7074 696f 6e20 666f 7220 7468 6520 636f  ption for the co
-0002d350: 6e74 656e 7420 6f66 2069 7473 2070 6172  ntent of its par
-0002d360: 656e 7420 5b60 3c66 6965 6c64 7365 743e  ent [`<fieldset>
-0002d370: 605d 2868 7474 7073 3a2f 2f64 6576 656c  `](https://devel
-0002d380: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-0002d390: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-0002d3a0: 4854 4d4c 2f45 6c65 6d65 6e74 2f66 6965  HTML/Element/fie
-0002d3b0: 6c64 7365 7429 2e0a 0a20 2020 2020 2020  ldset)...       
-0002d3c0: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-0002d3d0: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-0002d3e0: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-0002d3f0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002d400: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002d410: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f6c  b/HTML/Element/l
-0002d420: 6567 656e 6429 0a20 2020 2020 2020 2022  egend).        "
-0002d430: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
-0002d440: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
-0002d450: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0002d460: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
-0002d470: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
-0002d480: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
-0002d490: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
-0002d4a0: 6465 6620 5f67 6574 5f64 6566 6175 6c74  def _get_default
-0002d4b0: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
-0002d4c0: 2c20 6769 7665 6e3a 2064 6963 745b 7374  , given: dict[st
-0002d4d0: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
-0002d4e0: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
-0002d4f0: 4174 7472 6962 7574 6554 7970 655d 3a0a  AttributeType]:.
-0002d500: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-0002d510: 7d0a 0a0a 636c 6173 7320 6d65 7465 7228  }...class meter(
-0002d520: 5461 6729 3a0a 2020 2020 2222 220a 2020  Tag):.    """.  
-0002d530: 2020 5265 7072 6573 656e 7473 2065 6974    Represents eit
-0002d540: 6865 7220 6120 7363 616c 6172 2076 616c  her a scalar val
-0002d550: 7565 2077 6974 6869 6e20 6120 6b6e 6f77  ue within a know
-0002d560: 6e20 7261 6e67 6520 6f72 2061 2066 7261  n range or a fra
-0002d570: 6374 696f 6e61 6c20 7661 6c75 652e 0a0a  ctional value...
-0002d580: 2020 2020 0a0a 2020 2020 5b56 6965 7720      ..    [View 
-0002d590: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
-0002d5a0: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
-0002d5b0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
-0002d5c0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
-0002d5d0: 2f48 544d 4c2f 456c 656d 656e 742f 6d65  /HTML/Element/me
-0002d5e0: 7465 7229 0a20 2020 2022 2222 0a20 2020  ter).    """.   
-0002d5f0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0002d600: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002d610: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
-0002d620: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
-0002d630: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-0002d640: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
-0002d650: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
-0002d660: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0002d670: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0002d680: 6570 7265 7365 6e74 7320 6569 7468 6572  epresents either
-0002d690: 2061 2073 6361 6c61 7220 7661 6c75 6520   a scalar value 
-0002d6a0: 7769 7468 696e 2061 206b 6e6f 776e 2072  within a known r
-0002d6b0: 616e 6765 206f 7220 6120 6672 6163 7469  ange or a fracti
-0002d6c0: 6f6e 616c 2076 616c 7565 2e0a 0a20 2020  onal value...   
-0002d6d0: 2020 2020 200a 0a20 2020 2020 2020 205b       ..        [
-0002d6e0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-0002d6f0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-0002d700: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002d710: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002d720: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002d730: 6e74 2f6d 6574 6572 290a 2020 2020 2020  nt/meter).      
-0002d740: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
-0002d750: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
-0002d760: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-0002d770: 2020 207d 0a20 2020 2020 2020 2073 7570     }.        sup
-0002d780: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a63  er().__init__(*c
-0002d790: 6869 6c64 7265 6e2c 202a 2a61 7474 7269  hildren, **attri
-0002d7a0: 6275 7465 7329 0a0a 2020 2020 6465 6620  butes)..    def 
-0002d7b0: 5f5f 6361 6c6c 5f5f 2820 2023 2074 7970  __call__(  # typ
-0002d7c0: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-0002d7d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002d7e0: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
-0002d7f0: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
-0002d800: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
-0002d810: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
-0002d820: 6554 7970 652c 0a20 2020 2029 3a0a 2020  eType,.    ):.  
-0002d830: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0002d840: 2020 5265 7072 6573 656e 7473 2065 6974    Represents eit
-0002d850: 6865 7220 6120 7363 616c 6172 2076 616c  her a scalar val
-0002d860: 7565 2077 6974 6869 6e20 6120 6b6e 6f77  ue within a know
-0002d870: 6e20 7261 6e67 6520 6f72 2061 2066 7261  n range or a fra
-0002d880: 6374 696f 6e61 6c20 7661 6c75 652e 0a0a  ctional value...
-0002d890: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-0002d8a0: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-0002d8b0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-0002d8c0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-0002d8d0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-0002d8e0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-0002d8f0: 656d 656e 742f 6d65 7465 7229 0a20 2020  ement/meter).   
-0002d900: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002d910: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002d920: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-0002d930: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0002d940: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
-0002d950: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
-0002d960: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
-0002d970: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
-0002d980: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
-0002d990: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
-0002d9a0: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
-0002d9b0: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
-0002d9c0: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
-0002d9d0: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
-0002d9e0: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
-0002d9f0: 6f70 7467 726f 7570 2854 6167 293a 0a20  optgroup(Tag):. 
-0002da00: 2020 2022 2222 0a20 2020 2043 7265 6174     """.    Creat
-0002da10: 6573 2061 2067 726f 7570 696e 6720 6f66  es a grouping of
-0002da20: 206f 7074 696f 6e73 2077 6974 6869 6e20   options within 
-0002da30: 6120 5b60 3c73 656c 6563 743e 605d 2868  a [`<select>`](h
-0002da40: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-0002da50: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-0002da60: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-0002da70: 2f45 6c65 6d65 6e74 2f73 656c 6563 7429  /Element/select)
-0002da80: 2065 6c65 6d65 6e74 2e0a 0a20 2020 200a   element...    .
-0002da90: 0a20 2020 205b 5669 6577 2066 756c 6c20  .    [View full 
-0002daa0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-0002dab0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-0002dac0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-0002dad0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-0002dae0: 2f45 6c65 6d65 6e74 2f6f 7074 6772 6f75  /Element/optgrou
-0002daf0: 7029 0a20 2020 2022 2222 0a20 2020 2064  p).    """.    d
-0002db00: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002db10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002db20: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-0002db30: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-0002db40: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-0002db50: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-0002db60: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
-0002db70: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0002db80: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
-0002db90: 6174 6573 2061 2067 726f 7570 696e 6720  ates a grouping 
-0002dba0: 6f66 206f 7074 696f 6e73 2077 6974 6869  of options withi
-0002dbb0: 6e20 6120 5b60 3c73 656c 6563 743e 605d  n a [`<select>`]
-0002dbc0: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002dbd0: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002dbe0: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002dbf0: 4d4c 2f45 6c65 6d65 6e74 2f73 656c 6563  ML/Element/selec
-0002dc00: 7429 2065 6c65 6d65 6e74 2e0a 0a20 2020  t) element...   
-0002dc10: 2020 2020 200a 0a20 2020 2020 2020 205b       ..        [
-0002dc20: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
-0002dc30: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-0002dc40: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002dc50: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002dc60: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002dc70: 6e74 2f6f 7074 6772 6f75 7029 0a20 2020  nt/optgroup).   
-0002dc80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002dc90: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002dca0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-0002dcb0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0002dcc0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-0002dcd0: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
-0002dce0: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
-0002dcf0: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
-0002dd00: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0002dd10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002dd20: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-0002dd30: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-0002dd40: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-0002dd50: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-0002dd60: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
-0002dd70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002dd80: 2020 2020 2043 7265 6174 6573 2061 2067       Creates a g
-0002dd90: 726f 7570 696e 6720 6f66 206f 7074 696f  rouping of optio
-0002dda0: 6e73 2077 6974 6869 6e20 6120 5b60 3c73  ns within a [`<s
-0002ddb0: 656c 6563 743e 605d 2868 7474 7073 3a2f  elect>`](https:/
-0002ddc0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
-0002ddd0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
-0002dde0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
-0002ddf0: 6e74 2f73 656c 6563 7429 2065 6c65 6d65  nt/select) eleme
-0002de00: 6e74 2e0a 0a20 2020 2020 2020 200a 0a20  nt...        .. 
-0002de10: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
-0002de20: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-0002de30: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002de40: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002de50: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002de60: 4d4c 2f45 6c65 6d65 6e74 2f6f 7074 6772  ML/Element/optgr
-0002de70: 6f75 7029 0a20 2020 2020 2020 2022 2222  oup).        """
-0002de80: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
-0002de90: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
-0002dea0: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
-0002deb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002dec0: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-0002ded0: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
-0002dee0: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
-0002def0: 6620 5f67 6574 5f64 6566 6175 6c74 5f61  f _get_default_a
-0002df00: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
-0002df10: 6769 7665 6e3a 2064 6963 745b 7374 722c  given: dict[str,
-0002df20: 2041 7474 7269 6275 7465 5479 7065 5d29   AttributeType])
-0002df30: 202d 3e20 6469 6374 5b73 7472 2c20 4174   -> dict[str, At
-0002df40: 7472 6962 7574 6554 7970 655d 3a0a 2020  tributeType]:.  
-0002df50: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
-0002df60: 0a0a 636c 6173 7320 6f70 7469 6f6e 2854  ..class option(T
-0002df70: 6167 293a 0a20 2020 2022 2222 0a20 2020  ag):.    """.   
-0002df80: 2055 7365 6420 746f 2064 6566 696e 6520   Used to define 
-0002df90: 616e 2069 7465 6d20 636f 6e74 6169 6e65  an item containe
-0002dfa0: 6420 696e 2061 2073 656c 6563 742c 2061  d in a select, a
-0002dfb0: 6e20 5b60 3c6f 7074 6772 6f75 703e 605d  n [`<optgroup>`]
-0002dfc0: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002dfd0: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002dfe0: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002dff0: 4d4c 2f45 6c65 6d65 6e74 2f6f 7074 6772  ML/Element/optgr
-0002e000: 6f75 7029 2c20 6f72 2061 205b 603c 6461  oup), or a [`<da
-0002e010: 7461 6c69 7374 3e60 5d28 6874 7470 733a  talist>`](https:
-0002e020: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-0002e030: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-0002e040: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-0002e050: 656e 742f 6461 7461 6c69 7374 2920 656c  ent/datalist) el
-0002e060: 656d 656e 742e 2041 7320 7375 6368 2c20  ement. As such, 
-0002e070: 603c 6f70 7469 6f6e 3e60 2063 616e 2072  `<option>` can r
-0002e080: 6570 7265 7365 6e74 206d 656e 7520 6974  epresent menu it
-0002e090: 656d 7320 696e 2070 6f70 7570 7320 616e  ems in popups an
-0002e0a0: 6420 6f74 6865 7220 6c69 7374 7320 6f66  d other lists of
-0002e0b0: 2069 7465 6d73 2069 6e20 616e 2048 544d   items in an HTM
-0002e0c0: 4c20 646f 6375 6d65 6e74 2e0a 0a20 2020  L document...   
-0002e0d0: 200a 0a20 2020 205b 5669 6577 2066 756c   ..    [View ful
-0002e0e0: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-0002e0f0: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002e100: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002e110: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002e120: 4d4c 2f45 6c65 6d65 6e74 2f6f 7074 696f  ML/Element/optio
-0002e130: 6e29 0a20 2020 2022 2222 0a20 2020 2064  n).    """.    d
-0002e140: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002e150: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002e160: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-0002e170: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-0002e180: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-0002e190: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-0002e1a0: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
-0002e1b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0002e1c0: 2022 2222 0a20 2020 2020 2020 2055 7365   """.        Use
-0002e1d0: 6420 746f 2064 6566 696e 6520 616e 2069  d to define an i
-0002e1e0: 7465 6d20 636f 6e74 6169 6e65 6420 696e  tem contained in
-0002e1f0: 2061 2073 656c 6563 742c 2061 6e20 5b60   a select, an [`
-0002e200: 3c6f 7074 6772 6f75 703e 605d 2868 7474  <optgroup>`](htt
-0002e210: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-0002e220: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-0002e230: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
-0002e240: 6c65 6d65 6e74 2f6f 7074 6772 6f75 7029  lement/optgroup)
-0002e250: 2c20 6f72 2061 205b 603c 6461 7461 6c69  , or a [`<datali
-0002e260: 7374 3e60 5d28 6874 7470 733a 2f2f 6465  st>`](https://de
-0002e270: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-0002e280: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-0002e290: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-0002e2a0: 6461 7461 6c69 7374 2920 656c 656d 656e  datalist) elemen
-0002e2b0: 742e 2041 7320 7375 6368 2c20 603c 6f70  t. As such, `<op
-0002e2c0: 7469 6f6e 3e60 2063 616e 2072 6570 7265  tion>` can repre
-0002e2d0: 7365 6e74 206d 656e 7520 6974 656d 7320  sent menu items 
-0002e2e0: 696e 2070 6f70 7570 7320 616e 6420 6f74  in popups and ot
-0002e2f0: 6865 7220 6c69 7374 7320 6f66 2069 7465  her lists of ite
-0002e300: 6d73 2069 6e20 616e 2048 544d 4c20 646f  ms in an HTML do
-0002e310: 6375 6d65 6e74 2e0a 0a20 2020 2020 2020  cument...       
-0002e320: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
-0002e330: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
-0002e340: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-0002e350: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-0002e360: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-0002e370: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f6f  b/HTML/Element/o
-0002e380: 7074 696f 6e29 0a20 2020 2020 2020 2022  ption).        "
-0002e390: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
-0002e3a0: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
-0002e3b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0002e3c0: 7d0a 2020 2020 2020 2020 7375 7065 7228  }.        super(
-0002e3d0: 292e 5f5f 696e 6974 5f5f 282a 6368 696c  ).__init__(*chil
-0002e3e0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
-0002e3f0: 6573 290a 0a20 2020 2064 6566 205f 5f63  es)..    def __c
-0002e400: 616c 6c5f 5f28 2020 2320 7479 7065 3a20  all__(  # type: 
-0002e410: 6967 6e6f 7265 0a20 2020 2020 2020 2073  ignore.        s
-0002e420: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
-0002e430: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
-0002e440: 5479 7065 2c0a 2020 2020 2020 2020 0a20  Type,.        . 
-0002e450: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
-0002e460: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
-0002e470: 7065 2c0a 2020 2020 293a 0a20 2020 2020  pe,.    ):.     
-0002e480: 2020 2022 2222 0a20 2020 2020 2020 2055     """.        U
-0002e490: 7365 6420 746f 2064 6566 696e 6520 616e  sed to define an
-0002e4a0: 2069 7465 6d20 636f 6e74 6169 6e65 6420   item contained 
-0002e4b0: 696e 2061 2073 656c 6563 742c 2061 6e20  in a select, an 
-0002e4c0: 5b60 3c6f 7074 6772 6f75 703e 605d 2868  [`<optgroup>`](h
-0002e4d0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-0002e4e0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
-0002e4f0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
-0002e500: 2f45 6c65 6d65 6e74 2f6f 7074 6772 6f75  /Element/optgrou
-0002e510: 7029 2c20 6f72 2061 205b 603c 6461 7461  p), or a [`<data
-0002e520: 6c69 7374 3e60 5d28 6874 7470 733a 2f2f  list>`](https://
-0002e530: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-0002e540: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-0002e550: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-0002e560: 742f 6461 7461 6c69 7374 2920 656c 656d  t/datalist) elem
-0002e570: 656e 742e 2041 7320 7375 6368 2c20 603c  ent. As such, `<
-0002e580: 6f70 7469 6f6e 3e60 2063 616e 2072 6570  option>` can rep
-0002e590: 7265 7365 6e74 206d 656e 7520 6974 656d  resent menu item
-0002e5a0: 7320 696e 2070 6f70 7570 7320 616e 6420  s in popups and 
-0002e5b0: 6f74 6865 7220 6c69 7374 7320 6f66 2069  other lists of i
-0002e5c0: 7465 6d73 2069 6e20 616e 2048 544d 4c20  tems in an HTML 
-0002e5d0: 646f 6375 6d65 6e74 2e0a 0a20 2020 2020  document...     
-0002e5e0: 2020 200a 0a20 2020 2020 2020 205b 5669     ..        [Vi
-0002e5f0: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-0002e600: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-0002e610: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002e620: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002e630: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002e640: 2f6f 7074 696f 6e29 0a20 2020 2020 2020  /option).       
-0002e650: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-0002e660: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-0002e670: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0002e680: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
-0002e690: 726e 2073 7570 6572 2829 2e5f 5f63 616c  rn super().__cal
-0002e6a0: 6c5f 5f28 2a63 6869 6c64 7265 6e2c 202a  l__(*children, *
-0002e6b0: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
-0002e6c0: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
-0002e6d0: 6c74 5f61 7474 7269 6275 7465 7328 7365  lt_attributes(se
-0002e6e0: 6c66 2c20 6769 7665 6e3a 2064 6963 745b  lf, given: dict[
-0002e6f0: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
-0002e700: 7065 5d29 202d 3e20 6469 6374 5b73 7472  pe]) -> dict[str
-0002e710: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-0002e720: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0002e730: 207b 7d0a 0a0a 636c 6173 7320 6f75 7470   {}...class outp
-0002e740: 7574 2854 6167 293a 0a20 2020 2022 2222  ut(Tag):.    """
-0002e750: 0a20 2020 2043 6f6e 7461 696e 6572 2065  .    Container e
-0002e760: 6c65 6d65 6e74 2069 6e74 6f20 7768 6963  lement into whic
-0002e770: 6820 6120 7369 7465 206f 7220 6170 7020  h a site or app 
-0002e780: 6361 6e20 696e 6a65 6374 2074 6865 2072  can inject the r
-0002e790: 6573 756c 7473 206f 6620 6120 6361 6c63  esults of a calc
-0002e7a0: 756c 6174 696f 6e20 6f72 2074 6865 206f  ulation or the o
-0002e7b0: 7574 636f 6d65 206f 6620 6120 7573 6572  utcome of a user
-0002e7c0: 2061 6374 696f 6e2e 0a0a 2020 2020 0a0a   action...    ..
-0002e7d0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-0002e7e0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-0002e7f0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-0002e800: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-0002e810: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-0002e820: 456c 656d 656e 742f 6f75 7470 7574 290a  Element/output).
-0002e830: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0002e840: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0002e850: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002e860: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
-0002e870: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
-0002e880: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
-0002e890: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
-0002e8a0: 6554 7970 652c 0a20 2020 2029 202d 3e20  eType,.    ) -> 
-0002e8b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0002e8c0: 220a 2020 2020 2020 2020 436f 6e74 6169  ".        Contai
-0002e8d0: 6e65 7220 656c 656d 656e 7420 696e 746f  ner element into
-0002e8e0: 2077 6869 6368 2061 2073 6974 6520 6f72   which a site or
-0002e8f0: 2061 7070 2063 616e 2069 6e6a 6563 7420   app can inject 
-0002e900: 7468 6520 7265 7375 6c74 7320 6f66 2061  the results of a
-0002e910: 2063 616c 6375 6c61 7469 6f6e 206f 7220   calculation or 
-0002e920: 7468 6520 6f75 7463 6f6d 6520 6f66 2061  the outcome of a
-0002e930: 2075 7365 7220 6163 7469 6f6e 2e0a 0a20   user action... 
-0002e940: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-0002e950: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-0002e960: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-0002e970: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-0002e980: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-0002e990: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-0002e9a0: 6d65 6e74 2f6f 7574 7075 7429 0a20 2020  ment/output).   
-0002e9b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002e9c0: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
-0002e9d0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-0002e9e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0002e9f0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-0002ea00: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
-0002ea10: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
-0002ea20: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
-0002ea30: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0002ea40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002ea50: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
-0002ea60: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
-0002ea70: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
-0002ea80: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
-0002ea90: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
-0002eaa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002eab0: 2020 2020 2043 6f6e 7461 696e 6572 2065       Container e
-0002eac0: 6c65 6d65 6e74 2069 6e74 6f20 7768 6963  lement into whic
-0002ead0: 6820 6120 7369 7465 206f 7220 6170 7020  h a site or app 
-0002eae0: 6361 6e20 696e 6a65 6374 2074 6865 2072  can inject the r
-0002eaf0: 6573 756c 7473 206f 6620 6120 6361 6c63  esults of a calc
-0002eb00: 756c 6174 696f 6e20 6f72 2074 6865 206f  ulation or the o
-0002eb10: 7574 636f 6d65 206f 6620 6120 7573 6572  utcome of a user
-0002eb20: 2061 6374 696f 6e2e 0a0a 2020 2020 2020   action...      
-0002eb30: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
-0002eb40: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
-0002eb50: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
-0002eb60: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-0002eb70: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-0002eb80: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-0002eb90: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
-0002eba0: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
-0002ebb0: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
-0002ebc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002ebd0: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
-0002ebe0: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
-0002ebf0: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
-0002ec00: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
-0002ec10: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
-0002ec20: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
-0002ec30: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
-0002ec40: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
-0002ec50: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
-0002ec60: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
-0002ec70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002ec80: 7b7d 0a0a 0a63 6c61 7373 2070 726f 6772  {}...class progr
-0002ec90: 6573 7328 5461 6729 3a0a 2020 2020 2222  ess(Tag):.    ""
-0002eca0: 220a 2020 2020 4469 7370 6c61 7973 2061  ".    Displays a
-0002ecb0: 6e20 696e 6469 6361 746f 7220 7368 6f77  n indicator show
-0002ecc0: 696e 6720 7468 6520 636f 6d70 6c65 7469  ing the completi
-0002ecd0: 6f6e 2070 726f 6772 6573 7320 6f66 2061  on progress of a
-0002ece0: 2074 6173 6b2c 2074 7970 6963 616c 6c79   task, typically
-0002ecf0: 2064 6973 706c 6179 6564 2061 7320 6120   displayed as a 
-0002ed00: 7072 6f67 7265 7373 2062 6172 2e0a 0a20  progress bar... 
-0002ed10: 2020 200a 0a20 2020 205b 5669 6577 2066     ..    [View f
-0002ed20: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
-0002ed30: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
-0002ed40: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-0002ed50: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-0002ed60: 4854 4d4c 2f45 6c65 6d65 6e74 2f70 726f  HTML/Element/pro
-0002ed70: 6772 6573 7329 0a20 2020 2022 2222 0a20  gress).    """. 
-0002ed80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0002ed90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002eda0: 2020 2020 2020 202a 6368 696c 6472 656e         *children
-0002edb0: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
-0002edc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002edd0: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
-0002ede0: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
-0002edf0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-0002ee00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002ee10: 2044 6973 706c 6179 7320 616e 2069 6e64   Displays an ind
-0002ee20: 6963 6174 6f72 2073 686f 7769 6e67 2074  icator showing t
-0002ee30: 6865 2063 6f6d 706c 6574 696f 6e20 7072  he completion pr
-0002ee40: 6f67 7265 7373 206f 6620 6120 7461 736b  ogress of a task
-0002ee50: 2c20 7479 7069 6361 6c6c 7920 6469 7370  , typically disp
-0002ee60: 6c61 7965 6420 6173 2061 2070 726f 6772  layed as a progr
-0002ee70: 6573 7320 6261 722e 0a0a 2020 2020 2020  ess bar...      
-0002ee80: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
-0002ee90: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
-0002eea0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
-0002eeb0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-0002eec0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-0002eed0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-0002eee0: 7072 6f67 7265 7373 290a 2020 2020 2020  progress).      
-0002eef0: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
-0002ef00: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
-0002ef10: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-0002ef20: 2020 207d 0a20 2020 2020 2020 2073 7570     }.        sup
-0002ef30: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a63  er().__init__(*c
-0002ef40: 6869 6c64 7265 6e2c 202a 2a61 7474 7269  hildren, **attri
-0002ef50: 6275 7465 7329 0a0a 2020 2020 6465 6620  butes)..    def 
-0002ef60: 5f5f 6361 6c6c 5f5f 2820 2023 2074 7970  __call__(  # typ
-0002ef70: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-0002ef80: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002ef90: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
-0002efa0: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
-0002efb0: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
-0002efc0: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
-0002efd0: 6554 7970 652c 0a20 2020 2029 3a0a 2020  eType,.    ):.  
-0002efe0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0002eff0: 2020 4469 7370 6c61 7973 2061 6e20 696e    Displays an in
-0002f000: 6469 6361 746f 7220 7368 6f77 696e 6720  dicator showing 
-0002f010: 7468 6520 636f 6d70 6c65 7469 6f6e 2070  the completion p
-0002f020: 726f 6772 6573 7320 6f66 2061 2074 6173  rogress of a tas
-0002f030: 6b2c 2074 7970 6963 616c 6c79 2064 6973  k, typically dis
-0002f040: 706c 6179 6564 2061 7320 6120 7072 6f67  played as a prog
-0002f050: 7265 7373 2062 6172 2e0a 0a20 2020 2020  ress bar...     
-0002f060: 2020 200a 0a20 2020 2020 2020 205b 5669     ..        [Vi
-0002f070: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-0002f080: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-0002f090: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002f0a0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002f0b0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002f0c0: 2f70 726f 6772 6573 7329 0a20 2020 2020  /progress).     
-0002f0d0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-0002f0e0: 7474 7269 6275 7465 7320 7c3d 207b 0a20  ttributes |= {. 
-0002f0f0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0002f100: 2020 2020 7d0a 2020 2020 2020 2020 7265      }.        re
-0002f110: 7475 726e 2073 7570 6572 2829 2e5f 5f63  turn super().__c
-0002f120: 616c 6c5f 5f28 2a63 6869 6c64 7265 6e2c  all__(*children,
-0002f130: 202a 2a61 7474 7269 6275 7465 7329 0a0a   **attributes)..
-0002f140: 2020 2020 6465 6620 5f67 6574 5f64 6566      def _get_def
-0002f150: 6175 6c74 5f61 7474 7269 6275 7465 7328  ault_attributes(
-0002f160: 7365 6c66 2c20 6769 7665 6e3a 2064 6963  self, given: dic
-0002f170: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
-0002f180: 5479 7065 5d29 202d 3e20 6469 6374 5b73  Type]) -> dict[s
-0002f190: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
-0002f1a0: 655d 3a0a 2020 2020 2020 2020 7265 7475  e]:.        retu
-0002f1b0: 726e 207b 7d0a 0a0a 636c 6173 7320 7365  rn {}...class se
-0002f1c0: 6c65 6374 2854 6167 293a 0a20 2020 2022  lect(Tag):.    "
-0002f1d0: 2222 0a20 2020 2052 6570 7265 7365 6e74  "".    Represent
-0002f1e0: 7320 6120 636f 6e74 726f 6c20 7468 6174  s a control that
-0002f1f0: 2070 726f 7669 6465 7320 6120 6d65 6e75   provides a menu
-0002f200: 206f 6620 6f70 7469 6f6e 732e 0a0a 2020   of options...  
-0002f210: 2020 0a0a 2020 2020 5b56 6965 7720 6675    ..    [View fu
-0002f220: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
-0002f230: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-0002f240: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-0002f250: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-0002f260: 544d 4c2f 456c 656d 656e 742f 7365 6c65  TML/Element/sele
-0002f270: 6374 290a 2020 2020 2222 220a 2020 2020  ct).    """.    
-0002f280: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0002f290: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0002f2a0: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-0002f2b0: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-0002f2c0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-0002f2d0: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-0002f2e0: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-0002f2f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0002f300: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0002f310: 7072 6573 656e 7473 2061 2063 6f6e 7472  presents a contr
-0002f320: 6f6c 2074 6861 7420 7072 6f76 6964 6573  ol that provides
-0002f330: 2061 206d 656e 7520 6f66 206f 7074 696f   a menu of optio
-0002f340: 6e73 2e0a 0a20 2020 2020 2020 200a 0a20  ns...        .. 
-0002f350: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
-0002f360: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
-0002f370: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
-0002f380: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
-0002f390: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
-0002f3a0: 4d4c 2f45 6c65 6d65 6e74 2f73 656c 6563  ML/Element/selec
-0002f3b0: 7429 0a20 2020 2020 2020 2022 2222 0a20  t).        """. 
-0002f3c0: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
-0002f3d0: 7320 7c3d 207b 0a20 2020 2020 2020 2020  s |= {.         
-0002f3e0: 2020 200a 2020 2020 2020 2020 7d0a 2020     .        }.  
-0002f3f0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-0002f400: 696e 6974 5f5f 282a 6368 696c 6472 656e  init__(*children
-0002f410: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
-0002f420: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-0002f430: 5f28 2020 2320 7479 7065 3a20 6967 6e6f  _(  # type: igno
-0002f440: 7265 0a20 2020 2020 2020 2073 656c 662c  re.        self,
-0002f450: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-0002f460: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-0002f470: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-0002f480: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-0002f490: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-0002f4a0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0002f4b0: 2222 0a20 2020 2020 2020 2052 6570 7265  "".        Repre
-0002f4c0: 7365 6e74 7320 6120 636f 6e74 726f 6c20  sents a control 
-0002f4d0: 7468 6174 2070 726f 7669 6465 7320 6120  that provides a 
-0002f4e0: 6d65 6e75 206f 6620 6f70 7469 6f6e 732e  menu of options.
-0002f4f0: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
-0002f500: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-0002f510: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-0002f520: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-0002f530: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-0002f540: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-0002f550: 456c 656d 656e 742f 7365 6c65 6374 290a  Element/select).
-0002f560: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0002f570: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
-0002f580: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0002f590: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-0002f5a0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-0002f5b0: 292e 5f5f 6361 6c6c 5f5f 282a 6368 696c  ).__call__(*chil
-0002f5c0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
-0002f5d0: 6573 290a 0a20 2020 2064 6566 205f 6765  es)..    def _ge
-0002f5e0: 745f 6465 6661 756c 745f 6174 7472 6962  t_default_attrib
-0002f5f0: 7574 6573 2873 656c 662c 2067 6976 656e  utes(self, given
-0002f600: 3a20 6469 6374 5b73 7472 2c20 4174 7472  : dict[str, Attr
-0002f610: 6962 7574 6554 7970 655d 2920 2d3e 2064  ibuteType]) -> d
-0002f620: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
-0002f630: 7465 5479 7065 5d3a 0a20 2020 2020 2020  teType]:.       
-0002f640: 2072 6574 7572 6e20 7b7d 0a0a 0a63 6c61   return {}...cla
-0002f650: 7373 2074 6578 7461 7265 6128 5461 6729  ss textarea(Tag)
-0002f660: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-0002f670: 7072 6573 656e 7473 2061 206d 756c 7469  presents a multi
-0002f680: 2d6c 696e 6520 706c 6169 6e2d 7465 7874  -line plain-text
-0002f690: 2065 6469 7469 6e67 2063 6f6e 7472 6f6c   editing control
-0002f6a0: 2c20 7573 6566 756c 2077 6865 6e20 796f  , useful when yo
-0002f6b0: 7520 7761 6e74 2074 6f20 616c 6c6f 7720  u want to allow 
-0002f6c0: 7573 6572 7320 746f 2065 6e74 6572 2061  users to enter a
-0002f6d0: 2073 697a 6561 626c 6520 616d 6f75 6e74   sizeable amount
-0002f6e0: 206f 6620 6672 6565 2d66 6f72 6d20 7465   of free-form te
-0002f6f0: 7874 2c20 666f 7220 6578 616d 706c 652c  xt, for example,
-0002f700: 2061 2063 6f6d 6d65 6e74 206f 6e20 6120   a comment on a 
-0002f710: 7265 7669 6577 206f 7220 6665 6564 6261  review or feedba
-0002f720: 636b 2066 6f72 6d2e 0a0a 2020 2020 0a0a  ck form...    ..
-0002f730: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-0002f740: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-0002f750: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-0002f760: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-0002f770: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-0002f780: 456c 656d 656e 742f 7465 7874 6172 6561  Element/textarea
-0002f790: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
-0002f7a0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0002f7b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002f7c0: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
-0002f7d0: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
-0002f7e0: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
-0002f7f0: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
-0002f800: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
-0002f810: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0002f820: 2222 220a 2020 2020 2020 2020 5265 7072  """.        Repr
-0002f830: 6573 656e 7473 2061 206d 756c 7469 2d6c  esents a multi-l
-0002f840: 696e 6520 706c 6169 6e2d 7465 7874 2065  ine plain-text e
-0002f850: 6469 7469 6e67 2063 6f6e 7472 6f6c 2c20  diting control, 
-0002f860: 7573 6566 756c 2077 6865 6e20 796f 7520  useful when you 
-0002f870: 7761 6e74 2074 6f20 616c 6c6f 7720 7573  want to allow us
-0002f880: 6572 7320 746f 2065 6e74 6572 2061 2073  ers to enter a s
-0002f890: 697a 6561 626c 6520 616d 6f75 6e74 206f  izeable amount o
-0002f8a0: 6620 6672 6565 2d66 6f72 6d20 7465 7874  f free-form text
-0002f8b0: 2c20 666f 7220 6578 616d 706c 652c 2061  , for example, a
-0002f8c0: 2063 6f6d 6d65 6e74 206f 6e20 6120 7265   comment on a re
-0002f8d0: 7669 6577 206f 7220 6665 6564 6261 636b  view or feedback
-0002f8e0: 2066 6f72 6d2e 0a0a 2020 2020 2020 2020   form...        
-0002f8f0: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
-0002f900: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
-0002f910: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
-0002f920: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
-0002f930: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
-0002f940: 2f48 544d 4c2f 456c 656d 656e 742f 7465  /HTML/Element/te
-0002f950: 7874 6172 6561 290a 2020 2020 2020 2020  xtarea).        
-0002f960: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
-0002f970: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
-0002f980: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0002f990: 207d 0a20 2020 2020 2020 2073 7570 6572   }.        super
-0002f9a0: 2829 2e5f 5f69 6e69 745f 5f28 2a63 6869  ().__init__(*chi
-0002f9b0: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
-0002f9c0: 7465 7329 0a0a 2020 2020 6465 6620 5f5f  tes)..    def __
-0002f9d0: 6361 6c6c 5f5f 2820 2023 2074 7970 653a  call__(  # type:
-0002f9e0: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
-0002f9f0: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
-0002fa00: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
-0002fa10: 6e54 7970 652c 0a20 2020 2020 2020 200a  nType,.        .
-0002fa20: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
-0002fa30: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
-0002fa40: 7970 652c 0a20 2020 2029 3a0a 2020 2020  ype,.    ):.    
-0002fa50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002fa60: 5265 7072 6573 656e 7473 2061 206d 756c  Represents a mul
-0002fa70: 7469 2d6c 696e 6520 706c 6169 6e2d 7465  ti-line plain-te
-0002fa80: 7874 2065 6469 7469 6e67 2063 6f6e 7472  xt editing contr
-0002fa90: 6f6c 2c20 7573 6566 756c 2077 6865 6e20  ol, useful when 
-0002faa0: 796f 7520 7761 6e74 2074 6f20 616c 6c6f  you want to allo
-0002fab0: 7720 7573 6572 7320 746f 2065 6e74 6572  w users to enter
-0002fac0: 2061 2073 697a 6561 626c 6520 616d 6f75   a sizeable amou
-0002fad0: 6e74 206f 6620 6672 6565 2d66 6f72 6d20  nt of free-form 
-0002fae0: 7465 7874 2c20 666f 7220 6578 616d 706c  text, for exampl
-0002faf0: 652c 2061 2063 6f6d 6d65 6e74 206f 6e20  e, a comment on 
-0002fb00: 6120 7265 7669 6577 206f 7220 6665 6564  a review or feed
-0002fb10: 6261 636b 2066 6f72 6d2e 0a0a 2020 2020  back form...    
-0002fb20: 2020 2020 0a0a 2020 2020 2020 2020 5b56      ..        [V
-0002fb30: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
-0002fb40: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-0002fb50: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-0002fb60: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-0002fb70: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-0002fb80: 742f 7465 7874 6172 6561 290a 2020 2020  t/textarea).    
-0002fb90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002fba0: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
-0002fbb0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0002fbc0: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
-0002fbd0: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
-0002fbe0: 6361 6c6c 5f5f 282a 6368 696c 6472 656e  call__(*children
-0002fbf0: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
-0002fc00: 0a20 2020 2064 6566 205f 6765 745f 6465  .    def _get_de
-0002fc10: 6661 756c 745f 6174 7472 6962 7574 6573  fault_attributes
-0002fc20: 2873 656c 662c 2067 6976 656e 3a20 6469  (self, given: di
-0002fc30: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
-0002fc40: 6554 7970 655d 2920 2d3e 2064 6963 745b  eType]) -> dict[
-0002fc50: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
-0002fc60: 7065 5d3a 0a20 2020 2020 2020 2072 6574  pe]:.        ret
-0002fc70: 7572 6e20 7b7d 0a0a 0a63 6c61 7373 2064  urn {}...class d
-0002fc80: 6574 6169 6c73 2854 6167 293a 0a20 2020  etails(Tag):.   
-0002fc90: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
-0002fca0: 2061 2064 6973 636c 6f73 7572 6520 7769   a disclosure wi
-0002fcb0: 6467 6574 2069 6e20 7768 6963 6820 696e  dget in which in
-0002fcc0: 666f 726d 6174 696f 6e20 6973 2076 6973  formation is vis
-0002fcd0: 6962 6c65 206f 6e6c 7920 7768 656e 2074  ible only when t
-0002fce0: 6865 2077 6964 6765 7420 6973 2074 6f67  he widget is tog
-0002fcf0: 676c 6564 2069 6e74 6f20 616e 2022 6f70  gled into an "op
-0002fd00: 656e 2220 7374 6174 652e 2041 2073 756d  en" state. A sum
-0002fd10: 6d61 7279 206f 7220 6c61 6265 6c20 6d75  mary or label mu
-0002fd20: 7374 2062 6520 7072 6f76 6964 6564 2075  st be provided u
-0002fd30: 7369 6e67 2074 6865 205b 603c 7375 6d6d  sing the [`<summ
-0002fd40: 6172 793e 605d 2868 7474 7073 3a2f 2f64  ary>`](https://d
-0002fd50: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-0002fd60: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-0002fd70: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-0002fd80: 2f73 756d 6d61 7279 2920 656c 656d 656e  /summary) elemen
-0002fd90: 742e 0a0a 2020 2020 0a0a 2020 2020 5b56  t...    ..    [V
-0002fda0: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
-0002fdb0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-0002fdc0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
-0002fdd0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
-0002fde0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
-0002fdf0: 742f 6465 7461 696c 7329 0a20 2020 2022  t/details).    "
-0002fe00: 2222 0a20 2020 2064 6566 205f 5f69 6e69  "".    def __ini
-0002fe10: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0002fe20: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
-0002fe30: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
-0002fe40: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
-0002fe50: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
-0002fe60: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
-0002fe70: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0002fe80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002fe90: 2020 2020 2043 7265 6174 6573 2061 2064       Creates a d
-0002fea0: 6973 636c 6f73 7572 6520 7769 6467 6574  isclosure widget
-0002feb0: 2069 6e20 7768 6963 6820 696e 666f 726d   in which inform
-0002fec0: 6174 696f 6e20 6973 2076 6973 6962 6c65  ation is visible
-0002fed0: 206f 6e6c 7920 7768 656e 2074 6865 2077   only when the w
-0002fee0: 6964 6765 7420 6973 2074 6f67 676c 6564  idget is toggled
-0002fef0: 2069 6e74 6f20 616e 2022 6f70 656e 2220   into an "open" 
-0002ff00: 7374 6174 652e 2041 2073 756d 6d61 7279  state. A summary
-0002ff10: 206f 7220 6c61 6265 6c20 6d75 7374 2062   or label must b
-0002ff20: 6520 7072 6f76 6964 6564 2075 7369 6e67  e provided using
-0002ff30: 2074 6865 205b 603c 7375 6d6d 6172 793e   the [`<summary>
-0002ff40: 605d 2868 7474 7073 3a2f 2f64 6576 656c  `](https://devel
-0002ff50: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-0002ff60: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-0002ff70: 4854 4d4c 2f45 6c65 6d65 6e74 2f73 756d  HTML/Element/sum
-0002ff80: 6d61 7279 2920 656c 656d 656e 742e 0a0a  mary) element...
-0002ff90: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-0002ffa0: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-0002ffb0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-0002ffc0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-0002ffd0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-0002ffe0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-0002fff0: 656d 656e 742f 6465 7461 696c 7329 0a20  ement/details). 
-00030000: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00030010: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
-00030020: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
-00030030: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00030040: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00030050: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
-00030060: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
-00030070: 2064 6566 205f 5f63 616c 6c5f 5f28 2020   def __call__(  
-00030080: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
-00030090: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000300a0: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
-000300b0: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
-000300c0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000300d0: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
-000300e0: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
-000300f0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00030100: 2020 2020 2020 2043 7265 6174 6573 2061         Creates a
-00030110: 2064 6973 636c 6f73 7572 6520 7769 6467   disclosure widg
-00030120: 6574 2069 6e20 7768 6963 6820 696e 666f  et in which info
-00030130: 726d 6174 696f 6e20 6973 2076 6973 6962  rmation is visib
-00030140: 6c65 206f 6e6c 7920 7768 656e 2074 6865  le only when the
-00030150: 2077 6964 6765 7420 6973 2074 6f67 676c   widget is toggl
-00030160: 6564 2069 6e74 6f20 616e 2022 6f70 656e  ed into an "open
-00030170: 2220 7374 6174 652e 2041 2073 756d 6d61  " state. A summa
-00030180: 7279 206f 7220 6c61 6265 6c20 6d75 7374  ry or label must
-00030190: 2062 6520 7072 6f76 6964 6564 2075 7369   be provided usi
-000301a0: 6e67 2074 6865 205b 603c 7375 6d6d 6172  ng the [`<summar
-000301b0: 793e 605d 2868 7474 7073 3a2f 2f64 6576  y>`](https://dev
-000301c0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
-000301d0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
-000301e0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f73  b/HTML/Element/s
-000301f0: 756d 6d61 7279 2920 656c 656d 656e 742e  ummary) element.
-00030200: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
-00030210: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-00030220: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00030230: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-00030240: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-00030250: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-00030260: 456c 656d 656e 742f 6465 7461 696c 7329  Element/details)
-00030270: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00030280: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
-00030290: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
-000302a0: 200a 2020 2020 2020 2020 7d0a 2020 2020   .        }.    
-000302b0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-000302c0: 2829 2e5f 5f63 616c 6c5f 5f28 2a63 6869  ().__call__(*chi
-000302d0: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
-000302e0: 7465 7329 0a0a 2020 2020 6465 6620 5f67  tes)..    def _g
-000302f0: 6574 5f64 6566 6175 6c74 5f61 7474 7269  et_default_attri
-00030300: 6275 7465 7328 7365 6c66 2c20 6769 7665  butes(self, give
-00030310: 6e3a 2064 6963 745b 7374 722c 2041 7474  n: dict[str, Att
-00030320: 7269 6275 7465 5479 7065 5d29 202d 3e20  ributeType]) -> 
-00030330: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
-00030340: 7574 6554 7970 655d 3a0a 2020 2020 2020  uteType]:.      
-00030350: 2020 7265 7475 726e 207b 7d0a 0a0a 636c    return {}...cl
-00030360: 6173 7320 6469 616c 6f67 2854 6167 293a  ass dialog(Tag):
-00030370: 0a20 2020 2022 2222 0a20 2020 2052 6570  .    """.    Rep
-00030380: 7265 7365 6e74 7320 6120 6469 616c 6f67  resents a dialog
-00030390: 2062 6f78 206f 7220 6f74 6865 7220 696e   box or other in
-000303a0: 7465 7261 6374 6976 6520 636f 6d70 6f6e  teractive compon
-000303b0: 656e 742c 2073 7563 6820 6173 2061 2064  ent, such as a d
-000303c0: 6973 6d69 7373 6962 6c65 2061 6c65 7274  ismissible alert
-000303d0: 2c20 696e 7370 6563 746f 722c 206f 7220  , inspector, or 
-000303e0: 7375 6277 696e 646f 772e 0a0a 2020 2020  subwindow...    
-000303f0: 0a0a 2020 2020 5b56 6965 7720 6675 6c6c  ..    [View full
-00030400: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00030410: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00030420: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00030430: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00030440: 4c2f 456c 656d 656e 742f 6469 616c 6f67  L/Element/dialog
-00030450: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
-00030460: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00030470: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00030480: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
-00030490: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
-000304a0: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
-000304b0: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
-000304c0: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
-000304d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000304e0: 2222 220a 2020 2020 2020 2020 5265 7072  """.        Repr
-000304f0: 6573 656e 7473 2061 2064 6961 6c6f 6720  esents a dialog 
-00030500: 626f 7820 6f72 206f 7468 6572 2069 6e74  box or other int
-00030510: 6572 6163 7469 7665 2063 6f6d 706f 6e65  eractive compone
-00030520: 6e74 2c20 7375 6368 2061 7320 6120 6469  nt, such as a di
-00030530: 736d 6973 7369 626c 6520 616c 6572 742c  smissible alert,
-00030540: 2069 6e73 7065 6374 6f72 2c20 6f72 2073   inspector, or s
-00030550: 7562 7769 6e64 6f77 2e0a 0a20 2020 2020  ubwindow...     
-00030560: 2020 200a 0a20 2020 2020 2020 205b 5669     ..        [Vi
-00030570: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-00030580: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00030590: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-000305a0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-000305b0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-000305c0: 2f64 6961 6c6f 6729 0a20 2020 2020 2020  /dialog).       
-000305d0: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
-000305e0: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
-000305f0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00030600: 2020 7d0a 2020 2020 2020 2020 7375 7065    }.        supe
-00030610: 7228 292e 5f5f 696e 6974 5f5f 282a 6368  r().__init__(*ch
-00030620: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
-00030630: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
-00030640: 5f63 616c 6c5f 5f28 2020 2320 7479 7065  _call__(  # type
-00030650: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-00030660: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00030670: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
-00030680: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
-00030690: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
-000306a0: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
-000306b0: 5479 7065 2c0a 2020 2020 293a 0a20 2020  Type,.    ):.   
-000306c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000306d0: 2052 6570 7265 7365 6e74 7320 6120 6469   Represents a di
-000306e0: 616c 6f67 2062 6f78 206f 7220 6f74 6865  alog box or othe
-000306f0: 7220 696e 7465 7261 6374 6976 6520 636f  r interactive co
-00030700: 6d70 6f6e 656e 742c 2073 7563 6820 6173  mponent, such as
-00030710: 2061 2064 6973 6d69 7373 6962 6c65 2061   a dismissible a
-00030720: 6c65 7274 2c20 696e 7370 6563 746f 722c  lert, inspector,
-00030730: 206f 7220 7375 6277 696e 646f 772e 0a0a   or subwindow...
-00030740: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-00030750: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
-00030760: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00030770: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
-00030780: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
-00030790: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
-000307a0: 656d 656e 742f 6469 616c 6f67 290a 2020  ement/dialog).  
-000307b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000307c0: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-000307d0: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-000307e0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000307f0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00030800: 5f5f 6361 6c6c 5f5f 282a 6368 696c 6472  __call__(*childr
-00030810: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
-00030820: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-00030830: 6465 6661 756c 745f 6174 7472 6962 7574  default_attribut
-00030840: 6573 2873 656c 662c 2067 6976 656e 3a20  es(self, given: 
-00030850: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
-00030860: 7574 6554 7970 655d 2920 2d3e 2064 6963  uteType]) -> dic
-00030870: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
-00030880: 5479 7065 5d3a 0a20 2020 2020 2020 2072  Type]:.        r
-00030890: 6574 7572 6e20 7b7d 0a0a 0a63 6c61 7373  eturn {}...class
-000308a0: 2073 756d 6d61 7279 2854 6167 293a 0a20   summary(Tag):. 
-000308b0: 2020 2022 2222 0a20 2020 2053 7065 6369     """.    Speci
-000308c0: 6669 6573 2061 2073 756d 6d61 7279 2c20  fies a summary, 
-000308d0: 6361 7074 696f 6e2c 206f 7220 6c65 6765  caption, or lege
-000308e0: 6e64 2066 6f72 2061 2064 6574 6169 6c73  nd for a details
-000308f0: 2065 6c65 6d65 6e74 2773 2064 6973 636c   element's discl
-00030900: 6f73 7572 6520 626f 782e 2043 6c69 636b  osure box. Click
-00030910: 696e 6720 7468 6520 603c 7375 6d6d 6172  ing the `<summar
-00030920: 793e 6020 656c 656d 656e 7420 746f 6767  y>` element togg
-00030930: 6c65 7320 7468 6520 7374 6174 6520 6f66  les the state of
-00030940: 2074 6865 2070 6172 656e 7420 5b60 3c64   the parent [`<d
-00030950: 6574 6169 6c73 3e60 5d28 6874 7470 733a  etails>`](https:
-00030960: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00030970: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-00030980: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-00030990: 656e 742f 6465 7461 696c 7329 2065 6c65  ent/details) ele
-000309a0: 6d65 6e74 206f 7065 6e20 616e 6420 636c  ment open and cl
-000309b0: 6f73 6564 2e0a 0a20 2020 200a 0a20 2020  osed...    ..   
-000309c0: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-000309d0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-000309e0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-000309f0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-00030a00: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-00030a10: 6d65 6e74 2f73 756d 6d61 7279 290a 2020  ment/summary).  
-00030a20: 2020 2222 220a 2020 2020 6465 6620 5f5f    """.    def __
-00030a30: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00030a40: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
-00030a50: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
-00030a60: 6e54 7970 652c 0a20 2020 2020 2020 200a  nType,.        .
-00030a70: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
-00030a80: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
-00030a90: 7970 652c 0a20 2020 2029 202d 3e20 4e6f  ype,.    ) -> No
-00030aa0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00030ab0: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
-00030ac0: 7320 6120 7375 6d6d 6172 792c 2063 6170  s a summary, cap
-00030ad0: 7469 6f6e 2c20 6f72 206c 6567 656e 6420  tion, or legend 
-00030ae0: 666f 7220 6120 6465 7461 696c 7320 656c  for a details el
-00030af0: 656d 656e 7427 7320 6469 7363 6c6f 7375  ement's disclosu
-00030b00: 7265 2062 6f78 2e20 436c 6963 6b69 6e67  re box. Clicking
-00030b10: 2074 6865 2060 3c73 756d 6d61 7279 3e60   the `<summary>`
-00030b20: 2065 6c65 6d65 6e74 2074 6f67 676c 6573   element toggles
-00030b30: 2074 6865 2073 7461 7465 206f 6620 7468   the state of th
-00030b40: 6520 7061 7265 6e74 205b 603c 6465 7461  e parent [`<deta
-00030b50: 696c 733e 605d 2868 7474 7073 3a2f 2f64  ils>`](https://d
-00030b60: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-00030b70: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-00030b80: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-00030b90: 2f64 6574 6169 6c73 2920 656c 656d 656e  /details) elemen
-00030ba0: 7420 6f70 656e 2061 6e64 2063 6c6f 7365  t open and close
-00030bb0: 642e 0a0a 2020 2020 2020 2020 0a0a 2020  d...        ..  
-00030bc0: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
-00030bd0: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00030be0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
-00030bf0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
-00030c00: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
-00030c10: 4c2f 456c 656d 656e 742f 7375 6d6d 6172  L/Element/summar
-00030c20: 7929 0a20 2020 2020 2020 2022 2222 0a20  y).        """. 
-00030c30: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
-00030c40: 7320 7c3d 207b 0a20 2020 2020 2020 2020  s |= {.         
-00030c50: 2020 200a 2020 2020 2020 2020 7d0a 2020     .        }.  
-00030c60: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00030c70: 696e 6974 5f5f 282a 6368 696c 6472 656e  init__(*children
-00030c80: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
-00030c90: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-00030ca0: 5f28 2020 2320 7479 7065 3a20 6967 6e6f  _(  # type: igno
-00030cb0: 7265 0a20 2020 2020 2020 2073 656c 662c  re.        self,
-00030cc0: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
-00030cd0: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
-00030ce0: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
-00030cf0: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
-00030d00: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
-00030d10: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00030d20: 2222 0a20 2020 2020 2020 2053 7065 6369  "".        Speci
-00030d30: 6669 6573 2061 2073 756d 6d61 7279 2c20  fies a summary, 
-00030d40: 6361 7074 696f 6e2c 206f 7220 6c65 6765  caption, or lege
-00030d50: 6e64 2066 6f72 2061 2064 6574 6169 6c73  nd for a details
-00030d60: 2065 6c65 6d65 6e74 2773 2064 6973 636c   element's discl
-00030d70: 6f73 7572 6520 626f 782e 2043 6c69 636b  osure box. Click
-00030d80: 696e 6720 7468 6520 603c 7375 6d6d 6172  ing the `<summar
-00030d90: 793e 6020 656c 656d 656e 7420 746f 6767  y>` element togg
-00030da0: 6c65 7320 7468 6520 7374 6174 6520 6f66  les the state of
-00030db0: 2074 6865 2070 6172 656e 7420 5b60 3c64   the parent [`<d
-00030dc0: 6574 6169 6c73 3e60 5d28 6874 7470 733a  etails>`](https:
-00030dd0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
-00030de0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
-00030df0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
-00030e00: 656e 742f 6465 7461 696c 7329 2065 6c65  ent/details) ele
-00030e10: 6d65 6e74 206f 7065 6e20 616e 6420 636c  ment open and cl
-00030e20: 6f73 6564 2e0a 0a20 2020 2020 2020 200a  osed...        .
-00030e30: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
-00030e40: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
-00030e50: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
-00030e60: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-00030e70: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-00030e80: 4854 4d4c 2f45 6c65 6d65 6e74 2f73 756d  HTML/Element/sum
-00030e90: 6d61 7279 290a 2020 2020 2020 2020 2222  mary).        ""
-00030ea0: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-00030eb0: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-00030ec0: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
-00030ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00030ee0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
-00030ef0: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
-00030f00: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
-00030f10: 6566 205f 6765 745f 6465 6661 756c 745f  ef _get_default_
-00030f20: 6174 7472 6962 7574 6573 2873 656c 662c  attributes(self,
-00030f30: 2067 6976 656e 3a20 6469 6374 5b73 7472   given: dict[str
-00030f40: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
-00030f50: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
-00030f60: 7474 7269 6275 7465 5479 7065 5d3a 0a20  ttributeType]:. 
-00030f70: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
-00030f80: 0a0a 0a63 6c61 7373 2073 6c6f 7428 5461  ...class slot(Ta
-00030f90: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
-00030fa0: 5061 7274 206f 6620 7468 6520 5b57 6562  Part of the [Web
-00030fb0: 2043 6f6d 706f 6e65 6e74 735d 2868 7474   Components](htt
-00030fc0: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-00030fd0: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-00030fe0: 2f64 6f63 732f 5765 622f 4150 492f 5765  /docs/Web/API/We
-00030ff0: 625f 636f 6d70 6f6e 656e 7473 2920 7465  b_components) te
-00031000: 6368 6e6f 6c6f 6779 2073 7569 7465 2c20  chnology suite, 
-00031010: 7468 6973 2065 6c65 6d65 6e74 2069 7320  this element is 
-00031020: 6120 706c 6163 6568 6f6c 6465 7220 696e  a placeholder in
-00031030: 7369 6465 2061 2077 6562 2063 6f6d 706f  side a web compo
-00031040: 6e65 6e74 2074 6861 7420 796f 7520 6361  nent that you ca
-00031050: 6e20 6669 6c6c 2077 6974 6820 796f 7572  n fill with your
-00031060: 206f 776e 206d 6172 6b75 702c 2077 6869   own markup, whi
-00031070: 6368 206c 6574 7320 796f 7520 6372 6561  ch lets you crea
-00031080: 7465 2073 6570 6172 6174 6520 444f 4d20  te separate DOM 
-00031090: 7472 6565 7320 616e 6420 7072 6573 656e  trees and presen
-000310a0: 7420 7468 656d 2074 6f67 6574 6865 722e  t them together.
-000310b0: 0a0a 2020 2020 0a0a 2020 2020 5b56 6965  ..    ..    [Vie
-000310c0: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
-000310d0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
-000310e0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
-000310f0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
-00031100: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
-00031110: 736c 6f74 290a 2020 2020 2222 220a 2020  slot).    """.  
-00031120: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00031130: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00031140: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
-00031150: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
-00031160: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00031170: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
-00031180: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
-00031190: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-000311a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000311b0: 5061 7274 206f 6620 7468 6520 5b57 6562  Part of the [Web
-000311c0: 2043 6f6d 706f 6e65 6e74 735d 2868 7474   Components](htt
-000311d0: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
-000311e0: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
-000311f0: 2f64 6f63 732f 5765 622f 4150 492f 5765  /docs/Web/API/We
-00031200: 625f 636f 6d70 6f6e 656e 7473 2920 7465  b_components) te
-00031210: 6368 6e6f 6c6f 6779 2073 7569 7465 2c20  chnology suite, 
-00031220: 7468 6973 2065 6c65 6d65 6e74 2069 7320  this element is 
-00031230: 6120 706c 6163 6568 6f6c 6465 7220 696e  a placeholder in
-00031240: 7369 6465 2061 2077 6562 2063 6f6d 706f  side a web compo
-00031250: 6e65 6e74 2074 6861 7420 796f 7520 6361  nent that you ca
-00031260: 6e20 6669 6c6c 2077 6974 6820 796f 7572  n fill with your
-00031270: 206f 776e 206d 6172 6b75 702c 2077 6869   own markup, whi
-00031280: 6368 206c 6574 7320 796f 7520 6372 6561  ch lets you crea
-00031290: 7465 2073 6570 6172 6174 6520 444f 4d20  te separate DOM 
-000312a0: 7472 6565 7320 616e 6420 7072 6573 656e  trees and presen
-000312b0: 7420 7468 656d 2074 6f67 6574 6865 722e  t them together.
-000312c0: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
-000312d0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
-000312e0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000312f0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-00031300: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
-00031310: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
-00031320: 456c 656d 656e 742f 736c 6f74 290a 2020  Element/slot).  
-00031330: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00031340: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
-00031350: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
-00031360: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00031370: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00031380: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
-00031390: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
-000313a0: 6465 6620 5f5f 6361 6c6c 5f5f 2820 2023  def __call__(  #
-000313b0: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-000313c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000313d0: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
-000313e0: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
-000313f0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00031400: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
-00031410: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
-00031420: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00031430: 2020 2020 2020 5061 7274 206f 6620 7468        Part of th
-00031440: 6520 5b57 6562 2043 6f6d 706f 6e65 6e74  e [Web Component
-00031450: 735d 2868 7474 7073 3a2f 2f64 6576 656c  s](https://devel
-00031460: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
-00031470: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
-00031480: 4150 492f 5765 625f 636f 6d70 6f6e 656e  API/Web_componen
-00031490: 7473 2920 7465 6368 6e6f 6c6f 6779 2073  ts) technology s
-000314a0: 7569 7465 2c20 7468 6973 2065 6c65 6d65  uite, this eleme
-000314b0: 6e74 2069 7320 6120 706c 6163 6568 6f6c  nt is a placehol
-000314c0: 6465 7220 696e 7369 6465 2061 2077 6562  der inside a web
-000314d0: 2063 6f6d 706f 6e65 6e74 2074 6861 7420   component that 
-000314e0: 796f 7520 6361 6e20 6669 6c6c 2077 6974  you can fill wit
-000314f0: 6820 796f 7572 206f 776e 206d 6172 6b75  h your own marku
-00031500: 702c 2077 6869 6368 206c 6574 7320 796f  p, which lets yo
-00031510: 7520 6372 6561 7465 2073 6570 6172 6174  u create separat
-00031520: 6520 444f 4d20 7472 6565 7320 616e 6420  e DOM trees and 
-00031530: 7072 6573 656e 7420 7468 656d 2074 6f67  present them tog
-00031540: 6574 6865 722e 0a0a 2020 2020 2020 2020  ether...        
-00031550: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
-00031560: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
-00031570: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
-00031580: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
-00031590: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
-000315a0: 2f48 544d 4c2f 456c 656d 656e 742f 736c  /HTML/Element/sl
-000315b0: 6f74 290a 2020 2020 2020 2020 2222 220a  ot).        """.
-000315c0: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-000315d0: 6573 207c 3d20 7b0a 2020 2020 2020 2020  es |= {.        
-000315e0: 2020 2020 0a20 2020 2020 2020 207d 0a20      .        }. 
-000315f0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00031600: 7065 7228 292e 5f5f 6361 6c6c 5f5f 282a  per().__call__(*
-00031610: 6368 696c 6472 656e 2c20 2a2a 6174 7472  children, **attr
-00031620: 6962 7574 6573 290a 0a20 2020 2064 6566  ibutes)..    def
-00031630: 205f 6765 745f 6465 6661 756c 745f 6174   _get_default_at
-00031640: 7472 6962 7574 6573 2873 656c 662c 2067  tributes(self, g
-00031650: 6976 656e 3a20 6469 6374 5b73 7472 2c20  iven: dict[str, 
-00031660: 4174 7472 6962 7574 6554 7970 655d 2920  AttributeType]) 
-00031670: 2d3e 2064 6963 745b 7374 722c 2041 7474  -> dict[str, Att
-00031680: 7269 6275 7465 5479 7065 5d3a 0a20 2020  ributeType]:.   
-00031690: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
-000316a0: 0a63 6c61 7373 2074 656d 706c 6174 6528  .class template(
-000316b0: 5461 6729 3a0a 2020 2020 2222 220a 2020  Tag):.    """.  
-000316c0: 2020 4120 6d65 6368 616e 6973 6d20 666f    A mechanism fo
-000316d0: 7220 686f 6c64 696e 6720 4854 4d4c 2074  r holding HTML t
-000316e0: 6861 7420 6973 206e 6f74 2074 6f20 6265  hat is not to be
-000316f0: 2072 656e 6465 7265 6420 696d 6d65 6469   rendered immedi
-00031700: 6174 656c 7920 7768 656e 2061 2070 6167  ately when a pag
-00031710: 6520 6973 206c 6f61 6465 6420 6275 7420  e is loaded but 
-00031720: 6d61 7920 6265 2069 6e73 7461 6e74 6961  may be instantia
-00031730: 7465 6420 7375 6273 6571 7565 6e74 6c79  ted subsequently
-00031740: 2064 7572 696e 6720 7275 6e74 696d 6520   during runtime 
-00031750: 7573 696e 6720 4a61 7661 5363 7269 7074  using JavaScript
-00031760: 2e0a 0a20 2020 200a 0a20 2020 205b 5669  ...    ..    [Vi
-00031770: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
-00031780: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00031790: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
-000317a0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
-000317b0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
-000317c0: 2f74 656d 706c 6174 6529 0a20 2020 2022  /template).    "
-000317d0: 2222 0a20 2020 2064 6566 205f 5f69 6e69  "".    def __ini
-000317e0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000317f0: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
-00031800: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
-00031810: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
-00031820: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
-00031830: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
-00031840: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00031850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00031860: 2020 2020 2041 206d 6563 6861 6e69 736d       A mechanism
-00031870: 2066 6f72 2068 6f6c 6469 6e67 2048 544d   for holding HTM
-00031880: 4c20 7468 6174 2069 7320 6e6f 7420 746f  L that is not to
-00031890: 2062 6520 7265 6e64 6572 6564 2069 6d6d   be rendered imm
-000318a0: 6564 6961 7465 6c79 2077 6865 6e20 6120  ediately when a 
-000318b0: 7061 6765 2069 7320 6c6f 6164 6564 2062  page is loaded b
-000318c0: 7574 206d 6179 2062 6520 696e 7374 616e  ut may be instan
-000318d0: 7469 6174 6564 2073 7562 7365 7175 656e  tiated subsequen
-000318e0: 746c 7920 6475 7269 6e67 2072 756e 7469  tly during runti
-000318f0: 6d65 2075 7369 6e67 204a 6176 6153 6372  me using JavaScr
-00031900: 6970 742e 0a0a 2020 2020 2020 2020 0a0a  ipt...        ..
-00031910: 2020 2020 2020 2020 5b56 6965 7720 6675          [View fu
-00031920: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
-00031930: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00031940: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
-00031950: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
-00031960: 544d 4c2f 456c 656d 656e 742f 7465 6d70  TML/Element/temp
-00031970: 6c61 7465 290a 2020 2020 2020 2020 2222  late).        ""
-00031980: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
-00031990: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
-000319a0: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
-000319b0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-000319c0: 2e5f 5f69 6e69 745f 5f28 2a63 6869 6c64  .__init__(*child
-000319d0: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
-000319e0: 7329 0a0a 2020 2020 6465 6620 5f5f 6361  s)..    def __ca
-000319f0: 6c6c 5f5f 2820 2023 2074 7970 653a 2069  ll__(  # type: i
-00031a00: 676e 6f72 650a 2020 2020 2020 2020 7365  gnore.        se
-00031a10: 6c66 2c0a 2020 2020 2020 2020 2a63 6869  lf,.        *chi
-00031a20: 6c64 7265 6e3a 2043 6869 6c64 7265 6e54  ldren: ChildrenT
-00031a30: 7970 652c 0a20 2020 2020 2020 200a 2020  ype,.        .  
-00031a40: 2020 2020 2020 2a2a 6174 7472 6962 7574        **attribut
-00031a50: 6573 3a20 4174 7472 6962 7574 6554 7970  es: AttributeTyp
-00031a60: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00031a70: 2020 2222 220a 2020 2020 2020 2020 4120    """.        A 
-00031a80: 6d65 6368 616e 6973 6d20 666f 7220 686f  mechanism for ho
-00031a90: 6c64 696e 6720 4854 4d4c 2074 6861 7420  lding HTML that 
-00031aa0: 6973 206e 6f74 2074 6f20 6265 2072 656e  is not to be ren
-00031ab0: 6465 7265 6420 696d 6d65 6469 6174 656c  dered immediatel
-00031ac0: 7920 7768 656e 2061 2070 6167 6520 6973  y when a page is
-00031ad0: 206c 6f61 6465 6420 6275 7420 6d61 7920   loaded but may 
-00031ae0: 6265 2069 6e73 7461 6e74 6961 7465 6420  be instantiated 
-00031af0: 7375 6273 6571 7565 6e74 6c79 2064 7572  subsequently dur
-00031b00: 696e 6720 7275 6e74 696d 6520 7573 696e  ing runtime usin
-00031b10: 6720 4a61 7661 5363 7269 7074 2e0a 0a20  g JavaScript... 
-00031b20: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-00031b30: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
-00031b40: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00031b50: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
-00031b60: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
-00031b70: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
-00031b80: 6d65 6e74 2f74 656d 706c 6174 6529 0a20  ment/template). 
-00031b90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00031ba0: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
-00031bb0: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
-00031bc0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00031bd0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00031be0: 2e5f 5f63 616c 6c5f 5f28 2a63 6869 6c64  .__call__(*child
-00031bf0: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
-00031c00: 7329 0a0a 2020 2020 6465 6620 5f67 6574  s)..    def _get
-00031c10: 5f64 6566 6175 6c74 5f61 7474 7269 6275  _default_attribu
-00031c20: 7465 7328 7365 6c66 2c20 6769 7665 6e3a  tes(self, given:
-00031c30: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
-00031c40: 6275 7465 5479 7065 5d29 202d 3e20 6469  buteType]) -> di
-00031c50: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
-00031c60: 6554 7970 655d 3a0a 2020 2020 2020 2020  eType]:.        
-00031c70: 7265 7475 726e 207b 7d0a 0a0a 5f5f 616c  return {}...__al
-00031c80: 6c5f 5f20 3d20 5b0a 2020 2020 2768 746d  l__ = [.    'htm
-00031c90: 6c27 2c0a 2020 2020 2762 6173 6527 2c0a  l',.    'base',.
-00031ca0: 2020 2020 2768 6561 6427 2c0a 2020 2020      'head',.    
-00031cb0: 276c 696e 6b27 2c0a 2020 2020 276d 6574  'link',.    'met
-00031cc0: 6127 2c0a 2020 2020 2773 7479 6c65 272c  a',.    'style',
-00031cd0: 0a20 2020 2027 7469 746c 6527 2c0a 2020  .    'title',.  
-00031ce0: 2020 2762 6f64 7927 2c0a 2020 2020 2761    'body',.    'a
-00031cf0: 6464 7265 7373 272c 0a20 2020 2027 6172  ddress',.    'ar
-00031d00: 7469 636c 6527 2c0a 2020 2020 2761 7369  ticle',.    'asi
-00031d10: 6465 272c 0a20 2020 2027 666f 6f74 6572  de',.    'footer
-00031d20: 272c 0a20 2020 2027 6865 6164 6572 272c  ',.    'header',
-00031d30: 0a20 2020 2027 6831 272c 0a20 2020 2027  .    'h1',.    '
-00031d40: 6832 272c 0a20 2020 2027 6833 272c 0a20  h2',.    'h3',. 
-00031d50: 2020 2027 6834 272c 0a20 2020 2027 6835     'h4',.    'h5
-00031d60: 272c 0a20 2020 2027 6836 272c 0a20 2020  ',.    'h6',.   
-00031d70: 2027 6867 726f 7570 272c 0a20 2020 2027   'hgroup',.    '
-00031d80: 6d61 696e 272c 0a20 2020 2027 6e61 7627  main',.    'nav'
-00031d90: 2c0a 2020 2020 2773 6563 7469 6f6e 272c  ,.    'section',
-00031da0: 0a20 2020 2027 7365 6172 6368 272c 0a20  .    'search',. 
-00031db0: 2020 2027 626c 6f63 6b71 756f 7465 272c     'blockquote',
-00031dc0: 0a20 2020 2027 6464 272c 0a20 2020 2027  .    'dd',.    '
-00031dd0: 6469 7627 2c0a 2020 2020 2764 6c27 2c0a  div',.    'dl',.
-00031de0: 2020 2020 2764 7427 2c0a 2020 2020 2766      'dt',.    'f
-00031df0: 6967 6361 7074 696f 6e27 2c0a 2020 2020  igcaption',.    
-00031e00: 2766 6967 7572 6527 2c0a 2020 2020 2768  'figure',.    'h
-00031e10: 7227 2c0a 2020 2020 276c 6927 2c0a 2020  r',.    'li',.  
-00031e20: 2020 276d 656e 7527 2c0a 2020 2020 276f    'menu',.    'o
-00031e30: 6c27 2c0a 2020 2020 2770 272c 0a20 2020  l',.    'p',.   
-00031e40: 2027 7072 6527 2c0a 2020 2020 2775 6c27   'pre',.    'ul'
-00031e50: 2c0a 2020 2020 2761 272c 0a20 2020 2027  ,.    'a',.    '
-00031e60: 6162 6272 272c 0a20 2020 2027 6227 2c0a  abbr',.    'b',.
-00031e70: 2020 2020 2762 6469 272c 0a20 2020 2027      'bdi',.    '
-00031e80: 6264 6f27 2c0a 2020 2020 2762 7227 2c0a  bdo',.    'br',.
-00031e90: 2020 2020 2763 6974 6527 2c0a 2020 2020      'cite',.    
-00031ea0: 2763 6f64 6527 2c0a 2020 2020 2764 6174  'code',.    'dat
-00031eb0: 6127 2c0a 2020 2020 2764 666e 272c 0a20  a',.    'dfn',. 
-00031ec0: 2020 2027 656d 272c 0a20 2020 2027 6927     'em',.    'i'
-00031ed0: 2c0a 2020 2020 276b 6264 272c 0a20 2020  ,.    'kbd',.   
-00031ee0: 2027 6d61 726b 272c 0a20 2020 2027 7127   'mark',.    'q'
-00031ef0: 2c0a 2020 2020 2772 7027 2c0a 2020 2020  ,.    'rp',.    
-00031f00: 2772 7427 2c0a 2020 2020 2772 7562 7927  'rt',.    'ruby'
-00031f10: 2c0a 2020 2020 2773 272c 0a20 2020 2027  ,.    's',.    '
-00031f20: 7361 6d70 272c 0a20 2020 2027 736d 616c  samp',.    'smal
-00031f30: 6c27 2c0a 2020 2020 2773 7061 6e27 2c0a  l',.    'span',.
-00031f40: 2020 2020 2773 7472 6f6e 6727 2c0a 2020      'strong',.  
-00031f50: 2020 2773 7562 272c 0a20 2020 2027 7375    'sub',.    'su
-00031f60: 7027 2c0a 2020 2020 2774 696d 6527 2c0a  p',.    'time',.
-00031f70: 2020 2020 2775 272c 0a20 2020 2027 7661      'u',.    'va
-00031f80: 7227 2c0a 2020 2020 2777 6272 272c 0a20  r',.    'wbr',. 
-00031f90: 2020 2027 6172 6561 272c 0a20 2020 2027     'area',.    '
-00031fa0: 6175 6469 6f27 2c0a 2020 2020 2769 6d67  audio',.    'img
-00031fb0: 272c 0a20 2020 2027 6d61 7027 2c0a 2020  ',.    'map',.  
-00031fc0: 2020 2774 7261 636b 272c 0a20 2020 2027    'track',.    '
-00031fd0: 7669 6465 6f27 2c0a 2020 2020 2765 6d62  video',.    'emb
-00031fe0: 6564 272c 0a20 2020 2027 6966 7261 6d65  ed',.    'iframe
-00031ff0: 272c 0a20 2020 2027 6f62 6a65 6374 272c  ',.    'object',
-00032000: 0a20 2020 2027 7069 6374 7572 6527 2c0a  .    'picture',.
-00032010: 2020 2020 2770 6f72 7461 6c27 2c0a 2020      'portal',.  
-00032020: 2020 2773 6f75 7263 6527 2c0a 2020 2020    'source',.    
-00032030: 2763 616e 7661 7327 2c0a 2020 2020 276e  'canvas',.    'n
-00032040: 6f73 6372 6970 7427 2c0a 2020 2020 2773  oscript',.    's
-00032050: 6372 6970 7427 2c0a 2020 2020 2764 656c  cript',.    'del
-00032060: 5f27 2c0a 2020 2020 2769 6e73 272c 0a20  _',.    'ins',. 
-00032070: 2020 2027 6361 7074 696f 6e27 2c0a 2020     'caption',.  
-00032080: 2020 2763 6f6c 272c 0a20 2020 2027 636f    'col',.    'co
-00032090: 6c67 726f 7570 272c 0a20 2020 2027 7461  lgroup',.    'ta
-000320a0: 626c 6527 2c0a 2020 2020 2774 626f 6479  ble',.    'tbody
-000320b0: 272c 0a20 2020 2027 7464 272c 0a20 2020  ',.    'td',.   
-000320c0: 2027 7466 6f6f 7427 2c0a 2020 2020 2774   'tfoot',.    't
-000320d0: 6827 2c0a 2020 2020 2774 6865 6164 272c  h',.    'thead',
-000320e0: 0a20 2020 2027 7472 272c 0a20 2020 2027  .    'tr',.    '
-000320f0: 6275 7474 6f6e 272c 0a20 2020 2027 6461  button',.    'da
-00032100: 7461 6c69 7374 272c 0a20 2020 2027 6669  talist',.    'fi
-00032110: 656c 6473 6574 272c 0a20 2020 2027 666f  eldset',.    'fo
-00032120: 726d 272c 0a20 2020 2027 6c61 6265 6c27  rm',.    'label'
-00032130: 2c0a 2020 2020 276c 6567 656e 6427 2c0a  ,.    'legend',.
-00032140: 2020 2020 276d 6574 6572 272c 0a20 2020      'meter',.   
-00032150: 2027 6f70 7467 726f 7570 272c 0a20 2020   'optgroup',.   
-00032160: 2027 6f70 7469 6f6e 272c 0a20 2020 2027   'option',.    '
-00032170: 6f75 7470 7574 272c 0a20 2020 2027 7072  output',.    'pr
-00032180: 6f67 7265 7373 272c 0a20 2020 2027 7365  ogress',.    'se
-00032190: 6c65 6374 272c 0a20 2020 2027 7465 7874  lect',.    'text
-000321a0: 6172 6561 272c 0a20 2020 2027 6465 7461  area',.    'deta
-000321b0: 696c 7327 2c0a 2020 2020 2764 6961 6c6f  ils',.    'dialo
-000321c0: 6727 2c0a 2020 2020 2773 756d 6d61 7279  g',.    'summary
-000321d0: 272c 0a20 2020 2027 736c 6f74 272c 0a20  ',.    'slot',. 
-000321e0: 2020 2027 7465 6d70 6c61 7465 272c 0a5d     'template',.]
-000321f0: 0a                                       .
+00024c40: 0a0a 0a20 2020 2064 6566 205f 6573 6361  ...    def _esca
+00024c50: 7065 5f63 6869 6c64 7265 6e28 7365 6c66  pe_children(self
+00024c60: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00024c70: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00024c80: 0a0a 636c 6173 7320 6465 6c5f 2854 6167  ..class del_(Tag
+00024c90: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+00024ca0: 6570 7265 7365 6e74 7320 6120 7261 6e67  epresents a rang
+00024cb0: 6520 6f66 2074 6578 7420 7468 6174 2068  e of text that h
+00024cc0: 6173 2062 6565 6e20 6465 6c65 7465 6420  as been deleted 
+00024cd0: 6672 6f6d 2061 2064 6f63 756d 656e 742e  from a document.
+00024ce0: 2054 6869 7320 6361 6e20 6265 2075 7365   This can be use
+00024cf0: 6420 7768 656e 2072 656e 6465 7269 6e67  d when rendering
+00024d00: 2022 7472 6163 6b20 6368 616e 6765 7322   "track changes"
+00024d10: 206f 7220 736f 7572 6365 2063 6f64 6520   or source code 
+00024d20: 6469 6666 2069 6e66 6f72 6d61 7469 6f6e  diff information
+00024d30: 2c20 666f 7220 6578 616d 706c 652e 2054  , for example. T
+00024d40: 6865 2060 3c69 6e73 3e60 2065 6c65 6d65  he `<ins>` eleme
+00024d50: 6e74 2063 616e 2062 6520 7573 6564 2066  nt can be used f
+00024d60: 6f72 2074 6865 206f 7070 6f73 6974 6520  or the opposite 
+00024d70: 7075 7270 6f73 653a 2074 6f20 696e 6469  purpose: to indi
+00024d80: 6361 7465 2074 6578 7420 7468 6174 2068  cate text that h
+00024d90: 6173 2062 6565 6e20 6164 6465 6420 746f  as been added to
+00024da0: 2074 6865 2064 6f63 756d 656e 742e 0a0a   the document...
+00024db0: 2020 2020 0a0a 2020 2020 5b56 6965 7720      ..    [View 
+00024dc0: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+00024dd0: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+00024de0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+00024df0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+00024e00: 2f48 544d 4c2f 456c 656d 656e 742f 6465  /HTML/Element/de
+00024e10: 6c29 0a20 2020 2022 2222 0a20 2020 2064  l).    """.    d
+00024e20: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00024e30: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00024e40: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+00024e50: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+00024e60: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+00024e70: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+00024e80: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
+00024e90: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00024ea0: 2022 2222 0a20 2020 2020 2020 2052 6570   """.        Rep
+00024eb0: 7265 7365 6e74 7320 6120 7261 6e67 6520  resents a range 
+00024ec0: 6f66 2074 6578 7420 7468 6174 2068 6173  of text that has
+00024ed0: 2062 6565 6e20 6465 6c65 7465 6420 6672   been deleted fr
+00024ee0: 6f6d 2061 2064 6f63 756d 656e 742e 2054  om a document. T
+00024ef0: 6869 7320 6361 6e20 6265 2075 7365 6420  his can be used 
+00024f00: 7768 656e 2072 656e 6465 7269 6e67 2022  when rendering "
+00024f10: 7472 6163 6b20 6368 616e 6765 7322 206f  track changes" o
+00024f20: 7220 736f 7572 6365 2063 6f64 6520 6469  r source code di
+00024f30: 6666 2069 6e66 6f72 6d61 7469 6f6e 2c20  ff information, 
+00024f40: 666f 7220 6578 616d 706c 652e 2054 6865  for example. The
+00024f50: 2060 3c69 6e73 3e60 2065 6c65 6d65 6e74   `<ins>` element
+00024f60: 2063 616e 2062 6520 7573 6564 2066 6f72   can be used for
+00024f70: 2074 6865 206f 7070 6f73 6974 6520 7075   the opposite pu
+00024f80: 7270 6f73 653a 2074 6f20 696e 6469 6361  rpose: to indica
+00024f90: 7465 2074 6578 7420 7468 6174 2068 6173  te text that has
+00024fa0: 2062 6565 6e20 6164 6465 6420 746f 2074   been added to t
+00024fb0: 6865 2064 6f63 756d 656e 742e 0a0a 2020  he document...  
+00024fc0: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
+00024fd0: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+00024fe0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00024ff0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+00025000: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00025010: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+00025020: 656e 742f 6465 6c29 0a20 2020 2020 2020  ent/del).       
+00025030: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
+00025040: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
+00025050: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00025060: 2020 7d0a 2020 2020 2020 2020 7375 7065    }.        supe
+00025070: 7228 292e 5f5f 696e 6974 5f5f 282a 6368  r().__init__(*ch
+00025080: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
+00025090: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
+000250a0: 5f63 616c 6c5f 5f28 2020 2320 7479 7065  _call__(  # type
+000250b0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+000250c0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+000250d0: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
+000250e0: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
+000250f0: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
+00025100: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
+00025110: 5479 7065 2c0a 2020 2020 293a 0a20 2020  Type,.    ):.   
+00025120: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00025130: 2052 6570 7265 7365 6e74 7320 6120 7261   Represents a ra
+00025140: 6e67 6520 6f66 2074 6578 7420 7468 6174  nge of text that
+00025150: 2068 6173 2062 6565 6e20 6465 6c65 7465   has been delete
+00025160: 6420 6672 6f6d 2061 2064 6f63 756d 656e  d from a documen
+00025170: 742e 2054 6869 7320 6361 6e20 6265 2075  t. This can be u
+00025180: 7365 6420 7768 656e 2072 656e 6465 7269  sed when renderi
+00025190: 6e67 2022 7472 6163 6b20 6368 616e 6765  ng "track change
+000251a0: 7322 206f 7220 736f 7572 6365 2063 6f64  s" or source cod
+000251b0: 6520 6469 6666 2069 6e66 6f72 6d61 7469  e diff informati
+000251c0: 6f6e 2c20 666f 7220 6578 616d 706c 652e  on, for example.
+000251d0: 2054 6865 2060 3c69 6e73 3e60 2065 6c65   The `<ins>` ele
+000251e0: 6d65 6e74 2063 616e 2062 6520 7573 6564  ment can be used
+000251f0: 2066 6f72 2074 6865 206f 7070 6f73 6974   for the opposit
+00025200: 6520 7075 7270 6f73 653a 2074 6f20 696e  e purpose: to in
+00025210: 6469 6361 7465 2074 6578 7420 7468 6174  dicate text that
+00025220: 2068 6173 2062 6565 6e20 6164 6465 6420   has been added 
+00025230: 746f 2074 6865 2064 6f63 756d 656e 742e  to the document.
+00025240: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
+00025250: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
+00025260: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00025270: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+00025280: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+00025290: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+000252a0: 456c 656d 656e 742f 6465 6c29 0a20 2020  Element/del).   
+000252b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000252c0: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+000252d0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000252e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000252f0: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
+00025300: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
+00025310: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
+00025320: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
+00025330: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
+00025340: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
+00025350: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
+00025360: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
+00025370: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
+00025380: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
+00025390: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
+000253a0: 696e 7328 5461 6729 3a0a 2020 2020 2222  ins(Tag):.    ""
+000253b0: 220a 2020 2020 5265 7072 6573 656e 7473  ".    Represents
+000253c0: 2061 2072 616e 6765 206f 6620 7465 7874   a range of text
+000253d0: 2074 6861 7420 6861 7320 6265 656e 2061   that has been a
+000253e0: 6464 6564 2074 6f20 6120 646f 6375 6d65  dded to a docume
+000253f0: 6e74 2e20 596f 7520 6361 6e20 7573 6520  nt. You can use 
+00025400: 7468 6520 603c 6465 6c3e 6020 656c 656d  the `<del>` elem
+00025410: 656e 7420 746f 2073 696d 696c 6172 6c79  ent to similarly
+00025420: 2072 6570 7265 7365 6e74 2061 2072 616e   represent a ran
+00025430: 6765 206f 6620 7465 7874 2074 6861 7420  ge of text that 
+00025440: 6861 7320 6265 656e 2064 656c 6574 6564  has been deleted
+00025450: 2066 726f 6d20 7468 6520 646f 6375 6d65   from the docume
+00025460: 6e74 2e0a 0a20 2020 200a 0a20 2020 205b  nt...    ..    [
+00025470: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
+00025480: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00025490: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+000254a0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+000254b0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+000254c0: 6e74 2f69 6e73 290a 2020 2020 2222 220a  nt/ins).    """.
+000254d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000254e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000254f0: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+00025500: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+00025510: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00025520: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+00025530: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+00025540: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00025550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00025560: 2020 5265 7072 6573 656e 7473 2061 2072    Represents a r
+00025570: 616e 6765 206f 6620 7465 7874 2074 6861  ange of text tha
+00025580: 7420 6861 7320 6265 656e 2061 6464 6564  t has been added
+00025590: 2074 6f20 6120 646f 6375 6d65 6e74 2e20   to a document. 
+000255a0: 596f 7520 6361 6e20 7573 6520 7468 6520  You can use the 
+000255b0: 603c 6465 6c3e 6020 656c 656d 656e 7420  `<del>` element 
+000255c0: 746f 2073 696d 696c 6172 6c79 2072 6570  to similarly rep
+000255d0: 7265 7365 6e74 2061 2072 616e 6765 206f  resent a range o
+000255e0: 6620 7465 7874 2074 6861 7420 6861 7320  f text that has 
+000255f0: 6265 656e 2064 656c 6574 6564 2066 726f  been deleted fro
+00025600: 6d20 7468 6520 646f 6375 6d65 6e74 2e0a  m the document..
+00025610: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
+00025620: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+00025630: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00025640: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+00025650: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+00025660: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+00025670: 6c65 6d65 6e74 2f69 6e73 290a 2020 2020  lement/ins).    
+00025680: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00025690: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+000256a0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+000256b0: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
+000256c0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+000256d0: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
+000256e0: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+000256f0: 6620 5f5f 6361 6c6c 5f5f 2820 2023 2074  f __call__(  # t
+00025700: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+00025710: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00025720: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+00025730: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+00025740: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+00025750: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+00025760: 7574 6554 7970 652c 0a20 2020 2029 3a0a  uteType,.    ):.
+00025770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00025780: 2020 2020 5265 7072 6573 656e 7473 2061      Represents a
+00025790: 2072 616e 6765 206f 6620 7465 7874 2074   range of text t
+000257a0: 6861 7420 6861 7320 6265 656e 2061 6464  hat has been add
+000257b0: 6564 2074 6f20 6120 646f 6375 6d65 6e74  ed to a document
+000257c0: 2e20 596f 7520 6361 6e20 7573 6520 7468  . You can use th
+000257d0: 6520 603c 6465 6c3e 6020 656c 656d 656e  e `<del>` elemen
+000257e0: 7420 746f 2073 696d 696c 6172 6c79 2072  t to similarly r
+000257f0: 6570 7265 7365 6e74 2061 2072 616e 6765  epresent a range
+00025800: 206f 6620 7465 7874 2074 6861 7420 6861   of text that ha
+00025810: 7320 6265 656e 2064 656c 6574 6564 2066  s been deleted f
+00025820: 726f 6d20 7468 6520 646f 6375 6d65 6e74  rom the document
+00025830: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
+00025840: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
+00025850: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+00025860: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00025870: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00025880: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00025890: 2f45 6c65 6d65 6e74 2f69 6e73 290a 2020  /Element/ins).  
+000258a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000258b0: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
+000258c0: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
+000258d0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000258e0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+000258f0: 5f5f 6361 6c6c 5f5f 282a 6368 696c 6472  __call__(*childr
+00025900: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
+00025910: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
+00025920: 6465 6661 756c 745f 6174 7472 6962 7574  default_attribut
+00025930: 6573 2873 656c 662c 2067 6976 656e 3a20  es(self, given: 
+00025940: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
+00025950: 7574 6554 7970 655d 2920 2d3e 2064 6963  uteType]) -> dic
+00025960: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
+00025970: 5479 7065 5d3a 0a20 2020 2020 2020 2072  Type]:.        r
+00025980: 6574 7572 6e20 7b7d 0a0a 0a63 6c61 7373  eturn {}...class
+00025990: 2063 6170 7469 6f6e 2854 6167 293a 0a20   caption(Tag):. 
+000259a0: 2020 2022 2222 0a20 2020 2053 7065 6369     """.    Speci
+000259b0: 6669 6573 2074 6865 2063 6170 7469 6f6e  fies the caption
+000259c0: 2028 6f72 2074 6974 6c65 2920 6f66 2061   (or title) of a
+000259d0: 2074 6162 6c65 2e0a 0a20 2020 200a 0a20   table...    .. 
+000259e0: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+000259f0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00025a00: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+00025a10: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+00025a20: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+00025a30: 6c65 6d65 6e74 2f63 6170 7469 6f6e 290a  lement/caption).
+00025a40: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00025a50: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00025a60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00025a70: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
+00025a80: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
+00025a90: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
+00025aa0: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
+00025ab0: 6554 7970 652c 0a20 2020 2029 202d 3e20  eType,.    ) -> 
+00025ac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00025ad0: 220a 2020 2020 2020 2020 5370 6563 6966  ".        Specif
+00025ae0: 6965 7320 7468 6520 6361 7074 696f 6e20  ies the caption 
+00025af0: 286f 7220 7469 746c 6529 206f 6620 6120  (or title) of a 
+00025b00: 7461 626c 652e 0a0a 2020 2020 2020 2020  table...        
+00025b10: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+00025b20: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+00025b30: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+00025b40: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+00025b50: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+00025b60: 2f48 544d 4c2f 456c 656d 656e 742f 6361  /HTML/Element/ca
+00025b70: 7074 696f 6e29 0a20 2020 2020 2020 2022  ption).        "
+00025b80: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
+00025b90: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
+00025ba0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00025bb0: 7d0a 2020 2020 2020 2020 7375 7065 7228  }.        super(
+00025bc0: 292e 5f5f 696e 6974 5f5f 282a 6368 696c  ).__init__(*chil
+00025bd0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
+00025be0: 6573 290a 0a20 2020 2064 6566 205f 5f63  es)..    def __c
+00025bf0: 616c 6c5f 5f28 2020 2320 7479 7065 3a20  all__(  # type: 
+00025c00: 6967 6e6f 7265 0a20 2020 2020 2020 2073  ignore.        s
+00025c10: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
+00025c20: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
+00025c30: 5479 7065 2c0a 2020 2020 2020 2020 0a20  Type,.        . 
+00025c40: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
+00025c50: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
+00025c60: 7065 2c0a 2020 2020 293a 0a20 2020 2020  pe,.    ):.     
+00025c70: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00025c80: 7065 6369 6669 6573 2074 6865 2063 6170  pecifies the cap
+00025c90: 7469 6f6e 2028 6f72 2074 6974 6c65 2920  tion (or title) 
+00025ca0: 6f66 2061 2074 6162 6c65 2e0a 0a20 2020  of a table...   
+00025cb0: 2020 2020 200a 0a20 2020 2020 2020 205b       ..        [
+00025cc0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
+00025cd0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00025ce0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+00025cf0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+00025d00: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+00025d10: 6e74 2f63 6170 7469 6f6e 290a 2020 2020  nt/caption).    
+00025d20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00025d30: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+00025d40: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00025d50: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+00025d60: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+00025d70: 6361 6c6c 5f5f 282a 6368 696c 6472 656e  call__(*children
+00025d80: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
+00025d90: 0a20 2020 2064 6566 205f 6765 745f 6465  .    def _get_de
+00025da0: 6661 756c 745f 6174 7472 6962 7574 6573  fault_attributes
+00025db0: 2873 656c 662c 2067 6976 656e 3a20 6469  (self, given: di
+00025dc0: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
+00025dd0: 6554 7970 655d 2920 2d3e 2064 6963 745b  eType]) -> dict[
+00025de0: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
+00025df0: 7065 5d3a 0a20 2020 2020 2020 2072 6574  pe]:.        ret
+00025e00: 7572 6e20 7b7d 0a0a 0a63 6c61 7373 2063  urn {}...class c
+00025e10: 6f6c 2854 6167 293a 0a20 2020 2022 2222  ol(Tag):.    """
+00025e20: 0a20 2020 2044 6566 696e 6573 206f 6e65  .    Defines one
+00025e30: 206f 7220 6d6f 7265 2063 6f6c 756d 6e73   or more columns
+00025e40: 2069 6e20 6120 636f 6c75 6d6e 2067 726f   in a column gro
+00025e50: 7570 2072 6570 7265 7365 6e74 6564 2062  up represented b
+00025e60: 7920 6974 7320 696d 706c 6963 6974 206f  y its implicit o
+00025e70: 7220 6578 706c 6963 6974 2070 6172 656e  r explicit paren
+00025e80: 7420 5b60 3c63 6f6c 6772 6f75 703e 605d  t [`<colgroup>`]
+00025e90: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+00025ea0: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+00025eb0: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+00025ec0: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 6772  ML/Element/colgr
+00025ed0: 6f75 7029 2065 6c65 6d65 6e74 2e20 5468  oup) element. Th
+00025ee0: 6520 603c 636f 6c3e 6020 656c 656d 656e  e `<col>` elemen
+00025ef0: 7420 6973 206f 6e6c 7920 7661 6c69 6420  t is only valid 
+00025f00: 6173 2061 2063 6869 6c64 206f 6620 6120  as a child of a 
+00025f10: 5b60 3c63 6f6c 6772 6f75 703e 605d 2868  [`<colgroup>`](h
+00025f20: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00025f30: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00025f40: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00025f50: 2f45 6c65 6d65 6e74 2f63 6f6c 6772 6f75  /Element/colgrou
+00025f60: 7029 2065 6c65 6d65 6e74 2074 6861 7420  p) element that 
+00025f70: 6861 7320 6e6f 205b 6073 7061 6e60 5d28  has no [`span`](
+00025f80: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00025f90: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00025fa0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00025fb0: 4c2f 456c 656d 656e 742f 636f 6c67 726f  L/Element/colgro
+00025fc0: 7570 2373 7061 6e29 2061 7474 7269 6275  up#span) attribu
+00025fd0: 7465 2064 6566 696e 6564 2e0a 0a20 2020  te defined...   
+00025fe0: 200a 0a20 2020 205b 5669 6577 2066 756c   ..    [View ful
+00025ff0: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00026000: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+00026010: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+00026020: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+00026030: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 290a  ML/Element/col).
+00026040: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00026050: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00026060: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00026070: 2a63 6869 6c64 7265 6e3a 2043 6869 6c64  *children: Child
+00026080: 7265 6e54 7970 652c 0a20 2020 2020 2020  renType,.       
+00026090: 200a 2020 2020 2020 2020 2a2a 6174 7472   .        **attr
+000260a0: 6962 7574 6573 3a20 4174 7472 6962 7574  ibutes: Attribut
+000260b0: 6554 7970 652c 0a20 2020 2029 202d 3e20  eType,.    ) -> 
+000260c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000260d0: 220a 2020 2020 2020 2020 4465 6669 6e65  ".        Define
+000260e0: 7320 6f6e 6520 6f72 206d 6f72 6520 636f  s one or more co
+000260f0: 6c75 6d6e 7320 696e 2061 2063 6f6c 756d  lumns in a colum
+00026100: 6e20 6772 6f75 7020 7265 7072 6573 656e  n group represen
+00026110: 7465 6420 6279 2069 7473 2069 6d70 6c69  ted by its impli
+00026120: 6369 7420 6f72 2065 7870 6c69 6369 7420  cit or explicit 
+00026130: 7061 7265 6e74 205b 603c 636f 6c67 726f  parent [`<colgro
+00026140: 7570 3e60 5d28 6874 7470 733a 2f2f 6465  up>`](https://de
+00026150: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+00026160: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+00026170: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00026180: 636f 6c67 726f 7570 2920 656c 656d 656e  colgroup) elemen
+00026190: 742e 2054 6865 2060 3c63 6f6c 3e60 2065  t. The `<col>` e
+000261a0: 6c65 6d65 6e74 2069 7320 6f6e 6c79 2076  lement is only v
+000261b0: 616c 6964 2061 7320 6120 6368 696c 6420  alid as a child 
+000261c0: 6f66 2061 205b 603c 636f 6c67 726f 7570  of a [`<colgroup
+000261d0: 3e60 5d28 6874 7470 733a 2f2f 6465 7665  >`](https://deve
+000261e0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+000261f0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+00026200: 2f48 544d 4c2f 456c 656d 656e 742f 636f  /HTML/Element/co
+00026210: 6c67 726f 7570 2920 656c 656d 656e 7420  lgroup) element 
+00026220: 7468 6174 2068 6173 206e 6f20 5b60 7370  that has no [`sp
+00026230: 616e 605d 2868 7474 7073 3a2f 2f64 6576  an`](https://dev
+00026240: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+00026250: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+00026260: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f63  b/HTML/Element/c
+00026270: 6f6c 6772 6f75 7023 7370 616e 2920 6174  olgroup#span) at
+00026280: 7472 6962 7574 6520 6465 6669 6e65 642e  tribute defined.
+00026290: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
+000262a0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
+000262b0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+000262c0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+000262d0: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+000262e0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+000262f0: 456c 656d 656e 742f 636f 6c29 0a20 2020  Element/col).   
+00026300: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00026310: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+00026320: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00026330: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00026340: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00026350: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
+00026360: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
+00026370: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
+00026380: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00026390: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000263a0: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+000263b0: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+000263c0: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+000263d0: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+000263e0: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
+000263f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00026400: 2020 2020 2044 6566 696e 6573 206f 6e65       Defines one
+00026410: 206f 7220 6d6f 7265 2063 6f6c 756d 6e73   or more columns
+00026420: 2069 6e20 6120 636f 6c75 6d6e 2067 726f   in a column gro
+00026430: 7570 2072 6570 7265 7365 6e74 6564 2062  up represented b
+00026440: 7920 6974 7320 696d 706c 6963 6974 206f  y its implicit o
+00026450: 7220 6578 706c 6963 6974 2070 6172 656e  r explicit paren
+00026460: 7420 5b60 3c63 6f6c 6772 6f75 703e 605d  t [`<colgroup>`]
+00026470: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+00026480: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+00026490: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+000264a0: 4d4c 2f45 6c65 6d65 6e74 2f63 6f6c 6772  ML/Element/colgr
+000264b0: 6f75 7029 2065 6c65 6d65 6e74 2e20 5468  oup) element. Th
+000264c0: 6520 603c 636f 6c3e 6020 656c 656d 656e  e `<col>` elemen
+000264d0: 7420 6973 206f 6e6c 7920 7661 6c69 6420  t is only valid 
+000264e0: 6173 2061 2063 6869 6c64 206f 6620 6120  as a child of a 
+000264f0: 5b60 3c63 6f6c 6772 6f75 703e 605d 2868  [`<colgroup>`](h
+00026500: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00026510: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00026520: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00026530: 2f45 6c65 6d65 6e74 2f63 6f6c 6772 6f75  /Element/colgrou
+00026540: 7029 2065 6c65 6d65 6e74 2074 6861 7420  p) element that 
+00026550: 6861 7320 6e6f 205b 6073 7061 6e60 5d28  has no [`span`](
+00026560: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00026570: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00026580: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00026590: 4c2f 456c 656d 656e 742f 636f 6c67 726f  L/Element/colgro
+000265a0: 7570 2373 7061 6e29 2061 7474 7269 6275  up#span) attribu
+000265b0: 7465 2064 6566 696e 6564 2e0a 0a20 2020  te defined...   
+000265c0: 2020 2020 200a 0a20 2020 2020 2020 205b       ..        [
+000265d0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
+000265e0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+000265f0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+00026600: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+00026610: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+00026620: 6e74 2f63 6f6c 290a 2020 2020 2020 2020  nt/col).        
+00026630: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+00026640: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+00026650: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00026660: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+00026670: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
+00026680: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+00026690: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+000266a0: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
+000266b0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
+000266c0: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
+000266d0: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
+000266e0: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
+000266f0: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
+00026700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00026710: 7b7d 0a0a 0a63 6c61 7373 2063 6f6c 6772  {}...class colgr
+00026720: 6f75 7028 5461 6729 3a0a 2020 2020 2222  oup(Tag):.    ""
+00026730: 220a 2020 2020 4465 6669 6e65 7320 6120  ".    Defines a 
+00026740: 6772 6f75 7020 6f66 2063 6f6c 756d 6e73  group of columns
+00026750: 2077 6974 6869 6e20 6120 7461 626c 652e   within a table.
+00026760: 0a0a 2020 2020 0a0a 2020 2020 5b56 6965  ..    ..    [Vie
+00026770: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+00026780: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+00026790: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+000267a0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+000267b0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+000267c0: 636f 6c67 726f 7570 290a 2020 2020 2222  colgroup).    ""
+000267d0: 220a 2020 2020 6465 6620 5f5f 696e 6974  ".    def __init
+000267e0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000267f0: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
+00026800: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
+00026810: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
+00026820: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
+00026830: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
+00026840: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+00026850: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00026860: 2020 2020 4465 6669 6e65 7320 6120 6772      Defines a gr
+00026870: 6f75 7020 6f66 2063 6f6c 756d 6e73 2077  oup of columns w
+00026880: 6974 6869 6e20 6120 7461 626c 652e 0a0a  ithin a table...
+00026890: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
+000268a0: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
+000268b0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000268c0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+000268d0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+000268e0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+000268f0: 656d 656e 742f 636f 6c67 726f 7570 290a  ement/colgroup).
+00026900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00026910: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
+00026920: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00026930: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00026940: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00026950: 745f 5f28 2a63 6869 6c64 7265 6e2c 202a  t__(*children, *
+00026960: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
+00026970: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2820    def __call__( 
+00026980: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00026990: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000269a0: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+000269b0: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+000269c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000269d0: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
+000269e0: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
+000269f0: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
+00026a00: 2020 2020 2020 2020 4465 6669 6e65 7320          Defines 
+00026a10: 6120 6772 6f75 7020 6f66 2063 6f6c 756d  a group of colum
+00026a20: 6e73 2077 6974 6869 6e20 6120 7461 626c  ns within a tabl
+00026a30: 652e 0a0a 2020 2020 2020 2020 0a0a 2020  e...        ..  
+00026a40: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
+00026a50: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00026a60: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00026a70: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00026a80: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00026a90: 4c2f 456c 656d 656e 742f 636f 6c67 726f  L/Element/colgro
+00026aa0: 7570 290a 2020 2020 2020 2020 2222 220a  up).        """.
+00026ab0: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
+00026ac0: 6573 207c 3d20 7b0a 2020 2020 2020 2020  es |= {.        
+00026ad0: 2020 2020 0a20 2020 2020 2020 207d 0a20      .        }. 
+00026ae0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+00026af0: 7065 7228 292e 5f5f 6361 6c6c 5f5f 282a  per().__call__(*
+00026b00: 6368 696c 6472 656e 2c20 2a2a 6174 7472  children, **attr
+00026b10: 6962 7574 6573 290a 0a20 2020 2064 6566  ibutes)..    def
+00026b20: 205f 6765 745f 6465 6661 756c 745f 6174   _get_default_at
+00026b30: 7472 6962 7574 6573 2873 656c 662c 2067  tributes(self, g
+00026b40: 6976 656e 3a20 6469 6374 5b73 7472 2c20  iven: dict[str, 
+00026b50: 4174 7472 6962 7574 6554 7970 655d 2920  AttributeType]) 
+00026b60: 2d3e 2064 6963 745b 7374 722c 2041 7474  -> dict[str, Att
+00026b70: 7269 6275 7465 5479 7065 5d3a 0a20 2020  ributeType]:.   
+00026b80: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
+00026b90: 0a63 6c61 7373 2074 6162 6c65 2854 6167  .class table(Tag
+00026ba0: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+00026bb0: 6570 7265 7365 6e74 7320 7461 6275 6c61  epresents tabula
+00026bc0: 7220 6461 7461 e280 9474 6861 7420 6973  r data...that is
+00026bd0: 2c20 696e 666f 726d 6174 696f 6e20 7072  , information pr
+00026be0: 6573 656e 7465 6420 696e 2061 2074 776f  esented in a two
+00026bf0: 2d64 696d 656e 7369 6f6e 616c 2074 6162  -dimensional tab
+00026c00: 6c65 2063 6f6d 7072 6973 6564 206f 6620  le comprised of 
+00026c10: 726f 7773 2061 6e64 2063 6f6c 756d 6e73  rows and columns
+00026c20: 206f 6620 6365 6c6c 7320 636f 6e74 6169   of cells contai
+00026c30: 6e69 6e67 2064 6174 612e 0a0a 2020 2020  ning data...    
+00026c40: 0a0a 2020 2020 5b56 6965 7720 6675 6c6c  ..    [View full
+00026c50: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00026c60: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00026c70: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00026c80: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00026c90: 4c2f 456c 656d 656e 742f 7461 626c 6529  L/Element/table)
+00026ca0: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
+00026cb0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00026cc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00026cd0: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
+00026ce0: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
+00026cf0: 2020 0a20 2020 2020 2020 2069 643a 204f    .        id: O
+00026d00: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00026d10: 6f6e 652c 0a20 2020 2020 2020 205f 636c  one,.        _cl
+00026d20: 6173 733a 204f 7074 696f 6e61 6c5b 7374  ass: Optional[st
+00026d30: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00026d40: 2020 2073 7479 6c65 3a20 4f70 7469 6f6e     style: Option
+00026d50: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00026d60: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
+00026d70: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
+00026d80: 7970 652c 0a20 2020 2029 202d 3e20 4e6f  ype,.    ) -> No
+00026d90: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00026da0: 2020 2020 2020 2020 5265 7072 6573 656e          Represen
+00026db0: 7473 2074 6162 756c 6172 2064 6174 61e2  ts tabular data.
+00026dc0: 8094 7468 6174 2069 732c 2069 6e66 6f72  ..that is, infor
+00026dd0: 6d61 7469 6f6e 2070 7265 7365 6e74 6564  mation presented
+00026de0: 2069 6e20 6120 7477 6f2d 6469 6d65 6e73   in a two-dimens
+00026df0: 696f 6e61 6c20 7461 626c 6520 636f 6d70  ional table comp
+00026e00: 7269 7365 6420 6f66 2072 6f77 7320 616e  rised of rows an
+00026e10: 6420 636f 6c75 6d6e 7320 6f66 2063 656c  d columns of cel
+00026e20: 6c73 2063 6f6e 7461 696e 696e 6720 6461  ls containing da
+00026e30: 7461 2e0a 0a20 2020 2020 2020 200a 0a20  ta...        .. 
+00026e40: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
+00026e50: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00026e60: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+00026e70: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+00026e80: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+00026e90: 4d4c 2f45 6c65 6d65 6e74 2f74 6162 6c65  ML/Element/table
+00026ea0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00026eb0: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
+00026ec0: 207c 3d20 7b0a 2020 2020 2020 2020 2020   |= {.          
+00026ed0: 2020 275f 636c 6173 7327 3a20 5f63 6c61    '_class': _cla
+00026ee0: 7373 2c0a 2020 2020 2020 2020 2020 2020  ss,.            
+00026ef0: 2769 6427 3a20 6964 2c0a 2020 2020 2020  'id': id,.      
+00026f00: 2020 2020 2020 2773 7479 6c65 273a 2073        'style': s
+00026f10: 7479 6c65 2c0a 2020 2020 2020 2020 2020  tyle,.          
+00026f20: 2020 0a20 2020 2020 2020 207d 0a20 2020    .        }.   
+00026f30: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00026f40: 6e69 745f 5f28 2a63 6869 6c64 7265 6e2c  nit__(*children,
+00026f50: 202a 2a61 7474 7269 6275 7465 7329 0a0a   **attributes)..
+00026f60: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
+00026f70: 2820 2023 2074 7970 653a 2069 676e 6f72  (  # type: ignor
+00026f80: 650a 2020 2020 2020 2020 7365 6c66 2c0a  e.        self,.
+00026f90: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+00026fa0: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+00026fb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00026fc0: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
+00026fd0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00026fe0: 2020 2020 5f63 6c61 7373 3a20 4f70 7469      _class: Opti
+00026ff0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00027000: 2c0a 2020 2020 2020 2020 7374 796c 653a  ,.        style:
+00027010: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00027020: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+00027030: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
+00027040: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
+00027050: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00027060: 2020 2020 2020 2052 6570 7265 7365 6e74         Represent
+00027070: 7320 7461 6275 6c61 7220 6461 7461 e280  s tabular data..
+00027080: 9474 6861 7420 6973 2c20 696e 666f 726d  .that is, inform
+00027090: 6174 696f 6e20 7072 6573 656e 7465 6420  ation presented 
+000270a0: 696e 2061 2074 776f 2d64 696d 656e 7369  in a two-dimensi
+000270b0: 6f6e 616c 2074 6162 6c65 2063 6f6d 7072  onal table compr
+000270c0: 6973 6564 206f 6620 726f 7773 2061 6e64  ised of rows and
+000270d0: 2063 6f6c 756d 6e73 206f 6620 6365 6c6c   columns of cell
+000270e0: 7320 636f 6e74 6169 6e69 6e67 2064 6174  s containing dat
+000270f0: 612e 0a0a 2020 2020 2020 2020 0a0a 2020  a...        ..  
+00027100: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
+00027110: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00027120: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00027130: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00027140: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00027150: 4c2f 456c 656d 656e 742f 7461 626c 6529  L/Element/table)
+00027160: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00027170: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
+00027180: 7c3d 207b 0a20 2020 2020 2020 2020 2020  |= {.           
+00027190: 2027 5f63 6c61 7373 273a 205f 636c 6173   '_class': _clas
+000271a0: 732c 0a20 2020 2020 2020 2020 2020 2027  s,.            '
+000271b0: 6964 273a 2069 642c 0a20 2020 2020 2020  id': id,.       
+000271c0: 2020 2020 2027 7374 796c 6527 3a20 7374       'style': st
+000271d0: 796c 652c 0a20 2020 2020 2020 2020 2020  yle,.           
+000271e0: 200a 2020 2020 2020 2020 7d0a 2020 2020   .        }.    
+000271f0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00027200: 2829 2e5f 5f63 616c 6c5f 5f28 2a63 6869  ().__call__(*chi
+00027210: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
+00027220: 7465 7329 0a0a 2020 2020 6465 6620 5f67  tes)..    def _g
+00027230: 6574 5f64 6566 6175 6c74 5f61 7474 7269  et_default_attri
+00027240: 6275 7465 7328 7365 6c66 2c20 6769 7665  butes(self, give
+00027250: 6e3a 2064 6963 745b 7374 722c 2041 7474  n: dict[str, Att
+00027260: 7269 6275 7465 5479 7065 5d29 202d 3e20  ributeType]) -> 
+00027270: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
+00027280: 7574 6554 7970 655d 3a0a 2020 2020 2020  uteType]:.      
+00027290: 2020 7265 7475 726e 207b 7d0a 0a0a 636c    return {}...cl
+000272a0: 6173 7320 7462 6f64 7928 5461 6729 3a0a  ass tbody(Tag):.
+000272b0: 2020 2020 2222 220a 2020 2020 456e 6361      """.    Enca
+000272c0: 7073 756c 6174 6573 2061 2073 6574 206f  psulates a set o
+000272d0: 6620 7461 626c 6520 726f 7773 2028 5b60  f table rows ([`
+000272e0: 3c74 723e 605d 2868 7474 7073 3a2f 2f64  <tr>`](https://d
+000272f0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+00027300: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+00027310: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+00027320: 2f74 7229 2065 6c65 6d65 6e74 7329 2c20  /tr) elements), 
+00027330: 696e 6469 6361 7469 6e67 2074 6861 7420  indicating that 
+00027340: 7468 6579 2063 6f6d 7072 6973 6520 7468  they comprise th
+00027350: 6520 626f 6479 206f 6620 6120 7461 626c  e body of a tabl
+00027360: 6527 7320 286d 6169 6e29 2064 6174 612e  e's (main) data.
+00027370: 0a0a 2020 2020 0a0a 2020 2020 5b56 6965  ..    ..    [Vie
+00027380: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+00027390: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+000273a0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+000273b0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+000273c0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+000273d0: 7462 6f64 7929 0a20 2020 2022 2222 0a20  tbody).    """. 
+000273e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000273f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00027400: 2020 2020 2020 202a 6368 696c 6472 656e         *children
+00027410: 3a20 4368 696c 6472 656e 5479 7065 2c0a  : ChildrenType,.
+00027420: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00027430: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
+00027440: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
+00027450: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00027460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00027470: 2045 6e63 6170 7375 6c61 7465 7320 6120   Encapsulates a 
+00027480: 7365 7420 6f66 2074 6162 6c65 2072 6f77  set of table row
+00027490: 7320 285b 603c 7472 3e60 5d28 6874 7470  s ([`<tr>`](http
+000274a0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+000274b0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+000274c0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+000274d0: 656d 656e 742f 7472 2920 656c 656d 656e  ement/tr) elemen
+000274e0: 7473 292c 2069 6e64 6963 6174 696e 6720  ts), indicating 
+000274f0: 7468 6174 2074 6865 7920 636f 6d70 7269  that they compri
+00027500: 7365 2074 6865 2062 6f64 7920 6f66 2061  se the body of a
+00027510: 2074 6162 6c65 2773 2028 6d61 696e 2920   table's (main) 
+00027520: 6461 7461 2e0a 0a20 2020 2020 2020 200a  data...        .
+00027530: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
+00027540: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+00027550: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+00027560: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
+00027570: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
+00027580: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 626f  HTML/Element/tbo
+00027590: 6479 290a 2020 2020 2020 2020 2222 220a  dy).        """.
+000275a0: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
+000275b0: 6573 207c 3d20 7b0a 2020 2020 2020 2020  es |= {.        
+000275c0: 2020 2020 0a20 2020 2020 2020 207d 0a20      .        }. 
+000275d0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+000275e0: 5f69 6e69 745f 5f28 2a63 6869 6c64 7265  _init__(*childre
+000275f0: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
+00027600: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+00027610: 5f5f 2820 2023 2074 7970 653a 2069 676e  __(  # type: ign
+00027620: 6f72 650a 2020 2020 2020 2020 7365 6c66  ore.        self
+00027630: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
+00027640: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
+00027650: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
+00027660: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
+00027670: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
+00027680: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00027690: 2222 220a 2020 2020 2020 2020 456e 6361  """.        Enca
+000276a0: 7073 756c 6174 6573 2061 2073 6574 206f  psulates a set o
+000276b0: 6620 7461 626c 6520 726f 7773 2028 5b60  f table rows ([`
+000276c0: 3c74 723e 605d 2868 7474 7073 3a2f 2f64  <tr>`](https://d
+000276d0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+000276e0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+000276f0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+00027700: 2f74 7229 2065 6c65 6d65 6e74 7329 2c20  /tr) elements), 
+00027710: 696e 6469 6361 7469 6e67 2074 6861 7420  indicating that 
+00027720: 7468 6579 2063 6f6d 7072 6973 6520 7468  they comprise th
+00027730: 6520 626f 6479 206f 6620 6120 7461 626c  e body of a tabl
+00027740: 6527 7320 286d 6169 6e29 2064 6174 612e  e's (main) data.
+00027750: 0a0a 2020 2020 2020 2020 0a0a 2020 2020  ..        ..    
+00027760: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
+00027770: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00027780: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+00027790: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+000277a0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+000277b0: 456c 656d 656e 742f 7462 6f64 7929 0a20  Element/tbody). 
+000277c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000277d0: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
+000277e0: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
+000277f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00027800: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00027810: 2e5f 5f63 616c 6c5f 5f28 2a63 6869 6c64  .__call__(*child
+00027820: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
+00027830: 7329 0a0a 2020 2020 6465 6620 5f67 6574  s)..    def _get
+00027840: 5f64 6566 6175 6c74 5f61 7474 7269 6275  _default_attribu
+00027850: 7465 7328 7365 6c66 2c20 6769 7665 6e3a  tes(self, given:
+00027860: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
+00027870: 6275 7465 5479 7065 5d29 202d 3e20 6469  buteType]) -> di
+00027880: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
+00027890: 6554 7970 655d 3a0a 2020 2020 2020 2020  eType]:.        
+000278a0: 7265 7475 726e 207b 7d0a 0a0a 636c 6173  return {}...clas
+000278b0: 7320 7464 2854 6167 293a 0a20 2020 2022  s td(Tag):.    "
+000278c0: 2222 0a20 2020 2041 2063 6869 6c64 206f  "".    A child o
+000278d0: 6620 7468 6520 5b60 3c74 723e 605d 2868  f the [`<tr>`](h
+000278e0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+000278f0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00027900: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00027910: 2f45 6c65 6d65 6e74 2f74 7229 2065 6c65  /Element/tr) ele
+00027920: 6d65 6e74 2c20 6974 2064 6566 696e 6573  ment, it defines
+00027930: 2061 2063 656c 6c20 6f66 2061 2074 6162   a cell of a tab
+00027940: 6c65 2074 6861 7420 636f 6e74 6169 6e73  le that contains
+00027950: 2064 6174 612e 0a0a 2020 2020 2a20 6063   data...    * `c
+00027960: 6f6c 7370 616e 603a 2054 6865 206e 756d  olspan`: The num
+00027970: 6265 7220 6f66 2063 6f6c 756d 6e73 2069  ber of columns i
+00027980: 6e20 7468 6520 7461 626c 6520 7468 6174  n the table that
+00027990: 2074 6869 7320 6365 6c6c 2073 7061 6e73   this cell spans
+000279a0: 2e0a 2020 2020 2a20 6072 6f77 7370 616e  ..    * `rowspan
+000279b0: 603a 2054 6865 206e 756d 6265 7220 6f66  `: The number of
+000279c0: 2072 6f77 7320 696e 2074 6865 2074 6162   rows in the tab
+000279d0: 6c65 2074 6861 7420 7468 6973 2063 656c  le that this cel
+000279e0: 6c20 7370 616e 732e 0a0a 2020 2020 5b56  l spans...    [V
+000279f0: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+00027a00: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00027a10: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+00027a20: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+00027a30: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+00027a40: 742f 7464 290a 2020 2020 2222 220a 2020  t/td).    """.  
+00027a50: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00027a60: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00027a70: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+00027a80: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+00027a90: 2020 2020 2020 2063 6f6c 7370 616e 3a20         colspan: 
+00027aa0: 4174 7472 6962 7574 6554 7970 6520 3d20  AttributeType = 
+00027ab0: 4e6f 6e65 2c0a 2020 2020 2020 2020 726f  None,.        ro
+00027ac0: 7773 7061 6e3a 2041 7474 7269 6275 7465  wspan: Attribute
+00027ad0: 5479 7065 203d 204e 6f6e 652c 0a20 2020  Type = None,.   
+00027ae0: 2020 2020 2069 643a 204f 7074 696f 6e61       id: Optiona
+00027af0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00027b00: 2020 2020 2020 205f 636c 6173 733a 204f         _class: O
+00027b10: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00027b20: 6f6e 652c 0a20 2020 2020 2020 2073 7479  one,.        sty
+00027b30: 6c65 3a20 4f70 7469 6f6e 616c 5b73 7472  le: Optional[str
+00027b40: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00027b50: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+00027b60: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+00027b70: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00027b80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00027b90: 2020 4120 6368 696c 6420 6f66 2074 6865    A child of the
+00027ba0: 205b 603c 7472 3e60 5d28 6874 7470 733a   [`<tr>`](https:
+00027bb0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+00027bc0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00027bd0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+00027be0: 656e 742f 7472 2920 656c 656d 656e 742c  ent/tr) element,
+00027bf0: 2069 7420 6465 6669 6e65 7320 6120 6365   it defines a ce
+00027c00: 6c6c 206f 6620 6120 7461 626c 6520 7468  ll of a table th
+00027c10: 6174 2063 6f6e 7461 696e 7320 6461 7461  at contains data
+00027c20: 2e0a 0a20 2020 2020 2020 202a 2060 636f  ...        * `co
+00027c30: 6c73 7061 6e60 3a20 5468 6520 6e75 6d62  lspan`: The numb
+00027c40: 6572 206f 6620 636f 6c75 6d6e 7320 696e  er of columns in
+00027c50: 2074 6865 2074 6162 6c65 2074 6861 7420   the table that 
+00027c60: 7468 6973 2063 656c 6c20 7370 616e 732e  this cell spans.
+00027c70: 0a20 2020 2020 2020 202a 2060 726f 7773  .        * `rows
+00027c80: 7061 6e60 3a20 5468 6520 6e75 6d62 6572  pan`: The number
+00027c90: 206f 6620 726f 7773 2069 6e20 7468 6520   of rows in the 
+00027ca0: 7461 626c 6520 7468 6174 2074 6869 7320  table that this 
+00027cb0: 6365 6c6c 2073 7061 6e73 2e0a 0a20 2020  cell spans...   
+00027cc0: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
+00027cd0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+00027ce0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00027cf0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00027d00: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00027d10: 2f45 6c65 6d65 6e74 2f74 6429 0a20 2020  /Element/td).   
+00027d20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00027d30: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+00027d40: 0a20 2020 2020 2020 2020 2020 2027 5f63  .            '_c
+00027d50: 6c61 7373 273a 205f 636c 6173 732c 0a20  lass': _class,. 
+00027d60: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
+00027d70: 2069 642c 0a20 2020 2020 2020 2020 2020   id,.           
+00027d80: 2027 7374 796c 6527 3a20 7374 796c 652c   'style': style,
+00027d90: 0a20 2020 2020 2020 2020 2020 2027 636f  .            'co
+00027da0: 6c73 7061 6e27 3a20 636f 6c73 7061 6e2c  lspan': colspan,
+00027db0: 0a20 2020 2020 2020 2020 2020 2027 726f  .            'ro
+00027dc0: 7773 7061 6e27 3a20 726f 7773 7061 6e2c  wspan': rowspan,
+00027dd0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00027de0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00027df0: 745f 5f28 2a63 6869 6c64 7265 6e2c 202a  t__(*children, *
+00027e00: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
+00027e10: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2820    def __call__( 
+00027e20: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00027e30: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00027e40: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+00027e50: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+00027e60: 2020 2020 2020 2063 6f6c 7370 616e 3a20         colspan: 
+00027e70: 4174 7472 6962 7574 6554 7970 6520 3d20  AttributeType = 
+00027e80: 4e6f 6e65 2c0a 2020 2020 2020 2020 726f  None,.        ro
+00027e90: 7773 7061 6e3a 2041 7474 7269 6275 7465  wspan: Attribute
+00027ea0: 5479 7065 203d 204e 6f6e 652c 0a20 2020  Type = None,.   
+00027eb0: 2020 2020 2069 643a 204f 7074 696f 6e61       id: Optiona
+00027ec0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00027ed0: 2020 2020 2020 205f 636c 6173 733a 204f         _class: O
+00027ee0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00027ef0: 6f6e 652c 0a20 2020 2020 2020 2073 7479  one,.        sty
+00027f00: 6c65 3a20 4f70 7469 6f6e 616c 5b73 7472  le: Optional[str
+00027f10: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00027f20: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+00027f30: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+00027f40: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00027f50: 220a 2020 2020 2020 2020 4120 6368 696c  ".        A chil
+00027f60: 6420 6f66 2074 6865 205b 603c 7472 3e60  d of the [`<tr>`
+00027f70: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+00027f80: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+00027f90: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+00027fa0: 544d 4c2f 456c 656d 656e 742f 7472 2920  TML/Element/tr) 
+00027fb0: 656c 656d 656e 742c 2069 7420 6465 6669  element, it defi
+00027fc0: 6e65 7320 6120 6365 6c6c 206f 6620 6120  nes a cell of a 
+00027fd0: 7461 626c 6520 7468 6174 2063 6f6e 7461  table that conta
+00027fe0: 696e 7320 6461 7461 2e0a 0a20 2020 2020  ins data...     
+00027ff0: 2020 202a 2060 636f 6c73 7061 6e60 3a20     * `colspan`: 
+00028000: 5468 6520 6e75 6d62 6572 206f 6620 636f  The number of co
+00028010: 6c75 6d6e 7320 696e 2074 6865 2074 6162  lumns in the tab
+00028020: 6c65 2074 6861 7420 7468 6973 2063 656c  le that this cel
+00028030: 6c20 7370 616e 732e 0a20 2020 2020 2020  l spans..       
+00028040: 202a 2060 726f 7773 7061 6e60 3a20 5468   * `rowspan`: Th
+00028050: 6520 6e75 6d62 6572 206f 6620 726f 7773  e number of rows
+00028060: 2069 6e20 7468 6520 7461 626c 6520 7468   in the table th
+00028070: 6174 2074 6869 7320 6365 6c6c 2073 7061  at this cell spa
+00028080: 6e73 2e0a 0a20 2020 2020 2020 205b 5669  ns...        [Vi
+00028090: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
+000280a0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+000280b0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+000280c0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+000280d0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+000280e0: 2f74 6429 0a20 2020 2020 2020 2022 2222  /td).        """
+000280f0: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+00028100: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+00028110: 2020 2020 2027 5f63 6c61 7373 273a 205f       '_class': _
+00028120: 636c 6173 732c 0a20 2020 2020 2020 2020  class,.         
+00028130: 2020 2027 6964 273a 2069 642c 0a20 2020     'id': id,.   
+00028140: 2020 2020 2020 2020 2027 7374 796c 6527           'style'
+00028150: 3a20 7374 796c 652c 0a20 2020 2020 2020  : style,.       
+00028160: 2020 2020 2027 636f 6c73 7061 6e27 3a20       'colspan': 
+00028170: 636f 6c73 7061 6e2c 0a20 2020 2020 2020  colspan,.       
+00028180: 2020 2020 2027 726f 7773 7061 6e27 3a20       'rowspan': 
+00028190: 726f 7773 7061 6e2c 0a20 2020 2020 2020  rowspan,.       
+000281a0: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+000281b0: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
+000281c0: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+000281d0: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+000281e0: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
+000281f0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
+00028200: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
+00028210: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
+00028220: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
+00028230: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
+00028240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00028250: 7b27 636f 6c73 7061 6e27 3a20 4e6f 6e65  {'colspan': None
+00028260: 2c20 2772 6f77 7370 616e 273a 204e 6f6e  , 'rowspan': Non
+00028270: 657d 0a0a 0a63 6c61 7373 2074 666f 6f74  e}...class tfoot
+00028280: 2854 6167 293a 0a20 2020 2022 2222 0a20  (Tag):.    """. 
+00028290: 2020 2045 6e63 6170 7375 6c61 7465 7320     Encapsulates 
+000282a0: 6120 7365 7420 6f66 2074 6162 6c65 2072  a set of table r
+000282b0: 6f77 7320 285b 603c 7472 3e60 5d28 6874  ows ([`<tr>`](ht
+000282c0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+000282d0: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+000282e0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+000282f0: 456c 656d 656e 742f 7472 2920 656c 656d  Element/tr) elem
+00028300: 656e 7473 292c 2069 6e64 6963 6174 696e  ents), indicatin
+00028310: 6720 7468 6174 2074 6865 7920 636f 6d70  g that they comp
+00028320: 7269 7365 2074 6865 2066 6f6f 7420 6f66  rise the foot of
+00028330: 2061 2074 6162 6c65 2077 6974 6820 696e   a table with in
+00028340: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00028350: 7468 6520 7461 626c 6527 7320 636f 6c75  the table's colu
+00028360: 6d6e 732e 2054 6869 7320 6973 2075 7375  mns. This is usu
+00028370: 616c 6c79 2061 2073 756d 6d61 7279 206f  ally a summary o
+00028380: 6620 7468 6520 636f 6c75 6d6e 732c 2065  f the columns, e
+00028390: 2e67 2e2c 2061 2073 756d 206f 6620 7468  .g., a sum of th
+000283a0: 6520 6769 7665 6e20 6e75 6d62 6572 7320  e given numbers 
+000283b0: 696e 2061 2063 6f6c 756d 6e2e 0a0a 2020  in a column...  
+000283c0: 2020 0a0a 2020 2020 5b56 6965 7720 6675    ..    [View fu
+000283d0: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+000283e0: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+000283f0: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+00028400: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+00028410: 544d 4c2f 456c 656d 656e 742f 7466 6f6f  TML/Element/tfoo
+00028420: 7429 0a20 2020 2022 2222 0a20 2020 2064  t).    """.    d
+00028430: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00028440: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00028450: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+00028460: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+00028470: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+00028480: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+00028490: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
+000284a0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000284b0: 2022 2222 0a20 2020 2020 2020 2045 6e63   """.        Enc
+000284c0: 6170 7375 6c61 7465 7320 6120 7365 7420  apsulates a set 
+000284d0: 6f66 2074 6162 6c65 2072 6f77 7320 285b  of table rows ([
+000284e0: 603c 7472 3e60 5d28 6874 7470 733a 2f2f  `<tr>`](https://
+000284f0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+00028500: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+00028510: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+00028520: 742f 7472 2920 656c 656d 656e 7473 292c  t/tr) elements),
+00028530: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
+00028540: 2074 6865 7920 636f 6d70 7269 7365 2074   they comprise t
+00028550: 6865 2066 6f6f 7420 6f66 2061 2074 6162  he foot of a tab
+00028560: 6c65 2077 6974 6820 696e 666f 726d 6174  le with informat
+00028570: 696f 6e20 6162 6f75 7420 7468 6520 7461  ion about the ta
+00028580: 626c 6527 7320 636f 6c75 6d6e 732e 2054  ble's columns. T
+00028590: 6869 7320 6973 2075 7375 616c 6c79 2061  his is usually a
+000285a0: 2073 756d 6d61 7279 206f 6620 7468 6520   summary of the 
+000285b0: 636f 6c75 6d6e 732c 2065 2e67 2e2c 2061  columns, e.g., a
+000285c0: 2073 756d 206f 6620 7468 6520 6769 7665   sum of the give
+000285d0: 6e20 6e75 6d62 6572 7320 696e 2061 2063  n numbers in a c
+000285e0: 6f6c 756d 6e2e 0a0a 2020 2020 2020 2020  olumn...        
+000285f0: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+00028600: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+00028610: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+00028620: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+00028630: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+00028640: 2f48 544d 4c2f 456c 656d 656e 742f 7466  /HTML/Element/tf
+00028650: 6f6f 7429 0a20 2020 2020 2020 2022 2222  oot).        """
+00028660: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+00028670: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+00028680: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
+00028690: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+000286a0: 5f5f 696e 6974 5f5f 282a 6368 696c 6472  __init__(*childr
+000286b0: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
+000286c0: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
+000286d0: 6c5f 5f28 2020 2320 7479 7065 3a20 6967  l__(  # type: ig
+000286e0: 6e6f 7265 0a20 2020 2020 2020 2073 656c  nore.        sel
+000286f0: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
+00028700: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
+00028710: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
+00028720: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
+00028730: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
+00028740: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00028750: 2022 2222 0a20 2020 2020 2020 2045 6e63   """.        Enc
+00028760: 6170 7375 6c61 7465 7320 6120 7365 7420  apsulates a set 
+00028770: 6f66 2074 6162 6c65 2072 6f77 7320 285b  of table rows ([
+00028780: 603c 7472 3e60 5d28 6874 7470 733a 2f2f  `<tr>`](https://
+00028790: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+000287a0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+000287b0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+000287c0: 742f 7472 2920 656c 656d 656e 7473 292c  t/tr) elements),
+000287d0: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
+000287e0: 2074 6865 7920 636f 6d70 7269 7365 2074   they comprise t
+000287f0: 6865 2066 6f6f 7420 6f66 2061 2074 6162  he foot of a tab
+00028800: 6c65 2077 6974 6820 696e 666f 726d 6174  le with informat
+00028810: 696f 6e20 6162 6f75 7420 7468 6520 7461  ion about the ta
+00028820: 626c 6527 7320 636f 6c75 6d6e 732e 2054  ble's columns. T
+00028830: 6869 7320 6973 2075 7375 616c 6c79 2061  his is usually a
+00028840: 2073 756d 6d61 7279 206f 6620 7468 6520   summary of the 
+00028850: 636f 6c75 6d6e 732c 2065 2e67 2e2c 2061  columns, e.g., a
+00028860: 2073 756d 206f 6620 7468 6520 6769 7665   sum of the give
+00028870: 6e20 6e75 6d62 6572 7320 696e 2061 2063  n numbers in a c
+00028880: 6f6c 756d 6e2e 0a0a 2020 2020 2020 2020  olumn...        
+00028890: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+000288a0: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+000288b0: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+000288c0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+000288d0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+000288e0: 2f48 544d 4c2f 456c 656d 656e 742f 7466  /HTML/Element/tf
+000288f0: 6f6f 7429 0a20 2020 2020 2020 2022 2222  oot).        """
+00028900: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+00028910: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+00028920: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
+00028930: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00028940: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
+00028950: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
+00028960: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+00028970: 6620 5f67 6574 5f64 6566 6175 6c74 5f61  f _get_default_a
+00028980: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
+00028990: 6769 7665 6e3a 2064 6963 745b 7374 722c  given: dict[str,
+000289a0: 2041 7474 7269 6275 7465 5479 7065 5d29   AttributeType])
+000289b0: 202d 3e20 6469 6374 5b73 7472 2c20 4174   -> dict[str, At
+000289c0: 7472 6962 7574 6554 7970 655d 3a0a 2020  tributeType]:.  
+000289d0: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
+000289e0: 0a0a 636c 6173 7320 7468 2854 6167 293a  ..class th(Tag):
+000289f0: 0a20 2020 2022 2222 0a20 2020 2041 2063  .    """.    A c
+00028a00: 6869 6c64 206f 6620 7468 6520 5b60 3c74  hild of the [`<t
+00028a10: 723e 605d 2868 7474 7073 3a2f 2f64 6576  r>`](https://dev
+00028a20: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+00028a30: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+00028a40: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f74  b/HTML/Element/t
+00028a50: 7229 2065 6c65 6d65 6e74 2c20 6974 2064  r) element, it d
+00028a60: 6566 696e 6573 2061 2063 656c 6c20 6173  efines a cell as
+00028a70: 2074 6865 2068 6561 6465 7220 6f66 2061   the header of a
+00028a80: 2067 726f 7570 206f 6620 7461 626c 6520   group of table 
+00028a90: 6365 6c6c 732e 2054 6865 206e 6174 7572  cells. The natur
+00028aa0: 6520 6f66 2074 6869 7320 6772 6f75 7020  e of this group 
+00028ab0: 6361 6e20 6265 2065 7870 6c69 6369 746c  can be explicitl
+00028ac0: 7920 6465 6669 6e65 6420 6279 2074 6865  y defined by the
+00028ad0: 205b 6073 636f 7065 605d 2868 7474 7073   [`scope`](https
+00028ae0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+00028af0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+00028b00: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+00028b10: 6d65 6e74 2f74 6823 7363 6f70 6529 2061  ment/th#scope) a
+00028b20: 6e64 205b 6068 6561 6465 7273 605d 2868  nd [`headers`](h
+00028b30: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00028b40: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00028b50: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00028b60: 2f45 6c65 6d65 6e74 2f74 6823 6865 6164  /Element/th#head
+00028b70: 6572 7329 2061 7474 7269 6275 7465 732e  ers) attributes.
+00028b80: 0a0a 2020 2020 2a20 6073 636f 7065 603a  ..    * `scope`:
+00028b90: 2054 6865 2061 7265 6120 6f66 2074 6865   The area of the
+00028ba0: 2074 6162 6c65 2074 6861 7420 7468 6973   table that this
+00028bb0: 2068 6561 6469 6e67 2061 7070 6c69 6573   heading applies
+00028bc0: 2074 6f2e 2041 6c6c 6f77 6564 2076 616c   to. Allowed val
+00028bd0: 7565 733a 2060 2263 6f6c 2260 2c20 6022  ues: `"col"`, `"
+00028be0: 726f 7722 602c 2060 2263 6f6c 6772 6f75  row"`, `"colgrou
+00028bf0: 7022 602c 2060 2272 6f77 6772 6f75 7022  p"`, `"rowgroup"
+00028c00: 600a 2020 2020 2a20 6063 6f6c 7370 616e  `.    * `colspan
+00028c10: 603a 2054 6865 206e 756d 6265 7220 6f66  `: The number of
+00028c20: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+00028c30: 7461 626c 6520 7468 6174 2074 6869 7320  table that this 
+00028c40: 6865 6164 696e 6720 7370 616e 732e 0a20  heading spans.. 
+00028c50: 2020 202a 2060 726f 7773 7061 6e60 3a20     * `rowspan`: 
+00028c60: 5468 6520 6e75 6d62 6572 206f 6620 726f  The number of ro
+00028c70: 7773 2069 6e20 7468 6520 7461 626c 6520  ws in the table 
+00028c80: 7468 6174 2074 6869 7320 6865 6164 696e  that this headin
+00028c90: 6720 7370 616e 732e 0a0a 2020 2020 5b56  g spans...    [V
+00028ca0: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+00028cb0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00028cc0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+00028cd0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+00028ce0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+00028cf0: 742f 7468 290a 2020 2020 2222 220a 2020  t/th).    """.  
+00028d00: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00028d10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00028d20: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+00028d30: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+00028d40: 2020 2020 2020 2073 636f 7065 3a20 4174         scope: At
+00028d50: 7472 6962 7574 6554 7970 6520 3d20 4e6f  tributeType = No
+00028d60: 6e65 2c0a 2020 2020 2020 2020 636f 6c73  ne,.        cols
+00028d70: 7061 6e3a 2041 7474 7269 6275 7465 5479  pan: AttributeTy
+00028d80: 7065 203d 204e 6f6e 652c 0a20 2020 2020  pe = None,.     
+00028d90: 2020 2072 6f77 7370 616e 3a20 4174 7472     rowspan: Attr
+00028da0: 6962 7574 6554 7970 6520 3d20 4e6f 6e65  ibuteType = None
+00028db0: 2c0a 2020 2020 2020 2020 6964 3a20 4f70  ,.        id: Op
+00028dc0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00028dd0: 6e65 2c0a 2020 2020 2020 2020 5f63 6c61  ne,.        _cla
+00028de0: 7373 3a20 4f70 7469 6f6e 616c 5b73 7472  ss: Optional[str
+00028df0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00028e00: 2020 7374 796c 653a 204f 7074 696f 6e61    style: Optiona
+00028e10: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00028e20: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
+00028e30: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
+00028e40: 7065 2c0a 2020 2020 2920 2d3e 204e 6f6e  pe,.    ) -> Non
+00028e50: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00028e60: 2020 2020 2020 2041 2063 6869 6c64 206f         A child o
+00028e70: 6620 7468 6520 5b60 3c74 723e 605d 2868  f the [`<tr>`](h
+00028e80: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00028e90: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00028ea0: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00028eb0: 2f45 6c65 6d65 6e74 2f74 7229 2065 6c65  /Element/tr) ele
+00028ec0: 6d65 6e74 2c20 6974 2064 6566 696e 6573  ment, it defines
+00028ed0: 2061 2063 656c 6c20 6173 2074 6865 2068   a cell as the h
+00028ee0: 6561 6465 7220 6f66 2061 2067 726f 7570  eader of a group
+00028ef0: 206f 6620 7461 626c 6520 6365 6c6c 732e   of table cells.
+00028f00: 2054 6865 206e 6174 7572 6520 6f66 2074   The nature of t
+00028f10: 6869 7320 6772 6f75 7020 6361 6e20 6265  his group can be
+00028f20: 2065 7870 6c69 6369 746c 7920 6465 6669   explicitly defi
+00028f30: 6e65 6420 6279 2074 6865 205b 6073 636f  ned by the [`sco
+00028f40: 7065 605d 2868 7474 7073 3a2f 2f64 6576  pe`](https://dev
+00028f50: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+00028f60: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+00028f70: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f74  b/HTML/Element/t
+00028f80: 6823 7363 6f70 6529 2061 6e64 205b 6068  h#scope) and [`h
+00028f90: 6561 6465 7273 605d 2868 7474 7073 3a2f  eaders`](https:/
+00028fa0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+00028fb0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+00028fc0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+00028fd0: 6e74 2f74 6823 6865 6164 6572 7329 2061  nt/th#headers) a
+00028fe0: 7474 7269 6275 7465 732e 0a0a 2020 2020  ttributes...    
+00028ff0: 2020 2020 2a20 6073 636f 7065 603a 2054      * `scope`: T
+00029000: 6865 2061 7265 6120 6f66 2074 6865 2074  he area of the t
+00029010: 6162 6c65 2074 6861 7420 7468 6973 2068  able that this h
+00029020: 6561 6469 6e67 2061 7070 6c69 6573 2074  eading applies t
+00029030: 6f2e 2041 6c6c 6f77 6564 2076 616c 7565  o. Allowed value
+00029040: 733a 2060 2263 6f6c 2260 2c20 6022 726f  s: `"col"`, `"ro
+00029050: 7722 602c 2060 2263 6f6c 6772 6f75 7022  w"`, `"colgroup"
+00029060: 602c 2060 2272 6f77 6772 6f75 7022 600a  `, `"rowgroup"`.
+00029070: 2020 2020 2020 2020 2a20 6063 6f6c 7370          * `colsp
+00029080: 616e 603a 2054 6865 206e 756d 6265 7220  an`: The number 
+00029090: 6f66 2063 6f6c 756d 6e73 2069 6e20 7468  of columns in th
+000290a0: 6520 7461 626c 6520 7468 6174 2074 6869  e table that thi
+000290b0: 7320 6865 6164 696e 6720 7370 616e 732e  s heading spans.
+000290c0: 0a20 2020 2020 2020 202a 2060 726f 7773  .        * `rows
+000290d0: 7061 6e60 3a20 5468 6520 6e75 6d62 6572  pan`: The number
+000290e0: 206f 6620 726f 7773 2069 6e20 7468 6520   of rows in the 
+000290f0: 7461 626c 6520 7468 6174 2074 6869 7320  table that this 
+00029100: 6865 6164 696e 6720 7370 616e 732e 0a0a  heading spans...
+00029110: 2020 2020 2020 2020 5b56 6965 7720 6675          [View fu
+00029120: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+00029130: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+00029140: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+00029150: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+00029160: 544d 4c2f 456c 656d 656e 742f 7468 290a  TML/Element/th).
+00029170: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00029180: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
+00029190: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000291a0: 275f 636c 6173 7327 3a20 5f63 6c61 7373  '_class': _class
+000291b0: 2c0a 2020 2020 2020 2020 2020 2020 2769  ,.            'i
+000291c0: 6427 3a20 6964 2c0a 2020 2020 2020 2020  d': id,.        
+000291d0: 2020 2020 2773 7479 6c65 273a 2073 7479      'style': sty
+000291e0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+000291f0: 2773 636f 7065 273a 2073 636f 7065 2c0a  'scope': scope,.
+00029200: 2020 2020 2020 2020 2020 2020 2763 6f6c              'col
+00029210: 7370 616e 273a 2063 6f6c 7370 616e 2c0a  span': colspan,.
+00029220: 2020 2020 2020 2020 2020 2020 2772 6f77              'row
+00029230: 7370 616e 273a 2072 6f77 7370 616e 2c0a  span': rowspan,.
+00029240: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00029250: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00029260: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+00029270: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+00029280: 2064 6566 205f 5f63 616c 6c5f 5f28 2020   def __call__(  
+00029290: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
+000292a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000292b0: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
+000292c0: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
+000292d0: 2020 2020 2020 7363 6f70 653a 2041 7474        scope: Att
+000292e0: 7269 6275 7465 5479 7065 203d 204e 6f6e  ributeType = Non
+000292f0: 652c 0a20 2020 2020 2020 2063 6f6c 7370  e,.        colsp
+00029300: 616e 3a20 4174 7472 6962 7574 6554 7970  an: AttributeTyp
+00029310: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00029320: 2020 726f 7773 7061 6e3a 2041 7474 7269    rowspan: Attri
+00029330: 6275 7465 5479 7065 203d 204e 6f6e 652c  buteType = None,
+00029340: 0a20 2020 2020 2020 2069 643a 204f 7074  .        id: Opt
+00029350: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00029360: 652c 0a20 2020 2020 2020 205f 636c 6173  e,.        _clas
+00029370: 733a 204f 7074 696f 6e61 6c5b 7374 725d  s: Optional[str]
+00029380: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00029390: 2073 7479 6c65 3a20 4f70 7469 6f6e 616c   style: Optional
+000293a0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+000293b0: 2020 2020 2020 2a2a 6174 7472 6962 7574        **attribut
+000293c0: 6573 3a20 4174 7472 6962 7574 6554 7970  es: AttributeTyp
+000293d0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000293e0: 2020 2222 220a 2020 2020 2020 2020 4120    """.        A 
+000293f0: 6368 696c 6420 6f66 2074 6865 205b 603c  child of the [`<
+00029400: 7472 3e60 5d28 6874 7470 733a 2f2f 6465  tr>`](https://de
+00029410: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+00029420: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+00029430: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00029440: 7472 2920 656c 656d 656e 742c 2069 7420  tr) element, it 
+00029450: 6465 6669 6e65 7320 6120 6365 6c6c 2061  defines a cell a
+00029460: 7320 7468 6520 6865 6164 6572 206f 6620  s the header of 
+00029470: 6120 6772 6f75 7020 6f66 2074 6162 6c65  a group of table
+00029480: 2063 656c 6c73 2e20 5468 6520 6e61 7475   cells. The natu
+00029490: 7265 206f 6620 7468 6973 2067 726f 7570  re of this group
+000294a0: 2063 616e 2062 6520 6578 706c 6963 6974   can be explicit
+000294b0: 6c79 2064 6566 696e 6564 2062 7920 7468  ly defined by th
+000294c0: 6520 5b60 7363 6f70 6560 5d28 6874 7470  e [`scope`](http
+000294d0: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+000294e0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+000294f0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+00029500: 656d 656e 742f 7468 2373 636f 7065 2920  ement/th#scope) 
+00029510: 616e 6420 5b60 6865 6164 6572 7360 5d28  and [`headers`](
+00029520: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+00029530: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+00029540: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+00029550: 4c2f 456c 656d 656e 742f 7468 2368 6561  L/Element/th#hea
+00029560: 6465 7273 2920 6174 7472 6962 7574 6573  ders) attributes
+00029570: 2e0a 0a20 2020 2020 2020 202a 2060 7363  ...        * `sc
+00029580: 6f70 6560 3a20 5468 6520 6172 6561 206f  ope`: The area o
+00029590: 6620 7468 6520 7461 626c 6520 7468 6174  f the table that
+000295a0: 2074 6869 7320 6865 6164 696e 6720 6170   this heading ap
+000295b0: 706c 6965 7320 746f 2e20 416c 6c6f 7765  plies to. Allowe
+000295c0: 6420 7661 6c75 6573 3a20 6022 636f 6c22  d values: `"col"
+000295d0: 602c 2060 2272 6f77 2260 2c20 6022 636f  `, `"row"`, `"co
+000295e0: 6c67 726f 7570 2260 2c20 6022 726f 7767  lgroup"`, `"rowg
+000295f0: 726f 7570 2260 0a20 2020 2020 2020 202a  roup"`.        *
+00029600: 2060 636f 6c73 7061 6e60 3a20 5468 6520   `colspan`: The 
+00029610: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
+00029620: 7320 696e 2074 6865 2074 6162 6c65 2074  s in the table t
+00029630: 6861 7420 7468 6973 2068 6561 6469 6e67  hat this heading
+00029640: 2073 7061 6e73 2e0a 2020 2020 2020 2020   spans..        
+00029650: 2a20 6072 6f77 7370 616e 603a 2054 6865  * `rowspan`: The
+00029660: 206e 756d 6265 7220 6f66 2072 6f77 7320   number of rows 
+00029670: 696e 2074 6865 2074 6162 6c65 2074 6861  in the table tha
+00029680: 7420 7468 6973 2068 6561 6469 6e67 2073  t this heading s
+00029690: 7061 6e73 2e0a 0a20 2020 2020 2020 205b  pans...        [
+000296a0: 5669 6577 2066 756c 6c20 646f 6375 6d65  View full docume
+000296b0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+000296c0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+000296d0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+000296e0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+000296f0: 6e74 2f74 6829 0a20 2020 2020 2020 2022  nt/th).        "
+00029700: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
+00029710: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
+00029720: 2020 2020 2020 2027 5f63 6c61 7373 273a         '_class':
+00029730: 205f 636c 6173 732c 0a20 2020 2020 2020   _class,.       
+00029740: 2020 2020 2027 6964 273a 2069 642c 0a20       'id': id,. 
+00029750: 2020 2020 2020 2020 2020 2027 7374 796c             'styl
+00029760: 6527 3a20 7374 796c 652c 0a20 2020 2020  e': style,.     
+00029770: 2020 2020 2020 2027 7363 6f70 6527 3a20         'scope': 
+00029780: 7363 6f70 652c 0a20 2020 2020 2020 2020  scope,.         
+00029790: 2020 2027 636f 6c73 7061 6e27 3a20 636f     'colspan': co
+000297a0: 6c73 7061 6e2c 0a20 2020 2020 2020 2020  lspan,.         
+000297b0: 2020 2027 726f 7773 7061 6e27 3a20 726f     'rowspan': ro
+000297c0: 7773 7061 6e2c 0a20 2020 2020 2020 207d  wspan,.        }
+000297d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000297e0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
+000297f0: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
+00029800: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
+00029810: 6566 205f 6765 745f 6465 6661 756c 745f  ef _get_default_
+00029820: 6174 7472 6962 7574 6573 2873 656c 662c  attributes(self,
+00029830: 2067 6976 656e 3a20 6469 6374 5b73 7472   given: dict[str
+00029840: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
+00029850: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
+00029860: 7474 7269 6275 7465 5479 7065 5d3a 0a20  ttributeType]:. 
+00029870: 2020 2020 2020 2072 6574 7572 6e20 7b27         return {'
+00029880: 7363 6f70 6527 3a20 4e6f 6e65 2c20 2763  scope': None, 'c
+00029890: 6f6c 7370 616e 273a 204e 6f6e 652c 2027  olspan': None, '
+000298a0: 726f 7773 7061 6e27 3a20 4e6f 6e65 7d0a  rowspan': None}.
+000298b0: 0a0a 636c 6173 7320 7468 6561 6428 5461  ..class thead(Ta
+000298c0: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
+000298d0: 456e 6361 7073 756c 6174 6573 2061 2073  Encapsulates a s
+000298e0: 6574 206f 6620 7461 626c 6520 726f 7773  et of table rows
+000298f0: 2028 5b60 3c74 723e 605d 2868 7474 7073   ([`<tr>`](https
+00029900: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+00029910: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+00029920: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+00029930: 6d65 6e74 2f74 7229 2065 6c65 6d65 6e74  ment/tr) element
+00029940: 7329 2c20 696e 6469 6361 7469 6e67 2074  s), indicating t
+00029950: 6861 7420 7468 6579 2063 6f6d 7072 6973  hat they compris
+00029960: 6520 7468 6520 6865 6164 206f 6620 6120  e the head of a 
+00029970: 7461 626c 6520 7769 7468 2069 6e66 6f72  table with infor
+00029980: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+00029990: 2074 6162 6c65 2773 2063 6f6c 756d 6e73   table's columns
+000299a0: 2e20 5468 6973 2069 7320 7573 7561 6c6c  . This is usuall
+000299b0: 7920 696e 2074 6865 2066 6f72 6d20 6f66  y in the form of
+000299c0: 2063 6f6c 756d 6e20 6865 6164 6572 7320   column headers 
+000299d0: 285b 603c 7468 3e60 5d28 6874 7470 733a  ([`<th>`](https:
+000299e0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+000299f0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00029a00: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+00029a10: 656e 742f 7468 2920 656c 656d 656e 7473  ent/th) elements
+00029a20: 292e 0a0a 2020 2020 0a0a 2020 2020 5b56  )...    ..    [V
+00029a30: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+00029a40: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00029a50: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+00029a60: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+00029a70: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+00029a80: 742f 7468 6561 6429 0a20 2020 2022 2222  t/thead).    """
+00029a90: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00029aa0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00029ab0: 0a20 2020 2020 2020 202a 6368 696c 6472  .        *childr
+00029ac0: 656e 3a20 4368 696c 6472 656e 5479 7065  en: ChildrenType
+00029ad0: 2c0a 2020 2020 2020 2020 0a20 2020 2020  ,.        .     
+00029ae0: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
+00029af0: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
+00029b00: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+00029b10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00029b20: 2020 2045 6e63 6170 7375 6c61 7465 7320     Encapsulates 
+00029b30: 6120 7365 7420 6f66 2074 6162 6c65 2072  a set of table r
+00029b40: 6f77 7320 285b 603c 7472 3e60 5d28 6874  ows ([`<tr>`](ht
+00029b50: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+00029b60: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+00029b70: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+00029b80: 456c 656d 656e 742f 7472 2920 656c 656d  Element/tr) elem
+00029b90: 656e 7473 292c 2069 6e64 6963 6174 696e  ents), indicatin
+00029ba0: 6720 7468 6174 2074 6865 7920 636f 6d70  g that they comp
+00029bb0: 7269 7365 2074 6865 2068 6561 6420 6f66  rise the head of
+00029bc0: 2061 2074 6162 6c65 2077 6974 6820 696e   a table with in
+00029bd0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00029be0: 7468 6520 7461 626c 6527 7320 636f 6c75  the table's colu
+00029bf0: 6d6e 732e 2054 6869 7320 6973 2075 7375  mns. This is usu
+00029c00: 616c 6c79 2069 6e20 7468 6520 666f 726d  ally in the form
+00029c10: 206f 6620 636f 6c75 6d6e 2068 6561 6465   of column heade
+00029c20: 7273 2028 5b60 3c74 683e 605d 2868 7474  rs ([`<th>`](htt
+00029c30: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+00029c40: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+00029c50: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+00029c60: 6c65 6d65 6e74 2f74 6829 2065 6c65 6d65  lement/th) eleme
+00029c70: 6e74 7329 2e0a 0a20 2020 2020 2020 200a  nts)...        .
+00029c80: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
+00029c90: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+00029ca0: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+00029cb0: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
+00029cc0: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
+00029cd0: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 6865  HTML/Element/the
+00029ce0: 6164 290a 2020 2020 2020 2020 2222 220a  ad).        """.
+00029cf0: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
+00029d00: 6573 207c 3d20 7b0a 2020 2020 2020 2020  es |= {.        
+00029d10: 2020 2020 0a20 2020 2020 2020 207d 0a20      .        }. 
+00029d20: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00029d30: 5f69 6e69 745f 5f28 2a63 6869 6c64 7265  _init__(*childre
+00029d40: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
+00029d50: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+00029d60: 5f5f 2820 2023 2074 7970 653a 2069 676e  __(  # type: ign
+00029d70: 6f72 650a 2020 2020 2020 2020 7365 6c66  ore.        self
+00029d80: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
+00029d90: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
+00029da0: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
+00029db0: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
+00029dc0: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
+00029dd0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00029de0: 2222 220a 2020 2020 2020 2020 456e 6361  """.        Enca
+00029df0: 7073 756c 6174 6573 2061 2073 6574 206f  psulates a set o
+00029e00: 6620 7461 626c 6520 726f 7773 2028 5b60  f table rows ([`
+00029e10: 3c74 723e 605d 2868 7474 7073 3a2f 2f64  <tr>`](https://d
+00029e20: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+00029e30: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+00029e40: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+00029e50: 2f74 7229 2065 6c65 6d65 6e74 7329 2c20  /tr) elements), 
+00029e60: 696e 6469 6361 7469 6e67 2074 6861 7420  indicating that 
+00029e70: 7468 6579 2063 6f6d 7072 6973 6520 7468  they comprise th
+00029e80: 6520 6865 6164 206f 6620 6120 7461 626c  e head of a tabl
+00029e90: 6520 7769 7468 2069 6e66 6f72 6d61 7469  e with informati
+00029ea0: 6f6e 2061 626f 7574 2074 6865 2074 6162  on about the tab
+00029eb0: 6c65 2773 2063 6f6c 756d 6e73 2e20 5468  le's columns. Th
+00029ec0: 6973 2069 7320 7573 7561 6c6c 7920 696e  is is usually in
+00029ed0: 2074 6865 2066 6f72 6d20 6f66 2063 6f6c   the form of col
+00029ee0: 756d 6e20 6865 6164 6572 7320 285b 603c  umn headers ([`<
+00029ef0: 7468 3e60 5d28 6874 7470 733a 2f2f 6465  th>`](https://de
+00029f00: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+00029f10: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+00029f20: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00029f30: 7468 2920 656c 656d 656e 7473 292e 0a0a  th) elements)...
+00029f40: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
+00029f50: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
+00029f60: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+00029f70: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+00029f80: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+00029f90: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+00029fa0: 656d 656e 742f 7468 6561 6429 0a20 2020  ement/thead).   
+00029fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00029fc0: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+00029fd0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00029fe0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00029ff0: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
+0002a000: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
+0002a010: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
+0002a020: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
+0002a030: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
+0002a040: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
+0002a050: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
+0002a060: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
+0002a070: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
+0002a080: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
+0002a090: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
+0002a0a0: 7472 2854 6167 293a 0a20 2020 2022 2222  tr(Tag):.    """
+0002a0b0: 0a20 2020 2044 6566 696e 6573 2061 2072  .    Defines a r
+0002a0c0: 6f77 206f 6620 6365 6c6c 7320 696e 2061  ow of cells in a
+0002a0d0: 2074 6162 6c65 2e20 5468 6520 726f 7727   table. The row'
+0002a0e0: 7320 6365 6c6c 7320 6361 6e20 7468 656e  s cells can then
+0002a0f0: 2062 6520 6573 7461 626c 6973 6865 6420   be established 
+0002a100: 7573 696e 6720 6120 6d69 7820 6f66 205b  using a mix of [
+0002a110: 603c 7464 3e60 5d28 6874 7470 733a 2f2f  `<td>`](https://
+0002a120: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002a130: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002a140: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002a150: 742f 7464 2920 2864 6174 6120 6365 6c6c  t/td) (data cell
+0002a160: 2920 616e 6420 5b60 3c74 683e 605d 2868  ) and [`<th>`](h
+0002a170: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0002a180: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+0002a190: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+0002a1a0: 2f45 6c65 6d65 6e74 2f74 6829 2028 6865  /Element/th) (he
+0002a1b0: 6164 6572 2063 656c 6c29 2065 6c65 6d65  ader cell) eleme
+0002a1c0: 6e74 732e 0a0a 2020 2020 0a0a 2020 2020  nts...    ..    
+0002a1d0: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+0002a1e0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+0002a1f0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002a200: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002a210: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002a220: 656e 742f 7472 290a 2020 2020 2222 220a  ent/tr).    """.
+0002a230: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002a240: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002a250: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+0002a260: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+0002a270: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0002a280: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+0002a290: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+0002a2a0: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+0002a2b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002a2c0: 2020 4465 6669 6e65 7320 6120 726f 7720    Defines a row 
+0002a2d0: 6f66 2063 656c 6c73 2069 6e20 6120 7461  of cells in a ta
+0002a2e0: 626c 652e 2054 6865 2072 6f77 2773 2063  ble. The row's c
+0002a2f0: 656c 6c73 2063 616e 2074 6865 6e20 6265  ells can then be
+0002a300: 2065 7374 6162 6c69 7368 6564 2075 7369   established usi
+0002a310: 6e67 2061 206d 6978 206f 6620 5b60 3c74  ng a mix of [`<t
+0002a320: 643e 605d 2868 7474 7073 3a2f 2f64 6576  d>`](https://dev
+0002a330: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+0002a340: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+0002a350: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f74  b/HTML/Element/t
+0002a360: 6429 2028 6461 7461 2063 656c 6c29 2061  d) (data cell) a
+0002a370: 6e64 205b 603c 7468 3e60 5d28 6874 7470  nd [`<th>`](http
+0002a380: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+0002a390: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+0002a3a0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+0002a3b0: 656d 656e 742f 7468 2920 2868 6561 6465  ement/th) (heade
+0002a3c0: 7220 6365 6c6c 2920 656c 656d 656e 7473  r cell) elements
+0002a3d0: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
+0002a3e0: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
+0002a3f0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+0002a400: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0002a410: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+0002a420: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+0002a430: 2f45 6c65 6d65 6e74 2f74 7229 0a20 2020  /Element/tr).   
+0002a440: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002a450: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+0002a460: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+0002a470: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0002a480: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+0002a490: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
+0002a4a0: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
+0002a4b0: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
+0002a4c0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+0002a4d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0002a4e0: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+0002a4f0: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+0002a500: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+0002a510: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+0002a520: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
+0002a530: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0002a540: 2020 2020 2044 6566 696e 6573 2061 2072       Defines a r
+0002a550: 6f77 206f 6620 6365 6c6c 7320 696e 2061  ow of cells in a
+0002a560: 2074 6162 6c65 2e20 5468 6520 726f 7727   table. The row'
+0002a570: 7320 6365 6c6c 7320 6361 6e20 7468 656e  s cells can then
+0002a580: 2062 6520 6573 7461 626c 6973 6865 6420   be established 
+0002a590: 7573 696e 6720 6120 6d69 7820 6f66 205b  using a mix of [
+0002a5a0: 603c 7464 3e60 5d28 6874 7470 733a 2f2f  `<td>`](https://
+0002a5b0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002a5c0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002a5d0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002a5e0: 742f 7464 2920 2864 6174 6120 6365 6c6c  t/td) (data cell
+0002a5f0: 2920 616e 6420 5b60 3c74 683e 605d 2868  ) and [`<th>`](h
+0002a600: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0002a610: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+0002a620: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+0002a630: 2f45 6c65 6d65 6e74 2f74 6829 2028 6865  /Element/th) (he
+0002a640: 6164 6572 2063 656c 6c29 2065 6c65 6d65  ader cell) eleme
+0002a650: 6e74 732e 0a0a 2020 2020 2020 2020 0a0a  nts...        ..
+0002a660: 2020 2020 2020 2020 5b56 6965 7720 6675          [View fu
+0002a670: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+0002a680: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+0002a690: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+0002a6a0: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+0002a6b0: 544d 4c2f 456c 656d 656e 742f 7472 290a  TML/Element/tr).
+0002a6c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002a6d0: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
+0002a6e0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002a6f0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0002a700: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+0002a710: 292e 5f5f 6361 6c6c 5f5f 282a 6368 696c  ).__call__(*chil
+0002a720: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
+0002a730: 6573 290a 0a20 2020 2064 6566 205f 6765  es)..    def _ge
+0002a740: 745f 6465 6661 756c 745f 6174 7472 6962  t_default_attrib
+0002a750: 7574 6573 2873 656c 662c 2067 6976 656e  utes(self, given
+0002a760: 3a20 6469 6374 5b73 7472 2c20 4174 7472  : dict[str, Attr
+0002a770: 6962 7574 6554 7970 655d 2920 2d3e 2064  ibuteType]) -> d
+0002a780: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
+0002a790: 7465 5479 7065 5d3a 0a20 2020 2020 2020  teType]:.       
+0002a7a0: 2072 6574 7572 6e20 7b7d 0a0a 0a63 6c61   return {}...cla
+0002a7b0: 7373 2062 7574 746f 6e28 5461 6729 3a0a  ss button(Tag):.
+0002a7c0: 2020 2020 2222 220a 2020 2020 416e 2069      """.    An i
+0002a7d0: 6e74 6572 6163 7469 7665 2065 6c65 6d65  nteractive eleme
+0002a7e0: 6e74 2061 6374 6976 6174 6564 2062 7920  nt activated by 
+0002a7f0: 6120 7573 6572 2077 6974 6820 6120 6d6f  a user with a mo
+0002a800: 7573 652c 206b 6579 626f 6172 642c 2066  use, keyboard, f
+0002a810: 696e 6765 722c 2076 6f69 6365 2063 6f6d  inger, voice com
+0002a820: 6d61 6e64 2c20 6f72 206f 7468 6572 2061  mand, or other a
+0002a830: 7373 6973 7469 7665 2074 6563 686e 6f6c  ssistive technol
+0002a840: 6f67 792e 204f 6e63 6520 6163 7469 7661  ogy. Once activa
+0002a850: 7465 642c 2069 7420 7065 7266 6f72 6d73  ted, it performs
+0002a860: 2061 6e20 6163 7469 6f6e 2c20 7375 6368   an action, such
+0002a870: 2061 7320 7375 626d 6974 7469 6e67 2061   as submitting a
+0002a880: 205b 666f 726d 5d28 2f65 6e2d 5553 2f64   [form](/en-US/d
+0002a890: 6f63 732f 4c65 6172 6e2f 466f 726d 7329  ocs/Learn/Forms)
+0002a8a0: 206f 7220 6f70 656e 696e 6720 6120 6469   or opening a di
+0002a8b0: 616c 6f67 2e0a 0a20 2020 202a 2060 666f  alog...    * `fo
+0002a8c0: 726d 6d65 7468 6f64 603a 2054 6865 2048  rmmethod`: The H
+0002a8d0: 5454 5020 7265 7175 6573 7420 6d65 7468  TTP request meth
+0002a8e0: 6f64 2074 6f20 7573 6520 6f6e 2063 6c69  od to use on cli
+0002a8f0: 636b 2e20 4765 6e65 7261 6c6c 792c 2069  ck. Generally, i
+0002a900: 7420 6973 2070 7265 6665 7272 6564 2074  t is preferred t
+0002a910: 6f20 7365 7420 7468 6520 606d 6574 686f  o set the `metho
+0002a920: 6460 2061 7474 7269 6275 7465 206f 6e20  d` attribute on 
+0002a930: 7468 6520 603c 666f 726d 3e60 2065 6c65  the `<form>` ele
+0002a940: 6d65 6e74 2069 6e73 7465 6164 206f 6620  ment instead of 
+0002a950: 7468 6973 2e0a 2020 2020 2a20 6066 6f72  this..    * `for
+0002a960: 6d61 6374 696f 6e60 3a20 5468 6520 5552  maction`: The UR
+0002a970: 4c20 746f 2072 6571 7565 7374 2074 6f20  L to request to 
+0002a980: 6f6e 2063 6c69 636b 2e20 4765 6e65 7261  on click. Genera
+0002a990: 6c6c 792c 2069 7420 6973 2070 7265 6665  lly, it is prefe
+0002a9a0: 7272 6564 2074 6f20 7365 7420 7468 6520  rred to set the 
+0002a9b0: 6061 6374 696f 6e60 2061 7474 7269 6275  `action` attribu
+0002a9c0: 7465 206f 6e20 7468 6520 603c 666f 726d  te on the `<form
+0002a9d0: 3e60 2065 6c65 6d65 6e74 2069 6e73 7465  >` element inste
+0002a9e0: 6164 206f 6620 7468 6973 2e0a 0a20 2020  ad of this...   
+0002a9f0: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+0002aa00: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+0002aa10: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+0002aa20: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+0002aa30: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+0002aa40: 6d65 6e74 2f62 7574 746f 6e29 0a20 2020  ment/button).   
+0002aa50: 2022 2222 0a20 2020 2064 6566 205f 5f69   """.    def __i
+0002aa60: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+0002aa70: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
+0002aa80: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
+0002aa90: 5479 7065 2c0a 2020 2020 2020 2020 666f  Type,.        fo
+0002aaa0: 726d 6d65 7468 6f64 3a20 4174 7472 6962  rmmethod: Attrib
+0002aab0: 7574 6554 7970 6520 3d20 4e6f 6e65 2c0a  uteType = None,.
+0002aac0: 2020 2020 2020 2020 666f 726d 6163 7469          formacti
+0002aad0: 6f6e 3a20 4174 7472 6962 7574 6554 7970  on: AttributeTyp
+0002aae0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+0002aaf0: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
+0002ab00: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0002ab10: 2020 2020 5f63 6c61 7373 3a20 4f70 7469      _class: Opti
+0002ab20: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0002ab30: 2c0a 2020 2020 2020 2020 7374 796c 653a  ,.        style:
+0002ab40: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0002ab50: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+0002ab60: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
+0002ab70: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
+0002ab80: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0002ab90: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
+0002aba0: 6e20 696e 7465 7261 6374 6976 6520 656c  n interactive el
+0002abb0: 656d 656e 7420 6163 7469 7661 7465 6420  ement activated 
+0002abc0: 6279 2061 2075 7365 7220 7769 7468 2061  by a user with a
+0002abd0: 206d 6f75 7365 2c20 6b65 7962 6f61 7264   mouse, keyboard
+0002abe0: 2c20 6669 6e67 6572 2c20 766f 6963 6520  , finger, voice 
+0002abf0: 636f 6d6d 616e 642c 206f 7220 6f74 6865  command, or othe
+0002ac00: 7220 6173 7369 7374 6976 6520 7465 6368  r assistive tech
+0002ac10: 6e6f 6c6f 6779 2e20 4f6e 6365 2061 6374  nology. Once act
+0002ac20: 6976 6174 6564 2c20 6974 2070 6572 666f  ivated, it perfo
+0002ac30: 726d 7320 616e 2061 6374 696f 6e2c 2073  rms an action, s
+0002ac40: 7563 6820 6173 2073 7562 6d69 7474 696e  uch as submittin
+0002ac50: 6720 6120 5b66 6f72 6d5d 282f 656e 2d55  g a [form](/en-U
+0002ac60: 532f 646f 6373 2f4c 6561 726e 2f46 6f72  S/docs/Learn/For
+0002ac70: 6d73 2920 6f72 206f 7065 6e69 6e67 2061  ms) or opening a
+0002ac80: 2064 6961 6c6f 672e 0a0a 2020 2020 2020   dialog...      
+0002ac90: 2020 2a20 6066 6f72 6d6d 6574 686f 6460    * `formmethod`
+0002aca0: 3a20 5468 6520 4854 5450 2072 6571 7565  : The HTTP reque
+0002acb0: 7374 206d 6574 686f 6420 746f 2075 7365  st method to use
+0002acc0: 206f 6e20 636c 6963 6b2e 2047 656e 6572   on click. Gener
+0002acd0: 616c 6c79 2c20 6974 2069 7320 7072 6566  ally, it is pref
+0002ace0: 6572 7265 6420 746f 2073 6574 2074 6865  erred to set the
+0002acf0: 2060 6d65 7468 6f64 6020 6174 7472 6962   `method` attrib
+0002ad00: 7574 6520 6f6e 2074 6865 2060 3c66 6f72  ute on the `<for
+0002ad10: 6d3e 6020 656c 656d 656e 7420 696e 7374  m>` element inst
+0002ad20: 6561 6420 6f66 2074 6869 732e 0a20 2020  ead of this..   
+0002ad30: 2020 2020 202a 2060 666f 726d 6163 7469       * `formacti
+0002ad40: 6f6e 603a 2054 6865 2055 524c 2074 6f20  on`: The URL to 
+0002ad50: 7265 7175 6573 7420 746f 206f 6e20 636c  request to on cl
+0002ad60: 6963 6b2e 2047 656e 6572 616c 6c79 2c20  ick. Generally, 
+0002ad70: 6974 2069 7320 7072 6566 6572 7265 6420  it is preferred 
+0002ad80: 746f 2073 6574 2074 6865 2060 6163 7469  to set the `acti
+0002ad90: 6f6e 6020 6174 7472 6962 7574 6520 6f6e  on` attribute on
+0002ada0: 2074 6865 2060 3c66 6f72 6d3e 6020 656c   the `<form>` el
+0002adb0: 656d 656e 7420 696e 7374 6561 6420 6f66  ement instead of
+0002adc0: 2074 6869 732e 0a0a 2020 2020 2020 2020   this...        
+0002add0: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+0002ade0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+0002adf0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002ae00: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002ae10: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002ae20: 656e 742f 6275 7474 6f6e 290a 2020 2020  ent/button).    
+0002ae30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002ae40: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002ae50: 2020 2020 2020 2020 2020 2020 275f 636c              '_cl
+0002ae60: 6173 7327 3a20 5f63 6c61 7373 2c0a 2020  ass': _class,.  
+0002ae70: 2020 2020 2020 2020 2020 2769 6427 3a20            'id': 
+0002ae80: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002ae90: 2773 7479 6c65 273a 2073 7479 6c65 2c0a  'style': style,.
+0002aea0: 2020 2020 2020 2020 2020 2020 2766 6f72              'for
+0002aeb0: 6d6d 6574 686f 6427 3a20 666f 726d 6d65  mmethod': formme
+0002aec0: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
+0002aed0: 2020 2766 6f72 6d61 6374 696f 6e27 3a20    'formaction': 
+0002aee0: 666f 726d 6163 7469 6f6e 2c0a 2020 2020  formaction,.    
+0002aef0: 2020 2020 7d0a 2020 2020 2020 2020 7375      }.        su
+0002af00: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
+0002af10: 6368 696c 6472 656e 2c20 2a2a 6174 7472  children, **attr
+0002af20: 6962 7574 6573 290a 0a20 2020 2064 6566  ibutes)..    def
+0002af30: 205f 5f63 616c 6c5f 5f28 2020 2320 7479   __call__(  # ty
+0002af40: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+0002af50: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002af60: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
+0002af70: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
+0002af80: 2020 666f 726d 6d65 7468 6f64 3a20 4174    formmethod: At
+0002af90: 7472 6962 7574 6554 7970 6520 3d20 4e6f  tributeType = No
+0002afa0: 6e65 2c0a 2020 2020 2020 2020 666f 726d  ne,.        form
+0002afb0: 6163 7469 6f6e 3a20 4174 7472 6962 7574  action: Attribut
+0002afc0: 6554 7970 6520 3d20 4e6f 6e65 2c0a 2020  eType = None,.  
+0002afd0: 2020 2020 2020 6964 3a20 4f70 7469 6f6e        id: Option
+0002afe0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0002aff0: 2020 2020 2020 2020 5f63 6c61 7373 3a20          _class: 
+0002b000: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0002b010: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+0002b020: 796c 653a 204f 7074 696f 6e61 6c5b 7374  yle: Optional[st
+0002b030: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0002b040: 2020 202a 2a61 7474 7269 6275 7465 733a     **attributes:
+0002b050: 2041 7474 7269 6275 7465 5479 7065 2c0a   AttributeType,.
+0002b060: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+0002b070: 2222 0a20 2020 2020 2020 2041 6e20 696e  "".        An in
+0002b080: 7465 7261 6374 6976 6520 656c 656d 656e  teractive elemen
+0002b090: 7420 6163 7469 7661 7465 6420 6279 2061  t activated by a
+0002b0a0: 2075 7365 7220 7769 7468 2061 206d 6f75   user with a mou
+0002b0b0: 7365 2c20 6b65 7962 6f61 7264 2c20 6669  se, keyboard, fi
+0002b0c0: 6e67 6572 2c20 766f 6963 6520 636f 6d6d  nger, voice comm
+0002b0d0: 616e 642c 206f 7220 6f74 6865 7220 6173  and, or other as
+0002b0e0: 7369 7374 6976 6520 7465 6368 6e6f 6c6f  sistive technolo
+0002b0f0: 6779 2e20 4f6e 6365 2061 6374 6976 6174  gy. Once activat
+0002b100: 6564 2c20 6974 2070 6572 666f 726d 7320  ed, it performs 
+0002b110: 616e 2061 6374 696f 6e2c 2073 7563 6820  an action, such 
+0002b120: 6173 2073 7562 6d69 7474 696e 6720 6120  as submitting a 
+0002b130: 5b66 6f72 6d5d 282f 656e 2d55 532f 646f  [form](/en-US/do
+0002b140: 6373 2f4c 6561 726e 2f46 6f72 6d73 2920  cs/Learn/Forms) 
+0002b150: 6f72 206f 7065 6e69 6e67 2061 2064 6961  or opening a dia
+0002b160: 6c6f 672e 0a0a 2020 2020 2020 2020 2a20  log...        * 
+0002b170: 6066 6f72 6d6d 6574 686f 6460 3a20 5468  `formmethod`: Th
+0002b180: 6520 4854 5450 2072 6571 7565 7374 206d  e HTTP request m
+0002b190: 6574 686f 6420 746f 2075 7365 206f 6e20  ethod to use on 
+0002b1a0: 636c 6963 6b2e 2047 656e 6572 616c 6c79  click. Generally
+0002b1b0: 2c20 6974 2069 7320 7072 6566 6572 7265  , it is preferre
+0002b1c0: 6420 746f 2073 6574 2074 6865 2060 6d65  d to set the `me
+0002b1d0: 7468 6f64 6020 6174 7472 6962 7574 6520  thod` attribute 
+0002b1e0: 6f6e 2074 6865 2060 3c66 6f72 6d3e 6020  on the `<form>` 
+0002b1f0: 656c 656d 656e 7420 696e 7374 6561 6420  element instead 
+0002b200: 6f66 2074 6869 732e 0a20 2020 2020 2020  of this..       
+0002b210: 202a 2060 666f 726d 6163 7469 6f6e 603a   * `formaction`:
+0002b220: 2054 6865 2055 524c 2074 6f20 7265 7175   The URL to requ
+0002b230: 6573 7420 746f 206f 6e20 636c 6963 6b2e  est to on click.
+0002b240: 2047 656e 6572 616c 6c79 2c20 6974 2069   Generally, it i
+0002b250: 7320 7072 6566 6572 7265 6420 746f 2073  s preferred to s
+0002b260: 6574 2074 6865 2060 6163 7469 6f6e 6020  et the `action` 
+0002b270: 6174 7472 6962 7574 6520 6f6e 2074 6865  attribute on the
+0002b280: 2060 3c66 6f72 6d3e 6020 656c 656d 656e   `<form>` elemen
+0002b290: 7420 696e 7374 6561 6420 6f66 2074 6869  t instead of thi
+0002b2a0: 732e 0a0a 2020 2020 2020 2020 5b56 6965  s...        [Vie
+0002b2b0: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+0002b2c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+0002b2d0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002b2e0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002b2f0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002b300: 6275 7474 6f6e 290a 2020 2020 2020 2020  button).        
+0002b310: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+0002b320: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+0002b330: 2020 2020 2020 2020 275f 636c 6173 7327          '_class'
+0002b340: 3a20 5f63 6c61 7373 2c0a 2020 2020 2020  : _class,.      
+0002b350: 2020 2020 2020 2769 6427 3a20 6964 2c0a        'id': id,.
+0002b360: 2020 2020 2020 2020 2020 2020 2773 7479              'sty
+0002b370: 6c65 273a 2073 7479 6c65 2c0a 2020 2020  le': style,.    
+0002b380: 2020 2020 2020 2020 2766 6f72 6d6d 6574          'formmet
+0002b390: 686f 6427 3a20 666f 726d 6d65 7468 6f64  hod': formmethod
+0002b3a0: 2c0a 2020 2020 2020 2020 2020 2020 2766  ,.            'f
+0002b3b0: 6f72 6d61 6374 696f 6e27 3a20 666f 726d  ormaction': form
+0002b3c0: 6163 7469 6f6e 2c0a 2020 2020 2020 2020  action,.        
+0002b3d0: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
+0002b3e0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
+0002b3f0: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
+0002b400: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
+0002b410: 6465 6620 5f67 6574 5f64 6566 6175 6c74  def _get_default
+0002b420: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
+0002b430: 2c20 6769 7665 6e3a 2064 6963 745b 7374  , given: dict[st
+0002b440: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
+0002b450: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
+0002b460: 4174 7472 6962 7574 6554 7970 655d 3a0a  AttributeType]:.
+0002b470: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0002b480: 2766 6f72 6d6d 6574 686f 6427 3a20 4e6f  'formmethod': No
+0002b490: 6e65 2c20 2766 6f72 6d61 6374 696f 6e27  ne, 'formaction'
+0002b4a0: 3a20 4e6f 6e65 7d0a 0a0a 636c 6173 7320  : None}...class 
+0002b4b0: 6461 7461 6c69 7374 2854 6167 293a 0a20  datalist(Tag):. 
+0002b4c0: 2020 2022 2222 0a20 2020 2043 6f6e 7461     """.    Conta
+0002b4d0: 696e 7320 6120 7365 7420 6f66 205b 603c  ins a set of [`<
+0002b4e0: 6f70 7469 6f6e 3e60 5d28 6874 7470 733a  option>`](https:
+0002b4f0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002b500: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002b510: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002b520: 656e 742f 6f70 7469 6f6e 2920 656c 656d  ent/option) elem
+0002b530: 656e 7473 2074 6861 7420 7265 7072 6573  ents that repres
+0002b540: 656e 7420 7468 6520 7065 726d 6973 7369  ent the permissi
+0002b550: 626c 6520 6f72 2072 6563 6f6d 6d65 6e64  ble or recommend
+0002b560: 6564 206f 7074 696f 6e73 2061 7661 696c  ed options avail
+0002b570: 6162 6c65 2074 6f20 6368 6f6f 7365 2066  able to choose f
+0002b580: 726f 6d20 7769 7468 696e 206f 7468 6572  rom within other
+0002b590: 2063 6f6e 7472 6f6c 732e 0a0a 2020 2020   controls...    
+0002b5a0: 0a0a 2020 2020 5b56 6965 7720 6675 6c6c  ..    [View full
+0002b5b0: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+0002b5c0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002b5d0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002b5e0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002b5f0: 4c2f 456c 656d 656e 742f 6461 7461 6c69  L/Element/datali
+0002b600: 7374 290a 2020 2020 2222 220a 2020 2020  st).    """.    
+0002b610: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0002b620: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002b630: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
+0002b640: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
+0002b650: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+0002b660: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
+0002b670: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
+0002b680: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0002b690: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
+0002b6a0: 6e74 6169 6e73 2061 2073 6574 206f 6620  ntains a set of 
+0002b6b0: 5b60 3c6f 7074 696f 6e3e 605d 2868 7474  [`<option>`](htt
+0002b6c0: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+0002b6d0: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+0002b6e0: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+0002b6f0: 6c65 6d65 6e74 2f6f 7074 696f 6e29 2065  lement/option) e
+0002b700: 6c65 6d65 6e74 7320 7468 6174 2072 6570  lements that rep
+0002b710: 7265 7365 6e74 2074 6865 2070 6572 6d69  resent the permi
+0002b720: 7373 6962 6c65 206f 7220 7265 636f 6d6d  ssible or recomm
+0002b730: 656e 6465 6420 6f70 7469 6f6e 7320 6176  ended options av
+0002b740: 6169 6c61 626c 6520 746f 2063 686f 6f73  ailable to choos
+0002b750: 6520 6672 6f6d 2077 6974 6869 6e20 6f74  e from within ot
+0002b760: 6865 7220 636f 6e74 726f 6c73 2e0a 0a20  her controls... 
+0002b770: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+0002b780: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+0002b790: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+0002b7a0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+0002b7b0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+0002b7c0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+0002b7d0: 6d65 6e74 2f64 6174 616c 6973 7429 0a20  ment/datalist). 
+0002b7e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002b7f0: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
+0002b800: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
+0002b810: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0002b820: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+0002b830: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+0002b840: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+0002b850: 2064 6566 205f 5f63 616c 6c5f 5f28 2020   def __call__(  
+0002b860: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
+0002b870: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0002b880: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
+0002b890: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
+0002b8a0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+0002b8b0: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
+0002b8c0: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
+0002b8d0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0002b8e0: 2020 2020 2020 2043 6f6e 7461 696e 7320         Contains 
+0002b8f0: 6120 7365 7420 6f66 205b 603c 6f70 7469  a set of [`<opti
+0002b900: 6f6e 3e60 5d28 6874 7470 733a 2f2f 6465  on>`](https://de
+0002b910: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002b920: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002b930: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002b940: 6f70 7469 6f6e 2920 656c 656d 656e 7473  option) elements
+0002b950: 2074 6861 7420 7265 7072 6573 656e 7420   that represent 
+0002b960: 7468 6520 7065 726d 6973 7369 626c 6520  the permissible 
+0002b970: 6f72 2072 6563 6f6d 6d65 6e64 6564 206f  or recommended o
+0002b980: 7074 696f 6e73 2061 7661 696c 6162 6c65  ptions available
+0002b990: 2074 6f20 6368 6f6f 7365 2066 726f 6d20   to choose from 
+0002b9a0: 7769 7468 696e 206f 7468 6572 2063 6f6e  within other con
+0002b9b0: 7472 6f6c 732e 0a0a 2020 2020 2020 2020  trols...        
+0002b9c0: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+0002b9d0: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+0002b9e0: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+0002b9f0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002ba00: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002ba10: 2f48 544d 4c2f 456c 656d 656e 742f 6461  /HTML/Element/da
+0002ba20: 7461 6c69 7374 290a 2020 2020 2020 2020  talist).        
+0002ba30: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+0002ba40: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+0002ba50: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0002ba60: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+0002ba70: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
+0002ba80: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+0002ba90: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+0002baa0: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
+0002bab0: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
+0002bac0: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
+0002bad0: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
+0002bae0: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
+0002baf0: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
+0002bb00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002bb10: 7b7d 0a0a 0a63 6c61 7373 2066 6965 6c64  {}...class field
+0002bb20: 7365 7428 5461 6729 3a0a 2020 2020 2222  set(Tag):.    ""
+0002bb30: 220a 2020 2020 5573 6564 2074 6f20 6772  ".    Used to gr
+0002bb40: 6f75 7020 7365 7665 7261 6c20 636f 6e74  oup several cont
+0002bb50: 726f 6c73 2061 7320 7765 6c6c 2061 7320  rols as well as 
+0002bb60: 6c61 6265 6c73 2028 5b60 3c6c 6162 656c  labels ([`<label
+0002bb70: 3e60 5d28 6874 7470 733a 2f2f 6465 7665  >`](https://deve
+0002bb80: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002bb90: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002bba0: 2f48 544d 4c2f 456c 656d 656e 742f 6c61  /HTML/Element/la
+0002bbb0: 6265 6c29 2920 7769 7468 696e 2061 2077  bel)) within a w
+0002bbc0: 6562 2066 6f72 6d2e 0a0a 2020 2020 0a0a  eb form...    ..
+0002bbd0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
+0002bbe0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+0002bbf0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+0002bc00: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+0002bc10: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+0002bc20: 456c 656d 656e 742f 6669 656c 6473 6574  Element/fieldset
+0002bc30: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
+0002bc40: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002bc50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002bc60: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+0002bc70: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+0002bc80: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+0002bc90: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+0002bca0: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
+0002bcb0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0002bcc0: 2222 220a 2020 2020 2020 2020 5573 6564  """.        Used
+0002bcd0: 2074 6f20 6772 6f75 7020 7365 7665 7261   to group severa
+0002bce0: 6c20 636f 6e74 726f 6c73 2061 7320 7765  l controls as we
+0002bcf0: 6c6c 2061 7320 6c61 6265 6c73 2028 5b60  ll as labels ([`
+0002bd00: 3c6c 6162 656c 3e60 5d28 6874 7470 733a  <label>`](https:
+0002bd10: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002bd20: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002bd30: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002bd40: 656e 742f 6c61 6265 6c29 2920 7769 7468  ent/label)) with
+0002bd50: 696e 2061 2077 6562 2066 6f72 6d2e 0a0a  in a web form...
+0002bd60: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
+0002bd70: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
+0002bd80: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+0002bd90: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+0002bda0: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+0002bdb0: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+0002bdc0: 656d 656e 742f 6669 656c 6473 6574 290a  ement/fieldset).
+0002bdd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002bde0: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
+0002bdf0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002be00: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0002be10: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+0002be20: 745f 5f28 2a63 6869 6c64 7265 6e2c 202a  t__(*children, *
+0002be30: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
+0002be40: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2820    def __call__( 
+0002be50: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+0002be60: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002be70: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+0002be80: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+0002be90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0002bea0: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
+0002beb0: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
+0002bec0: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
+0002bed0: 2020 2020 2020 2020 5573 6564 2074 6f20          Used to 
+0002bee0: 6772 6f75 7020 7365 7665 7261 6c20 636f  group several co
+0002bef0: 6e74 726f 6c73 2061 7320 7765 6c6c 2061  ntrols as well a
+0002bf00: 7320 6c61 6265 6c73 2028 5b60 3c6c 6162  s labels ([`<lab
+0002bf10: 656c 3e60 5d28 6874 7470 733a 2f2f 6465  el>`](https://de
+0002bf20: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002bf30: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002bf40: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002bf50: 6c61 6265 6c29 2920 7769 7468 696e 2061  label)) within a
+0002bf60: 2077 6562 2066 6f72 6d2e 0a0a 2020 2020   web form...    
+0002bf70: 2020 2020 0a0a 2020 2020 2020 2020 5b56      ..        [V
+0002bf80: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+0002bf90: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+0002bfa0: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002bfb0: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002bfc0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002bfd0: 742f 6669 656c 6473 6574 290a 2020 2020  t/fieldset).    
+0002bfe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002bff0: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002c000: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0002c010: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+0002c020: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+0002c030: 6361 6c6c 5f5f 282a 6368 696c 6472 656e  call__(*children
+0002c040: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
+0002c050: 0a20 2020 2064 6566 205f 6765 745f 6465  .    def _get_de
+0002c060: 6661 756c 745f 6174 7472 6962 7574 6573  fault_attributes
+0002c070: 2873 656c 662c 2067 6976 656e 3a20 6469  (self, given: di
+0002c080: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
+0002c090: 6554 7970 655d 2920 2d3e 2064 6963 745b  eType]) -> dict[
+0002c0a0: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
+0002c0b0: 7065 5d3a 0a20 2020 2020 2020 2072 6574  pe]:.        ret
+0002c0c0: 7572 6e20 7b7d 0a0a 0a63 6c61 7373 2066  urn {}...class f
+0002c0d0: 6f72 6d28 5461 6729 3a0a 2020 2020 2222  orm(Tag):.    ""
+0002c0e0: 220a 2020 2020 5265 7072 6573 656e 7473  ".    Represents
+0002c0f0: 2061 2064 6f63 756d 656e 7420 7365 6374   a document sect
+0002c100: 696f 6e20 636f 6e74 6169 6e69 6e67 2069  ion containing i
+0002c110: 6e74 6572 6163 7469 7665 2063 6f6e 7472  nteractive contr
+0002c120: 6f6c 7320 666f 7220 7375 626d 6974 7469  ols for submitti
+0002c130: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2e0a  ng information..
+0002c140: 0a20 2020 202a 2060 6d65 7468 6f64 603a  .    * `method`:
+0002c150: 2054 6865 2048 5454 5020 7265 7175 6573   The HTTP reques
+0002c160: 7420 6d65 7468 6f64 2074 6f20 7573 6520  t method to use 
+0002c170: 7768 656e 2073 7562 6d69 7474 696e 6720  when submitting 
+0002c180: 7468 6973 2066 6f72 6d2e 2049 6e20 616c  this form. In al
+0002c190: 6d6f 7374 2061 6c6c 2063 6173 6573 2c20  most all cases, 
+0002c1a0: 796f 7527 6c6c 2077 616e 7420 7468 6973  you'll want this
+0002c1b0: 2074 6f20 6265 2050 4f53 542e 2028 6465   to be POST. (de
+0002c1c0: 6661 756c 7473 2074 6f20 6027 706f 7374  faults to `'post
+0002c1d0: 2760 290a 2020 2020 2a20 6061 6374 696f  '`).    * `actio
+0002c1e0: 6e60 3a20 5468 6520 5552 4c20 746f 2072  n`: The URL to r
+0002c1f0: 6571 7565 7374 2074 6f20 7768 656e 2073  equest to when s
+0002c200: 7562 6d69 7474 696e 6720 7468 6973 2066  ubmitting this f
+0002c210: 6f72 6d2e 2042 7920 6465 6661 756c 742c  orm. By default,
+0002c220: 2072 6571 7565 7374 7320 7769 6c6c 2062   requests will b
+0002c230: 6520 7365 6e74 2074 6f20 7468 6520 7361  e sent to the sa
+0002c240: 6d65 2055 524c 2061 7320 7468 6520 6375  me URL as the cu
+0002c250: 7272 656e 7420 7061 6765 2e0a 0a20 2020  rrent page...   
+0002c260: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+0002c270: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+0002c280: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+0002c290: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+0002c2a0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+0002c2b0: 6d65 6e74 2f66 6f72 6d29 0a20 2020 2022  ment/form).    "
+0002c2c0: 2222 0a20 2020 2064 6566 205f 5f69 6e69  "".    def __ini
+0002c2d0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002c2e0: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
+0002c2f0: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
+0002c300: 7065 2c0a 2020 2020 2020 2020 6d65 7468  pe,.        meth
+0002c310: 6f64 3a20 4f70 7469 6f6e 616c 5b4c 6974  od: Optional[Lit
+0002c320: 6572 616c 5b27 706f 7374 272c 2027 6765  eral['post', 'ge
+0002c330: 7427 5d5d 203d 204e 6f6e 652c 0a20 2020  t']] = None,.   
+0002c340: 2020 2020 2061 6374 696f 6e3a 2041 7474       action: Att
+0002c350: 7269 6275 7465 5479 7065 203d 204e 6f6e  ributeType = Non
+0002c360: 652c 0a20 2020 2020 2020 202a 2a61 7474  e,.        **att
+0002c370: 7269 6275 7465 733a 2041 7474 7269 6275  ributes: Attribu
+0002c380: 7465 5479 7065 2c0a 2020 2020 2920 2d3e  teType,.    ) ->
+0002c390: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0002c3a0: 2222 0a20 2020 2020 2020 2052 6570 7265  "".        Repre
+0002c3b0: 7365 6e74 7320 6120 646f 6375 6d65 6e74  sents a document
+0002c3c0: 2073 6563 7469 6f6e 2063 6f6e 7461 696e   section contain
+0002c3d0: 696e 6720 696e 7465 7261 6374 6976 6520  ing interactive 
+0002c3e0: 636f 6e74 726f 6c73 2066 6f72 2073 7562  controls for sub
+0002c3f0: 6d69 7474 696e 6720 696e 666f 726d 6174  mitting informat
+0002c400: 696f 6e2e 0a0a 2020 2020 2020 2020 2a20  ion...        * 
+0002c410: 606d 6574 686f 6460 3a20 5468 6520 4854  `method`: The HT
+0002c420: 5450 2072 6571 7565 7374 206d 6574 686f  TP request metho
+0002c430: 6420 746f 2075 7365 2077 6865 6e20 7375  d to use when su
+0002c440: 626d 6974 7469 6e67 2074 6869 7320 666f  bmitting this fo
+0002c450: 726d 2e20 496e 2061 6c6d 6f73 7420 616c  rm. In almost al
+0002c460: 6c20 6361 7365 732c 2079 6f75 276c 6c20  l cases, you'll 
+0002c470: 7761 6e74 2074 6869 7320 746f 2062 6520  want this to be 
+0002c480: 504f 5354 2e20 2864 6566 6175 6c74 7320  POST. (defaults 
+0002c490: 746f 2060 2770 6f73 7427 6029 0a20 2020  to `'post'`).   
+0002c4a0: 2020 2020 202a 2060 6163 7469 6f6e 603a       * `action`:
+0002c4b0: 2054 6865 2055 524c 2074 6f20 7265 7175   The URL to requ
+0002c4c0: 6573 7420 746f 2077 6865 6e20 7375 626d  est to when subm
+0002c4d0: 6974 7469 6e67 2074 6869 7320 666f 726d  itting this form
+0002c4e0: 2e20 4279 2064 6566 6175 6c74 2c20 7265  . By default, re
+0002c4f0: 7175 6573 7473 2077 696c 6c20 6265 2073  quests will be s
+0002c500: 656e 7420 746f 2074 6865 2073 616d 6520  ent to the same 
+0002c510: 5552 4c20 6173 2074 6865 2063 7572 7265  URL as the curre
+0002c520: 6e74 2070 6167 652e 0a0a 2020 2020 2020  nt page...      
+0002c530: 2020 5b56 6965 7720 6675 6c6c 2064 6f63    [View full doc
+0002c540: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+0002c550: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+0002c560: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+0002c570: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+0002c580: 656d 656e 742f 666f 726d 290a 2020 2020  ement/form).    
+0002c590: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002c5a0: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002c5b0: 2020 2020 2020 2020 2020 2020 276d 6574              'met
+0002c5c0: 686f 6427 3a20 6d65 7468 6f64 2c0a 2020  hod': method,.  
+0002c5d0: 2020 2020 2020 2020 2020 2761 6374 696f            'actio
+0002c5e0: 6e27 3a20 6163 7469 6f6e 2c0a 2020 2020  n': action,.    
+0002c5f0: 2020 2020 7d0a 2020 2020 2020 2020 7375      }.        su
+0002c600: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
+0002c610: 6368 696c 6472 656e 2c20 2a2a 6174 7472  children, **attr
+0002c620: 6962 7574 6573 290a 0a20 2020 2064 6566  ibutes)..    def
+0002c630: 205f 5f63 616c 6c5f 5f28 2020 2320 7479   __call__(  # ty
+0002c640: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+0002c650: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002c660: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
+0002c670: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
+0002c680: 2020 6d65 7468 6f64 3a20 4f70 7469 6f6e    method: Option
+0002c690: 616c 5b4c 6974 6572 616c 5b27 706f 7374  al[Literal['post
+0002c6a0: 272c 2027 6765 7427 5d5d 203d 204e 6f6e  ', 'get']] = Non
+0002c6b0: 652c 0a20 2020 2020 2020 2061 6374 696f  e,.        actio
+0002c6c0: 6e3a 2041 7474 7269 6275 7465 5479 7065  n: AttributeType
+0002c6d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002c6e0: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
+0002c6f0: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
+0002c700: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+0002c710: 0a20 2020 2020 2020 2052 6570 7265 7365  .        Represe
+0002c720: 6e74 7320 6120 646f 6375 6d65 6e74 2073  nts a document s
+0002c730: 6563 7469 6f6e 2063 6f6e 7461 696e 696e  ection containin
+0002c740: 6720 696e 7465 7261 6374 6976 6520 636f  g interactive co
+0002c750: 6e74 726f 6c73 2066 6f72 2073 7562 6d69  ntrols for submi
+0002c760: 7474 696e 6720 696e 666f 726d 6174 696f  tting informatio
+0002c770: 6e2e 0a0a 2020 2020 2020 2020 2a20 606d  n...        * `m
+0002c780: 6574 686f 6460 3a20 5468 6520 4854 5450  ethod`: The HTTP
+0002c790: 2072 6571 7565 7374 206d 6574 686f 6420   request method 
+0002c7a0: 746f 2075 7365 2077 6865 6e20 7375 626d  to use when subm
+0002c7b0: 6974 7469 6e67 2074 6869 7320 666f 726d  itting this form
+0002c7c0: 2e20 496e 2061 6c6d 6f73 7420 616c 6c20  . In almost all 
+0002c7d0: 6361 7365 732c 2079 6f75 276c 6c20 7761  cases, you'll wa
+0002c7e0: 6e74 2074 6869 7320 746f 2062 6520 504f  nt this to be PO
+0002c7f0: 5354 2e20 2864 6566 6175 6c74 7320 746f  ST. (defaults to
+0002c800: 2060 2770 6f73 7427 6029 0a20 2020 2020   `'post'`).     
+0002c810: 2020 202a 2060 6163 7469 6f6e 603a 2054     * `action`: T
+0002c820: 6865 2055 524c 2074 6f20 7265 7175 6573  he URL to reques
+0002c830: 7420 746f 2077 6865 6e20 7375 626d 6974  t to when submit
+0002c840: 7469 6e67 2074 6869 7320 666f 726d 2e20  ting this form. 
+0002c850: 4279 2064 6566 6175 6c74 2c20 7265 7175  By default, requ
+0002c860: 6573 7473 2077 696c 6c20 6265 2073 656e  ests will be sen
+0002c870: 7420 746f 2074 6865 2073 616d 6520 5552  t to the same UR
+0002c880: 4c20 6173 2074 6865 2063 7572 7265 6e74  L as the current
+0002c890: 2070 6167 652e 0a0a 2020 2020 2020 2020   page...        
+0002c8a0: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+0002c8b0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+0002c8c0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002c8d0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002c8e0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002c8f0: 656e 742f 666f 726d 290a 2020 2020 2020  ent/form).      
+0002c900: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
+0002c910: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
+0002c920: 2020 2020 2020 2020 2020 276d 6574 686f            'metho
+0002c930: 6427 3a20 6d65 7468 6f64 2c0a 2020 2020  d': method,.    
+0002c940: 2020 2020 2020 2020 2761 6374 696f 6e27          'action'
+0002c950: 3a20 6163 7469 6f6e 2c0a 2020 2020 2020  : action,.      
+0002c960: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
+0002c970: 726e 2073 7570 6572 2829 2e5f 5f63 616c  rn super().__cal
+0002c980: 6c5f 5f28 2a63 6869 6c64 7265 6e2c 202a  l__(*children, *
+0002c990: 2a61 7474 7269 6275 7465 7329 0a0a 2020  *attributes)..  
+0002c9a0: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
+0002c9b0: 6c74 5f61 7474 7269 6275 7465 7328 7365  lt_attributes(se
+0002c9c0: 6c66 2c20 6769 7665 6e3a 2064 6963 745b  lf, given: dict[
+0002c9d0: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
+0002c9e0: 7065 5d29 202d 3e20 6469 6374 5b73 7472  pe]) -> dict[str
+0002c9f0: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
+0002ca00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0002ca10: 207b 276d 6574 686f 6427 3a20 2770 6f73   {'method': 'pos
+0002ca20: 7427 2c20 2761 6374 696f 6e27 3a20 4e6f  t', 'action': No
+0002ca30: 6e65 7d0a 0a0a 636c 6173 7320 6c61 6265  ne}...class labe
+0002ca40: 6c28 5461 6729 3a0a 2020 2020 2222 220a  l(Tag):.    """.
+0002ca50: 2020 2020 5265 7072 6573 656e 7473 2061      Represents a
+0002ca60: 2063 6170 7469 6f6e 2066 6f72 2061 6e20   caption for an 
+0002ca70: 6974 656d 2069 6e20 6120 7573 6572 2069  item in a user i
+0002ca80: 6e74 6572 6661 6365 2e0a 0a20 2020 202a  nterface...    *
+0002ca90: 2060 666f 725f 603a 2049 4420 6f66 2069   `for_`: ID of i
+0002caa0: 6e70 7574 2066 6965 6c64 2074 6f20 6173  nput field to as
+0002cab0: 736f 6369 6174 6520 7468 6973 206c 6162  sociate this lab
+0002cac0: 656c 2077 6974 680a 0a20 2020 205b 5669  el with..    [Vi
+0002cad0: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
+0002cae0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+0002caf0: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+0002cb00: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+0002cb10: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+0002cb20: 2f6c 6162 656c 290a 2020 2020 2222 220a  /label).    """.
+0002cb30: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002cb40: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002cb50: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+0002cb60: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+0002cb70: 0a20 2020 2020 2020 2066 6f72 5f3a 2041  .        for_: A
+0002cb80: 7474 7269 6275 7465 5479 7065 203d 204e  ttributeType = N
+0002cb90: 6f6e 652c 0a20 2020 2020 2020 202a 2a61  one,.        **a
+0002cba0: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+0002cbb0: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
+0002cbc0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0002cbd0: 2022 2222 0a20 2020 2020 2020 2052 6570   """.        Rep
+0002cbe0: 7265 7365 6e74 7320 6120 6361 7074 696f  resents a captio
+0002cbf0: 6e20 666f 7220 616e 2069 7465 6d20 696e  n for an item in
+0002cc00: 2061 2075 7365 7220 696e 7465 7266 6163   a user interfac
+0002cc10: 652e 0a0a 2020 2020 2020 2020 2a20 6066  e...        * `f
+0002cc20: 6f72 5f60 3a20 4944 206f 6620 696e 7075  or_`: ID of inpu
+0002cc30: 7420 6669 656c 6420 746f 2061 7373 6f63  t field to assoc
+0002cc40: 6961 7465 2074 6869 7320 6c61 6265 6c20  iate this label 
+0002cc50: 7769 7468 0a0a 2020 2020 2020 2020 5b56  with..        [V
+0002cc60: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+0002cc70: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+0002cc80: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002cc90: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002cca0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002ccb0: 742f 6c61 6265 6c29 0a20 2020 2020 2020  t/label).       
+0002ccc0: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
+0002ccd0: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
+0002cce0: 2020 2020 2020 2020 2027 666f 725f 273a           'for_':
+0002ccf0: 2066 6f72 5f2c 0a20 2020 2020 2020 207d   for_,.        }
+0002cd00: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0002cd10: 2e5f 5f69 6e69 745f 5f28 2a63 6869 6c64  .__init__(*child
+0002cd20: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
+0002cd30: 7329 0a0a 2020 2020 6465 6620 5f5f 6361  s)..    def __ca
+0002cd40: 6c6c 5f5f 2820 2023 2074 7970 653a 2069  ll__(  # type: i
+0002cd50: 676e 6f72 650a 2020 2020 2020 2020 7365  gnore.        se
+0002cd60: 6c66 2c0a 2020 2020 2020 2020 2a63 6869  lf,.        *chi
+0002cd70: 6c64 7265 6e3a 2043 6869 6c64 7265 6e54  ldren: ChildrenT
+0002cd80: 7970 652c 0a20 2020 2020 2020 2066 6f72  ype,.        for
+0002cd90: 5f3a 2041 7474 7269 6275 7465 5479 7065  _: AttributeType
+0002cda0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002cdb0: 202a 2a61 7474 7269 6275 7465 733a 2041   **attributes: A
+0002cdc0: 7474 7269 6275 7465 5479 7065 2c0a 2020  ttributeType,.  
+0002cdd0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+0002cde0: 0a20 2020 2020 2020 2052 6570 7265 7365  .        Represe
+0002cdf0: 6e74 7320 6120 6361 7074 696f 6e20 666f  nts a caption fo
+0002ce00: 7220 616e 2069 7465 6d20 696e 2061 2075  r an item in a u
+0002ce10: 7365 7220 696e 7465 7266 6163 652e 0a0a  ser interface...
+0002ce20: 2020 2020 2020 2020 2a20 6066 6f72 5f60          * `for_`
+0002ce30: 3a20 4944 206f 6620 696e 7075 7420 6669  : ID of input fi
+0002ce40: 656c 6420 746f 2061 7373 6f63 6961 7465  eld to associate
+0002ce50: 2074 6869 7320 6c61 6265 6c20 7769 7468   this label with
+0002ce60: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+0002ce70: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+0002ce80: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+0002ce90: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002cea0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002ceb0: 2f48 544d 4c2f 456c 656d 656e 742f 6c61  /HTML/Element/la
+0002cec0: 6265 6c29 0a20 2020 2020 2020 2022 2222  bel).        """
+0002ced0: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+0002cee0: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+0002cef0: 2020 2020 2027 666f 725f 273a 2066 6f72       'for_': for
+0002cf00: 5f2c 0a20 2020 2020 2020 207d 0a20 2020  _,.        }.   
+0002cf10: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+0002cf20: 7228 292e 5f5f 6361 6c6c 5f5f 282a 6368  r().__call__(*ch
+0002cf30: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
+0002cf40: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
+0002cf50: 6765 745f 6465 6661 756c 745f 6174 7472  get_default_attr
+0002cf60: 6962 7574 6573 2873 656c 662c 2067 6976  ibutes(self, giv
+0002cf70: 656e 3a20 6469 6374 5b73 7472 2c20 4174  en: dict[str, At
+0002cf80: 7472 6962 7574 6554 7970 655d 2920 2d3e  tributeType]) ->
+0002cf90: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
+0002cfa0: 6275 7465 5479 7065 5d3a 0a20 2020 2020  buteType]:.     
+0002cfb0: 2020 2072 6574 7572 6e20 7b27 666f 725f     return {'for_
+0002cfc0: 273a 204e 6f6e 657d 0a0a 0a63 6c61 7373  ': None}...class
+0002cfd0: 206c 6567 656e 6428 5461 6729 3a0a 2020   legend(Tag):.  
+0002cfe0: 2020 2222 220a 2020 2020 5265 7072 6573    """.    Repres
+0002cff0: 656e 7473 2061 2063 6170 7469 6f6e 2066  ents a caption f
+0002d000: 6f72 2074 6865 2063 6f6e 7465 6e74 206f  or the content o
+0002d010: 6620 6974 7320 7061 7265 6e74 205b 603c  f its parent [`<
+0002d020: 6669 656c 6473 6574 3e60 5d28 6874 7470  fieldset>`](http
+0002d030: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+0002d040: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+0002d050: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+0002d060: 656d 656e 742f 6669 656c 6473 6574 292e  ement/fieldset).
+0002d070: 0a0a 2020 2020 0a0a 2020 2020 5b56 6965  ..    ..    [Vie
+0002d080: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+0002d090: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+0002d0a0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002d0b0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002d0c0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002d0d0: 6c65 6765 6e64 290a 2020 2020 2222 220a  legend).    """.
+0002d0e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002d0f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002d100: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+0002d110: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+0002d120: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0002d130: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+0002d140: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+0002d150: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+0002d160: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0002d170: 2020 5265 7072 6573 656e 7473 2061 2063    Represents a c
+0002d180: 6170 7469 6f6e 2066 6f72 2074 6865 2063  aption for the c
+0002d190: 6f6e 7465 6e74 206f 6620 6974 7320 7061  ontent of its pa
+0002d1a0: 7265 6e74 205b 603c 6669 656c 6473 6574  rent [`<fieldset
+0002d1b0: 3e60 5d28 6874 7470 733a 2f2f 6465 7665  >`](https://deve
+0002d1c0: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002d1d0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002d1e0: 2f48 544d 4c2f 456c 656d 656e 742f 6669  /HTML/Element/fi
+0002d1f0: 656c 6473 6574 292e 0a0a 2020 2020 2020  eldset)...      
+0002d200: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
+0002d210: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+0002d220: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+0002d230: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002d240: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002d250: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002d260: 6c65 6765 6e64 290a 2020 2020 2020 2020  legend).        
+0002d270: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+0002d280: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+0002d290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0002d2a0: 207d 0a20 2020 2020 2020 2073 7570 6572   }.        super
+0002d2b0: 2829 2e5f 5f69 6e69 745f 5f28 2a63 6869  ().__init__(*chi
+0002d2c0: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
+0002d2d0: 7465 7329 0a0a 2020 2020 6465 6620 5f5f  tes)..    def __
+0002d2e0: 6361 6c6c 5f5f 2820 2023 2074 7970 653a  call__(  # type:
+0002d2f0: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
+0002d300: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
+0002d310: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
+0002d320: 6e54 7970 652c 0a20 2020 2020 2020 200a  nType,.        .
+0002d330: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
+0002d340: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
+0002d350: 7970 652c 0a20 2020 2029 3a0a 2020 2020  ype,.    ):.    
+0002d360: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002d370: 5265 7072 6573 656e 7473 2061 2063 6170  Represents a cap
+0002d380: 7469 6f6e 2066 6f72 2074 6865 2063 6f6e  tion for the con
+0002d390: 7465 6e74 206f 6620 6974 7320 7061 7265  tent of its pare
+0002d3a0: 6e74 205b 603c 6669 656c 6473 6574 3e60  nt [`<fieldset>`
+0002d3b0: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+0002d3c0: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+0002d3d0: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+0002d3e0: 544d 4c2f 456c 656d 656e 742f 6669 656c  TML/Element/fiel
+0002d3f0: 6473 6574 292e 0a0a 2020 2020 2020 2020  dset)...        
+0002d400: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+0002d410: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+0002d420: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+0002d430: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002d440: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002d450: 2f48 544d 4c2f 456c 656d 656e 742f 6c65  /HTML/Element/le
+0002d460: 6765 6e64 290a 2020 2020 2020 2020 2222  gend).        ""
+0002d470: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
+0002d480: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
+0002d490: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
+0002d4a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002d4b0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
+0002d4c0: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
+0002d4d0: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
+0002d4e0: 6566 205f 6765 745f 6465 6661 756c 745f  ef _get_default_
+0002d4f0: 6174 7472 6962 7574 6573 2873 656c 662c  attributes(self,
+0002d500: 2067 6976 656e 3a20 6469 6374 5b73 7472   given: dict[str
+0002d510: 2c20 4174 7472 6962 7574 6554 7970 655d  , AttributeType]
+0002d520: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
+0002d530: 7474 7269 6275 7465 5479 7065 5d3a 0a20  ttributeType]:. 
+0002d540: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
+0002d550: 0a0a 0a63 6c61 7373 206d 6574 6572 2854  ...class meter(T
+0002d560: 6167 293a 0a20 2020 2022 2222 0a20 2020  ag):.    """.   
+0002d570: 2052 6570 7265 7365 6e74 7320 6569 7468   Represents eith
+0002d580: 6572 2061 2073 6361 6c61 7220 7661 6c75  er a scalar valu
+0002d590: 6520 7769 7468 696e 2061 206b 6e6f 776e  e within a known
+0002d5a0: 2072 616e 6765 206f 7220 6120 6672 6163   range or a frac
+0002d5b0: 7469 6f6e 616c 2076 616c 7565 2e0a 0a20  tional value... 
+0002d5c0: 2020 200a 0a20 2020 205b 5669 6577 2066     ..    [View f
+0002d5d0: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+0002d5e0: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+0002d5f0: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
+0002d600: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
+0002d610: 4854 4d4c 2f45 6c65 6d65 6e74 2f6d 6574  HTML/Element/met
+0002d620: 6572 290a 2020 2020 2222 220a 2020 2020  er).    """.    
+0002d630: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0002d640: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002d650: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
+0002d660: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
+0002d670: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+0002d680: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
+0002d690: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
+0002d6a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0002d6b0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0002d6c0: 7072 6573 656e 7473 2065 6974 6865 7220  presents either 
+0002d6d0: 6120 7363 616c 6172 2076 616c 7565 2077  a scalar value w
+0002d6e0: 6974 6869 6e20 6120 6b6e 6f77 6e20 7261  ithin a known ra
+0002d6f0: 6e67 6520 6f72 2061 2066 7261 6374 696f  nge or a fractio
+0002d700: 6e61 6c20 7661 6c75 652e 0a0a 2020 2020  nal value...    
+0002d710: 2020 2020 0a0a 2020 2020 2020 2020 5b56      ..        [V
+0002d720: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+0002d730: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+0002d740: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002d750: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002d760: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002d770: 742f 6d65 7465 7229 0a20 2020 2020 2020  t/meter).       
+0002d780: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
+0002d790: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
+0002d7a0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+0002d7b0: 2020 7d0a 2020 2020 2020 2020 7375 7065    }.        supe
+0002d7c0: 7228 292e 5f5f 696e 6974 5f5f 282a 6368  r().__init__(*ch
+0002d7d0: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
+0002d7e0: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
+0002d7f0: 5f63 616c 6c5f 5f28 2020 2320 7479 7065  _call__(  # type
+0002d800: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+0002d810: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0002d820: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
+0002d830: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
+0002d840: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
+0002d850: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
+0002d860: 5479 7065 2c0a 2020 2020 293a 0a20 2020  Type,.    ):.   
+0002d870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002d880: 2052 6570 7265 7365 6e74 7320 6569 7468   Represents eith
+0002d890: 6572 2061 2073 6361 6c61 7220 7661 6c75  er a scalar valu
+0002d8a0: 6520 7769 7468 696e 2061 206b 6e6f 776e  e within a known
+0002d8b0: 2072 616e 6765 206f 7220 6120 6672 6163   range or a frac
+0002d8c0: 7469 6f6e 616c 2076 616c 7565 2e0a 0a20  tional value... 
+0002d8d0: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+0002d8e0: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+0002d8f0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+0002d900: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+0002d910: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+0002d920: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+0002d930: 6d65 6e74 2f6d 6574 6572 290a 2020 2020  ment/meter).    
+0002d940: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002d950: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002d960: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0002d970: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+0002d980: 6574 7572 6e20 7375 7065 7228 292e 5f5f  eturn super().__
+0002d990: 6361 6c6c 5f5f 282a 6368 696c 6472 656e  call__(*children
+0002d9a0: 2c20 2a2a 6174 7472 6962 7574 6573 290a  , **attributes).
+0002d9b0: 0a20 2020 2064 6566 205f 6765 745f 6465  .    def _get_de
+0002d9c0: 6661 756c 745f 6174 7472 6962 7574 6573  fault_attributes
+0002d9d0: 2873 656c 662c 2067 6976 656e 3a20 6469  (self, given: di
+0002d9e0: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
+0002d9f0: 6554 7970 655d 2920 2d3e 2064 6963 745b  eType]) -> dict[
+0002da00: 7374 722c 2041 7474 7269 6275 7465 5479  str, AttributeTy
+0002da10: 7065 5d3a 0a20 2020 2020 2020 2072 6574  pe]:.        ret
+0002da20: 7572 6e20 7b7d 0a0a 0a63 6c61 7373 206f  urn {}...class o
+0002da30: 7074 6772 6f75 7028 5461 6729 3a0a 2020  ptgroup(Tag):.  
+0002da40: 2020 2222 220a 2020 2020 4372 6561 7465    """.    Create
+0002da50: 7320 6120 6772 6f75 7069 6e67 206f 6620  s a grouping of 
+0002da60: 6f70 7469 6f6e 7320 7769 7468 696e 2061  options within a
+0002da70: 205b 603c 7365 6c65 6374 3e60 5d28 6874   [`<select>`](ht
+0002da80: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+0002da90: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+0002daa0: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+0002dab0: 456c 656d 656e 742f 7365 6c65 6374 2920  Element/select) 
+0002dac0: 656c 656d 656e 742e 0a0a 2020 2020 0a0a  element...    ..
+0002dad0: 2020 2020 5b56 6965 7720 6675 6c6c 2064      [View full d
+0002dae0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+0002daf0: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+0002db00: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+0002db10: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+0002db20: 456c 656d 656e 742f 6f70 7467 726f 7570  Element/optgroup
+0002db30: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
+0002db40: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002db50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002db60: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+0002db70: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+0002db80: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+0002db90: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+0002dba0: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
+0002dbb0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0002dbc0: 2222 220a 2020 2020 2020 2020 4372 6561  """.        Crea
+0002dbd0: 7465 7320 6120 6772 6f75 7069 6e67 206f  tes a grouping o
+0002dbe0: 6620 6f70 7469 6f6e 7320 7769 7468 696e  f options within
+0002dbf0: 2061 205b 603c 7365 6c65 6374 3e60 5d28   a [`<select>`](
+0002dc00: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002dc10: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002dc20: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002dc30: 4c2f 456c 656d 656e 742f 7365 6c65 6374  L/Element/select
+0002dc40: 2920 656c 656d 656e 742e 0a0a 2020 2020  ) element...    
+0002dc50: 2020 2020 0a0a 2020 2020 2020 2020 5b56      ..        [V
+0002dc60: 6965 7720 6675 6c6c 2064 6f63 756d 656e  iew full documen
+0002dc70: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+0002dc80: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002dc90: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002dca0: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002dcb0: 742f 6f70 7467 726f 7570 290a 2020 2020  t/optgroup).    
+0002dcc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002dcd0: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002dce0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0002dcf0: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
+0002dd00: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+0002dd10: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
+0002dd20: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+0002dd30: 6620 5f5f 6361 6c6c 5f5f 2820 2023 2074  f __call__(  # t
+0002dd40: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+0002dd50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002dd60: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+0002dd70: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+0002dd80: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+0002dd90: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+0002dda0: 7574 6554 7970 652c 0a20 2020 2029 3a0a  uteType,.    ):.
+0002ddb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002ddc0: 2020 2020 4372 6561 7465 7320 6120 6772      Creates a gr
+0002ddd0: 6f75 7069 6e67 206f 6620 6f70 7469 6f6e  ouping of option
+0002dde0: 7320 7769 7468 696e 2061 205b 603c 7365  s within a [`<se
+0002ddf0: 6c65 6374 3e60 5d28 6874 7470 733a 2f2f  lect>`](https://
+0002de00: 6465 7665 6c6f 7065 722e 6d6f 7a69 6c6c  developer.mozill
+0002de10: 612e 6f72 672f 656e 2d55 532f 646f 6373  a.org/en-US/docs
+0002de20: 2f57 6562 2f48 544d 4c2f 456c 656d 656e  /Web/HTML/Elemen
+0002de30: 742f 7365 6c65 6374 2920 656c 656d 656e  t/select) elemen
+0002de40: 742e 0a0a 2020 2020 2020 2020 0a0a 2020  t...        ..  
+0002de50: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
+0002de60: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+0002de70: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002de80: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002de90: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002dea0: 4c2f 456c 656d 656e 742f 6f70 7467 726f  L/Element/optgro
+0002deb0: 7570 290a 2020 2020 2020 2020 2222 220a  up).        """.
+0002dec0: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
+0002ded0: 6573 207c 3d20 7b0a 2020 2020 2020 2020  es |= {.        
+0002dee0: 2020 2020 0a20 2020 2020 2020 207d 0a20      .        }. 
+0002def0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+0002df00: 7065 7228 292e 5f5f 6361 6c6c 5f5f 282a  per().__call__(*
+0002df10: 6368 696c 6472 656e 2c20 2a2a 6174 7472  children, **attr
+0002df20: 6962 7574 6573 290a 0a20 2020 2064 6566  ibutes)..    def
+0002df30: 205f 6765 745f 6465 6661 756c 745f 6174   _get_default_at
+0002df40: 7472 6962 7574 6573 2873 656c 662c 2067  tributes(self, g
+0002df50: 6976 656e 3a20 6469 6374 5b73 7472 2c20  iven: dict[str, 
+0002df60: 4174 7472 6962 7574 6554 7970 655d 2920  AttributeType]) 
+0002df70: 2d3e 2064 6963 745b 7374 722c 2041 7474  -> dict[str, Att
+0002df80: 7269 6275 7465 5479 7065 5d3a 0a20 2020  ributeType]:.   
+0002df90: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
+0002dfa0: 0a63 6c61 7373 206f 7074 696f 6e28 5461  .class option(Ta
+0002dfb0: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
+0002dfc0: 5573 6564 2074 6f20 6465 6669 6e65 2061  Used to define a
+0002dfd0: 6e20 6974 656d 2063 6f6e 7461 696e 6564  n item contained
+0002dfe0: 2069 6e20 6120 7365 6c65 6374 2c20 616e   in a select, an
+0002dff0: 205b 603c 6f70 7467 726f 7570 3e60 5d28   [`<optgroup>`](
+0002e000: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002e010: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002e020: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002e030: 4c2f 456c 656d 656e 742f 6f70 7467 726f  L/Element/optgro
+0002e040: 7570 292c 206f 7220 6120 5b60 3c64 6174  up), or a [`<dat
+0002e050: 616c 6973 743e 605d 2868 7474 7073 3a2f  alist>`](https:/
+0002e060: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+0002e070: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+0002e080: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+0002e090: 6e74 2f64 6174 616c 6973 7429 2065 6c65  nt/datalist) ele
+0002e0a0: 6d65 6e74 2e20 4173 2073 7563 682c 2060  ment. As such, `
+0002e0b0: 3c6f 7074 696f 6e3e 6020 6361 6e20 7265  <option>` can re
+0002e0c0: 7072 6573 656e 7420 6d65 6e75 2069 7465  present menu ite
+0002e0d0: 6d73 2069 6e20 706f 7075 7073 2061 6e64  ms in popups and
+0002e0e0: 206f 7468 6572 206c 6973 7473 206f 6620   other lists of 
+0002e0f0: 6974 656d 7320 696e 2061 6e20 4854 4d4c  items in an HTML
+0002e100: 2064 6f63 756d 656e 742e 0a0a 2020 2020   document...    
+0002e110: 0a0a 2020 2020 5b56 6965 7720 6675 6c6c  ..    [View full
+0002e120: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+0002e130: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002e140: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002e150: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002e160: 4c2f 456c 656d 656e 742f 6f70 7469 6f6e  L/Element/option
+0002e170: 290a 2020 2020 2222 220a 2020 2020 6465  ).    """.    de
+0002e180: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002e190: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002e1a0: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+0002e1b0: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+0002e1c0: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+0002e1d0: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+0002e1e0: 7574 6554 7970 652c 0a20 2020 2029 202d  uteType,.    ) -
+0002e1f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0002e200: 2222 220a 2020 2020 2020 2020 5573 6564  """.        Used
+0002e210: 2074 6f20 6465 6669 6e65 2061 6e20 6974   to define an it
+0002e220: 656d 2063 6f6e 7461 696e 6564 2069 6e20  em contained in 
+0002e230: 6120 7365 6c65 6374 2c20 616e 205b 603c  a select, an [`<
+0002e240: 6f70 7467 726f 7570 3e60 5d28 6874 7470  optgroup>`](http
+0002e250: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+0002e260: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+0002e270: 646f 6373 2f57 6562 2f48 544d 4c2f 456c  docs/Web/HTML/El
+0002e280: 656d 656e 742f 6f70 7467 726f 7570 292c  ement/optgroup),
+0002e290: 206f 7220 6120 5b60 3c64 6174 616c 6973   or a [`<datalis
+0002e2a0: 743e 605d 2868 7474 7073 3a2f 2f64 6576  t>`](https://dev
+0002e2b0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+0002e2c0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+0002e2d0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f64  b/HTML/Element/d
+0002e2e0: 6174 616c 6973 7429 2065 6c65 6d65 6e74  atalist) element
+0002e2f0: 2e20 4173 2073 7563 682c 2060 3c6f 7074  . As such, `<opt
+0002e300: 696f 6e3e 6020 6361 6e20 7265 7072 6573  ion>` can repres
+0002e310: 656e 7420 6d65 6e75 2069 7465 6d73 2069  ent menu items i
+0002e320: 6e20 706f 7075 7073 2061 6e64 206f 7468  n popups and oth
+0002e330: 6572 206c 6973 7473 206f 6620 6974 656d  er lists of item
+0002e340: 7320 696e 2061 6e20 4854 4d4c 2064 6f63  s in an HTML doc
+0002e350: 756d 656e 742e 0a0a 2020 2020 2020 2020  ument...        
+0002e360: 0a0a 2020 2020 2020 2020 5b56 6965 7720  ..        [View 
+0002e370: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+0002e380: 6f6e 5d28 6874 7470 733a 2f2f 6465 7665  on](https://deve
+0002e390: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+0002e3a0: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+0002e3b0: 2f48 544d 4c2f 456c 656d 656e 742f 6f70  /HTML/Element/op
+0002e3c0: 7469 6f6e 290a 2020 2020 2020 2020 2222  tion).        ""
+0002e3d0: 220a 2020 2020 2020 2020 6174 7472 6962  ".        attrib
+0002e3e0: 7574 6573 207c 3d20 7b0a 2020 2020 2020  utes |= {.      
+0002e3f0: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
+0002e400: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0002e410: 2e5f 5f69 6e69 745f 5f28 2a63 6869 6c64  .__init__(*child
+0002e420: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
+0002e430: 7329 0a0a 2020 2020 6465 6620 5f5f 6361  s)..    def __ca
+0002e440: 6c6c 5f5f 2820 2023 2074 7970 653a 2069  ll__(  # type: i
+0002e450: 676e 6f72 650a 2020 2020 2020 2020 7365  gnore.        se
+0002e460: 6c66 2c0a 2020 2020 2020 2020 2a63 6869  lf,.        *chi
+0002e470: 6c64 7265 6e3a 2043 6869 6c64 7265 6e54  ldren: ChildrenT
+0002e480: 7970 652c 0a20 2020 2020 2020 200a 2020  ype,.        .  
+0002e490: 2020 2020 2020 2a2a 6174 7472 6962 7574        **attribut
+0002e4a0: 6573 3a20 4174 7472 6962 7574 6554 7970  es: AttributeTyp
+0002e4b0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+0002e4c0: 2020 2222 220a 2020 2020 2020 2020 5573    """.        Us
+0002e4d0: 6564 2074 6f20 6465 6669 6e65 2061 6e20  ed to define an 
+0002e4e0: 6974 656d 2063 6f6e 7461 696e 6564 2069  item contained i
+0002e4f0: 6e20 6120 7365 6c65 6374 2c20 616e 205b  n a select, an [
+0002e500: 603c 6f70 7467 726f 7570 3e60 5d28 6874  `<optgroup>`](ht
+0002e510: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
+0002e520: 6d6f 7a69 6c6c 612e 6f72 672f 656e 2d55  mozilla.org/en-U
+0002e530: 532f 646f 6373 2f57 6562 2f48 544d 4c2f  S/docs/Web/HTML/
+0002e540: 456c 656d 656e 742f 6f70 7467 726f 7570  Element/optgroup
+0002e550: 292c 206f 7220 6120 5b60 3c64 6174 616c  ), or a [`<datal
+0002e560: 6973 743e 605d 2868 7474 7073 3a2f 2f64  ist>`](https://d
+0002e570: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+0002e580: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+0002e590: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+0002e5a0: 2f64 6174 616c 6973 7429 2065 6c65 6d65  /datalist) eleme
+0002e5b0: 6e74 2e20 4173 2073 7563 682c 2060 3c6f  nt. As such, `<o
+0002e5c0: 7074 696f 6e3e 6020 6361 6e20 7265 7072  ption>` can repr
+0002e5d0: 6573 656e 7420 6d65 6e75 2069 7465 6d73  esent menu items
+0002e5e0: 2069 6e20 706f 7075 7073 2061 6e64 206f   in popups and o
+0002e5f0: 7468 6572 206c 6973 7473 206f 6620 6974  ther lists of it
+0002e600: 656d 7320 696e 2061 6e20 4854 4d4c 2064  ems in an HTML d
+0002e610: 6f63 756d 656e 742e 0a0a 2020 2020 2020  ocument...      
+0002e620: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
+0002e630: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+0002e640: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+0002e650: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002e660: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002e670: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002e680: 6f70 7469 6f6e 290a 2020 2020 2020 2020  option).        
+0002e690: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+0002e6a0: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+0002e6b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0002e6c0: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+0002e6d0: 6e20 7375 7065 7228 292e 5f5f 6361 6c6c  n super().__call
+0002e6e0: 5f5f 282a 6368 696c 6472 656e 2c20 2a2a  __(*children, **
+0002e6f0: 6174 7472 6962 7574 6573 290a 0a20 2020  attributes)..   
+0002e700: 2064 6566 205f 6765 745f 6465 6661 756c   def _get_defaul
+0002e710: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
+0002e720: 662c 2067 6976 656e 3a20 6469 6374 5b73  f, given: dict[s
+0002e730: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
+0002e740: 655d 2920 2d3e 2064 6963 745b 7374 722c  e]) -> dict[str,
+0002e750: 2041 7474 7269 6275 7465 5479 7065 5d3a   AttributeType]:
+0002e760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e770: 7b7d 0a0a 0a63 6c61 7373 206f 7574 7075  {}...class outpu
+0002e780: 7428 5461 6729 3a0a 2020 2020 2222 220a  t(Tag):.    """.
+0002e790: 2020 2020 436f 6e74 6169 6e65 7220 656c      Container el
+0002e7a0: 656d 656e 7420 696e 746f 2077 6869 6368  ement into which
+0002e7b0: 2061 2073 6974 6520 6f72 2061 7070 2063   a site or app c
+0002e7c0: 616e 2069 6e6a 6563 7420 7468 6520 7265  an inject the re
+0002e7d0: 7375 6c74 7320 6f66 2061 2063 616c 6375  sults of a calcu
+0002e7e0: 6c61 7469 6f6e 206f 7220 7468 6520 6f75  lation or the ou
+0002e7f0: 7463 6f6d 6520 6f66 2061 2075 7365 7220  tcome of a user 
+0002e800: 6163 7469 6f6e 2e0a 0a20 2020 200a 0a20  action...    .. 
+0002e810: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+0002e820: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+0002e830: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+0002e840: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+0002e850: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+0002e860: 6c65 6d65 6e74 2f6f 7574 7075 7429 0a20  lement/output). 
+0002e870: 2020 2022 2222 0a20 2020 2064 6566 205f     """.    def _
+0002e880: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002e890: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0002e8a0: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
+0002e8b0: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
+0002e8c0: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
+0002e8d0: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
+0002e8e0: 5479 7065 2c0a 2020 2020 2920 2d3e 204e  Type,.    ) -> N
+0002e8f0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0002e900: 0a20 2020 2020 2020 2043 6f6e 7461 696e  .        Contain
+0002e910: 6572 2065 6c65 6d65 6e74 2069 6e74 6f20  er element into 
+0002e920: 7768 6963 6820 6120 7369 7465 206f 7220  which a site or 
+0002e930: 6170 7020 6361 6e20 696e 6a65 6374 2074  app can inject t
+0002e940: 6865 2072 6573 756c 7473 206f 6620 6120  he results of a 
+0002e950: 6361 6c63 756c 6174 696f 6e20 6f72 2074  calculation or t
+0002e960: 6865 206f 7574 636f 6d65 206f 6620 6120  he outcome of a 
+0002e970: 7573 6572 2061 6374 696f 6e2e 0a0a 2020  user action...  
+0002e980: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
+0002e990: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+0002e9a0: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+0002e9b0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+0002e9c0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+0002e9d0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+0002e9e0: 656e 742f 6f75 7470 7574 290a 2020 2020  ent/output).    
+0002e9f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002ea00: 6174 7472 6962 7574 6573 207c 3d20 7b0a  attributes |= {.
+0002ea10: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0002ea20: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
+0002ea30: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+0002ea40: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
+0002ea50: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+0002ea60: 6620 5f5f 6361 6c6c 5f5f 2820 2023 2074  f __call__(  # t
+0002ea70: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
+0002ea80: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002ea90: 2020 2a63 6869 6c64 7265 6e3a 2043 6869    *children: Chi
+0002eaa0: 6c64 7265 6e54 7970 652c 0a20 2020 2020  ldrenType,.     
+0002eab0: 2020 200a 2020 2020 2020 2020 2a2a 6174     .        **at
+0002eac0: 7472 6962 7574 6573 3a20 4174 7472 6962  tributes: Attrib
+0002ead0: 7574 6554 7970 652c 0a20 2020 2029 3a0a  uteType,.    ):.
+0002eae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002eaf0: 2020 2020 436f 6e74 6169 6e65 7220 656c      Container el
+0002eb00: 656d 656e 7420 696e 746f 2077 6869 6368  ement into which
+0002eb10: 2061 2073 6974 6520 6f72 2061 7070 2063   a site or app c
+0002eb20: 616e 2069 6e6a 6563 7420 7468 6520 7265  an inject the re
+0002eb30: 7375 6c74 7320 6f66 2061 2063 616c 6375  sults of a calcu
+0002eb40: 6c61 7469 6f6e 206f 7220 7468 6520 6f75  lation or the ou
+0002eb50: 7463 6f6d 6520 6f66 2061 2075 7365 7220  tcome of a user 
+0002eb60: 6163 7469 6f6e 2e0a 0a20 2020 2020 2020  action...       
+0002eb70: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
+0002eb80: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
+0002eb90: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
+0002eba0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+0002ebb0: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+0002ebc0: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f6f  b/HTML/Element/o
+0002ebd0: 7574 7075 7429 0a20 2020 2020 2020 2022  utput).        "
+0002ebe0: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
+0002ebf0: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
+0002ec00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0002ec10: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
+0002ec20: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
+0002ec30: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
+0002ec40: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
+0002ec50: 6465 6620 5f67 6574 5f64 6566 6175 6c74  def _get_default
+0002ec60: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
+0002ec70: 2c20 6769 7665 6e3a 2064 6963 745b 7374  , given: dict[st
+0002ec80: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
+0002ec90: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
+0002eca0: 4174 7472 6962 7574 6554 7970 655d 3a0a  AttributeType]:.
+0002ecb0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0002ecc0: 7d0a 0a0a 636c 6173 7320 7072 6f67 7265  }...class progre
+0002ecd0: 7373 2854 6167 293a 0a20 2020 2022 2222  ss(Tag):.    """
+0002ece0: 0a20 2020 2044 6973 706c 6179 7320 616e  .    Displays an
+0002ecf0: 2069 6e64 6963 6174 6f72 2073 686f 7769   indicator showi
+0002ed00: 6e67 2074 6865 2063 6f6d 706c 6574 696f  ng the completio
+0002ed10: 6e20 7072 6f67 7265 7373 206f 6620 6120  n progress of a 
+0002ed20: 7461 736b 2c20 7479 7069 6361 6c6c 7920  task, typically 
+0002ed30: 6469 7370 6c61 7965 6420 6173 2061 2070  displayed as a p
+0002ed40: 726f 6772 6573 7320 6261 722e 0a0a 2020  rogress bar...  
+0002ed50: 2020 0a0a 2020 2020 5b56 6965 7720 6675    ..    [View fu
+0002ed60: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+0002ed70: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+0002ed80: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+0002ed90: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+0002eda0: 544d 4c2f 456c 656d 656e 742f 7072 6f67  TML/Element/prog
+0002edb0: 7265 7373 290a 2020 2020 2222 220a 2020  ress).    """.  
+0002edc0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0002edd0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002ede0: 2020 2020 2020 2a63 6869 6c64 7265 6e3a        *children:
+0002edf0: 2043 6869 6c64 7265 6e54 7970 652c 0a20   ChildrenType,. 
+0002ee00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0002ee10: 2a2a 6174 7472 6962 7574 6573 3a20 4174  **attributes: At
+0002ee20: 7472 6962 7574 6554 7970 652c 0a20 2020  tributeType,.   
+0002ee30: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+0002ee40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0002ee50: 4469 7370 6c61 7973 2061 6e20 696e 6469  Displays an indi
+0002ee60: 6361 746f 7220 7368 6f77 696e 6720 7468  cator showing th
+0002ee70: 6520 636f 6d70 6c65 7469 6f6e 2070 726f  e completion pro
+0002ee80: 6772 6573 7320 6f66 2061 2074 6173 6b2c  gress of a task,
+0002ee90: 2074 7970 6963 616c 6c79 2064 6973 706c   typically displ
+0002eea0: 6179 6564 2061 7320 6120 7072 6f67 7265  ayed as a progre
+0002eeb0: 7373 2062 6172 2e0a 0a20 2020 2020 2020  ss bar...       
+0002eec0: 200a 0a20 2020 2020 2020 205b 5669 6577   ..        [View
+0002eed0: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
+0002eee0: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
+0002eef0: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+0002ef00: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+0002ef10: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f70  b/HTML/Element/p
+0002ef20: 726f 6772 6573 7329 0a20 2020 2020 2020  rogress).       
+0002ef30: 2022 2222 0a20 2020 2020 2020 2061 7474   """.        att
+0002ef40: 7269 6275 7465 7320 7c3d 207b 0a20 2020  ributes |= {.   
+0002ef50: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+0002ef60: 2020 7d0a 2020 2020 2020 2020 7375 7065    }.        supe
+0002ef70: 7228 292e 5f5f 696e 6974 5f5f 282a 6368  r().__init__(*ch
+0002ef80: 696c 6472 656e 2c20 2a2a 6174 7472 6962  ildren, **attrib
+0002ef90: 7574 6573 290a 0a20 2020 2064 6566 205f  utes)..    def _
+0002efa0: 5f63 616c 6c5f 5f28 2020 2320 7479 7065  _call__(  # type
+0002efb0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+0002efc0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0002efd0: 6368 696c 6472 656e 3a20 4368 696c 6472  children: Childr
+0002efe0: 656e 5479 7065 2c0a 2020 2020 2020 2020  enType,.        
+0002eff0: 0a20 2020 2020 2020 202a 2a61 7474 7269  .        **attri
+0002f000: 6275 7465 733a 2041 7474 7269 6275 7465  butes: Attribute
+0002f010: 5479 7065 2c0a 2020 2020 293a 0a20 2020  Type,.    ):.   
+0002f020: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002f030: 2044 6973 706c 6179 7320 616e 2069 6e64   Displays an ind
+0002f040: 6963 6174 6f72 2073 686f 7769 6e67 2074  icator showing t
+0002f050: 6865 2063 6f6d 706c 6574 696f 6e20 7072  he completion pr
+0002f060: 6f67 7265 7373 206f 6620 6120 7461 736b  ogress of a task
+0002f070: 2c20 7479 7069 6361 6c6c 7920 6469 7370  , typically disp
+0002f080: 6c61 7965 6420 6173 2061 2070 726f 6772  layed as a progr
+0002f090: 6573 7320 6261 722e 0a0a 2020 2020 2020  ess bar...      
+0002f0a0: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
+0002f0b0: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+0002f0c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+0002f0d0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002f0e0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002f0f0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002f100: 7072 6f67 7265 7373 290a 2020 2020 2020  progress).      
+0002f110: 2020 2222 220a 2020 2020 2020 2020 6174    """.        at
+0002f120: 7472 6962 7574 6573 207c 3d20 7b0a 2020  tributes |= {.  
+0002f130: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+0002f140: 2020 207d 0a20 2020 2020 2020 2072 6574     }.        ret
+0002f150: 7572 6e20 7375 7065 7228 292e 5f5f 6361  urn super().__ca
+0002f160: 6c6c 5f5f 282a 6368 696c 6472 656e 2c20  ll__(*children, 
+0002f170: 2a2a 6174 7472 6962 7574 6573 290a 0a20  **attributes).. 
+0002f180: 2020 2064 6566 205f 6765 745f 6465 6661     def _get_defa
+0002f190: 756c 745f 6174 7472 6962 7574 6573 2873  ult_attributes(s
+0002f1a0: 656c 662c 2067 6976 656e 3a20 6469 6374  elf, given: dict
+0002f1b0: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
+0002f1c0: 7970 655d 2920 2d3e 2064 6963 745b 7374  ype]) -> dict[st
+0002f1d0: 722c 2041 7474 7269 6275 7465 5479 7065  r, AttributeType
+0002f1e0: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
+0002f1f0: 6e20 7b7d 0a0a 0a63 6c61 7373 2073 656c  n {}...class sel
+0002f200: 6563 7428 5461 6729 3a0a 2020 2020 2222  ect(Tag):.    ""
+0002f210: 220a 2020 2020 5265 7072 6573 656e 7473  ".    Represents
+0002f220: 2061 2063 6f6e 7472 6f6c 2074 6861 7420   a control that 
+0002f230: 7072 6f76 6964 6573 2061 206d 656e 7520  provides a menu 
+0002f240: 6f66 206f 7074 696f 6e73 2e0a 0a20 2020  of options...   
+0002f250: 200a 0a20 2020 205b 5669 6577 2066 756c   ..    [View ful
+0002f260: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+0002f270: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+0002f280: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+0002f290: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+0002f2a0: 4d4c 2f45 6c65 6d65 6e74 2f73 656c 6563  ML/Element/selec
+0002f2b0: 7429 0a20 2020 2022 2222 0a20 2020 2064  t).    """.    d
+0002f2c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0002f2d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0002f2e0: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+0002f2f0: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+0002f300: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+0002f310: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+0002f320: 6275 7465 5479 7065 2c0a 2020 2020 2920  buteType,.    ) 
+0002f330: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0002f340: 2022 2222 0a20 2020 2020 2020 2052 6570   """.        Rep
+0002f350: 7265 7365 6e74 7320 6120 636f 6e74 726f  resents a contro
+0002f360: 6c20 7468 6174 2070 726f 7669 6465 7320  l that provides 
+0002f370: 6120 6d65 6e75 206f 6620 6f70 7469 6f6e  a menu of option
+0002f380: 732e 0a0a 2020 2020 2020 2020 0a0a 2020  s...        ..  
+0002f390: 2020 2020 2020 5b56 6965 7720 6675 6c6c        [View full
+0002f3a0: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+0002f3b0: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0002f3c0: 722e 6d6f 7a69 6c6c 612e 6f72 672f 656e  r.mozilla.org/en
+0002f3d0: 2d55 532f 646f 6373 2f57 6562 2f48 544d  -US/docs/Web/HTM
+0002f3e0: 4c2f 456c 656d 656e 742f 7365 6c65 6374  L/Element/select
+0002f3f0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+0002f400: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
+0002f410: 207c 3d20 7b0a 2020 2020 2020 2020 2020   |= {.          
+0002f420: 2020 0a20 2020 2020 2020 207d 0a20 2020    .        }.   
+0002f430: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+0002f440: 6e69 745f 5f28 2a63 6869 6c64 7265 6e2c  nit__(*children,
+0002f450: 202a 2a61 7474 7269 6275 7465 7329 0a0a   **attributes)..
+0002f460: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
+0002f470: 2820 2023 2074 7970 653a 2069 676e 6f72  (  # type: ignor
+0002f480: 650a 2020 2020 2020 2020 7365 6c66 2c0a  e.        self,.
+0002f490: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+0002f4a0: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+0002f4b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0002f4c0: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+0002f4d0: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+0002f4e0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0002f4f0: 220a 2020 2020 2020 2020 5265 7072 6573  ".        Repres
+0002f500: 656e 7473 2061 2063 6f6e 7472 6f6c 2074  ents a control t
+0002f510: 6861 7420 7072 6f76 6964 6573 2061 206d  hat provides a m
+0002f520: 656e 7520 6f66 206f 7074 696f 6e73 2e0a  enu of options..
+0002f530: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
+0002f540: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+0002f550: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+0002f560: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+0002f570: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+0002f580: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+0002f590: 6c65 6d65 6e74 2f73 656c 6563 7429 0a20  lement/select). 
+0002f5a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002f5b0: 2020 2061 7474 7269 6275 7465 7320 7c3d     attributes |=
+0002f5c0: 207b 0a20 2020 2020 2020 2020 2020 200a   {.            .
+0002f5d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0002f5e0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+0002f5f0: 2e5f 5f63 616c 6c5f 5f28 2a63 6869 6c64  .__call__(*child
+0002f600: 7265 6e2c 202a 2a61 7474 7269 6275 7465  ren, **attribute
+0002f610: 7329 0a0a 2020 2020 6465 6620 5f67 6574  s)..    def _get
+0002f620: 5f64 6566 6175 6c74 5f61 7474 7269 6275  _default_attribu
+0002f630: 7465 7328 7365 6c66 2c20 6769 7665 6e3a  tes(self, given:
+0002f640: 2064 6963 745b 7374 722c 2041 7474 7269   dict[str, Attri
+0002f650: 6275 7465 5479 7065 5d29 202d 3e20 6469  buteType]) -> di
+0002f660: 6374 5b73 7472 2c20 4174 7472 6962 7574  ct[str, Attribut
+0002f670: 6554 7970 655d 3a0a 2020 2020 2020 2020  eType]:.        
+0002f680: 7265 7475 726e 207b 7d0a 0a0a 636c 6173  return {}...clas
+0002f690: 7320 7465 7874 6172 6561 2854 6167 293a  s textarea(Tag):
+0002f6a0: 0a20 2020 2022 2222 0a20 2020 2052 6570  .    """.    Rep
+0002f6b0: 7265 7365 6e74 7320 6120 6d75 6c74 692d  resents a multi-
+0002f6c0: 6c69 6e65 2070 6c61 696e 2d74 6578 7420  line plain-text 
+0002f6d0: 6564 6974 696e 6720 636f 6e74 726f 6c2c  editing control,
+0002f6e0: 2075 7365 6675 6c20 7768 656e 2079 6f75   useful when you
+0002f6f0: 2077 616e 7420 746f 2061 6c6c 6f77 2075   want to allow u
+0002f700: 7365 7273 2074 6f20 656e 7465 7220 6120  sers to enter a 
+0002f710: 7369 7a65 6162 6c65 2061 6d6f 756e 7420  sizeable amount 
+0002f720: 6f66 2066 7265 652d 666f 726d 2074 6578  of free-form tex
+0002f730: 742c 2066 6f72 2065 7861 6d70 6c65 2c20  t, for example, 
+0002f740: 6120 636f 6d6d 656e 7420 6f6e 2061 2072  a comment on a r
+0002f750: 6576 6965 7720 6f72 2066 6565 6462 6163  eview or feedbac
+0002f760: 6b20 666f 726d 2e0a 0a20 2020 200a 0a20  k form...    .. 
+0002f770: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+0002f780: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+0002f790: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+0002f7a0: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+0002f7b0: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+0002f7c0: 6c65 6d65 6e74 2f74 6578 7461 7265 6129  lement/textarea)
+0002f7d0: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
+0002f7e0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0002f7f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002f800: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
+0002f810: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
+0002f820: 2020 0a20 2020 2020 2020 202a 2a61 7474    .        **att
+0002f830: 7269 6275 7465 733a 2041 7474 7269 6275  ributes: Attribu
+0002f840: 7465 5479 7065 2c0a 2020 2020 2920 2d3e  teType,.    ) ->
+0002f850: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0002f860: 2222 0a20 2020 2020 2020 2052 6570 7265  "".        Repre
+0002f870: 7365 6e74 7320 6120 6d75 6c74 692d 6c69  sents a multi-li
+0002f880: 6e65 2070 6c61 696e 2d74 6578 7420 6564  ne plain-text ed
+0002f890: 6974 696e 6720 636f 6e74 726f 6c2c 2075  iting control, u
+0002f8a0: 7365 6675 6c20 7768 656e 2079 6f75 2077  seful when you w
+0002f8b0: 616e 7420 746f 2061 6c6c 6f77 2075 7365  ant to allow use
+0002f8c0: 7273 2074 6f20 656e 7465 7220 6120 7369  rs to enter a si
+0002f8d0: 7a65 6162 6c65 2061 6d6f 756e 7420 6f66  zeable amount of
+0002f8e0: 2066 7265 652d 666f 726d 2074 6578 742c   free-form text,
+0002f8f0: 2066 6f72 2065 7861 6d70 6c65 2c20 6120   for example, a 
+0002f900: 636f 6d6d 656e 7420 6f6e 2061 2072 6576  comment on a rev
+0002f910: 6965 7720 6f72 2066 6565 6462 6163 6b20  iew or feedback 
+0002f920: 666f 726d 2e0a 0a20 2020 2020 2020 200a  form...        .
+0002f930: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
+0002f940: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+0002f950: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+0002f960: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
+0002f970: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
+0002f980: 4854 4d4c 2f45 6c65 6d65 6e74 2f74 6578  HTML/Element/tex
+0002f990: 7461 7265 6129 0a20 2020 2020 2020 2022  tarea).        "
+0002f9a0: 2222 0a20 2020 2020 2020 2061 7474 7269  "".        attri
+0002f9b0: 6275 7465 7320 7c3d 207b 0a20 2020 2020  butes |= {.     
+0002f9c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0002f9d0: 7d0a 2020 2020 2020 2020 7375 7065 7228  }.        super(
+0002f9e0: 292e 5f5f 696e 6974 5f5f 282a 6368 696c  ).__init__(*chil
+0002f9f0: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
+0002fa00: 6573 290a 0a20 2020 2064 6566 205f 5f63  es)..    def __c
+0002fa10: 616c 6c5f 5f28 2020 2320 7479 7065 3a20  all__(  # type: 
+0002fa20: 6967 6e6f 7265 0a20 2020 2020 2020 2073  ignore.        s
+0002fa30: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
+0002fa40: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
+0002fa50: 5479 7065 2c0a 2020 2020 2020 2020 0a20  Type,.        . 
+0002fa60: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
+0002fa70: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
+0002fa80: 7065 2c0a 2020 2020 293a 0a20 2020 2020  pe,.    ):.     
+0002fa90: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+0002faa0: 6570 7265 7365 6e74 7320 6120 6d75 6c74  epresents a mult
+0002fab0: 692d 6c69 6e65 2070 6c61 696e 2d74 6578  i-line plain-tex
+0002fac0: 7420 6564 6974 696e 6720 636f 6e74 726f  t editing contro
+0002fad0: 6c2c 2075 7365 6675 6c20 7768 656e 2079  l, useful when y
+0002fae0: 6f75 2077 616e 7420 746f 2061 6c6c 6f77  ou want to allow
+0002faf0: 2075 7365 7273 2074 6f20 656e 7465 7220   users to enter 
+0002fb00: 6120 7369 7a65 6162 6c65 2061 6d6f 756e  a sizeable amoun
+0002fb10: 7420 6f66 2066 7265 652d 666f 726d 2074  t of free-form t
+0002fb20: 6578 742c 2066 6f72 2065 7861 6d70 6c65  ext, for example
+0002fb30: 2c20 6120 636f 6d6d 656e 7420 6f6e 2061  , a comment on a
+0002fb40: 2072 6576 6965 7720 6f72 2066 6565 6462   review or feedb
+0002fb50: 6163 6b20 666f 726d 2e0a 0a20 2020 2020  ack form...     
+0002fb60: 2020 200a 0a20 2020 2020 2020 205b 5669     ..        [Vi
+0002fb70: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
+0002fb80: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+0002fb90: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+0002fba0: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+0002fbb0: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+0002fbc0: 2f74 6578 7461 7265 6129 0a20 2020 2020  /textarea).     
+0002fbd0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0002fbe0: 7474 7269 6275 7465 7320 7c3d 207b 0a20  ttributes |= {. 
+0002fbf0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0002fc00: 2020 2020 7d0a 2020 2020 2020 2020 7265      }.        re
+0002fc10: 7475 726e 2073 7570 6572 2829 2e5f 5f63  turn super().__c
+0002fc20: 616c 6c5f 5f28 2a63 6869 6c64 7265 6e2c  all__(*children,
+0002fc30: 202a 2a61 7474 7269 6275 7465 7329 0a0a   **attributes)..
+0002fc40: 2020 2020 6465 6620 5f67 6574 5f64 6566      def _get_def
+0002fc50: 6175 6c74 5f61 7474 7269 6275 7465 7328  ault_attributes(
+0002fc60: 7365 6c66 2c20 6769 7665 6e3a 2064 6963  self, given: dic
+0002fc70: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
+0002fc80: 5479 7065 5d29 202d 3e20 6469 6374 5b73  Type]) -> dict[s
+0002fc90: 7472 2c20 4174 7472 6962 7574 6554 7970  tr, AttributeTyp
+0002fca0: 655d 3a0a 2020 2020 2020 2020 7265 7475  e]:.        retu
+0002fcb0: 726e 207b 7d0a 0a0a 636c 6173 7320 6465  rn {}...class de
+0002fcc0: 7461 696c 7328 5461 6729 3a0a 2020 2020  tails(Tag):.    
+0002fcd0: 2222 220a 2020 2020 4372 6561 7465 7320  """.    Creates 
+0002fce0: 6120 6469 7363 6c6f 7375 7265 2077 6964  a disclosure wid
+0002fcf0: 6765 7420 696e 2077 6869 6368 2069 6e66  get in which inf
+0002fd00: 6f72 6d61 7469 6f6e 2069 7320 7669 7369  ormation is visi
+0002fd10: 626c 6520 6f6e 6c79 2077 6865 6e20 7468  ble only when th
+0002fd20: 6520 7769 6467 6574 2069 7320 746f 6767  e widget is togg
+0002fd30: 6c65 6420 696e 746f 2061 6e20 226f 7065  led into an "ope
+0002fd40: 6e22 2073 7461 7465 2e20 4120 7375 6d6d  n" state. A summ
+0002fd50: 6172 7920 6f72 206c 6162 656c 206d 7573  ary or label mus
+0002fd60: 7420 6265 2070 726f 7669 6465 6420 7573  t be provided us
+0002fd70: 696e 6720 7468 6520 5b60 3c73 756d 6d61  ing the [`<summa
+0002fd80: 7279 3e60 5d28 6874 7470 733a 2f2f 6465  ry>`](https://de
+0002fd90: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+0002fda0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+0002fdb0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+0002fdc0: 7375 6d6d 6172 7929 2065 6c65 6d65 6e74  summary) element
+0002fdd0: 2e0a 0a20 2020 200a 0a20 2020 205b 5669  ...    ..    [Vi
+0002fde0: 6577 2066 756c 6c20 646f 6375 6d65 6e74  ew full document
+0002fdf0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+0002fe00: 6576 656c 6f70 6572 2e6d 6f7a 696c 6c61  eveloper.mozilla
+0002fe10: 2e6f 7267 2f65 6e2d 5553 2f64 6f63 732f  .org/en-US/docs/
+0002fe20: 5765 622f 4854 4d4c 2f45 6c65 6d65 6e74  Web/HTML/Element
+0002fe30: 2f64 6574 6169 6c73 290a 2020 2020 2222  /details).    ""
+0002fe40: 220a 2020 2020 6465 6620 5f5f 696e 6974  ".    def __init
+0002fe50: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0002fe60: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
+0002fe70: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
+0002fe80: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
+0002fe90: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
+0002fea0: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
+0002feb0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+0002fec0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002fed0: 2020 2020 4372 6561 7465 7320 6120 6469      Creates a di
+0002fee0: 7363 6c6f 7375 7265 2077 6964 6765 7420  sclosure widget 
+0002fef0: 696e 2077 6869 6368 2069 6e66 6f72 6d61  in which informa
+0002ff00: 7469 6f6e 2069 7320 7669 7369 626c 6520  tion is visible 
+0002ff10: 6f6e 6c79 2077 6865 6e20 7468 6520 7769  only when the wi
+0002ff20: 6467 6574 2069 7320 746f 6767 6c65 6420  dget is toggled 
+0002ff30: 696e 746f 2061 6e20 226f 7065 6e22 2073  into an "open" s
+0002ff40: 7461 7465 2e20 4120 7375 6d6d 6172 7920  tate. A summary 
+0002ff50: 6f72 206c 6162 656c 206d 7573 7420 6265  or label must be
+0002ff60: 2070 726f 7669 6465 6420 7573 696e 6720   provided using 
+0002ff70: 7468 6520 5b60 3c73 756d 6d61 7279 3e60  the [`<summary>`
+0002ff80: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+0002ff90: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+0002ffa0: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+0002ffb0: 544d 4c2f 456c 656d 656e 742f 7375 6d6d  TML/Element/summ
+0002ffc0: 6172 7929 2065 6c65 6d65 6e74 2e0a 0a20  ary) element... 
+0002ffd0: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+0002ffe0: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+0002fff0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00030000: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+00030010: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+00030020: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+00030030: 6d65 6e74 2f64 6574 6169 6c73 290a 2020  ment/details).  
+00030040: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00030050: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
+00030060: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
+00030070: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00030080: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00030090: 5f28 2a63 6869 6c64 7265 6e2c 202a 2a61  _(*children, **a
+000300a0: 7474 7269 6275 7465 7329 0a0a 2020 2020  ttributes)..    
+000300b0: 6465 6620 5f5f 6361 6c6c 5f5f 2820 2023  def __call__(  #
+000300c0: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+000300d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000300e0: 2020 2020 2a63 6869 6c64 7265 6e3a 2043      *children: C
+000300f0: 6869 6c64 7265 6e54 7970 652c 0a20 2020  hildrenType,.   
+00030100: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+00030110: 6174 7472 6962 7574 6573 3a20 4174 7472  attributes: Attr
+00030120: 6962 7574 6554 7970 652c 0a20 2020 2029  ibuteType,.    )
+00030130: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00030140: 2020 2020 2020 4372 6561 7465 7320 6120        Creates a 
+00030150: 6469 7363 6c6f 7375 7265 2077 6964 6765  disclosure widge
+00030160: 7420 696e 2077 6869 6368 2069 6e66 6f72  t in which infor
+00030170: 6d61 7469 6f6e 2069 7320 7669 7369 626c  mation is visibl
+00030180: 6520 6f6e 6c79 2077 6865 6e20 7468 6520  e only when the 
+00030190: 7769 6467 6574 2069 7320 746f 6767 6c65  widget is toggle
+000301a0: 6420 696e 746f 2061 6e20 226f 7065 6e22  d into an "open"
+000301b0: 2073 7461 7465 2e20 4120 7375 6d6d 6172   state. A summar
+000301c0: 7920 6f72 206c 6162 656c 206d 7573 7420  y or label must 
+000301d0: 6265 2070 726f 7669 6465 6420 7573 696e  be provided usin
+000301e0: 6720 7468 6520 5b60 3c73 756d 6d61 7279  g the [`<summary
+000301f0: 3e60 5d28 6874 7470 733a 2f2f 6465 7665  >`](https://deve
+00030200: 6c6f 7065 722e 6d6f 7a69 6c6c 612e 6f72  loper.mozilla.or
+00030210: 672f 656e 2d55 532f 646f 6373 2f57 6562  g/en-US/docs/Web
+00030220: 2f48 544d 4c2f 456c 656d 656e 742f 7375  /HTML/Element/su
+00030230: 6d6d 6172 7929 2065 6c65 6d65 6e74 2e0a  mmary) element..
+00030240: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
+00030250: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+00030260: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00030270: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+00030280: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+00030290: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+000302a0: 6c65 6d65 6e74 2f64 6574 6169 6c73 290a  lement/details).
+000302b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000302c0: 2020 2020 6174 7472 6962 7574 6573 207c      attributes |
+000302d0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000302e0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+000302f0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00030300: 292e 5f5f 6361 6c6c 5f5f 282a 6368 696c  ).__call__(*chil
+00030310: 6472 656e 2c20 2a2a 6174 7472 6962 7574  dren, **attribut
+00030320: 6573 290a 0a20 2020 2064 6566 205f 6765  es)..    def _ge
+00030330: 745f 6465 6661 756c 745f 6174 7472 6962  t_default_attrib
+00030340: 7574 6573 2873 656c 662c 2067 6976 656e  utes(self, given
+00030350: 3a20 6469 6374 5b73 7472 2c20 4174 7472  : dict[str, Attr
+00030360: 6962 7574 6554 7970 655d 2920 2d3e 2064  ibuteType]) -> d
+00030370: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
+00030380: 7465 5479 7065 5d3a 0a20 2020 2020 2020  teType]:.       
+00030390: 2072 6574 7572 6e20 7b7d 0a0a 0a63 6c61   return {}...cla
+000303a0: 7373 2064 6961 6c6f 6728 5461 6729 3a0a  ss dialog(Tag):.
+000303b0: 2020 2020 2222 220a 2020 2020 5265 7072      """.    Repr
+000303c0: 6573 656e 7473 2061 2064 6961 6c6f 6720  esents a dialog 
+000303d0: 626f 7820 6f72 206f 7468 6572 2069 6e74  box or other int
+000303e0: 6572 6163 7469 7665 2063 6f6d 706f 6e65  eractive compone
+000303f0: 6e74 2c20 7375 6368 2061 7320 6120 6469  nt, such as a di
+00030400: 736d 6973 7369 626c 6520 616c 6572 742c  smissible alert,
+00030410: 2069 6e73 7065 6374 6f72 2c20 6f72 2073   inspector, or s
+00030420: 7562 7769 6e64 6f77 2e0a 0a20 2020 200a  ubwindow...    .
+00030430: 0a20 2020 205b 5669 6577 2066 756c 6c20  .    [View full 
+00030440: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+00030450: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00030460: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00030470: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00030480: 2f45 6c65 6d65 6e74 2f64 6961 6c6f 6729  /Element/dialog)
+00030490: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
+000304a0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000304b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000304c0: 202a 6368 696c 6472 656e 3a20 4368 696c   *children: Chil
+000304d0: 6472 656e 5479 7065 2c0a 2020 2020 2020  drenType,.      
+000304e0: 2020 0a20 2020 2020 2020 202a 2a61 7474    .        **att
+000304f0: 7269 6275 7465 733a 2041 7474 7269 6275  ributes: Attribu
+00030500: 7465 5479 7065 2c0a 2020 2020 2920 2d3e  teType,.    ) ->
+00030510: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00030520: 2222 0a20 2020 2020 2020 2052 6570 7265  "".        Repre
+00030530: 7365 6e74 7320 6120 6469 616c 6f67 2062  sents a dialog b
+00030540: 6f78 206f 7220 6f74 6865 7220 696e 7465  ox or other inte
+00030550: 7261 6374 6976 6520 636f 6d70 6f6e 656e  ractive componen
+00030560: 742c 2073 7563 6820 6173 2061 2064 6973  t, such as a dis
+00030570: 6d69 7373 6962 6c65 2061 6c65 7274 2c20  missible alert, 
+00030580: 696e 7370 6563 746f 722c 206f 7220 7375  inspector, or su
+00030590: 6277 696e 646f 772e 0a0a 2020 2020 2020  bwindow...      
+000305a0: 2020 0a0a 2020 2020 2020 2020 5b56 6965    ..        [Vie
+000305b0: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+000305c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+000305d0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+000305e0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+000305f0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00030600: 6469 616c 6f67 290a 2020 2020 2020 2020  dialog).        
+00030610: 2222 220a 2020 2020 2020 2020 6174 7472  """.        attr
+00030620: 6962 7574 6573 207c 3d20 7b0a 2020 2020  ibutes |= {.    
+00030630: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00030640: 207d 0a20 2020 2020 2020 2073 7570 6572   }.        super
+00030650: 2829 2e5f 5f69 6e69 745f 5f28 2a63 6869  ().__init__(*chi
+00030660: 6c64 7265 6e2c 202a 2a61 7474 7269 6275  ldren, **attribu
+00030670: 7465 7329 0a0a 2020 2020 6465 6620 5f5f  tes)..    def __
+00030680: 6361 6c6c 5f5f 2820 2023 2074 7970 653a  call__(  # type:
+00030690: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
+000306a0: 7365 6c66 2c0a 2020 2020 2020 2020 2a63  self,.        *c
+000306b0: 6869 6c64 7265 6e3a 2043 6869 6c64 7265  hildren: Childre
+000306c0: 6e54 7970 652c 0a20 2020 2020 2020 200a  nType,.        .
+000306d0: 2020 2020 2020 2020 2a2a 6174 7472 6962          **attrib
+000306e0: 7574 6573 3a20 4174 7472 6962 7574 6554  utes: AttributeT
+000306f0: 7970 652c 0a20 2020 2029 3a0a 2020 2020  ype,.    ):.    
+00030700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00030710: 5265 7072 6573 656e 7473 2061 2064 6961  Represents a dia
+00030720: 6c6f 6720 626f 7820 6f72 206f 7468 6572  log box or other
+00030730: 2069 6e74 6572 6163 7469 7665 2063 6f6d   interactive com
+00030740: 706f 6e65 6e74 2c20 7375 6368 2061 7320  ponent, such as 
+00030750: 6120 6469 736d 6973 7369 626c 6520 616c  a dismissible al
+00030760: 6572 742c 2069 6e73 7065 6374 6f72 2c20  ert, inspector, 
+00030770: 6f72 2073 7562 7769 6e64 6f77 2e0a 0a20  or subwindow... 
+00030780: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+00030790: 205b 5669 6577 2066 756c 6c20 646f 6375   [View full docu
+000307a0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+000307b0: 3a2f 2f64 6576 656c 6f70 6572 2e6d 6f7a  ://developer.moz
+000307c0: 696c 6c61 2e6f 7267 2f65 6e2d 5553 2f64  illa.org/en-US/d
+000307d0: 6f63 732f 5765 622f 4854 4d4c 2f45 6c65  ocs/Web/HTML/Ele
+000307e0: 6d65 6e74 2f64 6961 6c6f 6729 0a20 2020  ment/dialog).   
+000307f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00030800: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+00030810: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00030820: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00030830: 7265 7475 726e 2073 7570 6572 2829 2e5f  return super()._
+00030840: 5f63 616c 6c5f 5f28 2a63 6869 6c64 7265  _call__(*childre
+00030850: 6e2c 202a 2a61 7474 7269 6275 7465 7329  n, **attributes)
+00030860: 0a0a 2020 2020 6465 6620 5f67 6574 5f64  ..    def _get_d
+00030870: 6566 6175 6c74 5f61 7474 7269 6275 7465  efault_attribute
+00030880: 7328 7365 6c66 2c20 6769 7665 6e3a 2064  s(self, given: d
+00030890: 6963 745b 7374 722c 2041 7474 7269 6275  ict[str, Attribu
+000308a0: 7465 5479 7065 5d29 202d 3e20 6469 6374  teType]) -> dict
+000308b0: 5b73 7472 2c20 4174 7472 6962 7574 6554  [str, AttributeT
+000308c0: 7970 655d 3a0a 2020 2020 2020 2020 7265  ype]:.        re
+000308d0: 7475 726e 207b 7d0a 0a0a 636c 6173 7320  turn {}...class 
+000308e0: 7375 6d6d 6172 7928 5461 6729 3a0a 2020  summary(Tag):.  
+000308f0: 2020 2222 220a 2020 2020 5370 6563 6966    """.    Specif
+00030900: 6965 7320 6120 7375 6d6d 6172 792c 2063  ies a summary, c
+00030910: 6170 7469 6f6e 2c20 6f72 206c 6567 656e  aption, or legen
+00030920: 6420 666f 7220 6120 6465 7461 696c 7320  d for a details 
+00030930: 656c 656d 656e 7427 7320 6469 7363 6c6f  element's disclo
+00030940: 7375 7265 2062 6f78 2e20 436c 6963 6b69  sure box. Clicki
+00030950: 6e67 2074 6865 2060 3c73 756d 6d61 7279  ng the `<summary
+00030960: 3e60 2065 6c65 6d65 6e74 2074 6f67 676c  >` element toggl
+00030970: 6573 2074 6865 2073 7461 7465 206f 6620  es the state of 
+00030980: 7468 6520 7061 7265 6e74 205b 603c 6465  the parent [`<de
+00030990: 7461 696c 733e 605d 2868 7474 7073 3a2f  tails>`](https:/
+000309a0: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+000309b0: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+000309c0: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+000309d0: 6e74 2f64 6574 6169 6c73 2920 656c 656d  nt/details) elem
+000309e0: 656e 7420 6f70 656e 2061 6e64 2063 6c6f  ent open and clo
+000309f0: 7365 642e 0a0a 2020 2020 0a0a 2020 2020  sed...    ..    
+00030a00: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+00030a10: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00030a20: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+00030a30: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00030a40: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+00030a50: 656e 742f 7375 6d6d 6172 7929 0a20 2020  ent/summary).   
+00030a60: 2022 2222 0a20 2020 2064 6566 205f 5f69   """.    def __i
+00030a70: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00030a80: 656c 662c 0a20 2020 2020 2020 202a 6368  elf,.        *ch
+00030a90: 696c 6472 656e 3a20 4368 696c 6472 656e  ildren: Children
+00030aa0: 5479 7065 2c0a 2020 2020 2020 2020 0a20  Type,.        . 
+00030ab0: 2020 2020 2020 202a 2a61 7474 7269 6275         **attribu
+00030ac0: 7465 733a 2041 7474 7269 6275 7465 5479  tes: AttributeTy
+00030ad0: 7065 2c0a 2020 2020 2920 2d3e 204e 6f6e  pe,.    ) -> Non
+00030ae0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00030af0: 2020 2020 2020 2053 7065 6369 6669 6573         Specifies
+00030b00: 2061 2073 756d 6d61 7279 2c20 6361 7074   a summary, capt
+00030b10: 696f 6e2c 206f 7220 6c65 6765 6e64 2066  ion, or legend f
+00030b20: 6f72 2061 2064 6574 6169 6c73 2065 6c65  or a details ele
+00030b30: 6d65 6e74 2773 2064 6973 636c 6f73 7572  ment's disclosur
+00030b40: 6520 626f 782e 2043 6c69 636b 696e 6720  e box. Clicking 
+00030b50: 7468 6520 603c 7375 6d6d 6172 793e 6020  the `<summary>` 
+00030b60: 656c 656d 656e 7420 746f 6767 6c65 7320  element toggles 
+00030b70: 7468 6520 7374 6174 6520 6f66 2074 6865  the state of the
+00030b80: 2070 6172 656e 7420 5b60 3c64 6574 6169   parent [`<detai
+00030b90: 6c73 3e60 5d28 6874 7470 733a 2f2f 6465  ls>`](https://de
+00030ba0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+00030bb0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+00030bc0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00030bd0: 6465 7461 696c 7329 2065 6c65 6d65 6e74  details) element
+00030be0: 206f 7065 6e20 616e 6420 636c 6f73 6564   open and closed
+00030bf0: 2e0a 0a20 2020 2020 2020 200a 0a20 2020  ...        ..   
+00030c00: 2020 2020 205b 5669 6577 2066 756c 6c20       [View full 
+00030c10: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+00030c20: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00030c30: 2e6d 6f7a 696c 6c61 2e6f 7267 2f65 6e2d  .mozilla.org/en-
+00030c40: 5553 2f64 6f63 732f 5765 622f 4854 4d4c  US/docs/Web/HTML
+00030c50: 2f45 6c65 6d65 6e74 2f73 756d 6d61 7279  /Element/summary
+00030c60: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00030c70: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
+00030c80: 207c 3d20 7b0a 2020 2020 2020 2020 2020   |= {.          
+00030c90: 2020 0a20 2020 2020 2020 207d 0a20 2020    .        }.   
+00030ca0: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00030cb0: 6e69 745f 5f28 2a63 6869 6c64 7265 6e2c  nit__(*children,
+00030cc0: 202a 2a61 7474 7269 6275 7465 7329 0a0a   **attributes)..
+00030cd0: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
+00030ce0: 2820 2023 2074 7970 653a 2069 676e 6f72  (  # type: ignor
+00030cf0: 650a 2020 2020 2020 2020 7365 6c66 2c0a  e.        self,.
+00030d00: 2020 2020 2020 2020 2a63 6869 6c64 7265          *childre
+00030d10: 6e3a 2043 6869 6c64 7265 6e54 7970 652c  n: ChildrenType,
+00030d20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00030d30: 2020 2a2a 6174 7472 6962 7574 6573 3a20    **attributes: 
+00030d40: 4174 7472 6962 7574 6554 7970 652c 0a20  AttributeType,. 
+00030d50: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00030d60: 220a 2020 2020 2020 2020 5370 6563 6966  ".        Specif
+00030d70: 6965 7320 6120 7375 6d6d 6172 792c 2063  ies a summary, c
+00030d80: 6170 7469 6f6e 2c20 6f72 206c 6567 656e  aption, or legen
+00030d90: 6420 666f 7220 6120 6465 7461 696c 7320  d for a details 
+00030da0: 656c 656d 656e 7427 7320 6469 7363 6c6f  element's disclo
+00030db0: 7375 7265 2062 6f78 2e20 436c 6963 6b69  sure box. Clicki
+00030dc0: 6e67 2074 6865 2060 3c73 756d 6d61 7279  ng the `<summary
+00030dd0: 3e60 2065 6c65 6d65 6e74 2074 6f67 676c  >` element toggl
+00030de0: 6573 2074 6865 2073 7461 7465 206f 6620  es the state of 
+00030df0: 7468 6520 7061 7265 6e74 205b 603c 6465  the parent [`<de
+00030e00: 7461 696c 733e 605d 2868 7474 7073 3a2f  tails>`](https:/
+00030e10: 2f64 6576 656c 6f70 6572 2e6d 6f7a 696c  /developer.mozil
+00030e20: 6c61 2e6f 7267 2f65 6e2d 5553 2f64 6f63  la.org/en-US/doc
+00030e30: 732f 5765 622f 4854 4d4c 2f45 6c65 6d65  s/Web/HTML/Eleme
+00030e40: 6e74 2f64 6574 6169 6c73 2920 656c 656d  nt/details) elem
+00030e50: 656e 7420 6f70 656e 2061 6e64 2063 6c6f  ent open and clo
+00030e60: 7365 642e 0a0a 2020 2020 2020 2020 0a0a  sed...        ..
+00030e70: 2020 2020 2020 2020 5b56 6965 7720 6675          [View fu
+00030e80: 6c6c 2064 6f63 756d 656e 7461 7469 6f6e  ll documentation
+00030e90: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+00030ea0: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+00030eb0: 656e 2d55 532f 646f 6373 2f57 6562 2f48  en-US/docs/Web/H
+00030ec0: 544d 4c2f 456c 656d 656e 742f 7375 6d6d  TML/Element/summ
+00030ed0: 6172 7929 0a20 2020 2020 2020 2022 2222  ary).        """
+00030ee0: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+00030ef0: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+00030f00: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
+00030f10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00030f20: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
+00030f30: 2a63 6869 6c64 7265 6e2c 202a 2a61 7474  *children, **att
+00030f40: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+00030f50: 6620 5f67 6574 5f64 6566 6175 6c74 5f61  f _get_default_a
+00030f60: 7474 7269 6275 7465 7328 7365 6c66 2c20  ttributes(self, 
+00030f70: 6769 7665 6e3a 2064 6963 745b 7374 722c  given: dict[str,
+00030f80: 2041 7474 7269 6275 7465 5479 7065 5d29   AttributeType])
+00030f90: 202d 3e20 6469 6374 5b73 7472 2c20 4174   -> dict[str, At
+00030fa0: 7472 6962 7574 6554 7970 655d 3a0a 2020  tributeType]:.  
+00030fb0: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
+00030fc0: 0a0a 636c 6173 7320 736c 6f74 2854 6167  ..class slot(Tag
+00030fd0: 293a 0a20 2020 2022 2222 0a20 2020 2050  ):.    """.    P
+00030fe0: 6172 7420 6f66 2074 6865 205b 5765 6220  art of the [Web 
+00030ff0: 436f 6d70 6f6e 656e 7473 5d28 6874 7470  Components](http
+00031000: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+00031010: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+00031020: 646f 6373 2f57 6562 2f41 5049 2f57 6562  docs/Web/API/Web
+00031030: 5f63 6f6d 706f 6e65 6e74 7329 2074 6563  _components) tec
+00031040: 686e 6f6c 6f67 7920 7375 6974 652c 2074  hnology suite, t
+00031050: 6869 7320 656c 656d 656e 7420 6973 2061  his element is a
+00031060: 2070 6c61 6365 686f 6c64 6572 2069 6e73   placeholder ins
+00031070: 6964 6520 6120 7765 6220 636f 6d70 6f6e  ide a web compon
+00031080: 656e 7420 7468 6174 2079 6f75 2063 616e  ent that you can
+00031090: 2066 696c 6c20 7769 7468 2079 6f75 7220   fill with your 
+000310a0: 6f77 6e20 6d61 726b 7570 2c20 7768 6963  own markup, whic
+000310b0: 6820 6c65 7473 2079 6f75 2063 7265 6174  h lets you creat
+000310c0: 6520 7365 7061 7261 7465 2044 4f4d 2074  e separate DOM t
+000310d0: 7265 6573 2061 6e64 2070 7265 7365 6e74  rees and present
+000310e0: 2074 6865 6d20 746f 6765 7468 6572 2e0a   them together..
+000310f0: 0a20 2020 200a 0a20 2020 205b 5669 6577  .    ..    [View
+00031100: 2066 756c 6c20 646f 6375 6d65 6e74 6174   full documentat
+00031110: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
+00031120: 656c 6f70 6572 2e6d 6f7a 696c 6c61 2e6f  eloper.mozilla.o
+00031130: 7267 2f65 6e2d 5553 2f64 6f63 732f 5765  rg/en-US/docs/We
+00031140: 622f 4854 4d4c 2f45 6c65 6d65 6e74 2f73  b/HTML/Element/s
+00031150: 6c6f 7429 0a20 2020 2022 2222 0a20 2020  lot).    """.   
+00031160: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00031170: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00031180: 2020 2020 202a 6368 696c 6472 656e 3a20       *children: 
+00031190: 4368 696c 6472 656e 5479 7065 2c0a 2020  ChildrenType,.  
+000311a0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+000311b0: 2a61 7474 7269 6275 7465 733a 2041 7474  *attributes: Att
+000311c0: 7269 6275 7465 5479 7065 2c0a 2020 2020  ributeType,.    
+000311d0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000311e0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+000311f0: 6172 7420 6f66 2074 6865 205b 5765 6220  art of the [Web 
+00031200: 436f 6d70 6f6e 656e 7473 5d28 6874 7470  Components](http
+00031210: 733a 2f2f 6465 7665 6c6f 7065 722e 6d6f  s://developer.mo
+00031220: 7a69 6c6c 612e 6f72 672f 656e 2d55 532f  zilla.org/en-US/
+00031230: 646f 6373 2f57 6562 2f41 5049 2f57 6562  docs/Web/API/Web
+00031240: 5f63 6f6d 706f 6e65 6e74 7329 2074 6563  _components) tec
+00031250: 686e 6f6c 6f67 7920 7375 6974 652c 2074  hnology suite, t
+00031260: 6869 7320 656c 656d 656e 7420 6973 2061  his element is a
+00031270: 2070 6c61 6365 686f 6c64 6572 2069 6e73   placeholder ins
+00031280: 6964 6520 6120 7765 6220 636f 6d70 6f6e  ide a web compon
+00031290: 656e 7420 7468 6174 2079 6f75 2063 616e  ent that you can
+000312a0: 2066 696c 6c20 7769 7468 2079 6f75 7220   fill with your 
+000312b0: 6f77 6e20 6d61 726b 7570 2c20 7768 6963  own markup, whic
+000312c0: 6820 6c65 7473 2079 6f75 2063 7265 6174  h lets you creat
+000312d0: 6520 7365 7061 7261 7465 2044 4f4d 2074  e separate DOM t
+000312e0: 7265 6573 2061 6e64 2070 7265 7365 6e74  rees and present
+000312f0: 2074 6865 6d20 746f 6765 7468 6572 2e0a   them together..
+00031300: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
+00031310: 2020 205b 5669 6577 2066 756c 6c20 646f     [View full do
+00031320: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00031330: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6d  ps://developer.m
+00031340: 6f7a 696c 6c61 2e6f 7267 2f65 6e2d 5553  ozilla.org/en-US
+00031350: 2f64 6f63 732f 5765 622f 4854 4d4c 2f45  /docs/Web/HTML/E
+00031360: 6c65 6d65 6e74 2f73 6c6f 7429 0a20 2020  lement/slot).   
+00031370: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00031380: 2061 7474 7269 6275 7465 7320 7c3d 207b   attributes |= {
+00031390: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000313a0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000313b0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+000313c0: 282a 6368 696c 6472 656e 2c20 2a2a 6174  (*children, **at
+000313d0: 7472 6962 7574 6573 290a 0a20 2020 2064  tributes)..    d
+000313e0: 6566 205f 5f63 616c 6c5f 5f28 2020 2320  ef __call__(  # 
+000313f0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00031400: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00031410: 2020 202a 6368 696c 6472 656e 3a20 4368     *children: Ch
+00031420: 696c 6472 656e 5479 7065 2c0a 2020 2020  ildrenType,.    
+00031430: 2020 2020 0a20 2020 2020 2020 202a 2a61      .        **a
+00031440: 7474 7269 6275 7465 733a 2041 7474 7269  ttributes: Attri
+00031450: 6275 7465 5479 7065 2c0a 2020 2020 293a  buteType,.    ):
+00031460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00031470: 2020 2020 2050 6172 7420 6f66 2074 6865       Part of the
+00031480: 205b 5765 6220 436f 6d70 6f6e 656e 7473   [Web Components
+00031490: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
+000314a0: 7065 722e 6d6f 7a69 6c6c 612e 6f72 672f  per.mozilla.org/
+000314b0: 656e 2d55 532f 646f 6373 2f57 6562 2f41  en-US/docs/Web/A
+000314c0: 5049 2f57 6562 5f63 6f6d 706f 6e65 6e74  PI/Web_component
+000314d0: 7329 2074 6563 686e 6f6c 6f67 7920 7375  s) technology su
+000314e0: 6974 652c 2074 6869 7320 656c 656d 656e  ite, this elemen
+000314f0: 7420 6973 2061 2070 6c61 6365 686f 6c64  t is a placehold
+00031500: 6572 2069 6e73 6964 6520 6120 7765 6220  er inside a web 
+00031510: 636f 6d70 6f6e 656e 7420 7468 6174 2079  component that y
+00031520: 6f75 2063 616e 2066 696c 6c20 7769 7468  ou can fill with
+00031530: 2079 6f75 7220 6f77 6e20 6d61 726b 7570   your own markup
+00031540: 2c20 7768 6963 6820 6c65 7473 2079 6f75  , which lets you
+00031550: 2063 7265 6174 6520 7365 7061 7261 7465   create separate
+00031560: 2044 4f4d 2074 7265 6573 2061 6e64 2070   DOM trees and p
+00031570: 7265 7365 6e74 2074 6865 6d20 746f 6765  resent them toge
+00031580: 7468 6572 2e0a 0a20 2020 2020 2020 200a  ther...        .
+00031590: 0a20 2020 2020 2020 205b 5669 6577 2066  .        [View f
+000315a0: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+000315b0: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+000315c0: 6f70 6572 2e6d 6f7a 696c 6c61 2e6f 7267  oper.mozilla.org
+000315d0: 2f65 6e2d 5553 2f64 6f63 732f 5765 622f  /en-US/docs/Web/
+000315e0: 4854 4d4c 2f45 6c65 6d65 6e74 2f73 6c6f  HTML/Element/slo
+000315f0: 7429 0a20 2020 2020 2020 2022 2222 0a20  t).        """. 
+00031600: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
+00031610: 7320 7c3d 207b 0a20 2020 2020 2020 2020  s |= {.         
+00031620: 2020 200a 2020 2020 2020 2020 7d0a 2020     .        }.  
+00031630: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+00031640: 6572 2829 2e5f 5f63 616c 6c5f 5f28 2a63  er().__call__(*c
+00031650: 6869 6c64 7265 6e2c 202a 2a61 7474 7269  hildren, **attri
+00031660: 6275 7465 7329 0a0a 2020 2020 6465 6620  butes)..    def 
+00031670: 5f67 6574 5f64 6566 6175 6c74 5f61 7474  _get_default_att
+00031680: 7269 6275 7465 7328 7365 6c66 2c20 6769  ributes(self, gi
+00031690: 7665 6e3a 2064 6963 745b 7374 722c 2041  ven: dict[str, A
+000316a0: 7474 7269 6275 7465 5479 7065 5d29 202d  ttributeType]) -
+000316b0: 3e20 6469 6374 5b73 7472 2c20 4174 7472  > dict[str, Attr
+000316c0: 6962 7574 6554 7970 655d 3a0a 2020 2020  ibuteType]:.    
+000316d0: 2020 2020 7265 7475 726e 207b 7d0a 0a0a      return {}...
+000316e0: 636c 6173 7320 7465 6d70 6c61 7465 2854  class template(T
+000316f0: 6167 293a 0a20 2020 2022 2222 0a20 2020  ag):.    """.   
+00031700: 2041 206d 6563 6861 6e69 736d 2066 6f72   A mechanism for
+00031710: 2068 6f6c 6469 6e67 2048 544d 4c20 7468   holding HTML th
+00031720: 6174 2069 7320 6e6f 7420 746f 2062 6520  at is not to be 
+00031730: 7265 6e64 6572 6564 2069 6d6d 6564 6961  rendered immedia
+00031740: 7465 6c79 2077 6865 6e20 6120 7061 6765  tely when a page
+00031750: 2069 7320 6c6f 6164 6564 2062 7574 206d   is loaded but m
+00031760: 6179 2062 6520 696e 7374 616e 7469 6174  ay be instantiat
+00031770: 6564 2073 7562 7365 7175 656e 746c 7920  ed subsequently 
+00031780: 6475 7269 6e67 2072 756e 7469 6d65 2075  during runtime u
+00031790: 7369 6e67 204a 6176 6153 6372 6970 742e  sing JavaScript.
+000317a0: 0a0a 2020 2020 0a0a 2020 2020 5b56 6965  ..    ..    [Vie
+000317b0: 7720 6675 6c6c 2064 6f63 756d 656e 7461  w full documenta
+000317c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6465  tion](https://de
+000317d0: 7665 6c6f 7065 722e 6d6f 7a69 6c6c 612e  veloper.mozilla.
+000317e0: 6f72 672f 656e 2d55 532f 646f 6373 2f57  org/en-US/docs/W
+000317f0: 6562 2f48 544d 4c2f 456c 656d 656e 742f  eb/HTML/Element/
+00031800: 7465 6d70 6c61 7465 290a 2020 2020 2222  template).    ""
+00031810: 220a 2020 2020 6465 6620 5f5f 696e 6974  ".    def __init
+00031820: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00031830: 2c0a 2020 2020 2020 2020 2a63 6869 6c64  ,.        *child
+00031840: 7265 6e3a 2043 6869 6c64 7265 6e54 7970  ren: ChildrenTyp
+00031850: 652c 0a20 2020 2020 2020 200a 2020 2020  e,.        .    
+00031860: 2020 2020 2a2a 6174 7472 6962 7574 6573      **attributes
+00031870: 3a20 4174 7472 6962 7574 6554 7970 652c  : AttributeType,
+00031880: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+00031890: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000318a0: 2020 2020 4120 6d65 6368 616e 6973 6d20      A mechanism 
+000318b0: 666f 7220 686f 6c64 696e 6720 4854 4d4c  for holding HTML
+000318c0: 2074 6861 7420 6973 206e 6f74 2074 6f20   that is not to 
+000318d0: 6265 2072 656e 6465 7265 6420 696d 6d65  be rendered imme
+000318e0: 6469 6174 656c 7920 7768 656e 2061 2070  diately when a p
+000318f0: 6167 6520 6973 206c 6f61 6465 6420 6275  age is loaded bu
+00031900: 7420 6d61 7920 6265 2069 6e73 7461 6e74  t may be instant
+00031910: 6961 7465 6420 7375 6273 6571 7565 6e74  iated subsequent
+00031920: 6c79 2064 7572 696e 6720 7275 6e74 696d  ly during runtim
+00031930: 6520 7573 696e 6720 4a61 7661 5363 7269  e using JavaScri
+00031940: 7074 2e0a 0a20 2020 2020 2020 200a 0a20  pt...        .. 
+00031950: 2020 2020 2020 205b 5669 6577 2066 756c         [View ful
+00031960: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00031970: 2868 7474 7073 3a2f 2f64 6576 656c 6f70  (https://develop
+00031980: 6572 2e6d 6f7a 696c 6c61 2e6f 7267 2f65  er.mozilla.org/e
+00031990: 6e2d 5553 2f64 6f63 732f 5765 622f 4854  n-US/docs/Web/HT
+000319a0: 4d4c 2f45 6c65 6d65 6e74 2f74 656d 706c  ML/Element/templ
+000319b0: 6174 6529 0a20 2020 2020 2020 2022 2222  ate).        """
+000319c0: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+000319d0: 7465 7320 7c3d 207b 0a20 2020 2020 2020  tes |= {.       
+000319e0: 2020 2020 200a 2020 2020 2020 2020 7d0a       .        }.
+000319f0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00031a00: 5f5f 696e 6974 5f5f 282a 6368 696c 6472  __init__(*childr
+00031a10: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
+00031a20: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
+00031a30: 6c5f 5f28 2020 2320 7479 7065 3a20 6967  l__(  # type: ig
+00031a40: 6e6f 7265 0a20 2020 2020 2020 2073 656c  nore.        sel
+00031a50: 662c 0a20 2020 2020 2020 202a 6368 696c  f,.        *chil
+00031a60: 6472 656e 3a20 4368 696c 6472 656e 5479  dren: ChildrenTy
+00031a70: 7065 2c0a 2020 2020 2020 2020 0a20 2020  pe,.        .   
+00031a80: 2020 2020 202a 2a61 7474 7269 6275 7465       **attribute
+00031a90: 733a 2041 7474 7269 6275 7465 5479 7065  s: AttributeType
+00031aa0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00031ab0: 2022 2222 0a20 2020 2020 2020 2041 206d   """.        A m
+00031ac0: 6563 6861 6e69 736d 2066 6f72 2068 6f6c  echanism for hol
+00031ad0: 6469 6e67 2048 544d 4c20 7468 6174 2069  ding HTML that i
+00031ae0: 7320 6e6f 7420 746f 2062 6520 7265 6e64  s not to be rend
+00031af0: 6572 6564 2069 6d6d 6564 6961 7465 6c79  ered immediately
+00031b00: 2077 6865 6e20 6120 7061 6765 2069 7320   when a page is 
+00031b10: 6c6f 6164 6564 2062 7574 206d 6179 2062  loaded but may b
+00031b20: 6520 696e 7374 616e 7469 6174 6564 2073  e instantiated s
+00031b30: 7562 7365 7175 656e 746c 7920 6475 7269  ubsequently duri
+00031b40: 6e67 2072 756e 7469 6d65 2075 7369 6e67  ng runtime using
+00031b50: 204a 6176 6153 6372 6970 742e 0a0a 2020   JavaScript...  
+00031b60: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
+00031b70: 5b56 6965 7720 6675 6c6c 2064 6f63 756d  [View full docum
+00031b80: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00031b90: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+00031ba0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00031bb0: 6373 2f57 6562 2f48 544d 4c2f 456c 656d  cs/Web/HTML/Elem
+00031bc0: 656e 742f 7465 6d70 6c61 7465 290a 2020  ent/template).  
+00031bd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00031be0: 2020 6174 7472 6962 7574 6573 207c 3d20    attributes |= 
+00031bf0: 7b0a 2020 2020 2020 2020 2020 2020 0a20  {.            . 
+00031c00: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00031c10: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00031c20: 5f5f 6361 6c6c 5f5f 282a 6368 696c 6472  __call__(*childr
+00031c30: 656e 2c20 2a2a 6174 7472 6962 7574 6573  en, **attributes
+00031c40: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
+00031c50: 6465 6661 756c 745f 6174 7472 6962 7574  default_attribut
+00031c60: 6573 2873 656c 662c 2067 6976 656e 3a20  es(self, given: 
+00031c70: 6469 6374 5b73 7472 2c20 4174 7472 6962  dict[str, Attrib
+00031c80: 7574 6554 7970 655d 2920 2d3e 2064 6963  uteType]) -> dic
+00031c90: 745b 7374 722c 2041 7474 7269 6275 7465  t[str, Attribute
+00031ca0: 5479 7065 5d3a 0a20 2020 2020 2020 2072  Type]:.        r
+00031cb0: 6574 7572 6e20 7b7d 0a0a 0a5f 5f61 6c6c  eturn {}...__all
+00031cc0: 5f5f 203d 205b 0a20 2020 2027 6874 6d6c  __ = [.    'html
+00031cd0: 272c 0a20 2020 2027 6261 7365 272c 0a20  ',.    'base',. 
+00031ce0: 2020 2027 6865 6164 272c 0a20 2020 2027     'head',.    '
+00031cf0: 6c69 6e6b 272c 0a20 2020 2027 6d65 7461  link',.    'meta
+00031d00: 272c 0a20 2020 2027 7374 796c 6527 2c0a  ',.    'style',.
+00031d10: 2020 2020 2774 6974 6c65 272c 0a20 2020      'title',.   
+00031d20: 2027 626f 6479 272c 0a20 2020 2027 6164   'body',.    'ad
+00031d30: 6472 6573 7327 2c0a 2020 2020 2761 7274  dress',.    'art
+00031d40: 6963 6c65 272c 0a20 2020 2027 6173 6964  icle',.    'asid
+00031d50: 6527 2c0a 2020 2020 2766 6f6f 7465 7227  e',.    'footer'
+00031d60: 2c0a 2020 2020 2768 6561 6465 7227 2c0a  ,.    'header',.
+00031d70: 2020 2020 2768 3127 2c0a 2020 2020 2768      'h1',.    'h
+00031d80: 3227 2c0a 2020 2020 2768 3327 2c0a 2020  2',.    'h3',.  
+00031d90: 2020 2768 3427 2c0a 2020 2020 2768 3527    'h4',.    'h5'
+00031da0: 2c0a 2020 2020 2768 3627 2c0a 2020 2020  ,.    'h6',.    
+00031db0: 2768 6772 6f75 7027 2c0a 2020 2020 276d  'hgroup',.    'm
+00031dc0: 6169 6e27 2c0a 2020 2020 276e 6176 272c  ain',.    'nav',
+00031dd0: 0a20 2020 2027 7365 6374 696f 6e27 2c0a  .    'section',.
+00031de0: 2020 2020 2773 6561 7263 6827 2c0a 2020      'search',.  
+00031df0: 2020 2762 6c6f 636b 7175 6f74 6527 2c0a    'blockquote',.
+00031e00: 2020 2020 2764 6427 2c0a 2020 2020 2764      'dd',.    'd
+00031e10: 6976 272c 0a20 2020 2027 646c 272c 0a20  iv',.    'dl',. 
+00031e20: 2020 2027 6474 272c 0a20 2020 2027 6669     'dt',.    'fi
+00031e30: 6763 6170 7469 6f6e 272c 0a20 2020 2027  gcaption',.    '
+00031e40: 6669 6775 7265 272c 0a20 2020 2027 6872  figure',.    'hr
+00031e50: 272c 0a20 2020 2027 6c69 272c 0a20 2020  ',.    'li',.   
+00031e60: 2027 6d65 6e75 272c 0a20 2020 2027 6f6c   'menu',.    'ol
+00031e70: 272c 0a20 2020 2027 7027 2c0a 2020 2020  ',.    'p',.    
+00031e80: 2770 7265 272c 0a20 2020 2027 756c 272c  'pre',.    'ul',
+00031e90: 0a20 2020 2027 6127 2c0a 2020 2020 2761  .    'a',.    'a
+00031ea0: 6262 7227 2c0a 2020 2020 2762 272c 0a20  bbr',.    'b',. 
+00031eb0: 2020 2027 6264 6927 2c0a 2020 2020 2762     'bdi',.    'b
+00031ec0: 646f 272c 0a20 2020 2027 6272 272c 0a20  do',.    'br',. 
+00031ed0: 2020 2027 6369 7465 272c 0a20 2020 2027     'cite',.    '
+00031ee0: 636f 6465 272c 0a20 2020 2027 6461 7461  code',.    'data
+00031ef0: 272c 0a20 2020 2027 6466 6e27 2c0a 2020  ',.    'dfn',.  
+00031f00: 2020 2765 6d27 2c0a 2020 2020 2769 272c    'em',.    'i',
+00031f10: 0a20 2020 2027 6b62 6427 2c0a 2020 2020  .    'kbd',.    
+00031f20: 276d 6172 6b27 2c0a 2020 2020 2771 272c  'mark',.    'q',
+00031f30: 0a20 2020 2027 7270 272c 0a20 2020 2027  .    'rp',.    '
+00031f40: 7274 272c 0a20 2020 2027 7275 6279 272c  rt',.    'ruby',
+00031f50: 0a20 2020 2027 7327 2c0a 2020 2020 2773  .    's',.    's
+00031f60: 616d 7027 2c0a 2020 2020 2773 6d61 6c6c  amp',.    'small
+00031f70: 272c 0a20 2020 2027 7370 616e 272c 0a20  ',.    'span',. 
+00031f80: 2020 2027 7374 726f 6e67 272c 0a20 2020     'strong',.   
+00031f90: 2027 7375 6227 2c0a 2020 2020 2773 7570   'sub',.    'sup
+00031fa0: 272c 0a20 2020 2027 7469 6d65 272c 0a20  ',.    'time',. 
+00031fb0: 2020 2027 7527 2c0a 2020 2020 2776 6172     'u',.    'var
+00031fc0: 272c 0a20 2020 2027 7762 7227 2c0a 2020  ',.    'wbr',.  
+00031fd0: 2020 2761 7265 6127 2c0a 2020 2020 2761    'area',.    'a
+00031fe0: 7564 696f 272c 0a20 2020 2027 696d 6727  udio',.    'img'
+00031ff0: 2c0a 2020 2020 276d 6170 272c 0a20 2020  ,.    'map',.   
+00032000: 2027 7472 6163 6b27 2c0a 2020 2020 2776   'track',.    'v
+00032010: 6964 656f 272c 0a20 2020 2027 656d 6265  ideo',.    'embe
+00032020: 6427 2c0a 2020 2020 2769 6672 616d 6527  d',.    'iframe'
+00032030: 2c0a 2020 2020 276f 626a 6563 7427 2c0a  ,.    'object',.
+00032040: 2020 2020 2770 6963 7475 7265 272c 0a20      'picture',. 
+00032050: 2020 2027 706f 7274 616c 272c 0a20 2020     'portal',.   
+00032060: 2027 736f 7572 6365 272c 0a20 2020 2027   'source',.    '
+00032070: 6361 6e76 6173 272c 0a20 2020 2027 6e6f  canvas',.    'no
+00032080: 7363 7269 7074 272c 0a20 2020 2027 7363  script',.    'sc
+00032090: 7269 7074 272c 0a20 2020 2027 6465 6c5f  ript',.    'del_
+000320a0: 272c 0a20 2020 2027 696e 7327 2c0a 2020  ',.    'ins',.  
+000320b0: 2020 2763 6170 7469 6f6e 272c 0a20 2020    'caption',.   
+000320c0: 2027 636f 6c27 2c0a 2020 2020 2763 6f6c   'col',.    'col
+000320d0: 6772 6f75 7027 2c0a 2020 2020 2774 6162  group',.    'tab
+000320e0: 6c65 272c 0a20 2020 2027 7462 6f64 7927  le',.    'tbody'
+000320f0: 2c0a 2020 2020 2774 6427 2c0a 2020 2020  ,.    'td',.    
+00032100: 2774 666f 6f74 272c 0a20 2020 2027 7468  'tfoot',.    'th
+00032110: 272c 0a20 2020 2027 7468 6561 6427 2c0a  ',.    'thead',.
+00032120: 2020 2020 2774 7227 2c0a 2020 2020 2762      'tr',.    'b
+00032130: 7574 746f 6e27 2c0a 2020 2020 2764 6174  utton',.    'dat
+00032140: 616c 6973 7427 2c0a 2020 2020 2766 6965  alist',.    'fie
+00032150: 6c64 7365 7427 2c0a 2020 2020 2766 6f72  ldset',.    'for
+00032160: 6d27 2c0a 2020 2020 276c 6162 656c 272c  m',.    'label',
+00032170: 0a20 2020 2027 6c65 6765 6e64 272c 0a20  .    'legend',. 
+00032180: 2020 2027 6d65 7465 7227 2c0a 2020 2020     'meter',.    
+00032190: 276f 7074 6772 6f75 7027 2c0a 2020 2020  'optgroup',.    
+000321a0: 276f 7074 696f 6e27 2c0a 2020 2020 276f  'option',.    'o
+000321b0: 7574 7075 7427 2c0a 2020 2020 2770 726f  utput',.    'pro
+000321c0: 6772 6573 7327 2c0a 2020 2020 2773 656c  gress',.    'sel
+000321d0: 6563 7427 2c0a 2020 2020 2774 6578 7461  ect',.    'texta
+000321e0: 7265 6127 2c0a 2020 2020 2764 6574 6169  rea',.    'detai
+000321f0: 6c73 272c 0a20 2020 2027 6469 616c 6f67  ls',.    'dialog
+00032200: 272c 0a20 2020 2027 7375 6d6d 6172 7927  ',.    'summary'
+00032210: 2c0a 2020 2020 2773 6c6f 7427 2c0a 2020  ,.    'slot',.  
+00032220: 2020 2774 656d 706c 6174 6527 2c0a 5d0a    'template',.].
```

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__tags/input.py` & `pyhtml_enhanced-2.0.1/pyhtml/__tags/input.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__types.py` & `pyhtml_enhanced-2.0.1/pyhtml/__types.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.0/pyhtml/__util.py` & `pyhtml_enhanced-2.0.1/pyhtml/__util.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,37 +92,46 @@
     return {
         k: v
         for k, v in attributes.items()
         if v is not None and v is not False
     }
 
 
-def render_inline_element(ele: ChildElementType) -> list[str]:
+def render_inline_element(
+    ele: ChildElementType,
+    escape_strings: bool,
+) -> list[str]:
     """
     Render an element inline
     """
     from .__tag_base import Tag
     if isinstance(ele, Tag):
         return ele._render()
     elif isinstance(ele, type) and issubclass(ele, Tag):
         return ele()._render()
     else:
         # Remove newlines from strings when inline rendering
-        return [escape_string(str(ele))]
+        if escape_strings:
+            return [escape_string(str(ele))]
+        else:
+            return [str(ele)]
 
 
-def render_children(children: list[ChildElementType]) -> list[str]:
+def render_children(
+    children: list[ChildElementType],
+    escape_strings: bool,
+) -> list[str]:
     """
     Render child elements of tags.
 
     Elements are placed in the same string
     """
     rendered = []
     for ele in children:
-        rendered.extend(render_inline_element(ele))
+        rendered.extend(render_inline_element(ele, escape_strings))
     return increase_indent(rendered, 2)
 
 
 def flatten_list(the_list: list[ChildrenType]) -> list[ChildElementType]:
     """
     Flatten a list by taking any list elements and inserting their items
     individually. Note that other iterables (such as str and tuple) are not
```

### Comparing `pyhtml_enhanced-2.0.0/pyproject.toml` & `pyhtml_enhanced-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhtml-enhanced"
-version = "2.0.0"
+version = "2.0.1"
 description = "A library for building HTML documents with a simple and learnable syntax"
 authors = ["Miguel Guthridge <miguel.guthridge@unsw.edu.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyhtml"}]
 
 repository = "https://github.com/COMP1010UNSW/pyhtml-enhanced"
```

### Comparing `pyhtml_enhanced-2.0.0/PKG-INFO` & `pyhtml_enhanced-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtml-enhanced
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library for building HTML documents with a simple and learnable syntax
 Home-page: https://github.com/COMP1010UNSW/pyhtml-enhanced
 License: MIT
 Keywords: html,template,pyhtml,markup,documentation
 Author: Miguel Guthridge
 Author-email: miguel.guthridge@unsw.edu.au
 Requires-Python: >=3.9,<4.0
@@ -243,23 +243,30 @@
 
 ## Credits
 
 ### [Cenkalti/PyHTML](https://github.com/cenkalti/pyhtml)
 
 Cenk Altı's work was used as a source of inspiration and reference. Although
 all the code in `pyhtml-enhanced` was written by me, I want to thank them for
-the significant help their hard work provided while creating this project.
+the significant help their hard work provided while creating this project,
+going as far as to give design advice on request.
 
 ### [MDN Web Docs](https://developer.mozilla.org/en-US/)
 
 Almost all of the documentation was gathered from the MDN Web Docs. It's super
 neat that all their documentation is open (licensed as
 [CC-BY-SA-2.5](https://creativecommons.org/licenses/by-sa/2.5/) if you're
 interested).
 
+### COMP1010 students and staff
+
+COMP1010's students and staff members have uncovered and helped to resolve many
+bugs, and have suggested many improvements. I'd like to thank them for all of
+their help!
+
 ## License
 
 ### Source code
 
 Copyright (c) 2023 Miguel Guthridge, COMP1010 UNSW
 
 Source code for the library is open source, using the
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_f1t6j2wy_/tmp68jj2l5p_TarContainer/0/13", line 275, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyhtml-enhanced Version: 2.0.0 Summary: A library
+Metadata-Version: 2.1 Name: pyhtml-enhanced Version: 2.0.1 Summary: A library
 for building HTML documents with a simple and learnable syntax Home-page:
 https://github.com/COMP1010UNSW/pyhtml-enhanced License: MIT Keywords:
 html,template,pyhtml,markup,documentation Author: Miguel Guthridge Author-
 email: miguel.guthridge@unsw.edu.au Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

