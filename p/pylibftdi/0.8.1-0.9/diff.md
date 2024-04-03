# Comparing `tmp/pylibftdi-0.8.1.tar.gz` & `tmp/pylibftdi-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibftdi-0.8.1.tar", last modified: Thu Jun  2 21:04:34 2011, max compression, from Unix
+gzip compressed data, was "dist/pylibftdi-0.9.tar", last modified: Mon Jan 23 22:51:01 2012, max compression
```

## Comparing `pylibftdi-0.8.1.tar` & `pylibftdi-0.9.tar`

### file list

```diff
@@ -1,22 +1,12 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2011-06-02 21:04:34.000000 pylibftdi-0.8.1/
--rw-r--r--   0 ben        (501) staff       (20)     2686 2011-06-02 21:01:29.000000 pylibftdi-0.8.1/CHANGES.txt
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2011-06-02 21:04:34.000000 pylibftdi-0.8.1/examples/
--rw-r--r--   0 ben        (501) staff       (20)     1111 2011-02-02 22:39:36.000000 pylibftdi-0.8.1/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)     5684 2011-06-02 21:04:34.000000 pylibftdi-0.8.1/PKG-INFO
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2011-06-02 21:04:34.000000 pylibftdi-0.8.1/pylibftdi/
--rw-r--r--   0 ben        (501) staff       (20)     3975 2011-05-03 22:52:45.000000 pylibftdi-0.8.1/README.txt
--rwxr-xr-x   0 ben        (501) staff       (20)      987 2011-06-02 18:30:16.000000 pylibftdi-0.8.1/setup.py
--rw-r--r--   0 ben        (501) staff       (20)     1472 2011-06-02 18:30:54.000000 pylibftdi-0.8.1/pylibftdi/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)       82 2011-06-02 19:58:20.000000 pylibftdi-0.8.1/pylibftdi/.__base.py
--rw-r--r--   0 ben        (501) staff       (20)      985 2011-06-02 19:58:20.000000 pylibftdi-0.8.1/pylibftdi/_base.py
--rw-r--r--   0 ben        (501) staff       (20)     3294 2011-06-02 19:36:41.000000 pylibftdi-0.8.1/pylibftdi/bitbang.py
--rw-r--r--   0 ben        (501) staff       (20)    17078 2011-06-02 21:00:06.000000 pylibftdi-0.8.1/pylibftdi/driver.py
--rw-r--r--   0 ben        (501) staff       (20)     3312 2011-06-02 20:18:06.000000 pylibftdi-0.8.1/pylibftdi/test_bitbang.py
--rw-r--r--   0 ben        (501) staff       (20)     2843 2011-06-02 20:41:42.000000 pylibftdi-0.8.1/pylibftdi/test_common.py
--rw-r--r--   0 ben        (501) staff       (20)     2443 2011-06-02 20:55:29.000000 pylibftdi-0.8.1/pylibftdi/test_driver.py
--rw-r--r--   0 ben        (501) staff       (20)      171 2011-02-02 22:40:42.000000 pylibftdi-0.8.1/pylibftdi/._util.py
--rw-r--r--   0 ben        (501) staff       (20)     2273 2011-02-02 22:40:42.000000 pylibftdi-0.8.1/pylibftdi/util.py
--rw-r--r--   0 ben        (501) staff       (20)     2630 2011-02-09 20:57:38.000000 pylibftdi-0.8.1/examples/lcd.py
--rw-r--r--   0 ben        (501) staff       (20)      171 2011-02-02 22:45:09.000000 pylibftdi-0.8.1/examples/._led_flash.py
--rw-r--r--   0 ben        (501) staff       (20)      503 2011-02-02 22:45:09.000000 pylibftdi-0.8.1/examples/led_flash.py
--rw-r--r--   0 ben        (501) staff       (20)      136 2011-02-09 19:47:32.000000 pylibftdi-0.8.1/examples/list_devices.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2012-01-23 22:51:01.000000 pylibftdi-0.9/
+-rw-r--r--   0 ben        (501) staff       (20)     3155 2012-01-23 22:45:19.000000 pylibftdi-0.9/CHANGES.txt
+-rw-r--r--   0 ben        (501) staff       (20)     1111 2012-01-03 21:34:54.000000 pylibftdi-0.9/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     5737 2012-01-23 22:51:01.000000 pylibftdi-0.9/PKG-INFO
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2012-01-23 22:51:01.000000 pylibftdi-0.9/pylibftdi/
+-rw-r--r--   0 ben        (501) staff       (20)     1503 2012-01-23 22:47:13.000000 pylibftdi-0.9/pylibftdi/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)      991 2012-01-03 21:34:54.000000 pylibftdi-0.9/pylibftdi/_base.py
+-rw-r--r--   0 ben        (501) staff       (20)     3919 2012-01-03 21:34:54.000000 pylibftdi-0.9/pylibftdi/bitbang.py
+-rw-r--r--   0 ben        (501) staff       (20)    17120 2012-01-03 21:34:54.000000 pylibftdi-0.9/pylibftdi/driver.py
+-rw-r--r--   0 ben        (501) staff       (20)     1432 2012-01-03 21:34:54.000000 pylibftdi-0.9/pylibftdi/util.py
+-rw-r--r--   0 ben        (501) staff       (20)     3967 2012-01-23 22:42:22.000000 pylibftdi-0.9/README.txt
+-rwxr-xr-x   0 ben        (501) staff       (20)      985 2012-01-23 22:41:00.000000 pylibftdi-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pylibftdi-0.8.1/CHANGES.txt` & `pylibftdi-0.9/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 pylibftdi changes
 =================
 
