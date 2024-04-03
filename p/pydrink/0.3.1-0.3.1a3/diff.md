# Comparing `tmp/pydrink-0.3.1-py3-none-any.whl.zip` & `tmp/pydrink-0.3.1a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16214 bytes, number of entries: 10
+Zip file size: 16458 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     4169 b- defN 80-Jan-01 00:00 pydrink/config.py
--rw-r--r--  2.0 unx     8918 b- defN 80-Jan-01 00:00 pydrink/drink.py
+-rw-r--r--  2.0 unx     8655 b- defN 80-Jan-01 00:00 pydrink/drink.py
 -rw-r--r--  2.0 unx     8793 b- defN 80-Jan-01 00:00 pydrink/git.py
 -rw-r--r--  2.0 unx      958 b- defN 80-Jan-01 00:00 pydrink/log.py
 -rw-r--r--  2.0 unx     8373 b- defN 80-Jan-01 00:00 pydrink/obj.py
--rw-r--r--  2.0 unx      750 b- defN 80-Jan-01 00:00 pydrink-0.3.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     9343 b- defN 80-Jan-01 00:00 pydrink-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pydrink-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 pydrink-0.3.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      751 b- defN 16-Jan-01 00:00 pydrink-0.3.1.dist-info/RECORD
-10 files, 42186 bytes uncompressed, 14950 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx      750 b- defN 80-Jan-01 00:00 pydrink-0.3.1a3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10125 b- defN 80-Jan-01 00:00 pydrink-0.3.1a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pydrink-0.3.1a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 pydrink-0.3.1a3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      762 b- defN 16-Jan-01 00:00 pydrink-0.3.1a3.dist-info/RECORD
+10 files, 42716 bytes uncompressed, 15174 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pydrink/log.py
 Comment: 
 
 Filename: pydrink/obj.py
 Comment: 
 
-Filename: pydrink-0.3.1.dist-info/LICENSE.txt
+Filename: pydrink-0.3.1a3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pydrink-0.3.1.dist-info/METADATA
+Filename: pydrink-0.3.1a3.dist-info/METADATA
 Comment: 
 
-Filename: pydrink-0.3.1.dist-info/WHEEL
+Filename: pydrink-0.3.1a3.dist-info/WHEEL
 Comment: 
 
-Filename: pydrink-0.3.1.dist-info/entry_points.txt
+Filename: pydrink-0.3.1a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pydrink-0.3.1.dist-info/RECORD
+Filename: pydrink-0.3.1a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydrink/drink.py

```diff
@@ -205,15 +205,14 @@
     parser = createArgumentParser()
     args = parser.parse_args()
     debug(args)
     pydrink.log.DEBUG = args.debug
     pydrink.log.QUIET = args.quiet
     pydrink.log.VERBOSE = args.verbose
     p_name = __package__ or __name__
-    debug(f"p_name: {p_name}")
 
     if args.begin:
         return begin_setup()
 
     try:
         c = Config(find_drinkrc())
     except Exception as e:
@@ -271,21 +270,14 @@
         except InvalidKind:
             err(f"Import failed: {args.kind} is not a valid kind")
             return 2
         except InvalidDrinkObject as e:
             err(f"Import failed: {e}")
             return 2
     if args.readme:
-        if descr := metadata(p_name).get("Description"):
-            print(Markdown(descr))
-            return 0
-        else:
-            err("You need Python >= 3.10 to use this feature.")
-            return 5
-    if args.readme:
         meta = metadata(p_name)
         print(Markdown(meta["Description"]))
         return 0
     if args.version:
         p_version = version(p_name)
         notice(f"{p_name} {p_version}")
         return 0
```

## Comparing `pydrink-0.3.1.dist-info/LICENSE.txt` & `pydrink-0.3.1a3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pydrink-0.3.1.dist-info/METADATA` & `pydrink-0.3.1a3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrink
-Version: 0.3.1
+Version: 0.3.1a3
 Summary: Distributed Reusage of Invaluable Nerd Kit (dotfile management)
 Home-page: https://github.com/sstark/pydrink
 License: ISC
 Author: Sebastian Stark
 Author-email: sstark@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
@@ -17,16 +17,15 @@
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/sstark/pydrink
 Description-Content-Type: text/markdown
 
 pydrink
 =======
 
