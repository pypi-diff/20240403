# Comparing `tmp/qbee_gpio-3.0.1.tar.gz` & `tmp/qbee_gpio-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbee_gpio-3.0.1.tar", max compression
+gzip compressed data, was "qbee_gpio-3.0.2.tar", max compression
```

## Comparing `qbee_gpio-3.0.1.tar` & `qbee_gpio-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-04-02 12:48:22.201498 qbee_gpio-3.0.1/LICENSE
--rw-r--r--   0        0        0     1778 2024-04-02 12:48:22.201498 qbee_gpio-3.0.1/README.md
--rw-r--r--   0        0        0     1142 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      398 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/__init__.py
--rw-r--r--   0        0        0     2604 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/config.py
--rw-r--r--   0        0        0      181 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/gpio/__init__.py
--rw-r--r--   0        0        0     8335 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/gpio/lcd_display.py
--rw-r--r--   0        0        0      377 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/gpio/setup.py
--rw-r--r--   0        0        0      318 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/gpio/switch.py
--rw-r--r--   0        0        0      401 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/gpio/types.py
--rw-r--r--   0        0        0      192 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/__init__.py
--rw-r--r--   0        0        0      376 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/interface.py
--rw-r--r--   0        0        0     1674 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/librespot.py
--rw-r--r--   0        0        0      360 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/model.py
--rw-r--r--   0        0        0     2200 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/pipe_reader.py
--rw-r--r--   0        0        0     1894 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/metadata/shairport.py
--rw-r--r--   0        0        0     5959 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/orchestrator.py
--rw-r--r--   0        0        0        0 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/py.typed
--rw-r--r--   0        0        0      760 2024-04-02 12:48:22.205498 qbee_gpio-3.0.1/qbee_gpio/sound_poller.py
--rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 qbee_gpio-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-03 19:40:08.342552 qbee_gpio-3.0.2/LICENSE
+-rw-r--r--   0        0        0     1778 2024-04-03 19:40:08.342552 qbee_gpio-3.0.2/README.md
+-rw-r--r--   0        0        0     1142 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      398 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/__init__.py
+-rw-r--r--   0        0        0     2604 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/config.py
+-rw-r--r--   0        0        0      181 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/gpio/__init__.py
+-rw-r--r--   0        0        0     8353 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/gpio/lcd_display.py
+-rw-r--r--   0        0        0      377 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/gpio/setup.py
+-rw-r--r--   0        0        0      318 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/gpio/switch.py
+-rw-r--r--   0        0        0      401 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/gpio/types.py
+-rw-r--r--   0        0        0      192 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/interface.py
+-rw-r--r--   0        0        0     1674 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/librespot.py
+-rw-r--r--   0        0        0      360 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/model.py
+-rw-r--r--   0        0        0     2200 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/pipe_reader.py
+-rw-r--r--   0        0        0     1894 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/metadata/shairport.py
+-rw-r--r--   0        0        0     6305 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/orchestrator.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/py.typed
+-rw-r--r--   0        0        0      760 2024-04-03 19:40:08.346552 qbee_gpio-3.0.2/qbee_gpio/sound_poller.py
+-rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 qbee_gpio-3.0.2/PKG-INFO
```

### Comparing `qbee_gpio-3.0.1/LICENSE` & `qbee_gpio-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/README.md` & `qbee_gpio-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/pyproject.toml` & `qbee_gpio-3.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qbee-gpio"
-version = "3.0.1"
+version = "3.0.2"
 description = "Control an LCD display and amplifier relay for use in an AirPlay and/or Spotify Connect Raspberry Pi server."
 authors = ["Gabriel Pajot <gab@lescactus.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/qbee-gpio"
 include = ["qbee_gpio/py.typed"]
 
@@ -15,15 +15,15 @@
 concurrent-tasks = ">=1.7,<2"
 zenconfig = { version = ">=2.1.0,<3", extras = ["yaml", "attrs"] }
 
 [tool.poetry.group.test.dependencies]
 pytest = "==8.1.1"
 pytest-asyncio = "==0.23.6"
 pytest-mock = "==3.14.0"
-ruff = "==0.3.4"
+ruff = "==0.3.5"
 mypy = "==1.9.0"
 pre-commit = "==3.5.0"
 
 [tool.poetry.scripts]
 qbee = 'qbee_gpio:run'
 
 [build-system]
```

### Comparing `qbee_gpio-3.0.1/qbee_gpio/config.py` & `qbee_gpio-3.0.2/qbee_gpio/config.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/qbee_gpio/gpio/lcd_display.py` & `qbee_gpio-3.0.2/qbee_gpio/gpio/lcd_display.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import contextlib
 import unicodedata
 from dataclasses import dataclass, field
-from time import monotonic
+from time import monotonic, sleep
 from typing import Callable, Literal, Optional, Sequence, Tuple
 
 try:
     from RPi import GPIO
 except ModuleNotFoundError:
     from qbee_gpio.gpio.types import GPIO
 from qbee_gpio.gpio.types import Bit
@@ -33,15 +33,15 @@
     # Number of characters per line.
     width: int = 16
     # Number of lines.
     lines: Literal[1, 2, 4] = 2
     line_height: Literal[8, 10] = 8
 
     _line_addresses: Tuple[int, ...] = field(init=False)
-    _lock: asyncio.Lock = field(default_factory=asyncio.Lock)
+    _lock: asyncio.Lock = field(default_factory=asyncio.Lock, init=False)
     _init: bool = field(default=False, init=False)  # Has the LCD been initialized.
     _last_cmd_start: float = field(default=0, init=False)
     _last_cmd_wait: float = field(default=0, init=False)
 
     def __post_init__(self):
         # Set up the line addresses (based on width for more than 2 lines).
         self._line_addresses = (0x00, 0x40, 0x00 + self.width, 0x40 + self.width)
@@ -57,27 +57,25 @@
             GPIO.setup(pin, GPIO.OUT)
 
     async def __aenter__(self):
         await self.init()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
-        async with self._lock:
-            self._init = False
+        await self.close()
 
     async def init(self) -> None:
         async with self._lock:
             # Init LCD.
-            GPIO.output(self.pin_register_select, False)
             # No need to wait here as if the PI is booted power is already high enough.
             # Send 3 times the same command to ensure 8-bit mode.
             await self._write(
                 (0, 0, 1, 1),
                 # Wait more than 4.1ms here as per specs.
-                wait_for=0.0045,
+                wait_for=0.005,
             )
             await self._write(
                 (0, 0, 1, 1),
                 # Wait more than 100µs here as per specs.
                 wait_for=0.00011,
             )
             await self._write((0, 0, 1, 1))
@@ -100,56 +98,59 @@
                     1,
                     1,  # Screen on.
                     0,  # Cursor off.
                     0,  # Cursor blink off.
                 ),
             )
             # Clear display.
