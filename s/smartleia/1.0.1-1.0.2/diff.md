# Comparing `tmp/smartleia-1.0.1.tar.gz` & `tmp/smartleia-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartleia-1.0.1.tar", last modified: Thu Apr 29 21:30:28 2021, max compression
+gzip compressed data, was "smartleia-1.0.2.tar", last modified: Tue Apr  2 22:17:07 2024, max compression
```

## Comparing `smartleia-1.0.1.tar` & `smartleia-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2021-04-29 21:30:28.452902 smartleia-1.0.1/
--rw-r--r--   0 mre       (1000) mre       (1000)      151 2021-04-29 21:20:38.000000 smartleia-1.0.1/AUTHORS
--rw-r--r--   0 mre       (1000) mre       (1000)     1510 2021-04-29 21:20:38.000000 smartleia-1.0.1/LICENSE.bsd3
--rw-r--r--   0 mre       (1000) mre       (1000)    26539 2021-04-29 21:20:38.000000 smartleia-1.0.1/LICENSE.lgpl-2.1+
--rw-r--r--   0 mre       (1000) mre       (1000)     3397 2021-04-29 21:30:28.452902 smartleia-1.0.1/PKG-INFO
--rw-r--r--   0 mre       (1000) mre       (1000)     2408 2021-04-29 21:20:38.000000 smartleia-1.0.1/README.md
--rw-r--r--   0 mre       (1000) mre       (1000)       38 2021-04-29 21:30:28.452902 smartleia-1.0.1/setup.cfg
--rw-r--r--   0 mre       (1000) mre       (1000)     1509 2021-04-29 21:29:59.000000 smartleia-1.0.1/setup.py
-drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2021-04-29 21:30:28.452902 smartleia-1.0.1/smartleia/
--rw-r--r--   0 mre       (1000) mre       (1000)    42205 2021-04-29 21:20:38.000000 smartleia-1.0.1/smartleia/__init__.py
--rw-r--r--   0 mre       (1000) mre       (1000)     1640 2021-04-29 21:20:38.000000 smartleia-1.0.1/smartleia/__main__.py
--rw-r--r--   0 mre       (1000) mre       (1000)     7316 2021-04-29 21:20:38.000000 smartleia-1.0.1/smartleia/test_applet.py
-drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2021-04-29 21:30:28.452902 smartleia-1.0.1/smartleia.egg-info/
--rw-r--r--   0 mre       (1000) mre       (1000)     3397 2021-04-29 21:30:28.000000 smartleia-1.0.1/smartleia.egg-info/PKG-INFO
--rw-r--r--   0 mre       (1000) mre       (1000)      296 2021-04-29 21:30:28.000000 smartleia-1.0.1/smartleia.egg-info/SOURCES.txt
--rw-r--r--   0 mre       (1000) mre       (1000)        1 2021-04-29 21:30:28.000000 smartleia-1.0.1/smartleia.egg-info/dependency_links.txt
--rw-r--r--   0 mre       (1000) mre       (1000)      529 2021-04-29 21:30:28.000000 smartleia-1.0.1/smartleia.egg-info/requires.txt
--rw-r--r--   0 mre       (1000) mre       (1000)       10 2021-04-29 21:30:28.000000 smartleia-1.0.1/smartleia.egg-info/top_level.txt
+drwxr-xr-x   0 mre        (501) staff       (20)        0 2024-04-02 22:17:07.634763 smartleia-1.0.2/
+-rw-r--r--   0 mre        (501) staff       (20)      151 2024-04-02 22:12:38.000000 smartleia-1.0.2/AUTHORS
+-rw-r--r--   0 mre        (501) staff       (20)     1510 2024-04-02 22:12:38.000000 smartleia-1.0.2/LICENSE.bsd3
+-rw-r--r--   0 mre        (501) staff       (20)    26539 2024-04-02 22:12:38.000000 smartleia-1.0.2/LICENSE.lgpl-2.1+
+-rw-r--r--   0 mre        (501) staff       (20)     3847 2024-04-02 22:17:07.634557 smartleia-1.0.2/PKG-INFO
+-rw-r--r--   0 mre        (501) staff       (20)     2239 2024-04-02 22:12:38.000000 smartleia-1.0.2/README.md
+-rw-r--r--   0 mre        (501) staff       (20)       38 2024-04-02 22:17:07.634808 smartleia-1.0.2/setup.cfg
+-rw-r--r--   0 mre        (501) staff       (20)     1541 2024-04-02 22:14:47.000000 smartleia-1.0.2/setup.py
+drwxr-xr-x   0 mre        (501) staff       (20)        0 2024-04-02 22:17:07.632142 smartleia-1.0.2/smartleia/
+-rw-r--r--   0 mre        (501) staff       (20)    42922 2024-04-02 22:15:47.000000 smartleia-1.0.2/smartleia/__init__.py
+-rw-r--r--   0 mre        (501) staff       (20)     1663 2024-04-02 22:12:38.000000 smartleia-1.0.2/smartleia/__main__.py
+-rw-r--r--   0 mre        (501) staff       (20)     7316 2024-04-02 22:12:38.000000 smartleia-1.0.2/smartleia/test_applet.py
+drwxr-xr-x   0 mre        (501) staff       (20)        0 2024-04-02 22:17:07.633304 smartleia-1.0.2/smartleia.egg-info/
+-rw-r--r--   0 mre        (501) staff       (20)     3847 2024-04-02 22:17:07.000000 smartleia-1.0.2/smartleia.egg-info/PKG-INFO
+-rw-r--r--   0 mre        (501) staff       (20)      320 2024-04-02 22:17:07.000000 smartleia-1.0.2/smartleia.egg-info/SOURCES.txt
+-rw-r--r--   0 mre        (501) staff       (20)        1 2024-04-02 22:17:07.000000 smartleia-1.0.2/smartleia.egg-info/dependency_links.txt
+-rw-r--r--   0 mre        (501) staff       (20)      537 2024-04-02 22:17:07.000000 smartleia-1.0.2/smartleia.egg-info/requires.txt
+-rw-r--r--   0 mre        (501) staff       (20)       10 2024-04-02 22:17:07.000000 smartleia-1.0.2/smartleia.egg-info/top_level.txt
+drwxr-xr-x   0 mre        (501) staff       (20)        0 2024-04-02 22:17:07.633006 smartleia-1.0.2/tests/
+-rw-r--r--   0 mre        (501) staff       (20)       90 2024-04-02 22:15:22.000000 smartleia-1.0.2/tests/test_smartleia.py
```

### Comparing `smartleia-1.0.1/LICENSE.bsd3` & `smartleia-1.0.2/LICENSE.bsd3`

 * *Files identical despite different names*

### Comparing `smartleia-1.0.1/LICENSE.lgpl-2.1+` & `smartleia-1.0.2/LICENSE.lgpl-2.1+`

 * *Files identical despite different names*

### Comparing `smartleia-1.0.1/README.md` & `smartleia-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-[![GitHub license](https://img.shields.io/github/license/h2lab/smartleia)](https://github.com/h2lab/smartleia/blob/master/LICENSE.bsd3) [![Debian package](https://img.shields.io/debian/v/smartleia/unstable)](https://tracker.debian.org/pkg/smartleia) ![Build status](https://github.com/h2lab/smartleia/actions/workflows/main.yml/badge.svg) [![Sonarcloud Status](https://sonarcloud.io/api/project_badges/measure?project=h2lab_smartleia&metric=alert_status)](https://sonarcloud.io/dashboard?id=h2lab_smartleia)
+[![GitHub license](https://img.shields.io/github/license/h2lab/smartleia)](https://github.com/h2lab/smartleia/blob/master/LICENSE.bsd3) [![Debian package](https://img.shields.io/debian/v/smartleia/unstable)](https://tracker.debian.org/pkg/smartleia) ![Build status](https://github.com/h2lab/smartleia/actions/workflows/main.yml/badge.svg)
 
 
 # SmartLeia
 
 This repository holds the source of the python package used to drive the LEIA
 smartcard reader. With it, you will be able to:
```

### Comparing `smartleia-1.0.1/setup.py` & `smartleia-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,23 @@
     with open(readme_path, 'rb') as stream:
         readme = stream.read().decode('utf8')
 
 
 setup(
     long_description=readme,
     name='smartleia',
-    version='1.0.1',
+    version='1.0.2',
     description='Python toolkit for LEIA smartcard reader',
     python_requires='==3.*,>=3.6.0',
     project_urls={"homepage": "https://h2lab.org/devices/leia/quickstart/", "repository": "https://github.com/h2lab/smartleia"},
     author='LEIA Team',
     author_email='leia@h2lab.org',
     license='LGPL-2.1+',
     packages=['smartleia'],
     package_dir={"": "."},
     package_data={"smartleia": ["*.csv", "*.ipynb"]},
-    install_requires=['dephell==0.*,>=0.8.3', 'pyserial==3.*,>=3.4.0', 'pytest==5.*,>=5.2.0', 'pytest-csv==2.*,>=2.0.2'],
-    extras_require={"dev": ["black==19.*,>=19.10.0.b0", "bump2version==1.*,>=1.0.0", "coverage==5.*,>=5.1.0", "flake8==3.*,>=3.7.9", "ipython==7.*,>=7.14.0", "mypy==0.*,>=0.770.0", "nbsphinx==0.*,>=0.7.0", "pandoc==1.*,>=1.0.2", "pre-commit==2.*,>=2.3.0", "pylint==2.*,>=2.5.2", "pytest-runner==5.*,>=5.2.0", "recommonmark==0.*,>=0.6.0", "sphinx==3.*,>=3.0.0", "sphinx-autodoc-typehints==1.*,>=1.10.3", "sphinx-rtd-theme==0.*,>=0.5.0", "sphinxcontrib.spelling==5.*,>=5.0.0", "sphinxcontrib.wavedrom==2.*,>=2.1.0"]},
+    install_requires=['pyserial==3.*,>=3.4.0'],
+    extras_require={
+        "dev": ["dephell==0.*,>=0.8.3", "black==19.*,>=19.10.0.b0", "bump2version==1.*,>=1.0.0", "coverage==5.*,>=5.1.0", "flake8==3.*,>=3.7.9", "ipython==7.*,>=7.14.0", "mypy==0.*,>=0.770.0", "nbsphinx==0.*,>=0.7.0", "pandoc==1.*,>=1.0.2", "pre-commit==2.*,>=2.3.0", "pylint==2.*,>=2.5.2", "pytest-runner==5.*,>=5.2.0", "recommonmark==0.*,>=0.6.0", "sphinx==3.*,>=3.0.0", "sphinx-autodoc-typehints==1.*,>=1.10.3", "sphinx-rtd-theme==0.*,>=0.5.0", "sphinxcontrib.spelling==5.*,>=5.0.0", "sphinxcontrib.wavedrom==2.*,>=2.1.0"],
+        "test": ['pytest==5.*,>=5.2.0', 'pytest-csv==2.*,>=2.0.2']
+    },
 )
```

### Comparing `smartleia-1.0.1/smartleia/__init__.py` & `smartleia-1.0.2/smartleia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "create_APDU_from_bytes",
     "APDU",
     "RESP",
     "ATR",
     "LEIA",
 ]
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 name = "smartleia"
 
 
 COMMAND_LEN_SIZE = 4
 RESPONSE_LEN_SIZE = 4
 TRIGGER_DEPTH = 10
@@ -37,14 +37,32 @@
 # NOTE: because of firmware SRAM constraints, we only
 # support this size for now.
 MAX_APDU_PAYLOAD_SIZE = 16384
 
 ERR_FLAGS = {0x00: "OK", 0x01: "PLATFORM_ERR_CARD_NOT_INSERTED", 0xFF: "UNKNOWN_ERROR"}
 
 
+class LEIAException(Exception):
+    """A LEIA exception."""
+
+    pass
+
+
+class CardNotInsertedError(LEIAException):
+    """Card needs to be inserted and is not."""
+
+    pass
+
+
+class CardConfigureError(LEIAException):
+    """Card cannot be configured."""
+
+    pass
+
+
 class LEIAStructure(ctypes.Structure):
     """
     Base structure for exchanging data with LEIA.
     """
 
     def pack(self):
         return bytes(self)[:]
@@ -72,31 +90,32 @@
 class Timers(LEIAStructure):
     _pack_ = 1
     _fields_ = [
         ("delta_t", ctypes.c_uint32),
         ("delta_t_answer", ctypes.c_uint32),
     ]
 
-    def __init__(self, delta_t = 0, delta_t_answer = 0):
+    def __init__(self, delta_t=0, delta_t_answer=0):
         """
         Create a Timers structure.
 
         Parameters:
             delta_t (int) : total time for the APDU.
             delta_t_answer (int) : answer time for the APDU.
         """
-        LEIAStructure.__init__(self, delta_t = 0, delta_t_answer = 0)
+        LEIAStructure.__init__(self, delta_t=0, delta_t_answer=0)
         self.delta_t = self.delta_t_answer = 0
 
     def __str__(self) -> str:
         return f"""Timers(
         delta_t={self.delta_t:d} microseconds,
         delta_t_answer={self.delta_t_answer:d} microseconds,
         )"""
- 
+
+
 ##### Triggers handling ######
 class TriggerPoints(IntFlag):
     """
     Class utility to reference the trigger points available.
     """
 
     #: Point before getting the ATR.
@@ -149,15 +168,15 @@
     # Triggers after the first byte of an APDU has been sent: first trig
     # just after we have sent our APDU command, second trig when receiving
     # the first response byte from the card.
     MULTI_TRIG_AFTER_1ST_BYTE_SEND_APDU = [
         TriggerPoints.TRIG_PRE_SEND_APDU,
         TriggerPoints.TRIG_IRQ_PUTC,
     ]
-    
+
 
 class TriggerStrategy(LEIAStructure):
     """
     Attributes:
         delay (int): the delay between event detection and effective trig on GPIO in milliseconds.
         point_list (list[int]): the list of events to match.
     """
@@ -201,17 +220,17 @@
         return r
 
     @point_list.setter
     def point_list(self, value):
         value = self._translate_point_list(value)
 
         if not isinstance(value, list):
-            raise Exception("data should be a list")
+            raise TypeError("point_list should be a list")
         if len(value) > len(self._list):
-            raise Exception("Size of data too high")
+            raise ValueError("Size of point_list too large")
         for i, v in enumerate(value):
             self._list[i] = value[i]
         self.size = len(value)
 
     @property
     def point_list_trigged(self):
         _point_list_trigged = list(self._list_trigged)[0 : self.size]
@@ -231,43 +250,42 @@
     @property
     def event_time_list(self):
         _event_time_list = list(self._event_time)[0 : self.size]
 
         return _event_time_list
 
 
-
 class SetTriggerStrategy(LEIAStructure):
     _pack_ = 1
     _fields_ = [("index", ctypes.c_uint8), ("strategy", TriggerStrategy)]
 
     def __str__(self) -> str:
         return f"SetTriggerStrategy(index={self.index}, strategy={self.strategy})"
 
 
 class ATR(LEIAStructure):
     """This class is used to represent an ATR.
 
-       Attributes:
-           ts (ctypes.c_uint8): Description of `attr1`.
-           t0 (ctypes.c_uint8): Description of `attr2`.
-           ta (ctypes.c_uint8[4]): Description of `attr1`.
-           tb (ctypes.c_uint8[4]): Description of `attr2`.
-           tc (ctypes.c_uint8[4]): Description of `attr1`.
-           td (ctypes.c_uint8[4]): Description of `attr2`.
-           h (ctypes.c_uint8[16]): Description of `attr1`.
-           t_mask (ctypes.c_uint8[4]): Description of `attr2`.
-           h_num (ctypes.c_uint8): Description of `attr1`.
-           tck (ctypes.c_uint8): Description of `attr2`.
-           tck_present (ctypes.c_uint8): Description of `attr1`.
-           D_i_curr (ctypes.c_uint32): Description of `attr2`.
-           F_i_curr (ctypes.c_uint32): Description of `attr1`.
-           f_max_curr (ctypes.c_uint32): Description of `attr2`.
-           T_protocol_curr (ctypes.c_uint8): Description of `attr1`.
-           ifsc (ctypes.c_uint8): Description of `attr2`.
+    Attributes:
+        ts (ctypes.c_uint8): Description of `attr1`.
+        t0 (ctypes.c_uint8): Description of `attr2`.
+        ta (ctypes.c_uint8[4]): Description of `attr1`.
+        tb (ctypes.c_uint8[4]): Description of `attr2`.
+        tc (ctypes.c_uint8[4]): Description of `attr1`.
+        td (ctypes.c_uint8[4]): Description of `attr2`.
+        h (ctypes.c_uint8[16]): Description of `attr1`.
+        t_mask (ctypes.c_uint8[4]): Description of `attr2`.
+        h_num (ctypes.c_uint8): Description of `attr1`.
+        tck (ctypes.c_uint8): Description of `attr2`.
+        tck_present (ctypes.c_uint8): Description of `attr1`.
+        D_i_curr (ctypes.c_uint32): Description of `attr2`.
+        F_i_curr (ctypes.c_uint32): Description of `attr1`.
+        f_max_curr (ctypes.c_uint32): Description of `attr2`.
+        T_protocol_curr (ctypes.c_uint8): Description of `attr1`.
+        ifsc (ctypes.c_uint8): Description of `attr2`.
     """
 
     _pack_ = 1
     _fields_ = [
         ("ts", ctypes.c_uint8),
         ("t0", ctypes.c_uint8),
         ("ta", ctypes.c_uint8 * 4),
@@ -441,17 +459,17 @@
     @property
     def data(self):
         return list(self._data)[0 : self.lc]
 
     @data.setter
     def data(self, value):
         if not isinstance(value, list):
-            raise Exception("data should be a list")
+            raise TypeError("data should be a list")
         if len(value) > len(self._data):
-            raise Exception("Size of data too high")
+            raise ValueError("Size of data too high")
         for i, v in enumerate(value):
             self._data[i] = value[i]
         self.lc = len(value)
 
     def normalized(self) -> bytes:
         b = b""
         b += ctypes.string_at(ctypes.addressof(self), APDU.lc.offset)
@@ -472,21 +490,25 @@
         >>> create_APDU_from_bytes([0x00,0x01,0x02,0x03,0x04,0x05,0x06,0x07,0x08,0x09])
         APDU(cla=0x00, ins=0x01, p1=0x02, p2=0x03, lc=0x04, data=[0x05, 0x06, 0x07, 0x08], le=0x09, send_le=1)
     """
     apdu = APDU()
     apdu.cla, apdu.ins, apdu.p1, apdu.p2 = _bytes[:4]
     apdu.send_le = 0
 
-    if len(_bytes) < 5:
-        raise NotImplementedError(
-            "Error in decoding APDU buffer of size %d is too small" % (len(_bytes))
-        )
     if len(_bytes) == 5:
         apdu.lc, apdu.le = 0, _bytes[4]
         apdu.send_le = 1
+    elif len(_bytes) == 4:
+        # send_le = 0 and the below give a short 4-byte APDU
+        apdu.lc = 0
+        apdu.le = 0
+    elif len(_bytes) < 4:
+        raise NotImplementedError(
+            "Error in decoding APDU buffer of size %d is too small" % (len(_bytes))
+        )
     else:
         apdu.lc, apdu.le = _bytes[4], 0
         if apdu.lc == 0x00 and len(_bytes) >= 8:
             # This is an extended APDU, try to decode Lc on 16 bits
             apdu.send_le = 2
             apdu.lc = (_bytes[5] << 16) + _bytes[6]
             # Get the data
@@ -567,27 +589,29 @@
         )
         self.data = data
 
     def __str__(self) -> str:
         return (
             f"RESP(sw1=0x{self.sw1:02X}, sw2=0x{self.sw2:02X}, le={hex(self.le)}"
             + (f", data={self.data}" if self.le != 0 else "")
-            + (f")\ndelta_t={self.delta_t:d} microseconds, delta_t_answer={self.delta_t_answer:d} microseconds")
+            + (
+                f")\ndelta_t={self.delta_t:d} microseconds, delta_t_answer={self.delta_t_answer:d} microseconds"
+            )
         )
 
     @property
     def data(self):
         return list(self._data)[0 : self.le]
 
     @data.setter
     def data(self, value):
         if not isinstance(value, list):
-            raise Exception("data should be a list")
+            raise TypeError("data should be a list")
         if len(value) > len(self._data):
-            raise Exception("Size of data too high")
+            raise ValueError("Size of data too high")
         for i, v in enumerate(value):
             self._data[i] = value[i]
         self.le = len(value)
 
     def normalized(self) -> bytes:
         b = b""
         b += ctypes.string_at(ctypes.addressof(self) + RESP._data.offset, self.le)
@@ -606,25 +630,27 @@
 
     #: The protocol is T=0
     T0 = 0
 
     #: The protocol is T=1
     T1 = 1
 
+
 class Mode(IntEnum):
     """
     ISO7816 mode selection.
     """
-   
+
     # USART mode
     USART = 0
 
     # Bitbang mode
     BITBANG = 1
 
+
 class LEIAMode(LEIAStructure):
     _pack_ = 1
     _fields_ = [
         ("mode", ctypes.c_uint8),
     ]
 
     def __init__(
@@ -822,26 +848,22 @@
     # Set the mode to either USART or BITBANG
     def set_mode(self, mode: Mode):
         if mode == Mode.USART:
             self._send_command(b"e", LEIAMode(Mode.USART))
         elif mode == Mode.BITBANG:
             self._send_command(b"e", LEIAMode(Mode.BITBANG))
         else:
-            raise Exception(
-                "Invalid mode for 'set_mode' (e) command."
-            )
-        
+            raise ValueError("Invalid mode for 'set_mode' (e) command.")
+
     # Get the current mode
     def get_mode(self):
         self._send_command(b"g")
         r_size = self._read_response_size()
         if r_size != 1:
-            raise Exception(
-                "Invalid response size for 'get_mode' (g) command."
-            )
+            raise LEIAException("Invalid response size for 'get_mode' (g) command.")
         r = self.ser.read(1)
         if r == b"\x00":
             mode = Mode.USART
         elif r == b"\x01":
             mode = Mode.BITBANG
         else:
             mode = None
@@ -872,16 +894,18 @@
         Parameters:
             protocol_to_use: The protocol to use (0: T=0, 1: T=1).
             ETU_to_use: The ETU value to force. If None, will be negociated (or default will be used).
             freq_to_use: The ISO7816 clock frequency to use. If None, will be negociated (or default will be used).
             negotiate_pts: if LEIA can try to negotiate the PTS.
             negotiate_baudrate: if LEIA can negotiate the baudrate. There is not impact if `ETU_to_use` and `freq_to_use` are set.
         """
-        if self.is_card_inserted() == False:
-            raise Exception("Error: card not inserted! Please insert a card to configure it.")
+        if not self.is_card_inserted():
+            raise CardNotInsertedError(
+                "Card not inserted! Please insert a card to configure it."
+            )
 
         with self.lock:
             self._testWaitingFlag()
 
             self.reconfigured = True
             self.curr_atr = None
 
@@ -907,15 +931,15 @@
             if negotiate_baudrate is None:
                 _negotiate_baudrate = True
             else:
                 _negotiate_baudrate = negotiate_baudrate
 
             # We always try to negotiate a T=1 communication if not specifically asked otherwise
             # Fallback to auto if this is not possible!
-            if (protocol_to_use == T.AUTO):
+            if protocol_to_use == T.AUTO:
                 try:
                     struct = ConfigureSmartcardCommand(
                         T(T.T1).value + 1,
                         ETU_to_use,
                         freq_to_use,
                         _negotiate_pts,
                         _negotiate_baudrate,
@@ -928,101 +952,121 @@
                             ETU_to_use,
                             freq_to_use,
                             _negotiate_pts,
                             _negotiate_baudrate,
                         )
                         self._send_command(b"c", struct)
                     except Exception:
-                        if negotiate_pts == None:
+                        if negotiate_pts is None:
                             try:
                                 # If we have not been asked to specifically negotiate
                                 struct = ConfigureSmartcardCommand(
                                     T(T.AUTO).value + 1,
                                     ETU_to_use,
                                     freq_to_use,
                                     False,
                                     _negotiate_baudrate,
                                 )
                                 self._send_command(b"c", struct)
                             except Exception:
-                                raise Exception("Error: configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!")
+                                raise CardConfigureError(
+                                    "Configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!"
+                                )
                         else:
-                                raise Exception("Error: configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!")
+                            raise CardConfigureError(
+                                "Configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!"
+                            )
             else:
                 try:
                     struct = ConfigureSmartcardCommand(
                         _protocol_to_use,
                         ETU_to_use,
                         freq_to_use,
                         _negotiate_pts,
                         _negotiate_baudrate,
                     )
                     self._send_command(b"c", struct)
                 except Exception:
-                    if negotiate_pts == None:
+                    if negotiate_pts is None:
                         try:
                             # If we have not been asked to specifically negotiate
                             struct = ConfigureSmartcardCommand(
                                 _protocol_to_use,
                                 ETU_to_use,
                                 freq_to_use,
                                 False,
                                 _negotiate_baudrate,
                             )
                             self._send_command(b"c", struct)
                         except Exception:
-                            raise Exception("Error: configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!")
+                            raise CardConfigureError(
+                                "Configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!"
+                            )
                     else:
-                        raise Exception("Error: configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!")
+                        raise CardConfigureError(
+                            "Configure_smartcard failed with the asked parameters! Please check what your card supports (PTS, ETU, ...) and try other parameters!"
+                        )
 
     def get_trigger_strategy(self, SID: int) -> TriggerStrategy:
         """
         Returns the strategy N°SID.
 
         Parameters:
             SID: The trigger strategy's ID to get.
 
         Returns:
             TriggerStrategy: The trigger strategy N°SID.
         """
+        if SID >= STRATEGY_MAX:
+            raise ValueError(
+                "get_trigger_strategy: asked SID=%d exceeds STRATEGY_MAX=%d"
+                % (SID, STRATEGY_MAX)
+            )
 
         with self.lock:
-            if SID >= STRATEGY_MAX:
-                raise Exception("get_trigger_strategy: asked SID=%d exceeds STRATEGY_MAX=%d" % (SID, STRATEGY_MAX))
-           
+
             self._send_command(b"o", ByteStruct(SID))
 
             r_size = self._read_response_size()
             r = TriggerStrategy(TRIGGER_DEPTH).unpack(self.ser.read(r_size))
 
         return r
 
     def set_trigger_strategy(
-        self, SID: int, point_list: Union[int, List[int]], delay: int = 0, single: int = 0
+        self,
+        SID: int,
+        point_list: Union[int, List[int]],
+        delay: int = 0,
+        single: int = 0,
     ):
         """
         Set and activate a trigger strategy.
 
         Parameters:
             SID: the strategy bank ID to use.
             point_list: the sequence to match for the trigger.
             delay: the delay (in milliseconds) between the moment of the detection and the moment where the trigger is actually set high.
         """
+        if SID >= STRATEGY_MAX:
+            raise ValueError(
+                "get_trigger_strategy: asked SID=%d exceeds STRATEGY_MAX=%d"
+                % (SID, STRATEGY_MAX)
+            )
 
         with self.lock:
-            if SID >= STRATEGY_MAX:
-                raise Exception("get_trigger_strategy: asked SID=%d exceeds STRATEGY_MAX=%d" % (SID, STRATEGY_MAX))
 
             if isinstance(point_list, int):
                 size = 1
                 point_list = [point_list]
 
             size = len(point_list)
 
-            sts = SetTriggerStrategy(SID, TriggerStrategy(delay = delay, single = single, point_list = point_list))
+            sts = SetTriggerStrategy(
+                SID, TriggerStrategy(delay=delay, single=single, point_list=point_list)
+            )
 
             self._send_command(b"O", sts)
 
     def get_timers(self) -> Timers:
         """
         Return the `timers` of the last command.
 
@@ -1063,15 +1107,15 @@
         """
 
         with self.lock:
             self._send_command(b"?")
 
             r_size = self._read_response_size()
             if r_size != 1:
-                raise Exception(
+                raise LEIAException(
                     "Invalid response size for 'is_card_inserted' (?) command."
                 )
             r = self.ser.read(1)
 
         return True if r == b"\x01" else False
 
     # DFU mode
@@ -1091,15 +1135,15 @@
         Reboot LEIA in funcard flasher mode.
         """
         with self.lock:
             try:
                 self._send_command(b"f")
             except serial.SerialException:
                 pass
- 
+
     def smartreader(self) -> None:
         """
         Reboot LEIA in funcard smartreader mode.
         """
         with self.lock:
             try:
                 self._send_command(b"s")
@@ -1170,15 +1214,15 @@
             try:
                 s.connect((host, port))
             except Exception as e:
                 print(
                     "Error: cannot connect to %s:%d. Is PCSCD running with virtual smartcard readers?"
                     % (host, port)
                 )
-                raise (e)
+                raise e
 
             s.settimeout(10)
 
             while (
                 self.is_card_inserted() and not self.reconfigured and not self.pcsc_stop
             ):
                 # Now wait for data to come
```

### Comparing `smartleia-1.0.1/smartleia/__main__.py` & `smartleia-1.0.2/smartleia/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,30 +38,32 @@
         except:
             print("Error: are you sure that a smartcard is inserted in the LEIA board?")
             sys.exit(42)
 
     try:
         leia.pcsc_relay()
     except:
-        print("Error: error in pcsc_relay, is PCSCD running? Launch in a terminal with 'pcscd -fad'")
+        print(
+            "Error: error in pcsc_relay, is PCSCD running? Launch in a terminal with 'pcscd -fad'"
+        )
         sys.exit(42)
 
     code.interact(
         local=locals(),
         banner="""
 
         The connection with LEIA is opened and is connected to pcscd through virtualsmartcard.
 
         You can change the link with the smartcard with the following commands :
 
             configure( protocol_to_use=0,
                        ETU_to_use=...,
                        freq_to_use=...,
                        negotiate_pts=True,
-                       negotiate_baudate=True)
+                       negotiate_baudrate=True)
 
             t0()    Equivalent to configure(protocol_to_use=0)
             t1()    Equivalent to configure(protocol_to_use=1)
             dfu()
 
         You have access to leia through the `leia` variable.
```

### Comparing `smartleia-1.0.1/smartleia/test_applet.py` & `smartleia-1.0.2/smartleia/test_applet.py`

 * *Files identical despite different names*

### Comparing `smartleia-1.0.1/smartleia.egg-info/requires.txt` & `smartleia-1.0.2/smartleia.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-dephell==0.*,>=0.8.3
 pyserial==3.*,>=3.4.0
-pytest==5.*,>=5.2.0
-pytest-csv==2.*,>=2.0.2
 
 [dev]
+dephell==0.*,>=0.8.3
 black==19.*,>=19.10.0.b0
 bump2version==1.*,>=1.0.0
 coverage==5.*,>=5.1.0
 flake8==3.*,>=3.7.9
 ipython==7.*,>=7.14.0
 mypy==0.*,>=0.770.0
 nbsphinx==0.*,>=0.7.0
@@ -17,7 +15,11 @@
 pytest-runner==5.*,>=5.2.0
 recommonmark==0.*,>=0.6.0
 sphinx==3.*,>=3.0.0
 sphinx-autodoc-typehints==1.*,>=1.10.3
 sphinx-rtd-theme==0.*,>=0.5.0
 sphinxcontrib.spelling==5.*,>=5.0.0
 sphinxcontrib.wavedrom==2.*,>=2.1.0
+
+[test]
+pytest==5.*,>=5.2.0
+pytest-csv==2.*,>=2.0.2
```

