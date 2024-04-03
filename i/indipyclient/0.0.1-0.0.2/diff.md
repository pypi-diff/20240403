# Comparing `tmp/indipyclient-0.0.1.tar.gz` & `tmp/indipyclient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.1.tar` & `indipyclient-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.1/LICENSE
--rw-r--r--   0        0        0     2356 2024-03-29 22:45:11.765875 indipyclient-0.0.1/README.md
--rw-r--r--   0        0        0      291 2024-03-25 17:18:17.000000 indipyclient-0.0.1/indipyclient/__init__.py
--rw-r--r--   0        0        0     3462 2024-03-29 22:07:10.000000 indipyclient-0.0.1/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.1/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19659 2024-03-27 22:13:05.000000 indipyclient-0.0.1/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48603 2024-03-27 22:17:36.000000 indipyclient-0.0.1/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   148175 2024-03-27 22:11:13.000000 indipyclient-0.0.1/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.1/indipyclient/error.py
--rw-r--r--   0        0        0    23317 2024-03-27 20:34:01.000000 indipyclient-0.0.1/indipyclient/events.py
--rw-r--r--   0        0        0    30121 2024-03-28 15:36:13.000000 indipyclient-0.0.1/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    13556 2024-02-19 14:19:29.000000 indipyclient-0.0.1/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    25088 2024-03-27 20:34:01.000000 indipyclient-0.0.1/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-03-29 22:07:10.000000 indipyclient-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 indipyclient-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2686 2024-04-03 21:19:09.000000 indipyclient-0.0.2/README.md
+-rw-r--r--   0        0        0      291 2024-03-31 16:30:35.000000 indipyclient-0.0.2/indipyclient/__init__.py
+-rw-r--r--   0        0        0     2998 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.2/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48568 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   142902 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.2/indipyclient/error.py
+-rw-r--r--   0        0        0    24609 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/events.py
+-rw-r--r--   0        0        0    34076 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    13587 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    25114 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-03-31 16:29:51.000000 indipyclient-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 indipyclient-0.0.2/PKG-INFO
```

### Comparing `indipyclient-0.0.1/LICENSE` & `indipyclient-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.1/README.md` & `indipyclient-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # indipyclient
-INDI terminal client to communicate to an indi service.
+Terminal client to communicate to an INDI service.
+
+NOTE: CURRENTLY STILL UNDER DEVELOPMENT
 
 This is a pure python package, with no dependencies, providing an INDI client terminal
 
 It also provides a set of classes which can be used to create an INDI client. Either a script, or a GUI implementation could use this to generate the INDI protocol XML, and to create the connection to a port serving INDI drivers.
 
-The client can be called with python3 -m indipyclent.
+The client can be run with
+
+indipyclient [options]
+
+or with
+
+python3 -m indipyclient [options]
+
+The package help is:
 
-    usage: python3 -m indipyclient [options]
+    usage: indipyclient [options]
 
-    INDI terminal client communicating to indi service.
+    Terminal client to communicate to an INDI service.
 
     options:
       -h, --help            show this help message and exit
-      -p PORT, --port PORT  Port of the indi server (default 7624).
-      --host HOST           Hostname/IP of the indi server (default localhost).
+      -p PORT, --port PORT  Port of the INDI server (default 7624).
+      --host HOST           Hostname/IP of the INDI server (default localhost).
       -b BLOBS, --blobs BLOBS
                             Optional folder where BLOB's will be saved.
-      --loglevel LOGLEVEL   Enables logging, value 1, 2 or 3.
+      --loglevel LOGLEVEL   Enables logging, value 1, 2, 3 or 4.
       --logfile LOGFILE     File where logs will be saved
       --version             show program's version number and exit
 