-            await self._write((0, 0, 0, 0), (0, 0, 0, 1))
+            await self.clear(skip_lock=True)
             # Entry mode set.
             await self._write(
                 (0, 0, 0, 0),
                 (
                     0,
                     1,
                     1,  # Cursor moves right.
-                    0,  # Display does not shit.
+                    0,  # Display does not shift.
                 ),
             )
             self._init = True
 
+    async def close(self) -> None:
+        async with self._lock:
+            if not self._init:
+                return
+            await self.clear(skip_lock=True)
+            self._init = False
+
+    async def clear(self, skip_lock: bool = False) -> None:
+        # Wait for more than 1.52ms.
+        if skip_lock:
+            await self._write((0, 0, 0, 0), (0, 0, 0, 1), wait_for=0.002)
+        else:
+            if not self._init:
+                return
+            async with self._lock:
+                await self._write((0, 0, 0, 0), (0, 0, 0, 1), wait_for=0.002)
+
     async def display(
         self,
         message: str,
         *,
-        # Wrap content to spread on all available lines.
-        wrap: bool = False,
         # This should be a function that takes a string and the width of the display
         # as arguments and return a string whose length is the same as the display.
-        align: Callable[[str, int], str] = str.ljust,
+        align: Callable[[str, int], str] = str.center,
     ) -> None:
         """Display a message on the screen."""
-        if not message.strip():
-            await self._write((0, 0, 0, 0), (0, 0, 0, 1))
-            return
-        lines = message.split("\n")
-        if wrap:
-            wrapped_lines = []
-            for line in lines:
-                # Convert each line in multiple ones based on the display width.
-                wrapped_lines += [
-                    line[i : i + self.width] for i in range(0, len(line), self.width)
-                ]
-            lines = wrapped_lines
         # Only keep lines we can display.
-        lines = lines[: self.lines]
+        lines = message.split("\n")[: self.lines]
         # Add empty lines if needed.
         if len(lines) != self.lines:
             lines += [""] * (self.lines - len(lines))