+0.9
+ * improved and extended tests
+ * made a start on some Sphinx-based documentation
+ * fixed long-standing issue with input from a BitBangDevice
+ * allow the PID/VID to be changed
+ * add new examples
+   - basic web server to toggle / read IO bits
+   - magic_candle.py - example of using input and output together
+   - pin_read.py - read and match values on device pins
+ * All of this needs some tidying, but it fixes some key issues and has been unreleased too long.
 0.8.1
  * fix issue with bitbang following API changes in 0.8
  * add tests for bitbang mode
  * refactor tests; fix text-based tests in Python3
  * slight refactor Device() to improve testability (_read and _write methods)
 0.8
  * added some unit tests
```

### Comparing `pylibftdi-0.8.1/LICENSE.txt` & `pylibftdi-0.9/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2010-2011 Ben Bass
+Copyright (c) 2010-2012 Ben Bass
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylibftdi-0.8.1/PKG-INFO` & `pylibftdi-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 1.0
 Name: pylibftdi
-Version: 0.8.1
+Version: 0.9
 Summary: Pythonic interface to FTDI devices using libftdi
 Home-page: http://bitbucket.org/codedstructure/pylibftdi
 Author: Ben Bass
 Author-email: benbass@codedstructure.net
 License: UNKNOWN
 Description: pylibftdi
         =========
         
         pylibftdi is a minimal Pythonic interface to FTDI devices using libftdi_.
         
         .. _libftdi: http://www.intra2net.com/en/developer/libftdi/
         
         :Features:
         
-        - Supports Python 2 and Python 3
-        - Supports parallel and serial devices
-        - Support for multiple devices
-        - File-like interface wherever appropriate
-        - Cross-platform
+         - Supports Python 2 and Python 3
+         - Supports parallel and serial devices
+         - Support for multiple devices
+         - File-like interface wherever appropriate
+         - Cross-platform
         
         :Limitations:
         
-        - Currently only one port per device is used; I've not tested with dual
-        port devices yet.
-        - The API might change prior to reaching a 1.0 release.
+         - Currently only one port per device is used; I've not tested with dual
+           port devices yet.
+         - The API might change prior to reaching a 1.0 release.
         
         Usage
         -----
         
         The primary interface is the ``Device`` class in the pylibftdi package; this
         gives serial access on relevant FTDI devices (e.g. the UM232R), providing a
         file-like interface (read, write).  Baudrate is controlled with the ``baudrate``