-    The BLOB's folder can also be set from within the session.
-    Setting loglevel and logfile should only be used for brief
-    diagnostic purposes, the logfile could grow very big.
-    loglevel:1 log vector tags without members or contents,
-    loglevel:2 log vectors and members - but not BLOB contents,
-    loglevel:3 log vectors and all contents
+    The BLOB's folder can also be set from within the session. Setting loglevel
+    and logfile should only be used for brief diagnostic purposes, the logfile
+    could grow very big.
+    loglevel:1 Information and error messages only,
+    loglevel:2 log vector tags without members or contents,
+    loglevel:3 log vectors and members - but not BLOB contents,
+    loglevel:4 log vectors and all contents
 
 A typical sesssion would look like:
 
 ![Terminal screenshot](https://github.com/bernie-skipole/indipyclient/raw/main/image.png)
 
 
 This is a companion package to 'indipydriver' which can be used to create INDI drivers.
@@ -44,7 +55,15 @@
 The protocol defines the format of the data sent, such as light, number, text, switch or BLOB (Binary Large Object) and the client can send commands to control the instrument.  The client can be general purpose, taking the format of switches, numbers etc., from the protocol.
 
 INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 Further documentation is available at:
 
 https://indipyclient.readthedocs.io
+
+If you are only using the terminal client, I recommend pipx, so to install you would use:
+
+pipx install indipyclient
+
+or if you want to run it, without installing:
+
+pipx run indipyclient
```

### Comparing `indipyclient-0.0.1/indipyclient/__main__.py` & `indipyclient-0.0.2/indipyclient/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,51 +4,45 @@
 python3 -m indipyclient
 
 """
 
 
 import os, sys, argparse, asyncio, collections, contextlib, pathlib
 
-
 from . import version
 
 from .console.consoleclient import ConsoleClient, ConsoleControl
 
-from .console.widgets import ERRORDATA
-
 
 async def runclient(client, control):
-    try:
-        t1 = asyncio.create_task(client.asyncrun())
-        t2 = asyncio.create_task(control.asyncrun())
-        await asyncio.gather(t1, t2)
-    except Exception:
-         t1.cancel()
-         t2.cancel()
+    t1 = asyncio.create_task(client.asyncrun())
+    t2 = asyncio.create_task(control.asyncrun())
+    await asyncio.gather(t1, t2)
     # wait for tasks to be done
     while (not t1.done()) and (not t2.done()):
         await asyncio.sleep(0)
 
 
 def main():
     """The main routine."""
 
-    parser = argparse.ArgumentParser(usage="python3 -m indipyclient [options]",
-                                     description="INDI terminal client communicating to indi service.",
+    parser = argparse.ArgumentParser(usage="indipyclient [options]",
+                                     description="Terminal client to communicate to an INDI service.",
                                      epilog="""The BLOB's folder can also be set from within the session.
 Setting loglevel and logfile should only be used for brief
 diagnostic purposes, the logfile could grow very big.
-loglevel:1 log vector tags without members or contents,
-loglevel:2 log vectors and members - but not BLOB contents,
-loglevel:3 log vectors and all contents
+loglevel:1 Information and error messages only,
+loglevel:2 log vector tags without members or contents,
+loglevel:3 log vectors and members - but not BLOB contents,
+loglevel:4 log vectors and all contents
 """)
-    parser.add_argument("-p", "--port", type=int, default=7624, help="Port of the indi server (default 7624).")
-    parser.add_argument("--host", default="localhost", help="Hostname/IP of the indi server (default localhost).")
+    parser.add_argument("-p", "--port", type=int, default=7624, help="Port of the INDI server (default 7624).")
+    parser.add_argument("--host", default="localhost", help="Hostname/IP of the INDI server (default localhost).")
     parser.add_argument("-b", "--blobs", help="Optional folder where BLOB's will be saved.")
-    parser.add_argument("--loglevel", help="Enables logging, value 1, 2 or 3.")
+    parser.add_argument("--loglevel", help="Enables logging, value 1, 2, 3 or 4.")
     parser.add_argument("--logfile", help="File where logs will be saved")
 
     parser.add_argument("--version", action="version", version=version)
     args = parser.parse_args()
 
     eventque = collections.deque(maxlen=4)
 
@@ -67,35 +61,25 @@
 
     # On receiving an event, the client appends it into eventque
     client = ConsoleClient(indihost=args.host, indiport=args.port, eventque=eventque)
 
     if args.loglevel and args.logfile:
         try:
             loglevel = int(args.loglevel)
-            if loglevel not in (1,2,3):
-                print("Error: If given, the loglevel should be 1, 2 or 3")
+            if loglevel not in (1,2,3,4):
+                print("Error: If given, the loglevel should be 1, 2, 3 or 4")
                 return 1
         except:
-            print("Error: If given, the loglevel should be 1, 2 or 3")
+            print("Error: If given, the loglevel should be 1, 2, 3 or 4")
             return 1
         client.setlogging(loglevel, args.logfile)
 
     # Monitors eventque and acts on the events, creates the console screens
     control = ConsoleControl(client, blobfolder=blobfolder)
 
     asyncio.run(runclient(client, control))
 
-    # ERRORDATA is a list of any traceback.TracebackException() objects
-    # which records exceptions which may have occurred. They are printed
-    # here, after the console has closed down to avoid messing up
-    # the console formatting
-
-    if ERRORDATA:
-        for errortrace in ERRORDATA:
-            print("".join(errortrace.format()))
-            print("------------------")
-
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `indipyclient-0.0.1/indipyclient/console/consoleclient.py` & `indipyclient-0.0.2/indipyclient/console/consoleclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
-import asyncio, sys
+import asyncio, sys, traceback
 
 import curses
 
-from traceback import TracebackException as TBE
-
 from ..ipyclient import IPyClient
 from ..events import (delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector,
                      setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector, Message, VectorTimeOut)
 
 from . import windows
 from . import widgets
 
@@ -107,16 +105,21 @@
         return curses.color_pair(0)
 
     @property
     def connected(self):
         return self.client.connected
 
 
-    def shutdown(self):
+    def shutdown(self, exc=None):
+        """If exc is an exception, and logs are enabled, logs it.
+           Sets self._shutdown to True which shuts down the client"""
         self._shutdown = True
+        if self.client.level and not(exc is None):
+            bytex = "".join(traceback.format_exception(exc)).encode()
+            self.client.logfp.write(b"\n"+bytex)
 
 
     async def _checkshutdown(self):
         "If self._shutdown becomes True, shutdown"
         while not self._shutdown:
             await asyncio.sleep(0)
         await self.client.report("Shutting down client - please wait")
@@ -232,19 +235,18 @@
                     self.screen.update(event)
                     continue
                 if isinstance(self.screen, windows.VectorScreen) and (self.screen.vectorname == event.vectorname):
                     # The event refers to this vector
                     self.screen.update(event)
 
         except asyncio.CancelledError:
-            self._shutdown = True
+            self.shutdown()
             raise
         except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            self._shutdown = True
+            self.shutdown(e)
         finally:
             self.updatescreenstopped = True
 
 
     async def getinput(self):
         try:
             while not self.stop:
@@ -261,15 +263,15 @@
                             self.screen.show()
                             continue
                         # so resize has increased to proper size
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
 
                 if isinstance(self.screen, windows.MessagesScreen):
                     result = await self.screen.inputs()
                     if result == "Resize":
                         self.maxrows, self.maxcols = self.stdscr.getmaxyx()
                         if self.maxrows < 16 or self.maxcols < 40:
@@ -279,15 +281,15 @@
                             self.screen = windows.TooSmall(self.stdscr, self)
                             self.screen.show()
                             continue
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
                     if result == "Devices":
                         self.screen = windows.DevicesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "EnableBLOBs":
                         self.screen = windows.EnableBLOBsScreen(self.stdscr, self)
@@ -304,15 +306,15 @@
                             self.screen = windows.TooSmall(self.stdscr, self)
                             self.screen.show()
                             continue
                         self.screen = windows.EnableBLOBsScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
                     if result == "Messages":
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Devices":
                         self.screen = windows.DevicesScreen(self.stdscr, self)
@@ -329,15 +331,15 @@
                             self.screen = windows.TooSmall(self.stdscr, self)
                             self.screen.show()
                             continue
                         self.screen = windows.DevicesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
                     if result == "Messages":
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     devices = {devicename.lower():device for devicename, device in self.client.items() if device.enable}
                     if result in devices:
@@ -356,15 +358,15 @@
                             self.screen = windows.TooSmall(self.stdscr, self)
                             self.screen.show()
                             continue
                         self.screen = windows.ChooseVectorScreen(self.stdscr, self, self.screen.devicename, group=self.screen.groupwin.active)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
                     if result == "Messages":
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Devices":
                         self.screen = windows.DevicesScreen(self.stdscr, self)
@@ -386,15 +388,15 @@
                             self.screen = windows.TooSmall(self.stdscr, self)
                             self.screen.show()
                             continue
                         self.screen = windows.VectorScreen(self.stdscr, self, self.screen.devicename, self.screen.vectorname)
                         self.screen.show()
                         continue
                     if result == "Quit":
-                        self._shutdown = True
+                        self.shutdown()
                         break
                     if result == "Messages":
                         self.screen = windows.MessagesScreen(self.stdscr, self)
                         self.screen.show()
                         continue
                     if result == "Devices":
                         self.screen = windows.DevicesScreen(self.stdscr, self)
@@ -402,19 +404,18 @@
                         continue
                     if result == "Vectors":
                         self.screen = windows.ChooseVectorScreen(self.stdscr, self, self.screen.devicename, group=self.screen.vector.group)
                         self.screen.show()
                         continue
 
         except asyncio.CancelledError:
-            self._shutdown = True
+            self.shutdown()
             raise
         except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            self._shutdown = True
+            self.shutdown(e)
         finally:
             self.getinputstopped = True
 
 
     def send_enableBLOB(self):
         "Sends Also to enable blobs for all devices"
         if not self.blobenabled:
```

### Comparing `indipyclient-0.0.1/indipyclient/console/widgets.py` & `indipyclient-0.0.2/indipyclient/console/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 
 import asyncio, curses, sys, pathlib, time
 
 from decimal import Decimal
 
-from traceback import TracebackException as TBE
-
 from curses import ascii
 
-ERRORDATA = []
-
 def shorten(text, width=0, placeholder="..."):
     "Shorten text"
+    txt = text.replace("\n", " ")
     if not width:
-        return text
-    if len(text)<=width:
-        return text
+        return txt
+    if len(txt)<=width:
+        return txt
     if width <= len(placeholder):
         return placeholder[:width]
-    return text[:width - len(placeholder)] + placeholder
+    return txt[:width - len(placeholder)] + placeholder
 
 
 def drawmessage(window, message, bold=False, maxcols=None):
     """Shows message, message is either a text string, or a tuple of (timestamp, message text)"""
     window.clear()
     if not maxcols:
         maxrows, maxcols = window.getmaxyx()
```

### Comparing `indipyclient-0.0.1/indipyclient/console/windows.py` & `indipyclient-0.0.2/indipyclient/console/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 import asyncio, curses, sys, os, pathlib, time
 
-from traceback import TracebackException as TBE
-
 from . import widgets
 
 from .. import events
 
 
 
 class ParentScreen:
@@ -58,15 +56,14 @@
                     # return a tuple of the mouse coordinates
                     #          row     col
                     return (mouse[2], mouse[1])
                 continue
             return key
 
 
-
 class ConsoleClientScreen(ParentScreen):
 
     "Parent to windows which are set in self.control.screen"
 
     def __init__(self, stdscr, control):
         super().__init__(stdscr, control)
         self.stdscr.clear()
@@ -113,25 +110,20 @@
         self.stdscr.addstr(3, self.maxcols//2-2, "small")
         self.stdscr.addstr(4, self.maxcols//2-6, "Please resize")
         self.stdscr.noutrefresh()
         curses.doupdate()
 
     async def inputs(self):
         "Gets inputs from the screen"
-        try:
-            self.stdscr.nodelay(True)
-            while True:
-                key = await self.keyinput()
-                if key in ("Resize", "Stop"):
-                    return key
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
+        self.stdscr.nodelay(True)
+        while True:
+            key = await self.keyinput()
+            if key in ("Resize", "Stop"):
+                return key
+
 
 
 class MessagesScreen(ConsoleClientScreen):
 
     def __init__(self, stdscr, control):
         super().__init__(stdscr, control)
 
@@ -290,143 +282,137 @@
         self.disable_btn.draw()
         self.infowin.noutrefresh()
         curses.doupdate()
 
 
     async def inputs(self):
         "Gets inputs from the screen"
-        try:
-            self.stdscr.nodelay(True)
-            while True:
-                key = await self.keyinput()
-
-                if key == "Resize":
-                    return key
-
-                if not self.connected:
-                    # only accept quit
-                    if not self.quit_btn.focus:
-                        # defocus everything
-                        self.defocus()
-                        # and set quit into focus
-                        self.quit_btn.focus = True
-                        self.quit_btn.draw()
-                        self.buttwin.noutrefresh()
-                        self.infowin.noutrefresh()
-                        curses.doupdate()
-                    elif key == 10:
-                        return "Quit"
-                    elif isinstance(key, tuple) and (key in self.quit_btn):
-                        return "Quit"
-                    continue
-
-                if key in ("Devices", "Vectors", "Stop"):
-                    return key
 
-                if isinstance(key, tuple):
-                    for fld in self.fields:
-                        if key in fld:
-                            if fld.focus:
-                                # focus already set - return the button onclick
-                                value = fld.onclick
-                                if value == "DisableBLOBs":
-                                    await self.disableBLOBs()
-                                    break
-                                else:
-                                    return value
-                            # focus not set, defocus the one currently
-                            # in focus
-                            self.defocus()
-                            # and set this into focus
-                            fld.focus = True
-                            fld.draw()
-                            self.buttwin.noutrefresh()
-                            self.infowin.noutrefresh()
-                            curses.doupdate()
-                            break
-                    continue
+        self.stdscr.nodelay(True)
+        while True:
+            key = await self.keyinput()
 
-                # 32 space, 9 tab, 353 shift tab, 261 right arrow, 260 left arrow, 10 return, 339 page up, 338 page down, 259 up arrow, 258 down arrow
+            if key == "Resize":
+                return key
 
-                if key in (32, 9, 261, 338, 258):
-                    # go to next button
-                    if self.devices_btn.focus:
-                        self.devices_btn.focus = False
-                        self.quit_btn.focus = True
-                        self.devices_btn.draw()
-                        self.quit_btn.draw()
-                        self.buttwin.noutrefresh()
-                    elif self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        self.quit_btn.draw()
-                        self.buttwin.noutrefresh()
-                        self.enable_btn.focus = True
-                        self.enable_btn.draw()
-                        self.infowin.noutrefresh()
-                    elif self.enable_btn.focus:
-                        self.enable_btn.focus = False
-                        self.disable_btn.focus = True
-                        self.enable_btn.draw()
-                        self.disable_btn.draw()
-                        self.infowin.noutrefresh()
-                    elif self.disable_btn.focus:
-                        self.disable_btn.focus = False
-                        self.disable_btn.draw()
-                        self.infowin.noutrefresh()
-                        self.devices_btn.focus = True
-                        self.devices_btn.draw()
-                        self.buttwin.noutrefresh()
+            if not self.connected:
+                # only accept quit
+                if not self.quit_btn.focus:
+                    # defocus everything
+                    self.defocus()
+                    # and set quit into focus
+                    self.quit_btn.focus = True
+                    self.quit_btn.draw()
+                    self.buttwin.noutrefresh()
+                    self.infowin.noutrefresh()
                     curses.doupdate()
+                elif key == 10:
+                    return "Quit"
+                elif isinstance(key, tuple) and (key in self.quit_btn):
+                    return "Quit"
+                continue
 
-                elif key in (353, 260, 339, 259):
-                    # go to the previous button
-                    if self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        self.devices_btn.focus = True
-                        self.devices_btn.draw()
-                        self.quit_btn.draw()
-                        self.buttwin.noutrefresh()
-                    elif self.devices_btn.focus:
-                        self.devices_btn.focus = False
-                        self.devices_btn.draw()
-                        self.buttwin.noutrefresh()
-                        self.disable_btn.focus = True
-                        self.disable_btn.draw()
-                        self.infowin.noutrefresh()
-                    elif self.disable_btn.focus:
-                        self.disable_btn.focus = False
-                        self.disable_btn.draw()
-                        self.enable_btn.focus = True
-                        self.enable_btn.draw()
-                        self.infowin.noutrefresh()
-                    elif self.enable_btn.focus:
-                        self.enable_btn.focus = False
-                        self.enable_btn.draw()
-                        self.infowin.noutrefresh()
-                        self.quit_btn.focus = True
-                        self.quit_btn.draw()
-                        self.buttwin.noutrefresh()
-                    curses.doupdate()
+            if key in ("Devices", "Vectors", "Stop"):
+                return key
 
-                elif key == 10:
-                    # Enter has been pressed, check which field has focus
-                    for fld in self.fields:
+            if isinstance(key, tuple):
+                for fld in self.fields:
+                    if key in fld:
                         if fld.focus:
+                            # focus already set - return the button onclick
                             value = fld.onclick
                             if value == "DisableBLOBs":
                                 await self.disableBLOBs()
                                 break
                             else:
                                 return value
+                        # focus not set, defocus the one currently
+                        # in focus
+                        self.defocus()
+                        # and set this into focus
+                        fld.focus = True
+                        fld.draw()
+                        self.buttwin.noutrefresh()
+                        self.infowin.noutrefresh()
+                        curses.doupdate()
+                        break
+                continue
+
+            # 32 space, 9 tab, 353 shift tab, 261 right arrow, 260 left arrow, 10 return, 339 page up, 338 page down, 259 up arrow, 258 down arrow
+
+            if key in (32, 9, 261, 338, 258):
+                # go to next button
+                if self.devices_btn.focus:
+                    self.devices_btn.focus = False
+                    self.quit_btn.focus = True
+                    self.devices_btn.draw()
+                    self.quit_btn.draw()
+                    self.buttwin.noutrefresh()
+                elif self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    self.quit_btn.draw()
+                    self.buttwin.noutrefresh()
+                    self.enable_btn.focus = True
+                    self.enable_btn.draw()
+                    self.infowin.noutrefresh()
+                elif self.enable_btn.focus:
+                    self.enable_btn.focus = False
+                    self.disable_btn.focus = True
+                    self.enable_btn.draw()
+                    self.disable_btn.draw()
+                    self.infowin.noutrefresh()
+                elif self.disable_btn.focus:
+                    self.disable_btn.focus = False
+                    self.disable_btn.draw()
+                    self.infowin.noutrefresh()
+                    self.devices_btn.focus = True
+                    self.devices_btn.draw()
+                    self.buttwin.noutrefresh()
+                curses.doupdate()
+
+            elif key in (353, 260, 339, 259):
+                # go to the previous button
+                if self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    self.devices_btn.focus = True
+                    self.devices_btn.draw()
+                    self.quit_btn.draw()
+                    self.buttwin.noutrefresh()
+                elif self.devices_btn.focus:
+                    self.devices_btn.focus = False
+                    self.devices_btn.draw()
+                    self.buttwin.noutrefresh()
+                    self.disable_btn.focus = True
+                    self.disable_btn.draw()
+                    self.infowin.noutrefresh()
+                elif self.disable_btn.focus:
+                    self.disable_btn.focus = False
+                    self.disable_btn.draw()
+                    self.enable_btn.focus = True
+                    self.enable_btn.draw()
+                    self.infowin.noutrefresh()
+                elif self.enable_btn.focus:
+                    self.enable_btn.focus = False
+                    self.enable_btn.draw()
+                    self.infowin.noutrefresh()
+                    self.quit_btn.focus = True
+                    self.quit_btn.draw()
+                    self.buttwin.noutrefresh()
+                curses.doupdate()
 
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
+            elif key == 10:
+                # Enter has been pressed, check which field has focus
+                for fld in self.fields:
+                    if fld.focus:
+                        value = fld.onclick
+                        if value == "DisableBLOBs":
+                            await self.disableBLOBs()
+                            break
+                        else:
+                            return value
 
 
 class EnableBLOBsScreen(ConsoleClientScreen):
 
     def __init__(self, stdscr, control):
         super().__init__(stdscr, control)
 
@@ -539,124 +525,118 @@
         self.submit_btn.focus = False
         self.messages_btn.focus = True
 
 
     async def inputs(self):
         "Gets inputs from the screen"
 
-        try:
-            self.stdscr.nodelay(True)
-            while True:
-                if self.path_txt.focus:
-                    # text input here
-                    key = await self.textinput()
-                else:
-                    key = await self.keyinput()
-
-                if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
-                    return key
+        self.stdscr.nodelay(True)
+        while True:
+            if self.path_txt.focus:
+                # text input here
+                key = await self.textinput()
+            else:
+                key = await self.keyinput()
 
-                if isinstance(key, tuple):
-                    for fld in self.fields:
-                        if key in fld:
-                            if fld.focus:
-                                # focus already set - return the button onclick
-                                value = fld.onclick
-                                if value == "Submit":
-                                    await self.submit()
-                                    self.submit_btn.draw()
-                                    self.messages_btn.draw()
-                                    self.buttwin.noutrefresh()
-                                    self.pathwin.noutrefresh()
-                                    curses.doupdate()
-                                    break
-                                else:
-                                    return value
-                            # focus not set, defocus the one currently
-                            # in focus
-                            self.defocus()
-                            # and set this into focus
-                            fld.focus = True
-                            fld.draw()
-                            self.pathwin.noutrefresh()
-                            self.buttwin.noutrefresh()
-                            curses.doupdate()
-                            break
-                    continue
+            if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
+                return key
 
-                if key == 10:
-                    if self.quit_btn.focus:
-                        widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
-                        self.messwin.noutrefresh()
+            if isinstance(key, tuple):
+                for fld in self.fields:
+                    if key in fld:
+                        if fld.focus:
+                            # focus already set - return the button onclick
+                            value = fld.onclick
+                            if value == "Submit":
+                                await self.submit()
+                                self.submit_btn.draw()
+                                self.messages_btn.draw()
+                                self.buttwin.noutrefresh()
+                                self.pathwin.noutrefresh()
+                                curses.doupdate()
+                                break
+                            else:
+                                return value
+                        # focus not set, defocus the one currently
+                        # in focus
+                        self.defocus()
+                        # and set this into focus
+                        fld.focus = True
+                        fld.draw()
+                        self.pathwin.noutrefresh()
+                        self.buttwin.noutrefresh()
                         curses.doupdate()
-                        return "Quit"
-                    elif self.messages_btn.focus:
-                        return "Messages"
-                    elif self.devices_btn.focus:
-                        return "Messages"
-                    elif self.submit_btn.focus:
-                        await self.submit()
+                        break
+                continue
 
-                elif key in (32, 9, 261, 338, 258):
-                    # go to the next button
-                    if self.path_txt.focus:
-                        self.path_txt.focus = False
-                        self.submit_btn.focus = True
-                        self.path_txt.draw()
-                    elif self.submit_btn.focus:
-                        self.submit_btn.focus = False
-                        self.devices_btn.focus = True
-                    elif self.devices_btn.focus:
-                        self.devices_btn.focus = False
-                        self.messages_btn.focus = True
-                    elif self.messages_btn.focus:
-                        self.messages_btn.focus = False
-                        self.quit_btn.focus = True
-                    elif self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        self.path_txt.focus = True
-                        self.path_txt.draw()
+            if key == 10:
+                if self.quit_btn.focus:
+                    widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
+                    self.messwin.noutrefresh()
+                    curses.doupdate()
+                    return "Quit"
+                elif self.messages_btn.focus:
+                    return "Messages"
+                elif self.devices_btn.focus:
+                    return "Messages"
+                elif self.submit_btn.focus:
+                    await self.submit()
 
-                elif key in (353, 260, 339, 259):
-                    # go to previous button
-                    if self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        self.messages_btn.focus = True
-                    elif self.messages_btn.focus:
-                        self.messages_btn.focus = False
-                        self.devices_btn.focus = True
-                    elif self.devices_btn.focus:
-                        self.devices_btn.focus = False
-                        self.submit_btn.focus = True
-                    elif self.submit_btn.focus:
-                        self.submit_btn.focus = False
-                        self.path_txt.focus = True
-                        self.path_txt.draw()
-                    elif self.path_txt.focus:
-                        self.path_txt.focus = False
-                        self.quit_btn.focus = True
-                        self.path_txt.draw()
-                else:
-                    # button not recognised
-                    continue
+            elif key in (32, 9, 261, 338, 258):
+                # go to the next button
+                if self.path_txt.focus:
+                    self.path_txt.focus = False
+                    self.submit_btn.focus = True
+                    self.path_txt.draw()
+                elif self.submit_btn.focus:
+                    self.submit_btn.focus = False
+                    self.devices_btn.focus = True
+                elif self.devices_btn.focus:
+                    self.devices_btn.focus = False
+                    self.messages_btn.focus = True
+                elif self.messages_btn.focus:
+                    self.messages_btn.focus = False
+                    self.quit_btn.focus = True
+                elif self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    self.path_txt.focus = True
+                    self.path_txt.draw()
 
-                # draw buttons
-                self.submit_btn.draw()
-                self.messages_btn.draw()
-                self.devices_btn.draw()
-                self.quit_btn.draw()
-                self.buttwin.noutrefresh()
-                self.pathwin.noutrefresh()
-                curses.doupdate()
+            elif key in (353, 260, 339, 259):
+                # go to previous button
+                if self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    self.messages_btn.focus = True
+                elif self.messages_btn.focus:
+                    self.messages_btn.focus = False
+                    self.devices_btn.focus = True
+                elif self.devices_btn.focus:
+                    self.devices_btn.focus = False
+                    self.submit_btn.focus = True
+                elif self.submit_btn.focus:
+                    self.submit_btn.focus = False
+                    self.path_txt.focus = True
+                    self.path_txt.draw()
+                elif self.path_txt.focus:
+                    self.path_txt.focus = False
+                    self.quit_btn.focus = True
+                    self.path_txt.draw()
+            else:
+                # button not recognised
+                continue
+
+            # draw buttons
+            self.submit_btn.draw()
+            self.messages_btn.draw()
+            self.devices_btn.draw()
+            self.quit_btn.draw()
+            self.buttwin.noutrefresh()
+            self.pathwin.noutrefresh()
+            curses.doupdate()
 
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
 
 
     async def textinput(self):
         "Input text, set it into self._newvalue"
         # set cursor visible
         curses.curs_set(1)
         editstring = self.path_txt.editstring(self.stdscr)
@@ -980,249 +960,241 @@
         self.devwinrefresh()
 
 
 # 32 space, 9 tab, 353 shift tab, 261 right arrow, 260 left arrow, 10 return, 339 page up, 338 page down, 259 up arrow, 258 down arrow
 
     async def inputs(self):
         "Gets inputs from the screen"
-        try:
-            self.stdscr.nodelay(True)
 
+        self.stdscr.nodelay(True)
+        names = list(self.devices.keys())
+        lastidx = len(names)-1            # index of last device
 
-            names = list(self.devices.keys())
-            lastidx = len(names)-1            # index of last device
-
-            while True:
-                key = await self.keyinput()
-                if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
-                    return key
-                displayedbtns = list(self.devbuttons.values())
-                displayednames = list(self.devbuttons.keys())
-                bottomidx = self.botindex()       # index of last displayed device
-
-                if isinstance(key, tuple):
-                    # mouse pressed, find if its clicked in any field
-                    if key in self.quit_btn:
-                        if self.quit_btn.focus:
-                            widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
-                            self.messwin.noutrefresh()
-                            curses.doupdate()
-                            return "Quit"
-                        elif self.messages_btn.focus:
-                            self.messages_btn.focus = False
-                            self.quit_btn.focus = True
-                            self.messages_btn.draw()
-                            self.quit_btn.draw()
-                            self.buttwin.noutrefresh()
-                        else:
-                            # either a top or bottom more button or a device has focus
-                            self.defocus()
-                            self.devwinrefresh()
-                            self.quit_btn.focus = True
-                            self.quit_btn.draw()
-                            self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-                    if key in self.messages_btn:
-                        if self.messages_btn.focus:
-                            return "Messages"
-                        elif self.quit_btn.focus:
-                            self.quit_btn.focus = False
-                            self.messages_btn.focus = True
-                            self.messages_btn.draw()
-                            self.quit_btn.draw()
-                            self.buttwin.noutrefresh()
-                        else:
-                            # either a top or bottom more button or a device has focus
-                            self.defocus()
-                            self.devwinrefresh()
-                            self.messages_btn.focus = True
-                            self.messages_btn.draw()
-                            self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-                    if key in self.topmore_btn:
-                        if self.topmore_btn.focus:
-                            self.topmorechosen()
-                        else:
-                            self.defocus()
-                            self.topmore_btn.focus = True
-                            self.topmore_btn.draw()
-                            self.devwinrefresh()
-                            self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-                    if key in self.botmore_btn:
-                        if self.botmore_btn.focus:
-                            self.botmorechosen()
-                        else:
-                            self.defocus()
-                            self.botmore_btn.focus = True
-                            self.botmore_btn.draw()
-                            self.devwinrefresh()
-                            self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-
-                    # so now must check if mouse position is in any of the devices
-                    if key[0] > self.devwinbot:
-                        # no chance of device button being pressed as mouse point
-                        # is at a row greater than bottom line of the device window
-                        continue
-
-                    # displayedbtns button list, but only for buttons displayed
-
-                    for idx, btn in enumerate(displayedbtns):
-                        if key in btn:
-                            if btn.focus:
-                                return btn.onclick
-                            else:
-                                # button not in focus, so set it
-                                self.defocus()
-                                btn.focus = True
-                                btn.draw()
-                                self.focus = displayednames[idx]
-                                self.devwinrefresh()
-                                self.buttwin.noutrefresh()
-                                curses.doupdate()
-                                break
-                    continue
-
-                # so not a tuple/mouse press, its a key press
+        while True:
+            key = await self.keyinput()
+            if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
+                return key
+            displayedbtns = list(self.devbuttons.values())
+            displayednames = list(self.devbuttons.keys())
+            bottomidx = self.botindex()       # index of last displayed device
 
-                # which button has focus
-                if key == 10:
+            if isinstance(key, tuple):
+                # mouse pressed, find if its clicked in any field
+                if key in self.quit_btn:
                     if self.quit_btn.focus:
                         widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
                         self.messwin.noutrefresh()
                         curses.doupdate()
                         return "Quit"
+                    elif self.messages_btn.focus:
+                        self.messages_btn.focus = False
+                        self.quit_btn.focus = True
+                        self.messages_btn.draw()
+                        self.quit_btn.draw()
+                        self.buttwin.noutrefresh()
+                    else:
+                        # either a top or bottom more button or a device has focus
+                        self.defocus()
+                        self.devwinrefresh()
+                        self.quit_btn.focus = True
+                        self.quit_btn.draw()
+                        self.buttwin.noutrefresh()
+                    curses.doupdate()
+                    continue
+                if key in self.messages_btn:
                     if self.messages_btn.focus:
                         return "Messages"
+                    elif self.quit_btn.focus:
+                        self.quit_btn.focus = False
+                        self.messages_btn.focus = True
+                        self.messages_btn.draw()
+                        self.quit_btn.draw()
+                        self.buttwin.noutrefresh()
+                    else:
+                        # either a top or bottom more button or a device has focus
+                        self.defocus()
+                        self.devwinrefresh()
+                        self.messages_btn.focus = True
+                        self.messages_btn.draw()
+                        self.buttwin.noutrefresh()
+                    curses.doupdate()
+                    continue
+                if key in self.topmore_btn:
                     if self.topmore_btn.focus:
                         self.topmorechosen()
-                        curses.doupdate()
-                        continue
+                    else:
+                        self.defocus()
+                        self.topmore_btn.focus = True
+                        self.topmore_btn.draw()
+                        self.devwinrefresh()
+                        self.buttwin.noutrefresh()
+                    curses.doupdate()
+                    continue
+                if key in self.botmore_btn:
                     if self.botmore_btn.focus:
                         self.botmorechosen()
-                        curses.doupdate()
-                        continue
+                    else:
+                        self.defocus()
+                        self.botmore_btn.focus = True
+                        self.botmore_btn.draw()
+                        self.devwinrefresh()
+                        self.buttwin.noutrefresh()
+                    curses.doupdate()
+                    continue
 
-                    # If not Quit or Messages, return the lower case name
-                    # of the device in focus
-                    if self.focus:
-                        return self.focus.lower()
+                # so now must check if mouse position is in any of the devices
+                if key[0] > self.devwinbot:
+                    # no chance of device button being pressed as mouse point
+                    # is at a row greater than bottom line of the device window
                     continue
 
+                # displayedbtns button list, but only for buttons displayed
 
-                if key in (32, 9, 261, 338, 258):   # 32 space, 9 tab, 261 right arrow, 338 page down, 258 down arrow
-                    # go to the next button
-                    if self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        if self.topindex:
-                            # that is, if top button does not have index zero
-                            self.topmore_btn.focus = True
+                for idx, btn in enumerate(displayedbtns):
+                    if key in btn:
+                        if btn.focus:
+                            return btn.onclick
                         else:
-                            self.focus = displayednames[0]
-                    elif self.messages_btn.focus:
-                        self.messages_btn.focus = False
-                        self.quit_btn.focus = True
-                        self.drawbuttons()
-                        self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-                    elif self.topmore_btn.focus:
-                        self.topmore_btn.focus = False
+                            # button not in focus, so set it
+                            self.defocus()
+                            btn.focus = True
+                            btn.draw()
+                            self.focus = displayednames[idx]
+                            self.devwinrefresh()
+                            self.buttwin.noutrefresh()
+                            curses.doupdate()
+                            break
+                continue
+
+            # so not a tuple/mouse press, its a key press
+
+            # which button has focus
+            if key == 10:
+                if self.quit_btn.focus:
+                    widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
+                    self.messwin.noutrefresh()
+                    curses.doupdate()
+                    return "Quit"
+                if self.messages_btn.focus:
+                    return "Messages"
+                if self.topmore_btn.focus:
+                    self.topmorechosen()
+                    curses.doupdate()
+                    continue
+                if self.botmore_btn.focus:
+                    self.botmorechosen()
+                    curses.doupdate()
+                    continue
+
+                # If not Quit or Messages, return the lower case name
+                # of the device in focus
+                if self.focus:
+                    return self.focus.lower()
+                continue
+
+
+            if key in (32, 9, 261, 338, 258):   # 32 space, 9 tab, 261 right arrow, 338 page down, 258 down arrow
+                # go to the next button
+                if self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    if self.topindex:
+                        # that is, if top button does not have index zero
+                        self.topmore_btn.focus = True
+                    else:
                         self.focus = displayednames[0]
-                        self.drawdevices()
-                        self.devwinrefresh()
-                        curses.doupdate()
-                        continue
-                    elif self.botmore_btn.focus:
-                        self.botmore_btn.focus = False
+                elif self.messages_btn.focus:
+                    self.messages_btn.focus = False
+                    self.quit_btn.focus = True
+                    self.drawbuttons()
+                    self.buttwin.noutrefresh()
+                    curses.doupdate()
+                    continue
+                elif self.topmore_btn.focus:
+                    self.topmore_btn.focus = False
+                    self.focus = displayednames[0]
+                    self.drawdevices()
+                    self.devwinrefresh()
+                    curses.doupdate()
+                    continue
+                elif self.botmore_btn.focus:
+                    self.botmore_btn.focus = False
+                    self.messages_btn.focus = True
+                else:
+                    # one of the devices has focus
+                    try:
+                        indx = names.index(self.focus)
+                    except ValueError:
+                        continue
+                    # indx here is the index on the list of all devices, not just those displayed
+                    if indx == lastidx:
+                        # very last device, the botmore_btn should not be shown
+                        self.focus = None
                         self.messages_btn.focus = True
-                    else:
-                        # one of the devices has focus
-                        try:
-                            indx = names.index(self.focus)
-                        except ValueError:
-                            continue
-                        # indx here is the index on the list of all devices, not just those displayed
-                        if indx == lastidx:
-                            # very last device, the botmore_btn should not be shown
-                            self.focus = None
-                            self.messages_btn.focus = True
-                        elif indx == bottomidx:
-                            # last displayed device
-                            if key in (338, 258):      # 338 page down, 258 down arrow
-                                # display next device
-                                self.topindex += 1
-                                self.focus = names[indx+1]
-                            else:
-                                # last device on display
-                                self.focus = None
-                                self.botmore_btn.focus = True
-                        else:
+                    elif indx == bottomidx:
+                        # last displayed device
+                        if key in (338, 258):      # 338 page down, 258 down arrow
+                            # display next device
+                            self.topindex += 1
                             self.focus = names[indx+1]
-
-                elif key in (353, 260, 339, 259):  # 353 shift tab, 260 left arrow, 339 page up, 259 up arrow
-                    # go to previous button
-                    if self.quit_btn.focus:
-                        self.quit_btn.focus = False
-                        self.messages_btn.focus = True
-                        self.drawbuttons()
-                        self.buttwin.noutrefresh()
-                        curses.doupdate()
-                        continue
-                    elif self.messages_btn.focus:
-                        self.messages_btn.focus = False
-                        if self.botmore_btn.show:
-                            self.botmore_btn.focus = True
                         else:
-                            self.focus = displayednames[-1]
-                    elif self.botmore_btn.focus:
-                        self.botmore_btn.focus = False
-                        self.focus = displayednames[-1]
-                    elif self.topmore_btn.focus:
-                        self.topmore_btn.focus = False
-                        self.quit_btn.focus = True
-                    elif self.focus == names[0]:
-                        self.focus = None
-                        self.quit_btn.focus = True
+                            # last device on display
+                            self.focus = None
+                            self.botmore_btn.focus = True
                     else:
-                        try:
-                            indx = names.index(self.focus)
-                        except ValueError:
-                            continue
-                        if indx == self.topindex:
-                            if key in (339, 259): # 339 page up, 259 up arrow
-                                self.topindex -= 1
-                                self.focus = names[indx-1]
-                            else:
-                                self.focus = None
-                                self.topmore_btn.focus = True
-                        else:
-                            self.focus = names[indx-1]
+                        self.focus = names[indx+1]
 
-                else:
-                    # button not recognised
+            elif key in (353, 260, 339, 259):  # 353 shift tab, 260 left arrow, 339 page up, 259 up arrow
+                # go to previous button
+                if self.quit_btn.focus:
+                    self.quit_btn.focus = False
+                    self.messages_btn.focus = True
+                    self.drawbuttons()
+                    self.buttwin.noutrefresh()
+                    curses.doupdate()
                     continue
+                elif self.messages_btn.focus:
+                    self.messages_btn.focus = False
+                    if self.botmore_btn.show:
+                        self.botmore_btn.focus = True
+                    else:
+                        self.focus = displayednames[-1]
+                elif self.botmore_btn.focus:
+                    self.botmore_btn.focus = False
+                    self.focus = displayednames[-1]
+                elif self.topmore_btn.focus:
+                    self.topmore_btn.focus = False
+                    self.quit_btn.focus = True
+                elif self.focus == names[0]:
+                    self.focus = None
+                    self.quit_btn.focus = True
+                else:
+                    try:
+                        indx = names.index(self.focus)
+                    except ValueError:
+                        continue
+                    if indx == self.topindex:
+                        if key in (339, 259): # 339 page up, 259 up arrow
+                            self.topindex -= 1
+                            self.focus = names[indx-1]
+                        else:
+                            self.focus = None
+                            self.topmore_btn.focus = True
+                    else:
+                        self.focus = names[indx-1]
 
-                # draw devices and buttons
-                self.drawdevices()
-                self.drawbuttons()
-                self.devwinrefresh()
-                self.buttwin.noutrefresh()
-                curses.doupdate()
+            else:
+                # button not recognised
+                continue
 
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
+            # draw devices and buttons
+            self.drawdevices()
+            self.drawbuttons()
+            self.devwinrefresh()
+            self.buttwin.noutrefresh()
+            curses.doupdate()
 
 
 class ChooseVectorScreen(ConsoleClientScreen):
 
     def __init__(self, stdscr, control, devicename, group=None):
         super().__init__(stdscr, control)
 
@@ -1408,202 +1380,197 @@
         self.vectorswin.noutrefresh()
         curses.doupdate()
 
 
     async def inputs(self):
         "Gets inputs from the screen"
 
-        try:
-            self.stdscr.nodelay(True)
-            while True:
-                key = await self.keyinput()
-                if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
-                    return key
-
-                if isinstance(key, tuple):
-                    # mouse pressed, find if its clicked in any field
-                    # check all areas of the screen
-                    if key in self.quit_btn:
-                        if self.quit_btn.focus:
-                            widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
-                            self.messwin.noutrefresh()
-                            curses.doupdate()
-                            return "Quit"
-                        else:
-                            # focus is elsewhere
-                            self.setfocus("Quit")
-                        curses.doupdate()
-                        continue
-                    if key in self.messages_btn:
-                        if self.messages_btn.focus:
-                            return "Messages"
-                        else:
-                            self.setfocus("Messages")
-                        curses.doupdate()
-                        continue
-                    if key in self.devices_btn:
-                        if self.devices_btn.focus:
-                            return "Devices"
-                        else:
-                            self.setfocus("Devices")
-                        curses.doupdate()
-                        continue
+        self.stdscr.nodelay(True)
+        while True:
+            key = await self.keyinput()
+            if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
+                return key
 
-                    # check if mouse key in groupwin
-                    result = self.groupwin.setkey(key)
-                    if result == "Newfocus":
-                        # focus has been set onto a new group
-                        # must remove focus from other parts of the screen
-                        self.setfocus("Groups")
+            if isinstance(key, tuple):
+                # mouse pressed, find if its clicked in any field
+                # check all areas of the screen
+                if key in self.quit_btn:
+                    if self.quit_btn.focus:
+                        widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
+                        self.messwin.noutrefresh()
                         curses.doupdate()
-                        continue
-                    if result == "NewGroup":
-                        # must update the screen with a new group
-                        self.show()
-                        continue
+                        return "Quit"
+                    else:
+                        # focus is elsewhere
+                        self.setfocus("Quit")
+                    curses.doupdate()
+                    continue
+                if key in self.messages_btn:
+                    if self.messages_btn.focus:
+                        return "Messages"
+                    else:
+                        self.setfocus("Messages")
+                    curses.doupdate()
+                    continue
+                if key in self.devices_btn:
+                    if self.devices_btn.focus:
+                        return "Devices"
+                    else:
+                        self.setfocus("Devices")
+                    curses.doupdate()
+                    continue
 
-                    if not result:
-                        continue
-                    # otherwise mouse not pressed in a group, so self.groupwin.setkey(key)
-                    # just returns the key
-                    key = result
-
-                    # check if mouse key pressed in vectorswin
-                    result = self.vectorswin.setkey(key)
-                    if result == "Newfocus":
-                        # focus has been set onto a new vector
-                        # must remove focus from other parts of the screen
-                        self.setfocus("Vectors")
-                        curses.doupdate()
-                        continue
-                    if result == "NewVector":
-                        newvector = self.vectorswin.active
-                        if newvector in self.device:
-                            # newvector is a vector name, check if it is enabled
-                            if self.device[newvector].enable:
-                                self.vectorname = newvector
-                                return "Vectors"
+                # check if mouse key in groupwin
+                result = self.groupwin.setkey(key)
+                if result == "Newfocus":
+                    # focus has been set onto a new group
+                    # must remove focus from other parts of the screen
+                    self.setfocus("Groups")
+                    curses.doupdate()
+                    continue
+                if result == "NewGroup":
+                    # must update the screen with a new group
+                    self.show()
+                    continue
 
-                    # mouse press not on a field
+                if not result:
                     continue
+                # otherwise mouse not pressed in a group, so self.groupwin.setkey(key)
+                # just returns the key
+                key = result
+
+                # check if mouse key pressed in vectorswin
+                result = self.vectorswin.setkey(key)
+                if result == "Newfocus":
+                    # focus has been set onto a new vector
+                    # must remove focus from other parts of the screen
+                    self.setfocus("Vectors")
+                    curses.doupdate()
+                    continue
+                if result == "NewVector":
+                    newvector = self.vectorswin.active
+                    if newvector in self.device:
+                        # newvector is a vector name, check if it is enabled
+                        if self.device[newvector].enable:
+                            self.vectorname = newvector
+                            return "Vectors"
 
-                # so not a tuple/mouse press, its a key press
+                # mouse press not on a field
+                continue
 
-                if self.focus == "Groups":
-                    # focus has been given to the GroupWin
-                    result = self.groupwin.setkey(key)
-                    if result == "NewGroup":
-                        # must update the screen with a new group
-                        # which is available as self.groupwin.active
-                        self.show()
-                        continue
-                    if not result:
-                        continue
-                    key = result
-                    # key could be a down arrow for next item
-                    # but will not be 10 as Enter will be actioned within self.groupwin.setkey(key)
+            # so not a tuple/mouse press, its a key press
 
-                elif self.focus == "Vectors":
-                    # focus has been given to VectorListWin
-                    result = self.vectorswin.setkey(key)
-                    if not result:
-                        continue
-                    if result == "NewVector":
-                        newvector = self.vectorswin.active
-                        if newvector in self.device:
-                            # newvector is a vector name, check if it is enabled
-                            if self.device[newvector].enable:
-                                self.vectorname = newvector
-                                return "Vectors"
-                            else:
-                                continue
+            if self.focus == "Groups":
+                # focus has been given to the GroupWin
+                result = self.groupwin.setkey(key)
+                if result == "NewGroup":
+                    # must update the screen with a new group
+                    # which is available as self.groupwin.active
+                    self.show()
+                    continue
+                if not result:
+                    continue
+                key = result
+                # key could be a down arrow for next item
+                # but will not be 10 as Enter will be actioned within self.groupwin.setkey(key)
+
+            elif self.focus == "Vectors":
+                # focus has been given to VectorListWin
+                result = self.vectorswin.setkey(key)
+                if not result:
+                    continue
+                if result == "NewVector":
+                    newvector = self.vectorswin.active
+                    if newvector in self.device:
+                        # newvector is a vector name, check if it is enabled
+                        if self.device[newvector].enable:
+                            self.vectorname = newvector
+                            return "Vectors"
                         else:
                             continue
-                    key = result
-                    # key could be a down arrow for next item
-                    # but will not be 10 as Enter will be actioned within self.vectorswin.setkey(key)
-
-                if key == 10:
-                    # enter key pressed
-                    if self.focus == "Quit":
-                        widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
-                        self.messwin.noutrefresh()
-                        curses.doupdate()
-                    # return the focus value of whichever item was in focus when enter was pressed
-                    return self.focus
+                    else:
+                        continue
+                key = result
+                # key could be a down arrow for next item
+                # but will not be 10 as Enter will be actioned within self.vectorswin.setkey(key)
 
-                if key in (32, 9, 261, 338, 258):
-                    # go to the next widget
-                    if self.focus == "Quit":
-                        if len(self.groupwin.groups()) == 1:
-                            newfocus = "Vectors"
-                        else:
-                            newfocus = "Groups"
+            if key == 10:
+                # enter key pressed
+                if self.focus == "Quit":
+                    widgets.drawmessage(self.messwin, "Quit chosen ... Please wait", bold = True, maxcols=self.maxcols)
+                    self.messwin.noutrefresh()
+                    curses.doupdate()
+                # return the focus value of whichever item was in focus when enter was pressed
+                return self.focus
+
+            if key in (32, 9, 261, 338, 258):
+                # go to the next widget
+                if self.focus == "Quit":
+                    if len(self.groupwin.groups()) == 1:
+                        newfocus = "Vectors"
                     else:
-                        indx = self.screenparts.index(self.focus)
-                        newfocus = self.screenparts[indx+1]
-                elif key in (353, 260, 339, 259):
-                    # go to previous button
-                    if self.focus == "Groups":
+                        newfocus = "Groups"
+                else:
+                    indx = self.screenparts.index(self.focus)
+                    newfocus = self.screenparts[indx+1]
+            elif key in (353, 260, 339, 259):
+                # go to previous button
+                if self.focus == "Groups":
+                    newfocus = "Quit"
+                elif self.focus == "Vectors":
+                    if len(self.groupwin.groups()) == 1:
                         newfocus = "Quit"
-                    elif self.focus == "Vectors":
-                        if len(self.groupwin.groups()) == 1:
-                            newfocus = "Quit"
-                        else:
-                            newfocus = "Groups"
                     else:
-                        indx = self.screenparts.index(self.focus)
-                        newfocus = self.screenparts[indx-1]
+                        newfocus = "Groups"
                 else:
-                    # key not recognised
-                    continue
+                    indx = self.screenparts.index(self.focus)
+                    newfocus = self.screenparts[indx-1]
+            else:
+                # key not recognised
+                continue
 
-                if self.focus == "Vectors":
-                    self.vectorswin.defocus()
-                elif self.focus == "Groups":
-                    self.groupwin.defocus()
-                elif self.focus == "Devices":
-                    self.devices_btn.focus = False
-                elif self.focus == "Messages":
-                    self.messages_btn.focus = False
-                elif self.focus == "Quit":
-                    self.quit_btn.focus = False
-                if newfocus == "Vectors":
-                    if key in (32, 9, 261, 338, 258):
-                        # next button
-                        self.vectorswin.set_top_focus()
-                    else:
-                        self.vectorswin.set_bot_focus()
-                elif newfocus == "Groups":
-                    self.groupwin.set_left_focus()
-                elif newfocus == "Devices":
-                    self.devices_btn.focus = True
-                elif newfocus == "Messages":
-                    self.messages_btn.focus = True
-                elif newfocus == "Quit":
-                    self.quit_btn.focus = True
-                self.focus = newfocus
+            if self.focus == "Vectors":
+                self.vectorswin.defocus()
+            elif self.focus == "Groups":
+                self.groupwin.defocus()
+            elif self.focus == "Devices":
+                self.devices_btn.focus = False
+            elif self.focus == "Messages":
+                self.messages_btn.focus = False
+            elif self.focus == "Quit":
+                self.quit_btn.focus = False
+            if newfocus == "Vectors":
+                if key in (32, 9, 261, 338, 258):
+                    # next button
+                    self.vectorswin.set_top_focus()
+                else:
+                    self.vectorswin.set_bot_focus()
+            elif newfocus == "Groups":
+                self.groupwin.set_left_focus()
+            elif newfocus == "Devices":
+                self.devices_btn.focus = True
+            elif newfocus == "Messages":
+                self.messages_btn.focus = True
+            elif newfocus == "Quit":
+                self.quit_btn.focus = True
+            self.focus = newfocus
 
-                # so buttons have been set with the appropriate focus
-                # now draw them
-                self.groupwin.draw(self.devicename)
-                self.vectorswin.draw(self.devicename, self.groupwin.active, change=True)
-                self.devices_btn.draw()
-                self.messages_btn.draw()
-                self.quit_btn.draw()
+            # so buttons have been set with the appropriate focus
+            # now draw them
+            self.groupwin.draw(self.devicename)
+            self.vectorswin.draw(self.devicename, self.groupwin.active, change=True)
+            self.devices_btn.draw()
+            self.messages_btn.draw()
+            self.quit_btn.draw()
+
+            self.vectorswin.noutrefresh()
+            self.groupwin.noutrefresh()
+            self.buttwin.noutrefresh()
+            curses.doupdate()
 
-                self.vectorswin.noutrefresh()
-                self.groupwin.noutrefresh()
-                self.buttwin.noutrefresh()
-                curses.doupdate()
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
 
 
 # This class GroupBtns defines the position of group buttons on the row
 # and stores values used to check if any change has occurred
 
 class GroupBtns:
 
@@ -2886,148 +2853,140 @@
         "Gets inputs from the screen"
 
         # two loops formed here, one for the entire screen
         # and one for an editable field
         # result tracks the results of tests to see if an editable field loop is needed
         result = None
 
-        try:
-            self.stdscr.nodelay(True)
-            while True:
-                if result:
-                    key = result
-                    result = None
-                else:
-                    key = await self.keyinput()
+        self.stdscr.nodelay(True)
+        while True:
+            if result:
+                key = result
+                result = None
+            else:
+                key = await self.keyinput()
 
-                if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
-                    return key
+            if key in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
+                return key
 
-                key = self.check_bottom_btn(key)
-                if not key:
-                    continue
-                if key in ("Vectors", "Devices", "Messages", "Quit"):
-                    return key
+            key = self.check_bottom_btn(key)
+            if not key:
+                continue
+            if key in ("Vectors", "Devices", "Messages", "Quit"):
+                return key
 
-                # At this point, key could be a mouse tuple, or a keystroke
-                # But not clicked on any of the bottom buttons
-                # So could be mouse clicked away from anything, or on something in memberswin
-                # or maybe memberswin has the focus, and the keystroke should be handled there
-
-                if isinstance(key, tuple):
-                    # mouse pressed, find if its clicked in any of the MembersWin fields
-                    result = self.memberswin.handlemouse(key)
-                    # result is None if fully handled,
-                    # or is 'edit' if mouse clicked in an editable field in MembersWin
-                    # or is 'focused' if mouse clicked on a previously unfocused button
-                    # could also be one of "submitted", "next", "previous" if clicked
-                    # on a focused submit, or top or bottom widget
-                    if not result:
-                        # Handled, continue with while loop and get next key
-                        continue
+            # At this point, key could be a mouse tuple, or a keystroke
+            # But not clicked on any of the bottom buttons
+            # So could be mouse clicked away from anything, or on something in memberswin
+            # or maybe memberswin has the focus, and the keystroke should be handled there
 
-                # At this point, result is None if key is a keystroke,
-                # or result is value returned by memberswin.handlemouse(key)
+            if isinstance(key, tuple):
+                # mouse pressed, find if its clicked in any of the MembersWin fields
+                result = self.memberswin.handlemouse(key)
+                # result is None if fully handled,
+                # or is 'edit' if mouse clicked in an editable field in MembersWin
+                # or is 'focused' if mouse clicked on a previously unfocused button
+                # could also be one of "submitted", "next", "previous" if clicked
+                # on a focused submit, or top or bottom widget
+                if not result:
+                    # Handled, continue with while loop and get next key
+                    continue
 
-                if (result == "focused") or (result == "edit"):
-                    # a field in self.memberswin has been set into focus
-                    # ensure bottom buttons are defocused
-                    self.vectors_btn.focus = False
-                    self.vectors_btn.draw()
-                    self.devices_btn.focus = False
-                    self.devices_btn.draw()
-                    self.messages_btn.focus = False
-                    self.messages_btn.draw()
-                    self.quit_btn.focus = False
-                    self.quit_btn.draw()
-                    self.buttwin.noutrefresh()
-                    curses.doupdate()
+            # At this point, result is None if key is a keystroke,
+            # or result is value returned by memberswin.handlemouse(key)
 
-                if result == "focused":
-                    # A button has been set to focus, nothing more to do
-                    # continue and get the next key
-                    result = None
-                    continue
+            if (result == "focused") or (result == "edit"):
+                # a field in self.memberswin has been set into focus
+                # ensure bottom buttons are defocused
+                self.vectors_btn.focus = False
+                self.vectors_btn.draw()
+                self.devices_btn.focus = False
+                self.devices_btn.draw()
+                self.messages_btn.focus = False
+                self.messages_btn.draw()
+                self.quit_btn.focus = False
+                self.quit_btn.draw()
+                self.buttwin.noutrefresh()
+                curses.doupdate()
 
-                if (not result) and (not self.memberswin.focus):
-                    # if keystroke, then only of interest if memberswin has focus
-                    continue
+            if result == "focused":
+                # A button has been set to focus, nothing more to do
+                # continue and get the next key
+                result = None
+                continue
 
-                if not result:
-                    # key is a keystroke, and memberswin has focus, handle it
-                    result = self.memberswin.setkey(key)
-                    # this returns "edit" if an editable field has been given focus
-                    # could also be "submitted", "next", "previous" or a keystroke such
-                    # as 9 for tab
-
-                while result == "edit":
-                   # An editable field is in focus
-                    inputfield = self.memberswin.inputfield()
-                    if inputfield is None:
-                        break
-                    result = await inputfield()
-                    if result in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
-                        return result
-                    if not result:
-                        break
-                    if result in ("submitted", "next", "previous"):
-                        break
-                    if isinstance(result, tuple):
-                        # a mouse press, go to outer loop with result set
-                        break
-                    # inputfield has returned a keystroke, typically 9 for next tab
-                    # which is now tested again with self.memberswin.setkey(key)
-                    result = self.memberswin.setkey(result)
+            if (not result) and (not self.memberswin.focus):
+                # if keystroke, then only of interest if memberswin has focus
+                continue
 
+            if not result:
+                # key is a keystroke, and memberswin has focus, handle it
+                result = self.memberswin.setkey(key)
+                # this returns "edit" if an editable field has been given focus
+                # could also be "submitted", "next", "previous" or a keystroke such
+                # as 9 for tab
+
+            while result == "edit":
+               # An editable field is in focus
+                inputfield = self.memberswin.inputfield()
+                if inputfield is None:
+                    break
+                result = await inputfield()
                 if result in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
                     return result
+                if not result:
+                    break
+                if result in ("submitted", "next", "previous"):
+                    break
+                if isinstance(result, tuple):
+                    # a mouse press, go to outer loop with result set
+                    break
+                # inputfield has returned a keystroke, typically 9 for next tab
+                # which is now tested again with self.memberswin.setkey(key)
+                result = self.memberswin.setkey(result)
 
-                if result == "submitted":
-                    self.vector.state = 'Busy'
-                    # The vector has been submitted, draw vector state which is now busy
-                    widgets.draw_timestamp_state(self.control, self.tstatewin, self.vector)
-                    self.tstatewin.noutrefresh()
-                    self.vectors_btn.focus = True
-                    self.buttwin.clear()
-                    self.vectors_btn.draw()
-                    self.devices_btn.draw()
-                    self.messages_btn.draw()
-                    self.quit_btn.draw()
-                    self.buttwin.noutrefresh()
-                    curses.doupdate()
-                    result = None
-                elif result == "next":   # go to next button
-                    self.memberswin.defocus() # removes focus and calls draw and noutrefresh on memberswin
-                    self.vectors_btn.focus = True
-                    self.buttwin.clear()
-                    self.vectors_btn.draw()
-                    self.devices_btn.draw()
-                    self.messages_btn.draw()
-                    self.quit_btn.draw()
-                    self.buttwin.noutrefresh()
-                    curses.doupdate()
-                    result = None
-                elif result == "previous":   # go to prev button
-                    self.memberswin.defocus() # removes focus and calls draw and noutrefresh on memberswin
-                    self.quit_btn.focus = True
-                    self.buttwin.clear()
-                    self.vectors_btn.draw()
-                    self.devices_btn.draw()
-                    self.messages_btn.draw()
-                    self.quit_btn.draw()
-                    self.buttwin.noutrefresh()
-                    curses.doupdate()
-                    result = None
-
+            if result in ("Resize", "Messages", "Devices", "Vectors", "Stop"):
+                return result
 
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
+            if result == "submitted":
+                self.vector.state = 'Busy'
+                # The vector has been submitted, draw vector state which is now busy
+                widgets.draw_timestamp_state(self.control, self.tstatewin, self.vector)
+                self.tstatewin.noutrefresh()
+                self.vectors_btn.focus = True
+                self.buttwin.clear()
+                self.vectors_btn.draw()
+                self.devices_btn.draw()
+                self.messages_btn.draw()
+                self.quit_btn.draw()
+                self.buttwin.noutrefresh()
+                curses.doupdate()
+                result = None
+            elif result == "next":   # go to next button
+                self.memberswin.defocus() # removes focus and calls draw and noutrefresh on memberswin
+                self.vectors_btn.focus = True
+                self.buttwin.clear()
+                self.vectors_btn.draw()
+                self.devices_btn.draw()
+                self.messages_btn.draw()
+                self.quit_btn.draw()
+                self.buttwin.noutrefresh()
+                curses.doupdate()
+                result = None
+            elif result == "previous":   # go to prev button
+                self.memberswin.defocus() # removes focus and calls draw and noutrefresh on memberswin
+                self.quit_btn.focus = True
+                self.buttwin.clear()
+                self.vectors_btn.draw()
+                self.devices_btn.draw()
+                self.messages_btn.draw()
+                self.quit_btn.draw()
+                self.buttwin.noutrefresh()
+                curses.doupdate()
+                result = None
 
 
 # MembersWin is created within VectorScreen
 
 
 class MembersWin(ParentScreen):
 
@@ -3366,297 +3325,291 @@
             self._inputfield = widget.inputfield
         return result
 
 
 
     def setkey(self, key):
         "Handles a key stroke"
-        try:
 
-            # check if a widget is in focus
-            if self.vector.perm != "ro":
-                # if ro, nothing to set on widgets
-                for widget in self.displayed:
-                    if widget.focus:
-                        # a widget is in focus
-                        result = widget.setkey(key)
-                        if result == "edit":
-                            # this sets an input awaitable
-                            self._inputfield = widget.inputfield
-                            return result
-                        else:
-                            self._inputfield = None
-                        if result:
-                            # if the widget returns a key. then continue with
-                            # checking it
-                            key = result
-                            break
-                        # the widget has handled the key, and returns None
-                        # to indicate no further checks required.
-                        return
+        # check if a widget is in focus
+        if self.vector.perm != "ro":
+            # if ro, nothing to set on widgets
+            for widget in self.displayed:
+                if widget.focus:
+                    # a widget is in focus
+                    result = widget.setkey(key)
+                    if result == "edit":
+                        # this sets an input awaitable
+                        self._inputfield = widget.inputfield
+                        return result
+                    else:
+                        self._inputfield = None
+                    if result:
+                        # if the widget returns a key. then continue with
+                        # checking it
+                        key = result
+                        break
+                    # the widget has handled the key, and returns None
+                    # to indicate no further checks required.
+                    return
 
-            if key == 10:
-                # Enter key pressed
-                if self.topmore_btn.focus:
-                    # scroll the window down
-                    self.topindex -= 1
-                    self.displayedwidgets()
-                    if not self.topindex:
-                        # self.topindex is now zero, so self.topmore_btn will not be shown
-                        # and the top widget should get focus
-                        topwidget = self.displayed[0]
-                        topwidget.focus = True
-                    self.draw()
-                    self.noutrefresh()
+        if key == 10:
+            # Enter key pressed
+            if self.topmore_btn.focus:
+                # scroll the window down
+                self.topindex -= 1
+                self.displayedwidgets()
+                if not self.topindex:
+                    # self.topindex is now zero, so self.topmore_btn will not be shown
+                    # and the top widget should get focus
+                    topwidget = self.displayed[0]
+                    topwidget.focus = True
+                self.draw()
+                self.noutrefresh()
+                curses.doupdate()
+                return
+            elif self.botmore_btn.focus:
+                # scroll the window up
+                self.topindex += 1
+                self.displayedwidgets()
+                # displayedindex of last widget displayed
+                displayedindex = len(self.displayed) - 1
+                memberwidgetsindex = displayedindex + self.topindex
+                if memberwidgetsindex == len(self.memberwidgets) -1:
+                    # the last widget is being displayed, so self.botmore_btn will not be shown
+                    # and the bottom widget should get focus
+                    botwidget = self.memberwidgets[-1]
+                    botwidget.focus = True
+                self.draw()
+                self.noutrefresh()
+                curses.doupdate()
+                return
+            elif self.vector.perm == "ro":
+                # can scroll up or down, with more buttons,
+                # but nothing to submit, so Enter key ignored
+                return
+            elif self.submit_btn.focus:
+                if submitvector(self.vector, self.memberwidgets):
+                    # vector has been submitted, remove focus from this window
+                    self.focus = False
+                    self.submit_btn.focus = False
+                    self.submit_btn.ok()   # draw submit button in green with ok
+                    self.submitwin.noutrefresh()
                     curses.doupdate()
-                    return
-                elif self.botmore_btn.focus:
-                    # scroll the window up
-                    self.topindex += 1
-                    self.displayedwidgets()
-                    # displayedindex of last widget displayed
-                    displayedindex = len(self.displayed) - 1
-                    memberwidgetsindex = displayedindex + self.topindex
-                    if memberwidgetsindex == len(self.memberwidgets) -1:
-                        # the last widget is being displayed, so self.botmore_btn will not be shown
-                        # and the bottom widget should get focus
-                        botwidget = self.memberwidgets[-1]
-                        botwidget.focus = True
-                    self.draw()
-                    self.noutrefresh()
+                    time.sleep(0.3)      # blocking, to avoid screen being changed while this time elapses
+                    self.submitwin.clear()
+                    self.submit_btn.draw()
+                    self.cancel_btn.draw()
+                    self.submitwin.noutrefresh()
+                    # curses.doupdate() - not needed, called by vector window on submission
+                    return "submitted"
+                else:
+                    # error condition
+                    self.submit_btn.alert()
+                    self.submitwin.noutrefresh()
                     curses.doupdate()
-                    return
-                elif self.vector.perm == "ro":
-                    # can scroll up or down, with more buttons,
-                    # but nothing to submit, so Enter key ignored
-                    return
-                elif self.submit_btn.focus:
-                    if submitvector(self.vector, self.memberwidgets):
-                        # vector has been submitted, remove focus from this window
-                        self.focus = False
-                        self.submit_btn.focus = False
-                        self.submit_btn.ok()   # draw submit button in green with ok
-                        self.submitwin.noutrefresh()
-                        curses.doupdate()
-                        time.sleep(0.3)      # blocking, to avoid screen being changed while this time elapses
-                        self.submitwin.clear()
-                        self.submit_btn.draw()
-                        self.cancel_btn.draw()
-                        self.submitwin.noutrefresh()
-                        # curses.doupdate() - not needed, called by vector window on submission
-                        return "submitted"
-                    else:
-                        # error condition
-                        self.submit_btn.alert()
-                        self.submitwin.noutrefresh()
-                        curses.doupdate()
-                        time.sleep(0.3)        # blocking, to avoid screen being changed while this time elapses
-                        self.submitwin.clear()
-                        self.submit_btn.draw()
-                        self.cancel_btn.draw()
-                        self.submitwin.noutrefresh()
-                        curses.doupdate()
-                        return
-                elif self.cancel_btn.focus:
-                    # Cancel chosen, reset all widgets, removing any value changes
-                    for memberwidget in self.displayed:
-                        memberwidget.reset()
-                    self.memwin.noutrefresh()
+                    time.sleep(0.3)        # blocking, to avoid screen being changed while this time elapses
+                    self.submitwin.clear()
+                    self.submit_btn.draw()
+                    self.cancel_btn.draw()
+                    self.submitwin.noutrefresh()
                     curses.doupdate()
                     return
-                else:
-                    # Enter pressed, but none of the above have handled it
-                    return
+            elif self.cancel_btn.focus:
+                # Cancel chosen, reset all widgets, removing any value changes
+                for memberwidget in self.displayed:
+                    memberwidget.reset()
+                self.memwin.noutrefresh()
+                curses.doupdate()
+                return
+            else:
+                # Enter pressed, but none of the above have handled it
+                return
 
 # 32 space, 9 tab, 353 shift tab, 261 right arrow, 260 left arrow, 10 return, 339 page up, 338 page down, 259 up arrow, 258 down arrow
 
-            if key in (32, 9, 261, 338, 258):   # go to next button
-                if self.cancel_btn.focus:
-                    # last in this window
-                    return "next"
-                if self.submit_btn.focus:
-                    self.submit_btn.focus = False
-                    self.cancel_btn.focus = True
+        if key in (32, 9, 261, 338, 258):   # go to next button
+            if self.cancel_btn.focus:
+                # last in this window
+                return "next"
+            if self.submit_btn.focus:
+                self.submit_btn.focus = False
+                self.cancel_btn.focus = True
+                self.submit_btn.draw()
+                self.cancel_btn.draw()
+                self.submitwin.noutrefresh()
+                curses.doupdate()
+                return
+            if self.botmore_btn.focus:
+                if self.submit_btn.show:
+                    self.botmore_btn.focus = False
+                    self.botmore_btn.draw()
+                    self.submit_btn.focus = True
                     self.submit_btn.draw()
-                    self.cancel_btn.draw()
+                    self.botmorewin.noutrefresh()
                     self.submitwin.noutrefresh()
                     curses.doupdate()
                     return
-                if self.botmore_btn.focus:
-                    if self.submit_btn.show:
-                        self.botmore_btn.focus = False
-                        self.botmore_btn.draw()
-                        self.submit_btn.focus = True
-                        self.submit_btn.draw()
-                        self.botmorewin.noutrefresh()
-                        self.submitwin.noutrefresh()
-                        curses.doupdate()
-                        return
-                    else:
-                        return "next"
-                # get the top widget being displayed
-                if self.topmore_btn.focus:
-                    self.topmore_btn.focus = False
-                    self.topmore_btn.draw()
-                    nextwidget = self.displayed[0]
+                else:
+                    return "next"
+            # get the top widget being displayed
+            if self.topmore_btn.focus:
+                self.topmore_btn.focus = False
+                self.topmore_btn.draw()
+                nextwidget = self.displayed[0]
+                nextwidget.focus = True
+                nextwidget.draw()
+                self.topmorewin.noutrefresh()
+                self.memwin.noutrefresh()
+                curses.doupdate()
+                return
+
+            if (displayedindex := self.displayed_widgetindex_in_focus()) is not None:
+                # A widget is in focus
+                widget = self.displayed[displayedindex]
+                if displayedindex != len(self.displayed) - 1:
+                    # the displayed widget is not the last widget on the list of displayed widgets
+                    # so simply set the next widget into focus
+                    widget.focus = False
+                    widget.draw()
+                    nextwidget = self.displayed[displayedindex+1]
                     nextwidget.focus = True
                     nextwidget.draw()
-                    self.topmorewin.noutrefresh()
                     self.memwin.noutrefresh()
                     curses.doupdate()
                     return
-
-                if (displayedindex := self.displayed_widgetindex_in_focus()) is not None:
-                    # A widget is in focus
-                    widget = self.displayed[displayedindex]
-                    if displayedindex != len(self.displayed) - 1:
-                        # the displayed widget is not the last widget on the list of displayed widgets
-                        # so simply set the next widget into focus
-                        widget.focus = False
-                        widget.draw()
-                        nextwidget = self.displayed[displayedindex+1]
-                        nextwidget.focus = True
-                        nextwidget.draw()
-                        self.memwin.noutrefresh()
-                        curses.doupdate()
-                        return
-                    # The widget in focus is the last of the displayed widgets
-                    # Either scroll up, or jump to more ....
-                    widgetindex = displayedindex + self.topindex
-                    if widgetindex == len(self.memberwidgets) -1:
-                        # This is the last widget, the more button will not be shown, but the submit button may be
-                        if self.submit_btn.show:
-                            widget.focus = False
-                            widget.draw()
-                            self.submit_btn.focus = True
-                            self.submit_btn.draw()
-                            self.memwin.noutrefresh()
-                            self.submitwin.noutrefresh()
-                            curses.doupdate()
-                            return
-                        # last widget and the submit is not shown
-                        return "next"
-                    # last displayed widgets, but there are further widgets to be shown
-                    if key == 9:
-                        # tab key pressed, set the botmore button in focus
+                # The widget in focus is the last of the displayed widgets
+                # Either scroll up, or jump to more ....
+                widgetindex = displayedindex + self.topindex
+                if widgetindex == len(self.memberwidgets) -1:
+                    # This is the last widget, the more button will not be shown, but the submit button may be
+                    if self.submit_btn.show:
                         widget.focus = False
                         widget.draw()
-                        self.botmore_btn.focus = True
-                        self.botmore_btn.draw()
+                        self.submit_btn.focus = True
+                        self.submit_btn.draw()
                         self.memwin.noutrefresh()
-                        self.botmorewin.noutrefresh()
+                        self.submitwin.noutrefresh()
                         curses.doupdate()
                         return
-                    # next required, but not tab and not last widget,
-                    # so scroll the window up
+                    # last widget and the submit is not shown
+                    return "next"
+                # last displayed widgets, but there are further widgets to be shown
+                if key == 9:
+                    # tab key pressed, set the botmore button in focus
                     widget.focus = False
                     widget.draw()
-                    self.topindex += 1
-                    self.displayedwidgets()
-                    nextwidget = self.displayed[-1]
-                    nextwidget.focus = True
-                    self.draw()
-                    self.noutrefresh()
+                    self.botmore_btn.focus = True
+                    self.botmore_btn.draw()
+                    self.memwin.noutrefresh()
+                    self.botmorewin.noutrefresh()
                     curses.doupdate()
                     return
+                # next required, but not tab and not last widget,
+                # so scroll the window up
+                widget.focus = False
+                widget.draw()
+                self.topindex += 1
+                self.displayedwidgets()
+                nextwidget = self.displayed[-1]
+                nextwidget.focus = True
+                self.draw()
+                self.noutrefresh()
+                curses.doupdate()
+                return
 
 # 32 space, 9 tab, 353 shift tab, 261 right arrow, 260 left arrow, 10 return, 339 page up, 338 page down, 259 up arrow, 258 down arrow
 
-            if key in (353, 260, 339, 259):   # go to prev button
+        if key in (353, 260, 339, 259):   # go to prev button
 
-                if self.cancel_btn.focus:
-                    # go to submit button
-                    self.cancel_btn.focus = False
-                    self.submit_btn.focus = True
-                    self.cancel_btn.draw()
-                    self.submit_btn.draw()
-                    self.submitwin.noutrefresh()
-                    curses.doupdate()
-                    return
-                if self.submit_btn.focus:
-                    self.submit_btn.focus = False
-                    self.submit_btn.draw()
-                    self.submitwin.noutrefresh()
-                    if self.botmore_btn.show:
-                        self.botmore_btn.focus = True
-                        self.botmore_btn.draw()
-                        self.botmorewin.noutrefresh()
-                        curses.doupdate()
-                        return
-                    # set bottom displayed widget into focus
-                    widget = self.displayed[-1]
-                    widget.focus = True
-                    widget.draw()
-                    self.memwin.noutrefresh()
-                    curses.doupdate()
-                    return
-                if self.botmore_btn.focus:
-                    # set bottom displayed widget into focus
-                    self.botmore_btn.focus = False
+            if self.cancel_btn.focus:
+                # go to submit button
+                self.cancel_btn.focus = False
+                self.submit_btn.focus = True
+                self.cancel_btn.draw()
+                self.submit_btn.draw()
+                self.submitwin.noutrefresh()
+                curses.doupdate()
+                return
+            if self.submit_btn.focus:
+                self.submit_btn.focus = False
+                self.submit_btn.draw()
+                self.submitwin.noutrefresh()
+                if self.botmore_btn.show:
+                    self.botmore_btn.focus = True
                     self.botmore_btn.draw()
                     self.botmorewin.noutrefresh()
-                    widget = self.displayed[-1]
-                    widget.focus = True
+                    curses.doupdate()
+                    return
+                # set bottom displayed widget into focus
+                widget = self.displayed[-1]
+                widget.focus = True
+                widget.draw()
+                self.memwin.noutrefresh()
+                curses.doupdate()
+                return
+            if self.botmore_btn.focus:
+                # set bottom displayed widget into focus
+                self.botmore_btn.focus = False
+                self.botmore_btn.draw()
+                self.botmorewin.noutrefresh()
+                widget = self.displayed[-1]
+                widget.focus = True
+                widget.draw()
+                self.memwin.noutrefresh()
+                curses.doupdate()
+                return
+            if self.topmore_btn.focus:
+                # top button of this window
+                return "previous"
+            # So now check if a member button is in focus
+            if (displayedindex := self.displayed_widgetindex_in_focus()) is not None:
+                # A widget is in focus
+                widget = self.displayed[displayedindex]
+                if displayedindex:
+                    # not zero, so focus can just move up one
+                    widget.focus = False
                     widget.draw()
+                    prevwidget = self.displayed[displayedindex-1]
+                    prevwidget.focus = True
+                    prevwidget.draw()
                     self.memwin.noutrefresh()
                     curses.doupdate()
                     return
-                if self.topmore_btn.focus:
-                    # top button of this window
+                # showing top widget of the displayed widgets
+                # Either scroll down, or jump to more ....
+                # self.topindex is the widget index
+                if not self.topindex:
+                    # This is the first widget, the more button will not be shown
                     return "previous"
-                # So now check if a member button is in focus
-                if (displayedindex := self.displayed_widgetindex_in_focus()) is not None:
-                    # A widget is in focus
-                    widget = self.displayed[displayedindex]
-                    if displayedindex:
-                        # not zero, so focus can just move up one
-                        widget.focus = False
-                        widget.draw()
-                        prevwidget = self.displayed[displayedindex-1]
-                        prevwidget.focus = True
-                        prevwidget.draw()
-                        self.memwin.noutrefresh()
-                        curses.doupdate()
-                        return
-                    # showing top widget of the displayed widgets
-                    # Either scroll down, or jump to more ....
-                    # self.topindex is the widget index
-                    if not self.topindex:
-                        # This is the first widget, the more button will not be shown
-                        return "previous"
-                    # top displayed widgets, but more can be shown, if shift-tab pressed,
-                    # jump to topmore
-                    if key == 353:
-                        # shift tab key pressed, set the topmore button in focus
-                        widget.focus = False
-                        widget.draw()
-                        self.topmore_btn.focus = True
-                        self.topmore_btn.draw()
-                        self.memwin.noutrefresh()
-                        self.topmorewin.noutrefresh()
-                        curses.doupdate()
-                        return
-                    # prev required, but not shift-tab and not first widget,
-                    # so scroll the window down
+                # top displayed widgets, but more can be shown, if shift-tab pressed,
+                # jump to topmore
+                if key == 353:
+                    # shift tab key pressed, set the topmore button in focus
                     widget.focus = False
                     widget.draw()
-                    self.topindex -= 1
-                    self.displayedwidgets()
-                    prevwidget = self.displayed[0]
-                    prevwidget.focus = True
-                    self.draw()
-                    self.noutrefresh()
+                    self.topmore_btn.focus = True
+                    self.topmore_btn.draw()
+                    self.memwin.noutrefresh()
+                    self.topmorewin.noutrefresh()
                     curses.doupdate()
                     return
+                # prev required, but not shift-tab and not first widget,
+                # so scroll the window down
+                widget.focus = False
+                widget.draw()
+                self.topindex -= 1
+                self.displayedwidgets()
+                prevwidget = self.displayed[0]
+                prevwidget.focus = True
+                self.draw()
+                self.noutrefresh()
+                curses.doupdate()
+                return
 
-        except asyncio.CancelledError:
-            raise
-        except Exception as e:
-            widgets.ERRORDATA.append(TBE.from_exception(e))
-            return "Quit"
 
 
 def submitvector(vector, memberwidgets):
     "Checks and submits the vector, if ok returns True, if not returns False"
     if vector.vectortype == "SwitchVector":
         members = {member.name:member.newvalue() for member in memberwidgets}
         # members is a dictionary of membername : member value ('On' or 'Off')
```

### Comparing `indipyclient-0.0.1/indipyclient/events.py` & `indipyclient-0.0.2/indipyclient/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,18 @@
     """The remote driver is instructing the client to delete either a device or a vector property.
        This contains attribute vectorname, if it is None, then the whole device is to be deleted.
        A 'message' attribute contains any message sent by the client with this instruction."""
 
     def __init__(self, root, device, client):
         super().__init__(root, device, client)
         if self.devicename is None:
-            raise ParseException
+            raise ParseException("delProperty has no devicename")
         if not self.device.enable:
             # already deleted
-            raise ParseException
+            raise ParseException("device already deleted")
         self.vectorname = root.get("name")
         self.message = root.get("message", "")
         # properties is a dictionary of property name to propertyvector this device owns
         # This method updates a property vector and sets it into properties
         properties = device.data
         if self.vectorname:
             # does this vector already exist, if it does, disable it
@@ -117,22 +117,22 @@
 class defVector(Event, UserDict):
     "Parent to def vectors, adds a mapping of membername:value"
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
         UserDict.__init__(self)
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise ParseException
+            raise ParseException("defVector has no vector name")
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "DEFAULT GROUP")
         state = root.get("state")
         if not state:
-            raise ParseException
+            raise ParseException("defVector has no state given")
         if not state in ('Idle','Ok','Busy','Alert'):
-            raise ParseException
+            raise ParseException("defVector has invalid state")
         self.state = state
         self.message = root.get("message", "")
 
 
     def __setitem__(self, membername):
         raise KeyError
 
@@ -143,22 +143,22 @@
        attributes perm, rule, timeout, and memberlabels which is a dictionary of
        membername:label."""
 
     def __init__(self, root, device, client):
         defVector.__init__(self, root, device, client)
         self.perm = root.get("perm")
         if self.perm is None:
-            raise ParseException
+            raise ParseException("defSwitchVector has no perm given")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise ParseException
+            raise ParseException("defSwitchVector has invalid perm")
         self.rule = root.get("rule")
         if self.rule is None:
-            raise ParseException
+            raise ParseException("defSwitchVector has no rule given")
         if self.rule not in ('OneOfMany', 'AtMostOne', 'AnyOfMany'):
-            raise ParseException
+            raise ParseException("defSwitchVector has invalid rule")
         try:
             timeout = root.get("timeout")
             if not timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
         except:
@@ -166,28 +166,30 @@
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defSwitch":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("defSwitch member has no name")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
+                if not member.text:
+                    raise ParseException("defSwitch member has invalid value")
                 value = member.text.strip()
                 if value == "On":
                     self.data[membername] = "On"
                 elif value == "Off":
                     self.data[membername] = "Off"
                 else:
-                    raise ParseException
+                    raise ParseException("defSwitch member has invalid value")
             else:
-                raise ParseException
+                raise ParseException("defSwitchVector member has invalid tag")
         if not self.data:
-            raise ParseException
+            raise ParseException("defSwitchVector has no valid contents")
 
         # properties is a dictionary of property name to propertyvector this device owns
         # This method updates a property vector and sets it into properties
         properties = device.data
 
         # does this vector already exist
         if self.vectorname in properties:
@@ -229,15 +231,19 @@
         for member in root:
             if member.tag == "defText":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
-                self.data[membername] = member.text
+                if not member.text:
+                    value = ""
+                else:
+                    value = member.text.strip()
+                self.data[membername] = value
             else:
                 raise ParseException
         if not self.data:
             raise ParseException
 
         # properties is a dictionary of property name to propertyvector this device owns
         # This method updates a property vector and sets it into properties
@@ -298,14 +304,16 @@
                 membermax = member.get("max")
                 if not membermax:
                     raise ParseException
                 memberstep = member.get("step")
                 if not memberstep:
                     raise ParseException
                 self.memberlabels[membername] = (label, memberformat, membermin, membermax, memberstep)
+                if not member.text:
+                    raise ParseException
                 self.data[membername] = member.text.strip()
             else:
                 raise ParseException
         if not self.data:
             raise ParseException
 
 
@@ -340,14 +348,16 @@
         for member in root:
             if member.tag == "defLight":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
+                if not member.text:
+                    raise ParseException
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
                     raise ParseException
                 self.data[membername] = value
             else:
                 raise ParseException
         if not self.data:
@@ -485,14 +495,16 @@
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneSwitch":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
+                if not member.text:
+                    raise ParseException
                 value = member.text.strip()
                 if value == "On":
                     self.data[membername] = "On"
                 elif value == "Off":
                     self.data[membername] = "Off"
                 else:
                     raise ParseException
@@ -520,15 +532,19 @@
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneText":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
-                self.data[membername] = member.text
+                if not member.text:
+                    value = ""
+                else:
+                    value = member.text.strip()
+                self.data[membername] = value
             else:
                 raise ParseException
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
@@ -550,14 +566,16 @@
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneNumber":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
+                if not member.text:
+                    raise ParseException
                 self.data[membername] = member.text.strip()
             else:
                 raise ParseException
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
@@ -571,14 +589,16 @@
         setVector.__init__(self, root, device, client)
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneLight":
                 membername = member.get("name")
                 if not membername:
                     raise ParseException
+                if not member.text:
+                    raise ParseException
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
                     raise ParseException
                 self.data[membername] = value
             else:
                 raise ParseException
         properties = device.data
@@ -613,14 +633,16 @@
                     raise ParseException
                 membersize = member.get("size")
                 if not membersize:
                     raise ParseException
                 memberformat = member.get("format")
                 if not memberformat:
                     raise ParseException
+                if not member.text:
+                    raise ParseException
                 try:
                     self.data[membername] = standard_b64decode(member.text.encode('ascii'))
                     memberize = int(membersize)
                 except:
                     raise ParseException
                 self.sizeformat[membername] = (membersize, memberformat)
             else:
```

### Comparing `indipyclient-0.0.1/indipyclient/ipyclient.py` & `indipyclient-0.0.2/indipyclient/ipyclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,24 @@
         yield b"</oneBLOB>"
     yield b"</newBLOBVector>\n"
 
 
 
 class IPyClient(collections.UserDict):
 
+    """This class can be used to create your own scripts or client, and provides
+       a connection to an INDI service, with parsing of the XML protocol.
+       You should create your own class, inheriting from this, and overriding the
+       rxevent method.  Use asyncio.run() to run the asyncrun() method and a call
+       will be made to the given indihost and indiport.
+       The argument clientdata provides any named arguments you may wish to pass
+       into the object when instantiating it.
+       The IPyClient object is also a mapping of devicename to device object, populated
+       as devices and their vectors are learned from the INDI protocol."""
+
 
     def __init__(self, indihost="localhost", indiport=7624, **clientdata):
         "An instance of this is a mapping of devicename to device object"
 
         self.indihost = indihost
         self.indiport = indiport
 
@@ -131,73 +141,100 @@
 
         # and shutdown routine sets this to True to stop coroutines
         self._stop = False
         # this is set to True when asyncrun is finished
         self.stopped = False
 
         # logging level and filepointer to logfile
-        # level, None for no logging, 1 for parsed vector tags only,
-        #                             2 for parsed vectors and members (apart from BLOB's)
-        #                             3 for raw unparsed data
-        self.level = None
-        self.logfile = None
-        self.logfp = None
+        # level, None for no logging, 1 for informtion and errors only,
+        #                             2 for transmitted/received vector tags only,
+        #                             3 for transmitted/received vectors, members and contents (apart from BLOB's)
+        #                             4 for all transmitted/received data
+        self._level = None
+        self._logfile = None
+        self._logfp = None
+
+    @property
+    def level(self):
+        "Can be read, but only set via setlogging method"
+        return self._level
+
+    @property
+    def logfile(self):
+        "Can be read, but only set via setlogging method"
+        return self._logfile
+
+    @property
+    def logfp(self):
+        "Can be read, but only set via setlogging method"
+        return self._logfp
 
     def setlogging(self, level, logfile):
-        "Sets the logging level and logfile, returns the level, which will be None on failure"
+        """Sets the logging level and logfile, returns the level, which will be None on failure.
+           As default, the level is None, indicating no logging. Apart from None, level should
+           be an integer, one of 1, 2, 3 or 4"""
         try:
-            if level is None:
-                self.level = None
-                if self.logfp:
-                    self.logfp.close()
-                self.logfp = None
-                self.logfile = None
-                return None
-            if level in (1, 2, 3):
-                self.level = level
+            if self._logfp:
+                self._logfp.close()
+                self._logfp = None
+
+            if level in (1, 2, 3, 4):
+                self._level = level
             else:
-                self.level = None
-                if self.logfp:
-                    self.logfp.close()
-                self.logfp = None
-                self.logfile = None
+                self._level = None
+                self._logfile = None
                 return None
+
             logfile = pathlib.Path(logfile).expanduser().resolve()
-            self.logfp = open(logfile, "wb")
-            if not self.logfp.writable():
-                self.logfp.close()
-                self.level = None
-                self.logfp = None
-                self.logfile = None
+            self._logfp = open(logfile, "wb")
+            if not self._logfp.writable():
+                self._logfp.close()
+                self._level = None
+                self._logfp = None
+                self._logfile = None
                 return None
         except:
-            self.level = None
-            if self.logfp:
-                self.logfp.close()
-            self.logfp = None
-            self.logfile = None
+            self._level = None
+            if self._logfp:
+                self._logfp.close()
+            self._logfp = None
+            self._logfile = None
             return None
-        self.logfile = logfile
-        return self.level
+        self._logfile = logfile
+        return self._level
 
     def shutdown(self):
         "Shuts down the client"
-        if self.logfp:
-            self.logfp.close()
-            self.level = None
-            self.logfp = None
-            self.logfile = None
+        if self._logfp:
+            self._logfp.close()
+            self._level = None
+            self._logfp = None
+            self._logfile = None
         self._stop = True
 
     async def report(self, message):
-        timestamp = datetime.now(tz=timezone.utc)
-        timestamp = timestamp.replace(tzinfo=None)
-        root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
-        event = events.Message(root, None, self)
-        await self.rxevent(event)
+        """This injects a message into the received data, which will be
+           picked up by the rxevent method. It is a way to set a message
+           on to your client display, in the same way messages come from
+           the INDI service. If logging is enabled the message will be
+           written to the logfile"""
+        try:
+            timestamp = datetime.now(tz=timezone.utc)
+            timestamp = timestamp.replace(tzinfo=None)
+            if self._level:
+                reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}" 
+                self._logfp.write(reportmessage.encode())
+            root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
+            event = events.Message(root, None, self)
+            await self.rxevent(event)
+        except Exception as e:
+            if self._level:
+                bytex = "".join(traceback.format_exception(e)).encode()
+                self._logfp.write(bytex)
+
 
     def enabledlen(self):
         "Returns the number of enabled devices"
         return sum(map(lambda x:1 if x.enable else 0, self.data.values()))
 
 
     def __setitem__(self, device):