-        # Remove accents and align each line.
+        # Trim to width, remove accents and align each line.
         lines = [
             align(remove_accents(line[: self.width]), self.width) for line in lines
         ]
         await self._print_lines(lines)
 
     async def _print_lines(self, lines: Sequence[str]) -> None:
         async with self._lock:
@@ -160,57 +161,56 @@
                     *get_bits(0x80 + self._line_addresses[i]),
                 )
                 for char in line:
                     await self._write(*get_bits(ord(char)), is_cmd=False)
 
     async def _write(
         self,
-        *high_and_low_bits: Tuple[Bit, Bit, Bit, Bit],
+        high_bits: Tuple[Bit, Bit, Bit, Bit],
+        low_bits: Optional[Tuple[Bit, Bit, Bit, Bit]] = None,
         is_cmd: bool = True,
         wait_for: Optional[float] = None,
     ) -> None:
         GPIO.output(self.pin_register_select, not is_cmd)
-        for bits in high_and_low_bits:
-            await self._send_4_bits(*bits)
-        self._mark_start(
-            wait_for or 0.00155
-            if high_and_low_bits == ((0, 0, 0, 0), (0, 0, 0, 1))
-            else 0.000045,
-        )
+        self._send_4_bits(*high_bits)
+        # Wait until enough time has passed for the previous command to be taken into account.
+        if (wait := self._last_cmd_wait - (monotonic() - self._last_cmd_start)) > 0:
+            await asyncio.sleep(wait)
+            self._last_cmd_wait = 0
+        self._pulse_enable()
+        if low_bits:
+            self._send_4_bits(*low_bits)
+            self._pulse_enable()
+        if is_cmd:
+            # Mark the start of the command.
+            self._last_cmd_start = monotonic()
+            # Wait for more than 37µs unless otherwise specified.
+            self._last_cmd_wait = wait_for or 0.0001
 
