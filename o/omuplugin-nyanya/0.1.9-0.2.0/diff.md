# Comparing `tmp/omuplugin_nyanya-0.1.9.tar.gz` & `tmp/omuplugin_nyanya-0.2.0.tar.gz`

## Comparing `omuplugin_nyanya-0.1.9.tar` & `omuplugin_nyanya-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/.python-version
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/src/omuplugin_nyanya/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/src/omuplugin_nyanya/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/README.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/src/omuplugin_nyanya/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/src/omuplugin_nyanya/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.0/PKG-INFO
```

### Comparing `omuplugin_nyanya-0.1.9/src/omuplugin_nyanya/plugin.py` & `omuplugin_nyanya-0.2.0/src/omuplugin_nyanya/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+from omu.identifier import Identifier
 from omuchat import App, Client, content, model
 
+IDENTIFIER = Identifier("cc.omuchat", "plugin-nyanya")
 APP = App(
-    name="plugin-nyanya",
-    group="cc.omuchat",
+    IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
 replaces = {
     "な": "にゃ",
     "ナ": "ニャ",
 }
@@ -18,21 +19,17 @@
     for child in component.iter():
         if not isinstance(child, content.Text):
             continue
         child.text = "".join(replaces.get(char, char) for char in child.text)
     return component
 
 
-@client.messages.proxy
+@client.chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
     if not message.content:
         return message
     message.content = await translate(message.content)
     return message
 
 
-async def main():
-    await client.start()
-
-
 if __name__ == "__main__":
     client.run()
```