@@ -238,14 +275,18 @@
                 # that self._stop has not been set
                 count = 0
                 while not self._stop:
                     await asyncio.sleep(0.5)
                     count += 1
                     if count >= 10:
                         break
+        except Exception as e:
+            if self._level:
+                bytex = "".join(traceback.format_exception(e)).encode()
+                self._logfp.write(bytex)
         finally:
             self.shutdown()
 
 
     def _clear_connection(self):
         "On a connection closing down, clears queues"
         self.connected = False
@@ -262,15 +303,16 @@
                     self.readerque.task_done()
                 except asyncio.QueueEmpty:
                     break
 
 
 
     def send(self, xmldata):
-        "Transmits xmldata, this is an internal method, not normally called by a user."
+        """Transmits xmldata, this is an internal method, not normally called by a user.
+           xmldata is an xml.etree.ElementTree object"""
         if self.connected:
             self.writerque.append(xmldata)
 
     async def _check_alive(self, writer):
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
@@ -292,39 +334,39 @@
             self.shutdown()
         finally:
             self.connected = False
 
 
     def _logtx(self, txdata):
         "log data to file"
-        self.logfp.write(b"\nTX:: ")
-        if self.level == 1:
+        if (not self._level) or (self._level == 1):
+            return
+        self._logfp.write(b"\nTX:: ")
+        if self._level == 2:
             for element in txdata:
                 txdata.remove(element)
             txdata.text = ""