-    async def _send_4_bits(
+    def _send_4_bits(
         self,
         bit3: Bit,
         bit2: Bit,
         bit1: Bit,
         bit0: Bit,
     ) -> None:
         GPIO.output(self.pin_data_4, bit0)
         GPIO.output(self.pin_data_5, bit1)
         GPIO.output(self.pin_data_6, bit2)
         GPIO.output(self.pin_data_7, bit3)
-        await self._wait_ready()
-        await self._enable()
 
-    async def _enable(self) -> None:
+    def _pulse_enable(self) -> None:
+        """Note: this is called often when printing, to avoid too much context switching
+        and slowing down display printing if this is done synchronously.
+        """
         GPIO.output(self.pin_enable, True)
         # Wait more than 450ns.
-        # We need a bit more as we are using 3.3V signal on 5V LCD.
-        await asyncio.sleep(0.000002)
+        sleep(0.000001)
         GPIO.output(self.pin_enable, False)
 
-    async def _wait_ready(self) -> None:
-        """Wait until enough time has passed for the previous command to be taken into account."""
-        if (wait := self._last_cmd_wait - (monotonic() - self._last_cmd_start)) > 0:
-            await asyncio.sleep(wait)
-
-    def _mark_start(self, wait_for: float) -> None:
-        self._last_cmd_start = monotonic()
-        self._last_cmd_wait = wait_for
-
 
 def get_bits(
     byte: int,
 ) -> Tuple[Tuple[Bit, Bit, Bit, Bit], Tuple[Bit, Bit, Bit, Bit]]:
     high_bits = byte >> 4
     return (
         (
@@ -246,14 +246,14 @@
             pin_data_4=int(input("pin data 4: ")),
             pin_data_5=int(input("pin data 5: ")),
             pin_data_6=int(input("pin data 6: ")),
             pin_data_7=int(input("pin data 7: ")),
         )
         async with lcd:
             while True:
-                await lcd.display(input("message: "), align=str.center)
+                await lcd.display(input("message: "))
     finally:
         GPIO.cleanup()
 
 
 if __name__ == "__main__":
     asyncio.run(debug())
```

### Comparing `qbee_gpio-3.0.1/qbee_gpio/metadata/librespot.py` & `qbee_gpio-3.0.2/qbee_gpio/metadata/librespot.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/qbee_gpio/metadata/pipe_reader.py` & `qbee_gpio-3.0.2/qbee_gpio/metadata/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/qbee_gpio/metadata/shairport.py` & `qbee_gpio-3.0.2/qbee_gpio/metadata/shairport.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/qbee_gpio/orchestrator.py` & `qbee_gpio-3.0.2/qbee_gpio/orchestrator.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,28 +83,29 @@
         if self._cfg.lcd.enable and self._cfg.lcd.librespot_metadata_path:
             self._poll_now_playing_tasks.append(
                 BackgroundTask(
                     self._poll_now_playing,
                     LibrespotNowPlayingPoller(self._cfg.lcd.librespot_metadata_path),
                 )
             )
-        self._last_message = self._cfg.lcd.startup_message
+        self._now_playing = self._cfg.lcd.startup_message
         self._stop_event = asyncio.Event()
 
     async def __aenter__(self):
-        self._switch(False)
-        self.callback(self._switch, False)
+        await self._switch(False)
+        self.push_async_callback(self._switch, False)
+        # Init this initially to make sure the display is clean.
+        if self._lcd:
+            await self._lcd.init()
         if self._standby_task:
             self.enter_context(self._standby_task)
-        if self._poll_sound_task:
-            self.enter_context(self._poll_sound_task)
-        if self._lcd:
-            await self.enter_async_context(self._lcd)
         for task in self._poll_now_playing_tasks:
             self.enter_context(task)
+        if self._poll_sound_task:
+            self.enter_context(self._poll_sound_task)
         return self
 
     async def run(self) -> None:
         logger.debug("starting orchestrator...")
         async with LoopExceptionHandler(stop_func=self._stop):
             async with self:
                 logger.info("started orchestrator")
@@ -120,46 +121,53 @@
     async def _poll_sound(self) -> None:
         assert self._sound_poller
         assert self._standby_task
         async for output in self._sound_poller.poll():
             if output:
                 logger.debug("cancelling standby mode")
                 self._standby_task.cancel()
-                self._switch(True)
-                await self._print(self._last_message)
+                await self._switch(True)
+                await self._display_now_playing()
             else:
-                await self._print("")  # Clear the display.
+                if self._lcd:
+                    await self._lcd.clear()
                 self._standby_task.create()
 
     async def _standby(self) -> None:
         assert self._cfg.sound_detection
         if self._cfg.sound_detection.standby_duration is not None:
             logger.debug("entering standby mode")
             await asyncio.sleep(self._cfg.sound_detection.standby_duration)
             logger.debug("exiting standby mode")
-            self._switch(False)
+            await self._switch(False)
         if self._cfg.sound_detection.shutdown_command:
             logger.info("shutting down system...")
             await asyncio.create_subprocess_shell(
                 self._cfg.sound_detection.shutdown_command,
             )
 
     # LCD.
 
     async def _poll_now_playing(self, poller: NowPlayingPoller) -> None:
         async for event in poller.poll():
-            self._last_message = event.display(self._cfg.lcd.lines)
-            await self._print(self._last_message)
+            self._now_playing = event.display(self._cfg.lcd.lines)
+            await self._display_now_playing()
 
-    async def _print(self, message: str) -> None:
+    async def _display_now_playing(self) -> None:
         if not self._lcd:
             return
-        await self._lcd.display(message, align=str.center)
+        await self._lcd.display(self._now_playing)
 
     # Switches.
 
-    def _switch(self, value: bool) -> None:
-        if not self._standby_switch or not self._on_switch:
-            return
-        logger.debug("turning %s", "on" if value else "off")
-        self._on_switch(value)
-        self._standby_switch(not value)
+    async def _switch(self, value: bool) -> None:
+        if self._standby_switch and self._on_switch:
+            logger.debug("turning %s", "on" if value else "off")
+            self._on_switch(value)
+            self._standby_switch(not value)
+        # Reinitialize LCD even if it doesn't turn off with the amp as I get
+        # corrupted display when it has been idle for a while...
+        if self._lcd:
+            if value:
+                await self._lcd.init()
+            else:
+                await self._lcd.close()
```

### Comparing `qbee_gpio-3.0.1/qbee_gpio/sound_poller.py` & `qbee_gpio-3.0.2/qbee_gpio/sound_poller.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-3.0.1/PKG-INFO` & `qbee_gpio-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbee-gpio
-Version: 3.0.1
+Version: 3.0.2
 Summary: Control an LCD display and amplifier relay for use in an AirPlay and/or Spotify Connect Raspberry Pi server.
 Home-page: https://github.com/gpajot/qbee-gpio
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@lescactus.eu
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