@@ -47,47 +47,47 @@
         number fails.
         
         Examples
         ~~~~~~~~
         
         ::
         
-        >>> from pylibftdi import Device
-        >>>
-        >>> with Device(mode='t') as dev:
-        ...     dev.baudrate = 115200
-        ...     dev.write('Hello World')
+            >>> from pylibftdi import Device
+            >>>
+            >>> with Device(mode='t') as dev:
+            ...     dev.baudrate = 115200
+            ...     dev.write('Hello World')
         
         The pylibftdi.BitBangDevice wrapper provides access to the parallel IO mode of
         operation through the ``port`` and ``direction`` properties.  These provide an
         8 bit IO port including all the relevant bit operations to make things simple.
         
         ::
         
-        >>> from pylibftdi import BitBangDevice
-        >>>
-        >>> with BitBangDevice('FTE00P4L') as bb:
-        ...     bb.direction = 0x0F  # four LSB are output(1), four MSB are input(0)
-        ...     bb.port |= 2         # set bit 1
-        ...     bb.port &= 0xFE      # clear bit 0
+            >>> from pylibftdi import BitBangDevice
+            >>>
+            >>> with BitBangDevice('FTE00P4L') as bb:
+            ...     bb.direction = 0x0F  # four LSB are output(1), four MSB are input(0)
+            ...     bb.port |= 2         # set bit 1
+            ...     bb.port &= 0xFE      # clear bit 0
         
-        There is support for a number of external devices and protocols, specifically
-        for interfacing with HD44780 LCDs using the 4-bit interface.
+        There is support for a number of external devices and protocols, including
+        interfacing with HD44780 LCDs using the 4-bit interface.
         
         History & Motivation
         --------------------
         This package is the result of various bits of work using FTDI's
         devices, primarily for controlling external devices.  Some of this
         is documented on the codedstructure blog, codedstructure.blogspot.com
         
         At least two other open-source Python FTDI wrappers exist, and each
         of these may be best for some projects.
         
-        * ftd2xx_ - ctypes binding to FTDI's own D2XX driver
-        * pyftdi_ - a C extension libftdi binding
+         * ftd2xx_ - ctypes binding to FTDI's own D2XX driver
+         * pyftdi_ - a C extension libftdi binding
         
         .. _ftd2xx: http://pypi.python.org/pypi/ftd2xx
         .. _pyftdi: http://git.marcansoft.com/?p=pyftdi.git
         
         pylibftdi exists in the gap between these two projects; ftd2xx uses
         the (closed-source) D2XX driver, but provides a high-level Python
         interface, while pyftdi works with libftdi but is very low-level.
@@ -95,23 +95,23 @@
         a high-level Pythonic interface.  Various wrappers and utility
         functions are also part of the distribution; following Python's
         batteries included approach, there are various interesting devices
         supported out-of-the-box - or at least there will be soon!
         
         Plans
         -----
-        * Add more examples: SPI devices, knight-rider effects, input devices, MIDI...
-        * Perhaps add support for D2XX driver, though the name then becomes a
-        slight liability ;)
-        * General code quality improvements: solid unit tests, decent documentation.
+         * Add more examples: SPI devices, knight-rider effects, input devices, MIDI...
+         * Perhaps add support for D2XX driver, though the name then becomes a
+           slight liability ;)
+         * General code quality improvements: solid unit tests, decent documentation.
         
         License
         -------
         
-        Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+        Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
         
         pylibftdi is released under the MIT licence; see the file "LICENSE.txt"
         for information.
         
         All trademarks referenced herein are property of their respective
         holders.
         libFTDI itself is developed by Intra2net AG.  No association with