-            binarydata = ET.tostring(txdata, short_empty_elements=False)
-            self.logfp.write(binarydata)
-        if self.level == 2:
+            binarydata = ET.tostring(txdata, short_empty_elements=False).split(b">")
+            self._logfp.write(binarydata[0]+b">")
+        if self._level == 3:
             tag = txdata.tag
             for element in txdata:
                 if tag  == "newBLOBVector":
                     element.text = "NOT LOGGED"
             binarydata = ET.tostring(txdata)
-            self.logfp.write(binarydata)
-        if self.level == 3:
+            self._logfp.write(binarydata)
+        if self._level == 4:
             if txdata.tag == "newBLOBVector" and len(txdata):
                 # txdata is a newBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
-                    self.logfp.write(binarydata)
+                    self._logfp.write(binarydata)
             else:
                 binarydata = ET.tostring(txdata)
-                self.logfp.write(binarydata)
-
-
+                self._logfp.write(binarydata)
 
 
     async def _run_tx(self, writer):
         "Monitors self.writerque and if it has data, uses writer to send it"
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
@@ -349,39 +391,41 @@
 
                 # data has been transmitted set timers going, do not set timer
                 # for enableBLOB as no answer is expected for that
                 if (self.tx_timer is None) and (txdata.tag != "enableBLOB"):
                     self.tx_timer = time.time()
                 self.idle_timer = time.time()
 