-Simple, low friction Python implementation of the *drink* dotfile management
-system. Almost no configuration required. Closely integrated with your shell.
+Python implemenation of the *drink* dotfile management system.
 
 This will maintain files in a git repository and create symlinks to them in
 appropriate places in your home directory. You will only need a single
 repository for all your different environments. Drink will only symlink the
 files that are configured for a _target_.
 
 The **interactive git menu** of drink provides a convenient way to manage and
@@ -86,63 +85,37 @@
 dedicated place where it will be linked to in the users home directory.
 
 (The _pydrink_ code is structured such that new kinds could be easily added. For
 example, somebody might want to add a kind for storing bash aliases. Currently
 this needs changes to the code, but with modest effort.)
 
 
-Why Symlinks?
--------------
-
-  - Symlinks make it very easy to see whether a file is managed by drink or
-    not.
-
-  - With symlinks it is extremely simple to check what has changed, because
-    everything just happens within the git repository.
-
-  - Saving space is probably not a point for everyone, since the kind of files
-    we are dealing with here are usually very small, but still it's a point.
-
-
 Interface
 ---------
 
 Screenshot of the `drink --help` output:
 
 ![drink-help](https://github.com/sstark/pydrink/assets/837918/11d8f0fa-4892-4113-b012-3bfb75cca3be)
 
 
-Install
--------
-
-The recommended way is to use pipx:
-
-    pipx install pydrink
-
-pip should also work.
-
-Visit the project page on pypi for all releases: https://pypi.org/project/pydrink/
-
-
 Getting Started
 ----------------
 
 If you have not used drink before, you need to create a configuration file
 and a repository. For both, drink offers you some assistance:
 
      $ drink -b
      New drinkrc created in /home/user/.config/drinkrc.
      Please review or change the contents and run this command again.
 
 Now you can open `drinkrc` and customize it before proceeding. See next chapter
 for details (and then jump back here). Most importantly you will want to make
 at least one of these changes to it before proceeding:
 
-  - Add a **DRINKBASEURL** parameter to it, if you want to use the distribution
-    features of drink.
+  - Add a **DRINKBASEURL** parameter to it.
   - If you have a shared home directory (e. g. NFS) and your drink repository
     is located on it, you likely want to adjust your **TARGET** parameter to
     not use the hostname, but some broader term.
   - Adjust the location where your drink repository will be created. For that,
     change to **DRINKDIR** parameter to point to some (not yet existing)
     directory. This can be relative to your home.
 
@@ -234,14 +207,78 @@
     format = """... $env_var ..."""
     [env_var.drink_prompt_info]
     format = '[$env_value]($style)'
     default = ''
     style = "green"
 
 
+'Destination' vs. 'Target'
+--------------------------
+
+The term 'target' in this project is used for the context in which an object
+should be linked or not. Usually this is a hostname or the word 'global'.
+
+The term 'target' as it is normally used for symlinks, refers to the file or
+directory, a symlink points to. It could be a symlink too, but usually is a
+plain file or directory that is the target of the symbolic link.
+
+To avoid confusion, this project uses the word 'dest' or 'destination' when it
+is referring to what is normally a 'target' in symlink world.
+
+
+Development
+-----------
+
+_pydrink_ tries to use modern Python technology:
+
+  - Dependencies and packaging are managed with **poetry**.
+
+  - Typing hints are used and checked with **mypy**.
+
+  - A **Makefile** (the author could not find a pythonic alternative that is not
+    completely over the top for the task) offers targets for typical
+    development tasks like testing, cleaning, running debugpy.
+
+  - Tests should be provided for all functionalities through **pytest**.
+
+Enter shell inside development environment:
+
+    make shell
+
+Running tests:
+
+    make test
+
+Typecheck:
+
+    make typecheck
+
+Both:
+
+    make
+
+Verbose:
+
+    make VERBOSE=1
+
+Run a debugpy server, suitable for connecting with e. g. nvim-dap:
+
+    make debug OPTS="-s -d"
+
+Bootstrap development environment:
+
+    <distro-specific-tool> install pipx
+    pipx install poetry
+    git clone https://github.com/sstark/pydrink
+    cd pydrink
+    poetry shell
+    poetry update
+    make
+
+
 History
 -------
 
 This is yet another dotfile management system. I wrote this originally in zsh
 (first commit Mar 14 2008) and use it daily since then.
 
 The zsh version was never published because it is too much entangeled with my
```