```

### Comparing `pylibftdi-0.8.1/README.txt` & `pylibftdi-0.9/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     >>> from pylibftdi import BitBangDevice
     >>>
     >>> with BitBangDevice('FTE00P4L') as bb:
     ...     bb.direction = 0x0F  # four LSB are output(1), four MSB are input(0)
     ...     bb.port |= 2         # set bit 1
     ...     bb.port &= 0xFE      # clear bit 0
 
-There is support for a number of external devices and protocols, specifically
-for interfacing with HD44780 LCDs using the 4-bit interface.
+There is support for a number of external devices and protocols, including
+interfacing with HD44780 LCDs using the 4-bit interface.
 
 History & Motivation
 --------------------
 This package is the result of various bits of work using FTDI's
 devices, primarily for controlling external devices.  Some of this
 is documented on the codedstructure blog, codedstructure.blogspot.com
 
 At least two other open-source Python FTDI wrappers exist, and each
 of these may be best for some projects.
 
  * ftd2xx_ - ctypes binding to FTDI's own D2XX driver
  * pyftdi_ - a C extension libftdi binding
- 
+
 .. _ftd2xx: http://pypi.python.org/pypi/ftd2xx
 .. _pyftdi: http://git.marcansoft.com/?p=pyftdi.git
 
 pylibftdi exists in the gap between these two projects; ftd2xx uses
 the (closed-source) D2XX driver, but provides a high-level Python
 interface, while pyftdi works with libftdi but is very low-level.
 The aim for pylibftdi is to work with the libftdi, but to provide
@@ -95,15 +95,15 @@
  * Perhaps add support for D2XX driver, though the name then becomes a
    slight liability ;)
  * General code quality improvements: solid unit tests, decent documentation.
 
 License
 -------
 
-Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
 
 pylibftdi is released under the MIT licence; see the file "LICENSE.txt"
 for information.
 
 All trademarks referenced herein are property of their respective
 holders.
 libFTDI itself is developed by Intra2net AG.  No association with