-                if self.level:
+                if self._level:
                     self._logtx(txdata)
         except KeyboardInterrupt:
             self.shutdown()
 
     def _logrx(self, rxdata):
         "log data to file"
+        if (not self._level) or (self._level == 1):
+            return
         data = copy.deepcopy(rxdata)
-        self.logfp.write(b"\nRX:: ")
-        if self.level == 1:
+        self._logfp.write(b"\nRX:: ")
+        if self._level == 2:
             for element in data:
                 data.remove(element)
             data.text = ""
-            binarydata = ET.tostring(data, short_empty_elements=False)
-            self.logfp.write(binarydata)
-        if self.level == 2:
+            binarydata = ET.tostring(data, short_empty_elements=False).split(b">")
+            self._logfp.write(binarydata[0]+b">")
+        if self._level == 3:
             tag = data.tag
             for element in data:
                 if tag  == "newBLOBVector":
                     element.text = "NOT LOGGED"
             binarydata = ET.tostring(data)
-            self.logfp.write(binarydata)
-        if self.level == 3:
+            self._logfp.write(binarydata)
+        if self._level == 4:
             binarydata = ET.tostring(data)
-            self.logfp.write(binarydata)
+            self._logfp.write(binarydata)
 
 
     async def _run_rx(self, reader):
         "pass xml.etree.ElementTree data to readerque"
         try:
             source = self._datasource(reader)
             while self.connected and (not self._stop):
@@ -393,25 +437,25 @@
                     # and place rxdata into readerque
                     try:
                         self.readerque.put_nowait(rxdata)
                     except asyncio.QueueFull:
                         # The queue is full, something may be wrong
                         # discard this data and continue
                         pass
-                if self.level:
+                if self._level:
                     self._logrx(rxdata)
         except RuntimeError:
             # catches StopAsyncIteration and stops this coroutine
             pass
         except KeyboardInterrupt:
             self.shutdown()
 
 
     async def _datasource(self, reader):
-        # get received data, parse it, and yield it as xml.etree.ElementTree object
+        "get received data, parse it, and yield it as xml.etree.ElementTree object"
         data_in = self._datainput(reader)
         message = b''
         messagetagnumber = None
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
                 # get blocks of data from _datainput
@@ -508,15 +552,14 @@
         except KeyboardInterrupt:
             self.shutdown()
         except asyncio.CancelledError:
             self.shutdown()
             raise
 
 
-
     async def _rxhandler(self):
         """Populates the events using data from self.readerque"""
         try:
             while not self._stop:
                 # get block of data from the self.readerque
                 await asyncio.sleep(0)
                 try:
@@ -553,34 +596,47 @@
                     await self.report(f"Error: {pe}")
                     continue
                 finally:
                     self.readerque.task_done()
                 # and to get here, continue has not been called
                 # and an event has been created, call the user event handling function
                 await self.rxevent(event)