```

### Comparing `pylibftdi-0.8.1/setup.py` & `pylibftdi-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 
 from distutils.core import setup
 
 setup(
     name="pylibftdi",
-    version="0.8.1",
+    version="0.9",
     description="Pythonic interface to FTDI devices using libftdi",
     long_description=open('README.txt').read(),
     author="Ben Bass",
     author_email="benbass@codedstructure.net",
     url="http://bitbucket.org/codedstructure/pylibftdi",
     packages=["pylibftdi"],
     classifiers=[
```

### Comparing `pylibftdi-0.8.1/pylibftdi/__init__.py` & `pylibftdi-0.9/pylibftdi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 pylibftdi - python wrapper for libftdi
 
-Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
 See LICENSE file for details and (absence of) warranty
 
 pylibftdi: http://bitbucket.org/codedstructure/pylibftdi
 
 
 libftdi can be found at:
  http://www.intra2net.com/en/developer/libftdi/
 Neither libftdi or Intra2net are associated with this project;
 if something goes wrong here, it's almost definitely my fault
 rather than a problem with the libftdi library.
 """
 
-__VERSION__ = "0.8.1"
+__VERSION__ = "0.9"
 __AUTHOR__ = "Ben Bass"
 
 
 __ALL__ = ['Driver', 'Device', 'BitBangDevice', 'Bus', 'FtdiError',
-           'ALL_OUTPUTS', 'ALL_INPUTS', 'BB_OUTPUT', 'BB_INPUT']
+           'ALL_OUTPUTS', 'ALL_INPUTS', 'BB_OUTPUT', 'BB_INPUT',
+           'examples', 'tests']
 
 from pylibftdi import _base, driver, util, bitbang
 
 # Bring them in to package scope so we can treat pylibftdi
 # as a module if we want.
 FtdiError = _base.FtdiError
 Bus = util.Bus
@@ -37,13 +38,14 @@
 BB_INPUT = bitbang.BB_INPUT
 FLUSH_BOTH = driver.FLUSH_BOTH
 FLUSH_INPUT = driver.FLUSH_INPUT
 FLUSH_OUTPUT = driver.FLUSH_OUTPUT
 
 # LEGACY SUPPORT
 
+
 class BitBangDriver(bitbang.BitBangDevice):
     def __init__(self, direction=ALL_OUTPUTS):
         import warnings
         warnings.warn('change BitBangDriver reference to BitBangDevice',
                       DeprecationWarning)
         return BitBangDevice.__init__(self, direction=direction, lazy_open=True)
```

### Comparing `pylibftdi-0.8.1/pylibftdi/_base.py` & `pylibftdi-0.9/pylibftdi/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """
 pylibftdi - python wrapper for libftdi
 
-Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
 See LICENSE file for details and (absence of) warranty
 
 pylibftdi: http://bitbucket.org/codedstructure/pylibftdi
 
 """
 
 # This module contains things needed by at least one other
 # module so as to prevent circular imports.
 
 __ALL__ = ['Refuser', 'ParrotEgg', 'DeadParrot', 'FtdiError']
 
+
 class Refuser(object):
+
     def __getattribute__(self, key):
         # perhaps we should produce an appropriate quote at random...
         raise TypeError(object.__getattribute__(self, 'message'))
+
     def __setattr__(self, key, val):
         raise TypeError(object.__getattribute__(self, 'message'))
+
     def __call__(self, *o, **kw):
         raise TypeError(object.__getattribute__(self, 'message'))
 
+
 class ParrotEgg(Refuser):
     message = "This object is not yet... (missing open()?)"
 
+
 class DeadParrot(Refuser):
     message = "This object is no more!"
 
+
 class FtdiError(Exception):
     pass
-
```

### Comparing `pylibftdi-0.8.1/pylibftdi/bitbang.py` & `pylibftdi-0.9/pylibftdi/bitbang.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 """
 pylibftdi - python wrapper for libftdi
 
-Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
 See LICENSE file for details and (absence of) warranty
 
 pylibftdi: http://bitbucket.org/codedstructure/pylibftdi
 
 """
 
 from pylibftdi.driver import Device, FtdiError
+from ctypes import c_ubyte, byref
 
 ALL_OUTPUTS = 0xFF
 ALL_INPUTS = 0x00
 BB_OUTPUT = 1
 BB_INPUT = 0
 
+
 class BitBangDevice(Device):
     """
     simple subclass to support bit-bang mode
 
-    Only uses async mode at the moment.
+    Internally uses async mode at the moment, but provides a 'sync'
+    flag (defaulting to True) which controls the behaviour of port
+    reading and writing - if set, the FIFOs are ignored (read) or
+    cleared (write) so operations will appear synchronous
 
     Adds two read/write properties to the base class:
      direction: 8 bit input(0)/output(1) direction control.
      port: 8 bit IO port, as defined by direction.
     """
     def __init__(self,
-                 device_id = None,
-                 direction = ALL_OUTPUTS,
-                 lazy_open = False):
+                 device_id=None,
+                 direction=ALL_OUTPUTS,
+                 lazy_open=False,
+                 sync=True):
         # initialise the super-class, but don't open yet. We really want
         # two-part initialisation here - set up all the instance variables
         # here in the super class, then open it after having set more
         # of our own variables.
-        super(BitBangDevice, self).__init__(device_id = device_id,
-                                            mode = 'b',
-                                            lazy_open = True)
+        super(BitBangDevice, self).__init__(device_id=device_id,
+                                            mode='b',
+                                            lazy_open=True)
         self.direction = direction
+        self.sync = sync
         self._last_set_dir = None
         self._latch = 0
         if not lazy_open:
             self.open()
 
     def open(self):
         "open connection to a FTDI device"
         # in case someone sets the direction before we are open()ed,
         # we intercept this call...
         super(BitBangDevice, self).open()
         if self.direction != self._last_set_dir:
             self.direction = self._direction
         return self
 
-
     # direction property - 8 bit value determining whether an IO line
     # is output (if set to 1) or input (set to 0)
     @property
     def direction(self):
         """
         get or set the direction of each of the IO lines. LSB=D0, MSB=D7
         1 for output, 0 for input
@@ -67,31 +73,39 @@
         if not (0 <= dir <= 255):
             raise FtdiError("invalid direction bitmask")
         self._direction = dir
         if not self.closed:
             self.ftdi_fn.ftdi_set_bitmode(dir, 0x01)
             self._last_set_dir = dir
 
-
     # port property - 8 bit read/write value
     @property
     def port(self):
         """
         get or set the state of the IO lines.  The value of output
         lines is persisted in this object for the purposes of reading,
         so read-modify-write operations (e.g. drv.port+=1) are valid.
         """
-        # the coercion to bytearray here is to make this work
-        # transparently between Python2 and Python3 - equivalent
-        # of ord() for Python2, a time-wasting do-nothing on Python3
-        result = bytearray(super(BitBangDevice, self).read(1))[0]
+        if self.sync:
+            pin_byte = c_ubyte()
+            res = self.fdll.ftdi_read_pins(self.ctx, byref(pin_byte))
+            if res != 0:
+                raise FtdiError("Could not read device pins")
+            result = pin_byte.value
+        else:
+            # the coercion to bytearray here is to make this work
+            # transparently between Python2 and Python3 - equivalent
+            # of ord() for Python2, a time-wasting do-nothing on Python3
+            result = bytearray(super(BitBangDevice, self).read(1))[0]
+
         # replace the 'output' bits with current value of _latch -
         # the last written value. This makes read-modify-write
         # operations (e.g. 'drv.port |= 0x10') work as expected
         result = (result & ~self._direction) | (self._latch & self._direction)
         return result
 
     @port.setter
     def port(self, value):
         self._latch = value
+        if self.sync:
+            self.flush_output()
         return super(BitBangDevice, self).write(chr(value))
-
```

### Comparing `pylibftdi-0.8.1/pylibftdi/driver.py` & `pylibftdi-0.9/pylibftdi/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 pylibftdi - python wrapper for libftdi
 
-Copyright (c) 2010-2011 Ben Bass <benbass@codedstructure.net>
+Copyright (c) 2010-2012 Ben Bass <benbass@codedstructure.net>
 See LICENSE file for details and (absence of) warranty
 
 pylibftdi: http://bitbucket.org/codedstructure/pylibftdi
 
 """
 
 import os
@@ -15,32 +15,37 @@
 # be disciplined so pyflakes can check us...
 from ctypes import (CDLL, byref, c_int, c_char_p, c_void_p, cast,
                     create_string_buffer, Structure, pointer, POINTER)
 from ctypes.util import find_library
 
 from pylibftdi._base import FtdiError
 
+
 class UsbDevList(Structure):
     _fields_ = [('next', c_void_p),
                 ('usb_dev', c_void_p)]
 
 # Note I gave up on attempts to use ftdi_new/ftdi_free (just using
 # ctx instead of byref(ctx) in first param of most ftdi_* functions) as
 # (at least for 64-bit) they only worked if argtypes was declared
 # (c_void_p for ctx), and that's too much like hard work to maintain.
 # So I've reverted to using create_string_buffer for memory management,
-# byref(ctx) to pass in the context instance, and ftdi_init() / 
+# byref(ctx) to pass in the context instance, and ftdi_init() /
 # ftdi_deinit() pair to manage the driver resources. It's very nice
 # how layered the libftdi code is, with access to each layer.
 
 # These constants determine what type of flush operation to perform
 FLUSH_BOTH = 1
 FLUSH_INPUT = 2
 FLUSH_OUTPUT = 3
 
+USB_VID = 0x0403
+USB_PID = 0x6001
+
+
 class Driver(object):
     """
     This is where it all happens...
     We load the libftdi library, and use it.
     """
 
     _instance = None
@@ -71,32 +76,35 @@
 
     ## Legacy support - prior to version 0.7, Device and Driver
     ## were unified (and named 'Driver'). This provides basic
     ## backwards compatiblity support.
     LEGACY_ATTRIBUTES = ['open', 'close', 'ftdi_fn', 'baudrate',
                          'read', 'write', 'get_error_string',
                          '__enter__', '__exit__']
+
     @property
     def legacy_device(self):
         warnings.warn("using Device() methods on Driver(); see CHANGES.txt",
                 DeprecationWarning)
         if not hasattr(self, '_legacy_device'):
             self._legacy_device = Device(lazy_open=True)
         return self._legacy_device
 
     def __getattr__(self, key):
         if key in Driver.LEGACY_ATTRIBUTES:
             return getattr(self.legacy_device, key)
         else:
             return object.__getattr__(self, key)
+
     def __setattr__(self, key, value):
         if key in Driver.LEGACY_ATTRIBUTES:
             return setattr(self.legacy_device, key, value)
         else:
             self.__dict__[key] = value
+
     def __delattr__(self, key):
         if key in Driver.LEGACY_ATTRIBUTES:
             delattr(self.legacy_device, key)
         else:
             del self.__dict__[key]
 
     def list_devices(self):
@@ -125,26 +133,26 @@
         if self.fdll.ftdi_init(byref(ctx)) != 0:
             msg = self.fdll.ftdi_get_error_string(byref(ctx))
             raise FtdiError(msg)
 
         try:
             res = self.fdll.ftdi_usb_find_all(byref(ctx),
                                               byref(dev_list_ptr),
-                                              0x0403, 0x6001)
+                                              USB_VID, USB_PID)
             if res < 0:
                 raise FtdiError(self.fdll.ftdi_get_error_string(byref(ctx)))
             elif res > 0:
                 # take a copy of the dev_list for subsequent list_free
                 dev_list_base = pointer(dev_list_ptr.contents)
                 # traverse the linked list...
                 try:
                     while dev_list_ptr:
                         self.fdll.ftdi_usb_get_strings(byref(ctx),
                                 dev_list_ptr.contents.usb_dev,
-                                manuf,127, desc,127, serial,127)
+                                manuf, 127, desc, 127, serial, 127)
                         devices.append((manuf.value, desc.value, serial.value))
                         # step to next in linked-list if not
                         dev_list_ptr = cast(dev_list_ptr.contents.next,
                                             devlistptrtype)
                 finally:
                     self.fdll.ftdi_list_free(dev_list_base)
         finally:
@@ -221,15 +229,15 @@
             del self.ctx
             raise FtdiError(msg)
 
         # Try to open the device.  If this fails, reset things to how
         # they were, but we can't use self.close as that assumes things
         # have already been setup.
         # FTDI vendor/product ids required here.
-        open_args = [byref(self.ctx), 0x0403, 0x6001]
+        open_args = [byref(self.ctx), USB_VID, USB_PID]
         if self.device_id is None:
             res = self.fdll.ftdi_usb_open(*tuple(open_args))
         else:
             # attempt to match device_id to serial number
             open_args.extend([0, c_char_p(self.device_id.encode('latin1'))])
             res = self.fdll.ftdi_usb_open_desc(*tuple(open_args))
             if res != 0:
@@ -392,19 +400,18 @@
         >>>     ...
         """
         # note this class is constructed on each call, so this
         # won't be particularly quick.  It does ensure that the
         # fdll and ctx objects in the closure are up-to-date, though.
         class FtdiForwarder(object):
             def __getattr__(innerself, key):
-                 return functools.partial(getattr(self.fdll, key),
-                                          byref(self.ctx))
+                return functools.partial(getattr(self.fdll, key),
+                                         byref(self.ctx))
         return FtdiForwarder()
 
-
     def __enter__(self):
         """
         support for context manager.
         Note the driver is opened and closed automatically
         when used in a with statement, and the driver object
         itself is returned:
         >>> with Driver(mode='t') as drv:
@@ -478,8 +485,7 @@
         while True:
             line = self.readline()
             if line:
                 return line
             else:
                 raise StopIteration
     next = __next__
-
```