+        except asyncio.CancelledError:
+            raise
+        except Exception as e:
+            if self._level:
+                bytex = "".join(traceback.format_exception(e)).encode()
+                self._logfp.write(bytex)
         finally:
             self.shutdown()
 
 
     def snapshot(self):
-        "Take snapshot of the devices"
+        """Take a snapshot of the devices and returns a dictionary of device
+           names to objects which are copies of the current state of devices and
+           vectors.
+           These copies will not be updated. This is provided so that you can
+           handle the device data in another thread, without fear of their
+           values changing."""
         with threading.Lock():
             # other threads cannot change the client.data dictionary
+            # while the snapshot is being taken
             snap = {}
             if self.data:
                 for devicename, device in self.data.items():
                     snap[devicename] = device._snapshot()
         # other threads can now access client.data
         # return the snapshot
         return snap
 
 
     def send_newVector(self, devicename, vectorname, timestamp=None, members={}):
-        """Send a new Vector, note members is a membername to value dictionary,
-           It could also be a vector, which is itself a membername to value mapping"""
+        """Send a Vector with updated member values, members is a membername
+           to value dictionary. It could also be a vector, which is itself a
+           membername to value mapping"""
         if devicename not in self.data:
             return
         device = self.data[devicename]
         if vectorname not in device:
             return
         try:
             propertyvector = device[vectorname]
@@ -592,14 +648,23 @@
                 propertyvector.send_newNumberVector(timestamp, members)
             elif propertyvector.vectortype == "BLOBVector":
                 propertyvector.send_newBLOBVector(timestamp, members)
         except KeyboardInterrupt:
             self.shutdown()
 
     def set_vector_timeouts(self, timeout_enable=None, timeout_min=None, timeout_max=None):
+        """Whenever you send updated values, a timer is started and if a timeout occurs
+           before the server responds with a new vector setting, a VectorTimeOut event
+           will be created, which you could choose to ignore, or take action such as
+           setting a vector Alert flag.
+           The protocol allows the server to set a timeout for each vector, this method
+           allows you to set minimum and maximum timeouts, which should be given as integer
+           values. If any parameter is not provided (left at None) then that value will not be
+           changed. If timeout_enable is set to False, no VectorTimeOut events will occur.
+           As default, timeouts are enabled, minimum is set to 2 seconds, maximum 10 seconds."""
         if not timeout_enable is None:
             self.vector_timeout_enable = timeout_enable
         if not timeout_min is None:
             self.vector_timeout_min = timeout_min
         if not timeout_max is None:
             self.vector_timeout_max = timeout_max
 
@@ -638,79 +703,85 @@
                         # then send a getProperties, every five seconds, when count is zero
                         if not count:
                             self.send_getProperties()
                             await self.report("getProperties sent")
                         count += 1
                         if count >= 10:
                             count = 0
-        except KeyboardInterrupt:
-            self.shutdown()
         except asyncio.CancelledError:
+             raise
+        except Exception as e:
+            if self._level:
+                bytex = "".join(traceback.format_exception(e)).encode()
+                self._logfp.write(bytex)
+        finally:
             self.shutdown()
-            raise
 
 
 
     def send_getProperties(self, devicename=None, vectorname=None):
-        """Sends a getProperties request."""
+        """Sends a getProperties request. On startup the IPyClient object
+           will automatically send getProperties, so typically you will
+           not have to use this method."""
         if self.connected:
             xmldata = ET.Element('getProperties')
             xmldata.set("version", "1.7")
             if not devicename:
                 self.send(xmldata)
                 return
             xmldata.set("device", devicename)
             if vectorname:
                 xmldata.set("name", vectorname)
             self.send(xmldata)
 
     def send_enableBLOB(self, value, devicename, vectorname=None):
-        """Sends an enableBLOB instruction."""
+        """Sends an enableBLOB instruction. The value should be one of "Never", "Also", "Only"."""
         if self.connected:
             if value not in ("Never", "Also", "Only"):
                 return
             xmldata = ET.Element('enableBLOB')
             if not devicename:
                 # a devicename is required
                 return
             xmldata.set("device", devicename)
             if vectorname:
                 xmldata.set("name", vectorname)
             xmldata.text = value
             self.send(xmldata)
 
     async def rxevent(self, event):
-        """Override this if this client is operating a script to act on received data.
+        """Override this.
            On receiving data, this is called, and should handle any necessary actions.
            event is an object with attributes according to the data received."""
         pass
 
 
     async def asyncrun(self):
-        """Gathers tasks to be run simultaneously"""
+        """Runs this object to start communications."""
         self._stop = False
         await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor(), return_exceptions=True)
         self.stopped = True
 
 
 class Device(collections.UserDict):
 
+    "Each device is a mapping of vector name to vector object."
+
     def __init__(self, devicename):
         super().__init__()
 
         # This device name
         self.devicename = devicename
 
         # this is a dictionary of property name to propertyvector this device owns
         self.data = {}
 
     @property
     def enable(self):
         "Returns True if any vector of this device has enable True, otherwise False"
-        ebl = False
         for vector in self.data.values():
             if vector.enable:
                 return True
         return False
 
 
 class _Device(Device):
@@ -733,15 +804,15 @@
         raise KeyError
 
 
     def rxvector(self, root):
         """Handle received data, sets new propertyvector into self.data,
            or updates existing property vector and returns an event"""
         if root.tag == "delProperty":
-            return events.delProperty(root, self._client)
+            return events.delProperty(root, self, self._client)
         elif root.tag == "message":
             return events.Message(root, self, self._client)
         elif root.tag == "defSwitchVector":
             return events.defSwitchVector(root, self, self._client)
         elif root.tag == "setSwitchVector":
             return events.setSwitchVector(root, self, self._client)
         elif root.tag == "defLightVector":
@@ -757,15 +828,15 @@
         elif root.tag == "setNumberVector":
             return events.setNumberVector(root, self, self._client)
         elif root.tag == "defBLOBVector":
             return events.defBLOBVector(root, self, self._client)
         elif root.tag == "setBLOBVector":
             return events.setBLOBVector(root, self, self._client)
         else:
-            raise ParseException
+            raise ParseException("Unrecognised tag received")
 
     def _snapshot(self):
         snapdevice = Device(self.devicename)
         for vectorname, vector in self.data:
             snapdevice[vectorname] = vector._snapshot()
         snapdevice.messages = list(self.messages)
         return snapdevice
```

### Comparing `indipyclient-0.0.1/indipyclient/propertymembers.py` & `indipyclient-0.0.2/indipyclient/propertymembers.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,38 +28,38 @@
 
 class PropertyMember(Member):
     "Parent class of SwitchMember etc"
 
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
         if value not in allowed:
-            raise ParseException(f"Invalid value:{value}")
+            raise ParseException(f"Error: Invalid value:{value}")
         return value
 
     def _snapshot(self):
         snapmember = Member(self.name, self.label, self._membervalue)
         return snapmember
 
 
 class SwitchMember(PropertyMember):
     """A SwitchMember can only have one of 'On' or 'Off' values"""
 
     def __init__(self, name, label=None, membervalue="Off"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('On', 'Off'):
-            raise ParseException(f"Invalid switch value {membervalue}, should be either On or Off")
+            raise ParseException(f"Error: Invalid value {membervalue}, should be On or Off")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("No value given, should be either On or Off")
+            raise ParseException("Error: No value given, should be On or Off")
         newvalue = self.checkvalue(value, ['On', 'Off'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
     def oneswitch(self, newvalue):
         """Returns xml of a oneSwitch with the new value to send"""
         xmldata = ET.Element('oneSwitch')
@@ -70,45 +70,45 @@
 
 class LightMember(PropertyMember):
     """A LightMember can only have one of 'Idle', 'Ok', 'Busy' or 'Alert' values"""
 
     def __init__(self, name, label=None, membervalue="Idle"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('Idle','Ok','Busy','Alert'):
-            raise ParseException(f"Invalid light value {membervalue}, should be one of 'Idle','Ok','Busy','Alert'")
+            raise ParseException(f"Error: Invalid light value {membervalue}")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("No value given, should be one of 'Idle','Ok','Busy','Alert'")
+            raise ParseException("Error: No light value given")
         newvalue = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
 
 class TextMember(PropertyMember):
     """Contains a text string"""
 
     def __init__(self, name, label=None, membervalue=""):
         super().__init__(name, label, membervalue)
         if not isinstance(membervalue, str):
-            raise ParseException("The text value must be given as a string")
+            raise ParseException("Error: The text value should be a string")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not isinstance(value, str):
-            raise ParseException("The text value must be given as a string")
+            raise ParseException("Error: The text value should be a string")
         if self._membervalue != value:
             self._membervalue = value
 
     def onetext(self, newvalue):
         """Returns xml of a oneText"""
         xmldata = ET.Element('oneText')
         xmldata.set("name", self.name)
@@ -174,15 +174,15 @@
                 except ValueError:
                     num = float(part)
                 number_list.append(num)
             floatvalue = number_list[0] + (number_list[1]/60) + (number_list[2]/360)
             if negative:
                 floatvalue = -1 * floatvalue
         except:
-            raise TypeError("Unable to parse the value")
+            raise TypeError("Error: Unable to parse number value")
         return floatvalue
 
 
     def getformattedvalue(self):
         """This method returns this members value as a float."""
         return self.getformattedstring(self._membervalue)
 
@@ -266,35 +266,35 @@
        controls how numbers are placed in the xml protocol.
     """
 
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, format, min, max, step, membervalue)
         self.format = format
         if not isinstance(min, str):
-            raise ParseException("minimum value must be given as a string")
+            raise ParseException("Error: minimum value must be given as a string")
         self.min = min
         if not isinstance(max, str):
-            raise ParseException("maximum value must be given as a string")
+            raise ParseException("Error: maximum value must be given as a string")
         self.max = max
         if not isinstance(step, str):
-            raise ParseException("step value must be given as a string")
+            raise ParseException("Error: step value must be given as a string")
         self.step = step
         if not isinstance(membervalue, str):
-            raise ParseException("number value must be given as a string")
+            raise ParseException("Error: number value must be given as a string")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not isinstance(value, str):
-            raise ParseException("number value must be given as a string")
+            raise ParseException("Error: number value must be given as a string")
         if not value:
-            raise ParseException("No number value given")
+            raise ParseException("Error: no number value given")
         if self._membervalue != value:
             self._membervalue = value
 
 
     def onenumber(self, newvalue):
         """Returns xml of a oneNumber"""
         xmldata = ET.Element('oneNumber')
@@ -323,27 +323,27 @@
 
        The BLOB format should be a string describing the BLOB, such as .jpeg
     """
 
     def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=None):
         super().__init__(name, label, membervalue)
         if not isinstance(blobsize, int):
-            raise ParseException("blobsize must be given as an integer")
+            raise ParseException("Error: blobsize must be given as an integer")
         # membervalue can be a byte string, path, string path or file like object
         self.blobsize = blobsize
         self.blobformat = blobformat
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not value:
-            raise ParseException("No BLOB value given")
+            raise ParseException("Error: No BLOB value given")
         self._membervalue = value
 
 
     def oneblob(self, newvalue, newsize, newformat):
         """Returns xml of a oneBLOB"""
         xmldata = ET.Element('oneBLOB')
         xmldata.set("name", self.name)
@@ -352,35 +352,35 @@
         # the value set in the xmldata object should be a bytes object
         if isinstance(newvalue, bytes):
             xmldata.text = newvalue
         elif isinstance(newvalue, pathlib.Path):
             try:
                 xmldata.text = newvalue.read_bytes()
             except:
-                raise ParseException("Unable to read the given file")
+                raise ParseException("Error: Unable to read the given file")
         elif hasattr(newvalue, "seek") and hasattr(newvalue, "read") and callable(newvalue.read):
             # a file-like object
             # set seek(0) so is read from start of file
             newvalue.seek(0)
             bytescontent = newvalue.read()
             newvalue.close()
             if not isinstance(bytescontent, bytes):
-                raise ParseException("The read BLOB is not a bytes object")
+                raise ParseException("Error: The read BLOB is not a bytes object")
             if bytescontent == b"":
-                raise ParseException("The read BLOB value is empty")
+                raise ParseException("Error: The read BLOB value is empty")
             xmldata.text = bytescontent
         else:
             # could be a path to a file
             try:
                 with open(newvalue, "rb") as fp:
                     bytescontent = fp.read()
             except:
-                raise ParseException("Unable to read the given file")
+                raise ParseException("Error: Unable to read the given file")
             if bytescontent == b"":
-                raise ParseException("The read BLOB value is empty")
+                raise ParseException("Error: The read BLOB value is empty")
             xmldata.text = bytescontent
         return xmldata
 
 
     def _snapshot(self):
         snapmember = ParentBLOBMember(self.name, self.label, self.blobsize, self.blobformat, self._membervalue)
         return snapmember
```

### Comparing `indipyclient-0.0.1/indipyclient/propertyvectors.py` & `indipyclient-0.0.2/indipyclient/propertyvectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             self._timer = False
             return True
         return False
 
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
         if value not in allowed:
-            raise ParseException
+            raise ParseException(f"Invalid value:{value}")
         return value
 
     @property
     def state(self):
         return self._state
 
     @state.setter
```

### Comparing `indipyclient-0.0.1/pyproject.toml` & `indipyclient-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.1"
+version = "0.0.2"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.1/PKG-INFO` & `indipyclient-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Project-URL: Documentation, https://indipyclient.readthedocs.io
 Project-URL: Source, https://github.com/bernie-skipole/indipyclient
 
 # indipyclient
-INDI terminal client to communicate to an indi service.
+Terminal client to communicate to an INDI service.
+
+NOTE: CURRENTLY STILL UNDER DEVELOPMENT
 
 This is a pure python package, with no dependencies, providing an INDI client terminal
 
 It also provides a set of classes which can be used to create an INDI client. Either a script, or a GUI implementation could use this to generate the INDI protocol XML, and to create the connection to a port serving INDI drivers.
 
-The client can be called with python3 -m indipyclent.
+The client can be run with
+
+indipyclient [options]
+
+or with
+
+python3 -m indipyclient [options]
+
+The package help is:
 
-    usage: python3 -m indipyclient [options]
+    usage: indipyclient [options]
 
-    INDI terminal client communicating to indi service.
+    Terminal client to communicate to an INDI service.
 
     options:
       -h, --help            show this help message and exit
-      -p PORT, --port PORT  Port of the indi server (default 7624).
-      --host HOST           Hostname/IP of the indi server (default localhost).
+      -p PORT, --port PORT  Port of the INDI server (default 7624).
+      --host HOST           Hostname/IP of the INDI server (default localhost).
       -b BLOBS, --blobs BLOBS
                             Optional folder where BLOB's will be saved.
-      --loglevel LOGLEVEL   Enables logging, value 1, 2 or 3.
+      --loglevel LOGLEVEL   Enables logging, value 1, 2, 3 or 4.
       --logfile LOGFILE     File where logs will be saved
       --version             show program's version number and exit
 
-    The BLOB's folder can also be set from within the session.
-    Setting loglevel and logfile should only be used for brief
-    diagnostic purposes, the logfile could grow very big.
-    loglevel:1 log vector tags without members or contents,
-    loglevel:2 log vectors and members - but not BLOB contents,
-    loglevel:3 log vectors and all contents
+    The BLOB's folder can also be set from within the session. Setting loglevel
+    and logfile should only be used for brief diagnostic purposes, the logfile
+    could grow very big.
+    loglevel:1 Information and error messages only,
+    loglevel:2 log vector tags without members or contents,
+    loglevel:3 log vectors and members - but not BLOB contents,
+    loglevel:4 log vectors and all contents
 
 A typical sesssion would look like:
 
 ![Terminal screenshot](https://github.com/bernie-skipole/indipyclient/raw/main/image.png)
 
 
 This is a companion package to 'indipydriver' which can be used to create INDI drivers.
@@ -60,7 +71,15 @@
 
 INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 Further documentation is available at:
 
 https://indipyclient.readthedocs.io
 
+If you are only using the terminal client, I recommend pipx, so to install you would use:
+
+pipx install indipyclient
+
+or if you want to run it, without installing:
+
+pipx run indipyclient
+
```

