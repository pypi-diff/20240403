# Comparing `tmp/mycli-1.8.1.tar.gz` & `tmp/mycli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mycli-1.8.1.tar", last modified: Mon Oct 24 13:45:27 2016, max compression
+gzip compressed data, was "dist/mycli-1.9.0.tar", last modified: Sun Mar 19 01:07:17 2017, max compression
```

## Comparing `mycli-1.8.1.tar` & `mycli-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 amjith     (502) staff       (20)        0 2016-10-24 13:45:27.000000 mycli-1.8.1/
--rw-r--r--   0 amjith     (502) staff       (20)      694 2016-10-24 13:44:16.000000 mycli-1.8.1/AUTHORS
--rw-r--r--   0 amjith     (502) staff       (20)    11404 2016-10-24 13:44:16.000000 mycli-1.8.1/changelog.md
--rw-r--r--   0 amjith     (502) staff       (20)     1798 2015-08-02 01:50:59.000000 mycli-1.8.1/LICENSE.txt
--rw-r--r--   0 amjith     (502) staff       (20)       25 2015-08-02 01:50:59.000000 mycli-1.8.1/MANIFEST.in
-drwxr-xr-x   0 amjith     (502) staff       (20)        0 2016-10-24 13:45:27.000000 mycli-1.8.1/mycli/
--rw-r--r--   0 amjith     (502) staff       (20)       22 2016-10-24 13:45:08.000000 mycli-1.8.1/mycli/__init__.py
--rw-r--r--   0 amjith     (502) staff       (20)     1421 2015-10-16 13:27:27.000000 mycli-1.8.1/mycli/clibuffer.py
--rw-r--r--   0 amjith     (502) staff       (20)      623 2016-05-13 04:06:34.000000 mycli-1.8.1/mycli/clistyle.py
--rw-r--r--   0 amjith     (502) staff       (20)     1231 2016-05-13 04:06:34.000000 mycli-1.8.1/mycli/clitoolbar.py
--rw-r--r--   0 amjith     (502) staff       (20)     4475 2016-03-03 17:35:09.000000 mycli-1.8.1/mycli/completion_refresher.py
--rw-r--r--   0 amjith     (502) staff       (20)     6226 2016-02-26 04:18:37.000000 mycli-1.8.1/mycli/config.py
--rw-r--r--   0 amjith     (502) staff       (20)      574 2015-04-08 06:03:52.000000 mycli-1.8.1/mycli/encodingutils.py
--rw-r--r--   0 amjith     (502) staff       (20)      414 2015-10-16 18:20:20.000000 mycli-1.8.1/mycli/filters.py
--rw-r--r--   0 amjith     (502) staff       (20)     2817 2016-05-13 04:06:34.000000 mycli-1.8.1/mycli/key_bindings.py
--rw-r--r--   0 amjith     (502) staff       (20)      310 2016-03-03 05:48:25.000000 mycli-1.8.1/mycli/lexer.py
--rw-r--r--   0 amjith     (502) staff       (20)     1496 2015-05-19 00:02:42.000000 mycli-1.8.1/mycli/magic.py
--rwxr-xr-x   0 amjith     (502) staff       (20)    39460 2016-09-18 03:58:42.000000 mycli-1.8.1/mycli/main.py
--rw-r--r--   0 amjith     (502) staff       (20)     3264 2016-09-18 03:58:42.000000 mycli-1.8.1/mycli/myclirc
-drwxr-xr-x   0 amjith     (502) staff       (20)        0 2016-10-24 13:45:27.000000 mycli-1.8.1/mycli/packages/
--rw-r--r--   0 amjith     (502) staff       (20)        0 2015-04-08 06:03:52.000000 mycli-1.8.1/mycli/packages/__init__.py
--rw-r--r--   0 amjith     (502) staff       (20)    12150 2016-09-18 04:19:04.000000 mycli-1.8.1/mycli/packages/completion_engine.py
--rw-r--r--   0 amjith     (502) staff       (20)     1522 2015-10-16 13:27:27.000000 mycli-1.8.1/mycli/packages/connection.py
--rw-r--r--   0 amjith     (502) staff       (20)     6315 2015-10-16 13:27:27.000000 mycli-1.8.1/mycli/packages/counter.py
--rw-r--r--   0 amjith     (502) staff       (20)     1466 2015-10-20 10:12:51.000000 mycli-1.8.1/mycli/packages/expanded.py
--rw-r--r--   0 amjith     (502) staff       (20)     4221 2015-10-31 13:54:13.000000 mycli-1.8.1/mycli/packages/ordereddict.py
--rw-r--r--   0 amjith     (502) staff       (20)     7176 2015-10-16 13:27:27.000000 mycli-1.8.1/mycli/packages/parseutils.py
-drwxr-xr-x   0 amjith     (502) staff       (20)        0 2016-10-24 13:45:27.000000 mycli-1.8.1/mycli/packages/special/
--rw-r--r--   0 amjith     (502) staff       (20)      245 2015-06-20 06:17:57.000000 mycli-1.8.1/mycli/packages/special/__init__.py
--rw-r--r--   0 amjith     (502) staff       (20)     4428 2016-03-03 05:48:25.000000 mycli-1.8.1/mycli/packages/special/dbcommands.py
--rw-r--r--   0 amjith     (502) staff       (20)     2112 2015-11-22 18:31:21.000000 mycli-1.8.1/mycli/packages/special/favoritequeries.py
--rw-r--r--   0 amjith     (502) staff       (20)     7200 2016-02-26 04:18:37.000000 mycli-1.8.1/mycli/packages/special/iocommands.py
--rw-r--r--   0 amjith     (502) staff       (20)     3852 2015-07-23 05:32:34.000000 mycli-1.8.1/mycli/packages/special/main.py
--rw-r--r--   0 amjith     (502) staff       (20)     1440 2016-03-03 05:48:25.000000 mycli-1.8.1/mycli/packages/special/utils.py
--rw-r--r--   0 amjith     (502) staff       (20)    38179 2015-12-11 13:26:57.000000 mycli-1.8.1/mycli/packages/tabulate.py
--rw-r--r--   0 amjith     (502) staff       (20)    16909 2016-09-20 16:46:21.000000 mycli-1.8.1/mycli/sqlcompleter.py
--rw-r--r--   0 amjith     (502) staff       (20)     8360 2016-08-20 22:33:40.000000 mycli-1.8.1/mycli/sqlexecute.py
-drwxr-xr-x   0 amjith     (502) staff       (20)        0 2016-10-24 13:45:27.000000 mycli-1.8.1/mycli.egg-info/
--rw-r--r--   0 amjith     (502) staff       (20)        1 2016-10-24 13:45:26.000000 mycli-1.8.1/mycli.egg-info/dependency_links.txt
--rw-r--r--   0 amjith     (502) staff       (20)       72 2016-10-24 13:45:26.000000 mycli-1.8.1/mycli.egg-info/entry_points.txt
--rw-r--r--   0 amjith     (502) staff       (20)       47 2016-05-13 04:15:29.000000 mycli-1.8.1/mycli.egg-info/pbr.json
--rw-r--r--   0 amjith     (502) staff       (20)     1041 2016-10-24 13:45:26.000000 mycli-1.8.1/mycli.egg-info/PKG-INFO
--rw-r--r--   0 amjith     (502) staff       (20)      135 2016-10-24 13:45:26.000000 mycli-1.8.1/mycli.egg-info/requires.txt
--rw-r--r--   0 amjith     (502) staff       (20)     1028 2016-10-24 13:45:27.000000 mycli-1.8.1/mycli.egg-info/SOURCES.txt
--rw-r--r--   0 amjith     (502) staff       (20)        6 2016-10-24 13:45:26.000000 mycli-1.8.1/mycli.egg-info/top_level.txt
--rw-r--r--   0 amjith     (502) staff       (20)     1041 2016-10-24 13:45:27.000000 mycli-1.8.1/PKG-INFO
--rw-r--r--   0 amjith     (502) staff       (20)     6234 2016-10-22 03:54:05.000000 mycli-1.8.1/README.md
--rw-r--r--   0 amjith     (502) staff       (20)       88 2016-10-24 13:45:27.000000 mycli-1.8.1/setup.cfg
--rw-r--r--   0 amjith     (502) staff       (20)     2198 2016-09-20 16:46:21.000000 mycli-1.8.1/setup.py
--rw-r--r--   0 amjith     (502) staff       (20)      484 2015-09-18 04:56:38.000000 mycli-1.8.1/SPONSORS
+drwxr-xr-x   0 troten   (880106680) 2064858183        0 2017-03-19 01:07:17.000000 mycli-1.9.0/
+-rw-r--r--   0 troten   (880106680) 2064858183      821 2017-03-18 23:33:42.000000 mycli-1.9.0/AUTHORS
+-rw-r--r--   0 troten   (880106680) 2064858183    12970 2017-03-18 23:33:42.000000 mycli-1.9.0/changelog.md
+-rw-r--r--   0 troten   (880106680) 2064858183     1798 2015-09-22 21:20:16.000000 mycli-1.9.0/LICENSE.txt
+-rw-r--r--   0 troten   (880106680) 2064858183       25 2015-09-22 21:20:16.000000 mycli-1.9.0/MANIFEST.in
+drwxr-xr-x   0 troten   (880106680) 2064858183        0 2017-03-19 01:07:17.000000 mycli-1.9.0/mycli/
+-rw-r--r--   0 troten   (880106680) 2064858183       22 2017-03-19 01:00:56.000000 mycli-1.9.0/mycli/__init__.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1421 2015-10-10 04:44:13.000000 mycli-1.9.0/mycli/clibuffer.py
+-rw-r--r--   0 troten   (880106680) 2064858183      615 2017-03-11 19:06:00.000000 mycli-1.9.0/mycli/clistyle.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1231 2016-06-07 14:02:12.000000 mycli-1.9.0/mycli/clitoolbar.py
+-rw-r--r--   0 troten   (880106680) 2064858183     4396 2017-03-11 19:06:00.000000 mycli-1.9.0/mycli/completion_refresher.py
+-rw-r--r--   0 troten   (880106680) 2064858183     6238 2017-03-11 19:05:57.000000 mycli-1.9.0/mycli/config.py
+-rw-r--r--   0 troten   (880106680) 2064858183      574 2015-09-22 21:20:16.000000 mycli-1.9.0/mycli/encodingutils.py
+-rw-r--r--   0 troten   (880106680) 2064858183      414 2016-03-05 15:27:35.000000 mycli-1.9.0/mycli/filters.py
+-rw-r--r--   0 troten   (880106680) 2064858183     2817 2016-06-07 14:02:12.000000 mycli-1.9.0/mycli/key_bindings.py
+-rw-r--r--   0 troten   (880106680) 2064858183      310 2016-03-13 03:04:25.000000 mycli-1.9.0/mycli/lexer.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1496 2016-03-12 11:42:12.000000 mycli-1.9.0/mycli/magic.py
+-rwxr-xr-x   0 troten   (880106680) 2064858183    40993 2017-03-18 23:33:37.000000 mycli-1.9.0/mycli/main.py
+-rw-r--r--   0 troten   (880106680) 2064858183     3484 2017-03-18 21:13:06.000000 mycli-1.9.0/mycli/myclirc
+drwxr-xr-x   0 troten   (880106680) 2064858183        0 2017-03-19 01:07:17.000000 mycli-1.9.0/mycli/packages/
+-rw-r--r--   0 troten   (880106680) 2064858183        0 2015-09-22 21:20:16.000000 mycli-1.9.0/mycli/packages/__init__.py
+-rw-r--r--   0 troten   (880106680) 2064858183    12240 2017-03-07 04:16:45.000000 mycli-1.9.0/mycli/packages/completion_engine.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1522 2015-09-25 20:59:41.000000 mycli-1.9.0/mycli/packages/connection.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1466 2016-03-12 11:42:12.000000 mycli-1.9.0/mycli/packages/expanded.py
+-rw-r--r--   0 troten   (880106680) 2064858183     7174 2017-01-24 13:27:16.000000 mycli-1.9.0/mycli/packages/parseutils.py
+drwxr-xr-x   0 troten   (880106680) 2064858183        0 2017-03-19 01:07:17.000000 mycli-1.9.0/mycli/packages/special/
+-rw-r--r--   0 troten   (880106680) 2064858183      245 2016-03-06 02:05:10.000000 mycli-1.9.0/mycli/packages/special/__init__.py
+-rw-r--r--   0 troten   (880106680) 2064858183     4428 2016-03-13 03:04:25.000000 mycli-1.9.0/mycli/packages/special/dbcommands.py
+-rw-r--r--   0 troten   (880106680) 2064858183     2112 2016-03-05 21:03:13.000000 mycli-1.9.0/mycli/packages/special/favoritequeries.py
+-rw-r--r--   0 troten   (880106680) 2064858183     8207 2017-03-11 19:06:00.000000 mycli-1.9.0/mycli/packages/special/iocommands.py
+-rw-r--r--   0 troten   (880106680) 2064858183     3852 2016-03-12 11:42:12.000000 mycli-1.9.0/mycli/packages/special/main.py
+-rw-r--r--   0 troten   (880106680) 2064858183     1440 2016-03-13 03:04:25.000000 mycli-1.9.0/mycli/packages/special/utils.py
+-rw-r--r--   0 troten   (880106680) 2064858183    38504 2017-03-01 20:51:03.000000 mycli-1.9.0/mycli/packages/tabulate.py
+-rw-r--r--   0 troten   (880106680) 2064858183    17007 2017-03-11 19:06:00.000000 mycli-1.9.0/mycli/sqlcompleter.py
+-rw-r--r--   0 troten   (880106680) 2064858183     8951 2017-03-18 03:01:26.000000 mycli-1.9.0/mycli/sqlexecute.py
+drwxr-xr-x   0 troten   (880106680) 2064858183        0 2017-03-19 01:07:17.000000 mycli-1.9.0/mycli.egg-info/
+-rw-r--r--   0 troten   (880106680) 2064858183        1 2017-03-19 01:07:16.000000 mycli-1.9.0/mycli.egg-info/dependency_links.txt
+-rw-r--r--   0 troten   (880106680) 2064858183       72 2017-03-19 01:07:16.000000 mycli-1.9.0/mycli.egg-info/entry_points.txt
+-rw-r--r--   0 troten   (880106680) 2064858183     1041 2017-03-19 01:07:16.000000 mycli-1.9.0/mycli.egg-info/PKG-INFO
+-rw-r--r--   0 troten   (880106680) 2064858183      130 2017-03-19 01:07:16.000000 mycli-1.9.0/mycli.egg-info/requires.txt
+-rw-r--r--   0 troten   (880106680) 2064858183      948 2017-03-19 01:07:17.000000 mycli-1.9.0/mycli.egg-info/SOURCES.txt
+-rw-r--r--   0 troten   (880106680) 2064858183        6 2017-03-19 01:07:16.000000 mycli-1.9.0/mycli.egg-info/top_level.txt
+-rw-r--r--   0 troten   (880106680) 2064858183     1041 2017-03-19 01:07:17.000000 mycli-1.9.0/PKG-INFO
+-rw-r--r--   0 troten   (880106680) 2064858183     6369 2017-03-11 19:06:00.000000 mycli-1.9.0/README.md
+-rw-r--r--   0 troten   (880106680) 2064858183       88 2017-03-19 01:07:17.000000 mycli-1.9.0/setup.cfg
+-rw-r--r--   0 troten   (880106680) 2064858183     1906 2017-03-11 19:06:00.000000 mycli-1.9.0/setup.py
+-rw-r--r--   0 troten   (880106680) 2064858183      484 2015-09-22 21:20:16.000000 mycli-1.9.0/SPONSORS
```

### Comparing `mycli-1.8.1/AUTHORS` & `mycli-1.9.0/AUTHORS`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-Many thanks to the following contributors. 
+Project Lead:
+-------------
+  * Thomas Roten
+
 
 Core Developers:
 ----------------
 
-  * Thomas Roten
   * Iryna Cherniavska
   * Matheus Rosa
   * Darik Gamble
+  * Dick Marinus
+  * Amjith Ramanujam
 
 Contributors:
 -------------
 
   * Steve Robbins
   * Shoma Suzuki
   * Daniel West
   * Scrappy Soft
-  * Dick Marinus
   * Daniel Black
   * Jonathan Bruno
   * Casper Langemeijer
   * Jonathan Slenders
   * Artem Bezsmertnyi
   * Mikhail Borisov
   * Heath Naylor
@@ -34,12 +37,20 @@
   * Tyler Kuipers
   * William GARCIA
   * Yasuhiro Matsumoto
   * bjarnagin
   * jbruno
   * mrdeathless
   * Abirami P
+  * John Sterling
+  * Jialong Liu
+  * Zhidong
+  * Daniël van Eeden
+  * zer09
+  * cxbig
+  * chainkite
+  * Michał Górny
 
 Creator:
 --------
 
 Amjith Ramanujam
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mycli-1.8.1/changelog.md` & `mycli-1.9.0/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+1.9.0:
+======
+
+Features:
+---------
+
+* Add tee/notee commands for outputing results to a file. (Thanks: [Dick Marinus]).
+* Add date, port, and whitespace options to prompt configuration. (Thanks: [Matheus Rosa]).
+* Allow user to specify LESS pager flags. (Thanks: [John Sterling]).
+* Add support for auto-reconnect. (Thanks: [Jialong Liu]).
+* Add CSV batch output. (Thanks: [Matheus Rosa]).
+* Add auto_vertical_output config to myclirc. (Thanks: [Matheus Rosa]).
+* Improve Fedora install instructions. (Thanks: [Dick Marinus]).
+
+Bug Fixes:
+----------
+
+* Fix crashes occuring from commands starting with #. (Thanks: [Zhidong]).
+* Fix broken PyMySQL link in README. (Thanks: [Daniël van Eeden]).
+* Add various missing keywords for highlighting and autocompletion. (Thanks: [zer09]).
+* Add the missing REGEXP keyword for highlighting and autocompletion. (Thanks: [cxbig]).
+* Fix duplicate username entries in completion list. (Thanks: [John Sterling]).
+* Remove extra spaces in TSV table format output. (Thanks: [Dick Marinus]).
+* Kill running query when interrupted via Ctrl-C. (Thanks: [chainkite]).
+* Read the smart_completion config from myclirc. (Thanks: [Thomas Roten]).
+
+Internal Changes:
+-----------------
+
+* Improve handling of test database credentials. (Thanks: [Dick Marinus]).
+* Add Python 3.6 to test environments and PyPI metadata. (Thanks: [Thomas Roten]).
+* Drop Python 2.6 support. (Thanks: [Thomas Roten]).
+* Swap pycrypto dependency for pycryptodome. (Thanks: [Michał Górny]).
+* Bump sqlparse version so pgcli and mycli can be installed together. (Thanks: [darikg]).
+
 1.8.1:
 ======
 
 Bug Fixes:
 ----------
 * Remove duplicate listing of DISTINCT keyword. (Thanks: [Amjith Ramanujam]).
 * Add an try/except for AS keyword crash. (Thanks: [Amjith Ramanujam]).
@@ -56,15 +91,15 @@
 
 1.6.0:
 ======
 
 Features:
 ---------
 
-* Change continuation prompt for multi-line mode to match default mysql. 
+* Change continuation prompt for multi-line mode to match default mysql.
 * Add `status` command to match mysql's `status` command. (Thanks: [Thomas Roten]).
 * Add SSL support for `mycli`. (Thanks: [Artem Bezsmertnyi]).
 * Add auto-completion and highlight support for OFFSET keyword. (Thanks: [Matheus Rosa]).
 * Add support for `MYSQL_TEST_LOGIN_FILE` env variable to specify alternate login file. (Thanks: [Thomas Roten]).
 * Add support for `--auto-vertical-output` to automatically switch to vertical output if the output doesn't fit in the table format.
 * Add support for system-wide config. Now /etc/myclirc will be honored. (Thanks: [Thomas Roten]).
 * Add support for `nopager` and `\n` to turn off the pager. (Thanks: [Thomas Roten]).
@@ -98,28 +133,28 @@
 
 1.5.1:
 ======
 
 Bug Fixes:
 ----------
 
-* Cast the value of port read from my.cnf to int. 
+* Cast the value of port read from my.cnf to int.
 
 1.5.0:
 ======
 
 Features:
 ---------
 
 * Make a config option to enable `audit_log`. (Thanks: [Matheus Rosa]).
 * Add support for reading .mylogin.cnf to get user credentials. (Thanks: [Thomas Roten]).
   This feature is only available when `pycrypto` package is installed.
 * Register the special command `prompt` with the `\R` as alias. (Thanks: [Matheus Rosa]).
   Users can now change the mysql prompt at runtime using `prompt` command.
-  eg: 
+  eg:
   ```
   mycli> prompt \u@\h>
   Changed prompt format to \u@\h>
   Time: 0.001s
   amjith@localhost>
   ```
 * Perform completion refresh in a background thread. Now mycli can handle
@@ -158,49 +193,49 @@
 
 1.4.0:
 ======
 
 Features:
 ---------
 
-* Add `source` command. This allows running sql statement from a file. 
+* Add `source` command. This allows running sql statement from a file.
 
-  eg: 
+  eg:
   ```
   mycli> source filename.sql
   ```
 
 * Added a config option to make the warning before destructive commands optional. (Thanks: [Daniel West](https://github.com/danieljwest))
 
   In the config file ~/.myclirc set `destructive_warning = False` which will
   disable the warning before running `DROP` commands.
 
 * Add completion support for CHANGE TO and other master/slave commands. This is
-  still preliminary and it will be enhanced in the future. 
+  still preliminary and it will be enhanced in the future.
 
-* Add custom styles to color the menus and toolbars. 
+* Add custom styles to color the menus and toolbars.
 
-* Upgrade prompt_toolkit to 0.46. (Thanks: [Jonathan Slenders]) 
+* Upgrade prompt_toolkit to 0.46. (Thanks: [Jonathan Slenders])
 
-  Multi-line queries are automatically indented. 
+  Multi-line queries are automatically indented.
 
 Bug Fixes:
 ----------
 
 * Fix keyword completion after the `WHERE` clause.
 * Add `\g` and `\G` as valid query terminators. Previously in multi-line mode
   ending a query with a `\G` wouldn't run the query. This is now fixed.
 
 1.3.0:
 ======
 
 Features:
 ---------
 * Add a new special command (\T) to change the table format on the fly. (Thanks: [Jonathan Bruno](https://github.com/brewneaux))
-  eg: 
+  eg:
   ```
   mycli> \T tsv
   ```
 * Add `--defaults-group-suffix` to the command line. This lets the user specify
   a group to use in the my.cnf files. (Thanks: [Iryna Cherniavska](http://github.com/j-bennet))
 
   In the my.cnf file a user can specify credentials for different databases and
@@ -213,38 +248,38 @@
   socket = '/tmp/mysql.sock'
   pager = 'less -RXSF'
   database = 'account'
 
   [clientamjith]
   user     = 'amjith'
   database  = 'user_management'
-  
+
   $ mycli --defaults-group-suffix=amjith   # uses the [clientamjith] section in my.cnf
   ```
 
 * Add `--defaults-file` option to the command line. This allows specifying a
   `my.cnf` to use at launch. This also makes it play nice with mysql sandbox.
 
 * Make `-p` and `--password` take the password in commandline. This makes mycli
-  a drop in replacement for mysql. 
+  a drop in replacement for mysql.
 
 1.2.0:
 ======
 
 Features:
 ---------
 
 * Add support for wider completion menus in the config file.
 
   Add `wider_completion_menu = True` in the config file (~/.myclirc) to enable this feature.
 
 Bug Fixes:
 ---------
 
-* Prevent Ctrl-C from quitting mycli while the pager is active. 
+* Prevent Ctrl-C from quitting mycli while the pager is active.
 * Refresh auto-completions after the database is changed via a CONNECT command.
 
 Internal Changes:
 -----------------
 
 * Upgrade prompt_toolkit dependency version to 0.45.
 * Added Travis CI to run the tests automatically.
@@ -285,28 +320,28 @@
 ===========
 
 Features:
 ---------
 
 * Customizable prompt. (Thanks [Steve Robbins](https://github.com/steverobbins))
 * Make `\G` formatting to behave more like mysql.
-   
+
 Bug Fixes:
 ----------
 
 * Formatting issue in \G for really long column values.
 
 
 2015/06/07:
 ===========
 
 Features:
 ---------
 
-* Upgrade prompt_toolkit to 0.38. This improves the performance of pasting long queries. 
+* Upgrade prompt_toolkit to 0.38. This improves the performance of pasting long queries.
 * Add support for reading my.cnf files.
 * Add editor command \e.
 * Replace ConfigParser with ConfigObj.
 * Add \dt to show all tables.
 * Add fuzzy completion for table names and column names.
 * Automatically reconnect when connection is lost to the database.
 
@@ -323,30 +358,30 @@
 
 Features:
 ---------
 
 * Add support for connecting via socket.
 * Add completion for SQL functions.
 * Add completion support for SHOW statements.
-* Made the timing of sql statements human friendly. 
+* Made the timing of sql statements human friendly.
 * Automatically prompt for a password if needed.
 
 Bug Fixes:
 ----------
-* Fixed the installation issues with PyMySQL dependency on case-sensitive file systems. 
+* Fixed the installation issues with PyMySQL dependency on case-sensitive file systems.
 
 [Daniel West]: http://github.com/danieljwest
 [Iryna Cherniavska]: https://github.com/j-bennet
 [Kacper Kwapisz]: https://github.com/KKKas
 [Martijn Engler]: https://github.com/martijnengler
 [Matheus Rosa]:  https://github.com/mdsrosa
 [Shoma Suzuki]: https://github.com/shoma
 [spacewander]: https://github.com/spacewander
 [Thomas Roten]: https://github.com/tsroten
-[Artem Bezsmertnyi]: https://github.com/mrdeathless 
+[Artem Bezsmertnyi]: https://github.com/mrdeathless
 [Mikhail Borisov]: https://github.com/borman
 [Casper Langemeijer]: Casper Langemeijer
 [Lennart Weller]: https://github.com/lhw
 [Phil Cohen]: https://github.com/phlipper
 [Terseus]: https://github.com/Terseus
 [William GARCIA]: https://github.com/willgarcia
 [Jonathan Slenders]: https://github.com/jonathanslenders
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mycli-1.8.1/LICENSE.txt` & `mycli-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/clibuffer.py` & `mycli-1.9.0/mycli/clibuffer.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/clistyle.py` & `mycli-1.9.0/mycli/clistyle.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,11 +9,11 @@
         style = pygments.styles.get_style_by_name(name)
     except ClassNotFound:
         style = pygments.styles.get_style_by_name('native')
 
     styles = {}
     styles.update(style.styles)
     styles.update(default_style_extensions)
-    custom_styles = dict([(string_to_tokentype(x), y) for x, y in cli_style.items()])
+    custom_styles = {string_to_tokentype(x): y for x, y in cli_style.items()}
     styles.update(custom_styles)
 
     return style_from_dict(styles)
```

### Comparing `mycli-1.8.1/mycli/clitoolbar.py` & `mycli-1.9.0/mycli/clitoolbar.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/completion_refresher.py` & `mycli-1.9.0/mycli/completion_refresher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import threading
 from .packages.special.main import COMMANDS
-try:
-    from collections import OrderedDict
-except ImportError:
-    from .packages.ordereddict import OrderedDict
+from collections import OrderedDict
 
 from .sqlcompleter import SQLCompleter
 from .sqlexecute import SQLExecute
 
 class CompletionRefresher(object):
 
     refreshers = OrderedDict()
```

### Comparing `mycli-1.8.1/mycli/config.py` & `mycli-1.9.0/mycli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from Crypto.Cipher import AES
 except ImportError:
     AES = None
 
 
 class CryptoError(Exception):
     """
-    Exception to signal about pycrypto not available.
+    Exception to signal about pycrypto(dome) not available.
     """
     pass
 
 logger = logging.getLogger(__name__)
 
 def log(logger, level, message):
     """Logs message to stderr if logging isn't initialized."""
@@ -122,15 +122,15 @@
     to generate the real key used in the AES cipher.
 
     :param f: an I/O object opened in binary mode
     :return: the decrypted login path file
     :rtype: io.BytesIO or None
     """
     if AES is None:
-        raise CryptoError('pycrypto is not available.')
+        raise CryptoError('pycrypto(dome) is not available.')
 
     # Number of bytes used to store the length of ciphertext.
     MAX_CIPHER_STORE_LEN = 4
 
     LOGIN_KEY_LEN = 20
 
     # Move past the unused buffer.
```

### Comparing `mycli-1.8.1/mycli/encodingutils.py` & `mycli-1.9.0/mycli/encodingutils.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/key_bindings.py` & `mycli-1.9.0/mycli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/magic.py` & `mycli-1.9.0/mycli/magic.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/main.py` & `mycli-1.9.0/mycli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 #!/usr/bin/env python
 from __future__ import unicode_literals
 from __future__ import print_function
 
 import os
 import os.path
 import sys
+import csv
 import traceback
+import socket
 import logging
 import threading
 from time import time
 from datetime import datetime
 from random import choice
 from io import open
 
+# support StringIO for Python 2 and 3
+try:
+    from cStringIO import StringIO
+except ImportError:
+    from io import StringIO
+
 import click
 import sqlparse
 from prompt_toolkit import CommandLineInterface, Application, AbortAction
 from prompt_toolkit.interface import AcceptAction
 from prompt_toolkit.enums import DEFAULT_BUFFER, EditingMode
 from prompt_toolkit.shortcuts import create_prompt_layout, create_eventloop
 from prompt_toolkit.document import Document
@@ -90,15 +98,14 @@
     def __init__(self, sqlexecute=None, prompt=None,
             logfile=None, defaults_suffix=None, defaults_file=None,
             login_path=None, auto_vertical_output=False, warn=None):
         self.sqlexecute = sqlexecute
         self.logfile = logfile
         self.defaults_suffix = defaults_suffix
         self.login_path = login_path
-        self.auto_vertical_output = auto_vertical_output
 
         # self.cnf_files is a class variable that stores the list of mysql
         # config files to read in at launch.
         # If defaults_file is specified then override the class variable with
         # defaults_file.
         if defaults_file:
             self.cnf_files = [defaults_file]
@@ -115,14 +122,18 @@
         self.less_chatty = c['main'].as_bool('less_chatty')
         self.cli_style = c['colors']
         self.wider_completion_menu = c['main'].as_bool('wider_completion_menu')
         c_dest_warning = c['main'].as_bool('destructive_warning')
         self.destructive_warning = c_dest_warning if warn is None else warn
         self.login_path_as_host = c['main'].as_bool('login_path_as_host')
 
+        # read from cli argument or user config file
+        self.auto_vertical_output = auto_vertical_output or \
+                                c['main'].as_bool('auto_vertical_output')
+
         # Write user config if system config wasn't the last config loaded.
         if c.filename not in self.system_config_files:
             write_default_config(self.default_config_file, self.user_config_file)
 
         # audit log
         if self.logfile is None and 'audit_log' in c['main']:
             try:
@@ -140,16 +151,16 @@
         self.prompt_format = prompt or prompt_cnf or c['main']['prompt'] or \
                              self.default_prompt
         self.prompt_continuation_format = c['main']['prompt_continuation']
 
         self.query_history = []
 
         # Initialize completer.
-        smart_completion = c['main'].as_bool('smart_completion')
-        self.completer = SQLCompleter(smart_completion)
+        self.smart_completion = c['main'].as_bool('smart_completion')
+        self.completer = SQLCompleter(self.smart_completion)
         self._completer_lock = threading.Lock()
 
         # Register custom special commands.
         self.register_special_commands()
 
         # Load .mylogin.cnf if it exists.
         mylogin_cnf_path = get_mylogin_cnf_path()
@@ -159,15 +170,15 @@
                 if mylogin_cnf_path and mylogin_cnf:
                     # .mylogin.cnf gets read last, even if defaults_file is specified.
                     self.cnf_files.append(mylogin_cnf)
                 elif mylogin_cnf_path and not mylogin_cnf:
                     # There was an error reading the login path file.
                     print('Error: Unable to read login path file.')
             except CryptoError:
-                click.secho('Warning: .mylogin.cnf was not read: pycrypto '
+                click.secho('Warning: .mylogin.cnf was not read: pycrypto(dome) '
                             'module is not available.')
 
         self.cli = None
 
     def register_special_commands(self):
         special.register_special_command(self.change_db, 'use',
                 '\\u', 'Change to a new database.', aliases=('\\u',))
@@ -256,19 +267,15 @@
 
         handler.setFormatter(formatter)
 
         root_logger = logging.getLogger('mycli')
         root_logger.addHandler(handler)
         root_logger.setLevel(level_map[log_level.upper()])
 
-        # Only capture warnings on Python 2.7 and later.
-        try:
-            logging.captureWarnings(True)
-        except AttributeError:
-            pass
+        logging.captureWarnings(True)
 
         root_logger.debug('Initializing mycli logging.')
         root_logger.debug('Log file %r.', log_file)
 
     def connect_uri(self, uri, local_infile=None, ssl=None):
         uri = urlparse(uri)
         database = uri.path[1:]  # ignore the leading fwd slash
@@ -294,15 +301,15 @@
         def get(key):
             result = None
             for sect in cnf:
                 if sect in sections and key in cnf[sect]:
                     result = cnf[sect][key]
             return result
 
-        return dict([(x, get(x)) for x in keys])
+        return {x: get(x) for x in keys}
 
     def merge_ssl_with_cnf(self, ssl, cnf):
         """Merge SSL configuration dict with cnf dict"""
 
         merged = {}
         merged.update(ssl)
         prefix = 'ssl-'
@@ -428,15 +435,16 @@
         return document
 
     def run_cli(self):
         sqlexecute = self.sqlexecute
         logger = self.logger
         self.configure_pager()
 
-        self.refresh_completions()
+        if self.smart_completion:
+            self.refresh_completions()
 
         project_root = os.path.dirname(PACKAGE_ROOT)
         author_file = os.path.join(project_root, 'AUTHORS')
         sponsor_file = os.path.join(project_root, 'SPONSORS')
 
         key_binding_manager = mycli_bindings()
 
@@ -450,14 +458,162 @@
         def prompt_tokens(cli):
             return [(Token.Prompt, self.get_prompt(self.prompt_format))]
 
         def get_continuation_tokens(cli, width):
             continuation_prompt = self.get_prompt(self.prompt_continuation_format)
             return [(Token.Continuation, ' ' * (width - len(continuation_prompt)) + continuation_prompt)]
 
+        def one_iteration(document=None):
+            if document is None:
+                document = self.cli.run(reset_current_buffer=True)
+
+                special.set_expanded_output(False)
+
+                # The reason we check here instead of inside the sqlexecute is
+                # because we want to raise the Exit exception which will be
+                # caught by the try/except block that wraps the
+                # sqlexecute.run() statement.
+                if quit_command(document.text):
+                    raise EOFError
+
+                try:
+                    document = self.handle_editor_command(self.cli, document)
+                except RuntimeError as e:
+                    logger.error("sql: %r, error: %r", document.text, e)
+                    logger.error("traceback: %r", traceback.format_exc())
+                    self.output(str(e), err=True, fg='red')
+                    return
+
+            if self.destructive_warning:
+                destroy = confirm_destructive_query(document.text)
+                if destroy is None:
+                    pass  # Query was not destructive. Nothing to do here.
+                elif destroy is True:
+                    self.output('Your call!')
+                else:
+                    self.output('Wise choice!')
+                    return
+
+            # Keep track of whether or not the query is mutating. In case
+            # of a multi-statement query, the overall query is considered
+            # mutating if any one of the component statements is mutating
+            mutating = False
+
+            try:
+                logger.debug('sql: %r', document.text)
+
+                special.write_tee(self.get_prompt(self.prompt_format) + document.text)
+                if self.logfile:
+                    self.logfile.write('\n# %s\n' % datetime.now())
+                    self.logfile.write(document.text)
+                    self.logfile.write('\n')
+
+                successful = False
+                start = time()
+                res = sqlexecute.run(document.text)
+                successful = True
+                output = []
+                total = 0
+                for title, cur, headers, status in res:
+                    logger.debug("headers: %r", headers)
+                    logger.debug("rows: %r", cur)
+                    logger.debug("status: %r", status)
+                    threshold = 1000
+                    if (is_select(status) and
+                            cur and cur.rowcount > threshold):
+                        self.output('The result set has more than %s rows.'
+                                % threshold, fg='red')
+                        if not click.confirm('Do you want to continue?'):
+                            self.output("Aborted!", err=True, fg='red')
+                            break
+
+                    if self.auto_vertical_output:
+                        max_width = self.cli.output.get_size().columns
+                    else:
+                        max_width = None
+
+                    formatted = format_output(title, cur, headers,
+                        status, self.table_format,
+                        special.is_expanded_output(), max_width)
+
+                    output.extend(formatted)
+                    end = time()
+                    total += end - start
+                    mutating = mutating or is_mutating(status)
+            except UnicodeDecodeError as e:
+                import pymysql
+                if pymysql.VERSION < (0, 6, 7):
+                    message = ('You are running an older version of pymysql.\n'
+                            'Please upgrade to 0.6.7 or above to view binary data.\n'
+                            'Try \'pip install -U pymysql\'.')
+                    self.output(message)
+                else:
+                    raise e
+            except KeyboardInterrupt:
+                # get last connection id
+                connection_id_to_kill = sqlexecute.connection_id
+                logger.debug("connection id to kill: %r", connection_id_to_kill)
+                # Restart connection to the database
+                sqlexecute.connect()
+                try:
+                    for title, cur, headers, status in sqlexecute.run('kill %s' % connection_id_to_kill):
+                        status_str = str(status).lower()
+                        if status_str.find('ok') > -1:
+                            logger.debug("cancelled query, connection id: %r, sql: %r",
+                                         connection_id_to_kill, document.text)
+                            self.output("cancelled query", err=True, fg='red')
+                except Exception as e:
+                    self.output('Encountered error while cancelling query: %s' % str(e), err=True, fg='red')
+            except NotImplementedError:
+                self.output('Not Yet Implemented.', fg="yellow")
+            except OperationalError as e:
+                logger.debug("Exception: %r", e)
+                if (e.args[0] in (2003, 2006, 2013)):
+                    logger.debug('Attempting to reconnect.')
+                    self.output('Reconnecting...', fg='yellow')
+                    try:
+                        sqlexecute.connect()
+                        logger.debug('Reconnected successfully.')
+                        one_iteration(document)
+                        return  # OK to just return, cuz the recursion call runs to the end.
+                    except OperationalError as e:
+                        logger.debug('Reconnect failed. e: %r', e)
+                        self.output(str(e), err=True, fg='red')
+                        return  # If reconnection failed, don't proceed further.
+                else:
+                    logger.error("sql: %r, error: %r", document.text, e)
+                    logger.error("traceback: %r", traceback.format_exc())
+                    self.output(str(e), err=True, fg='red')
+            except Exception as e:
+                logger.error("sql: %r, error: %r", document.text, e)
+                logger.error("traceback: %r", traceback.format_exc())
+                self.output(str(e), err=True, fg='red')
+            else:
+                try:
+                    special.write_tee('\n'.join(output))
+                    if special.is_pager_enabled():
+                        self.output_via_pager('\n'.join(output))
+                    else:
+                        self.output('\n'.join(output))
+                except KeyboardInterrupt:
+                    pass
+                if special.is_timing_enabled():
+                    self.output('Time: %0.03fs' % total)
+
+                # Refresh the table names and column names if necessary.
+                if need_completion_refresh(document.text):
+                    self.refresh_completions(
+                            reset=need_completion_reset(document.text))
+            finally:
+                if self.logfile is False:
+                    self.output("Warning: This query was not logged.", err=True, fg='red')
+            query = Query(document.text, successful, mutating)
+            self.query_history.append(query)
+
+
         get_toolbar_tokens = create_toolbar_tokens_func(self.completion_refresher.is_refreshing)
 
         layout = create_prompt_layout(lexer=MyCliLexer,
                                       multiline=True,
                                       get_prompt_tokens=prompt_tokens,
                                       get_continuation_tokens=get_continuation_tokens,
                                       get_bottom_toolbar_tokens=get_toolbar_tokens,
@@ -485,169 +641,37 @@
                                       editing_mode=editing_mode,
                                       ignore_case=True)
             self.cli = CommandLineInterface(application=application,
                                        eventloop=create_eventloop())
 
         try:
             while True:
-                document = self.cli.run(reset_current_buffer=True)
-
-                special.set_expanded_output(False)
-
-                # The reason we check here instead of inside the sqlexecute is
-                # because we want to raise the Exit exception which will be
-                # caught by the try/except block that wraps the
-                # sqlexecute.run() statement.
-                if quit_command(document.text):
-                    raise EOFError
-
-                try:
-                    document = self.handle_editor_command(self.cli, document)
-                except RuntimeError as e:
-                    logger.error("sql: %r, error: %r", document.text, e)
-                    logger.error("traceback: %r", traceback.format_exc())
-                    self.output(str(e), err=True, fg='red')
-                    continue
-                if self.destructive_warning:
-                    destroy = confirm_destructive_query(document.text)
-                    if destroy is None:
-                        pass  # Query was not destructive. Nothing to do here.
-                    elif destroy is True:
-                        self.output('Your call!')
-                    else:
-                        self.output('Wise choice!')
-                        continue
-
-                # Keep track of whether or not the query is mutating. In case
-                # of a multi-statement query, the overall query is considered
-                # mutating if any one of the component statements is mutating
-                mutating = False
-
-                try:
-                    logger.debug('sql: %r', document.text)
-
-                    if self.logfile:
-                        self.logfile.write('\n# %s\n' % datetime.now())
-                        self.logfile.write(document.text)
-                        self.logfile.write('\n')
-
-                    successful = False
-                    start = time()
-                    res = sqlexecute.run(document.text)
-                    successful = True
-                    output = []
-                    total = 0
-                    for title, cur, headers, status in res:
-                        logger.debug("headers: %r", headers)
-                        logger.debug("rows: %r", cur)
-                        logger.debug("status: %r", status)
-                        threshold = 1000
-                        if (is_select(status) and
-                                cur and cur.rowcount > threshold):
-                            self.output('The result set has more than %s rows.'
-                                    % threshold, fg='red')
-                            if not click.confirm('Do you want to continue?'):
-                                self.output("Aborted!", err=True, fg='red')
-                                break
-
-                        if self.auto_vertical_output:
-                            max_width = self.cli.output.get_size().columns
-                        else:
-                            max_width = None
-
-                        formatted = format_output(title, cur, headers,
-                            status, self.table_format,
-                            special.is_expanded_output(), max_width)
-
-                        output.extend(formatted)
-                        end = time()
-                        total += end - start
-                        mutating = mutating or is_mutating(status)
-                except UnicodeDecodeError as e:
-                    import pymysql
-                    if pymysql.VERSION < (0, 6, 7):
-                        message = ('You are running an older version of pymysql.\n'
-                                'Please upgrade to 0.6.7 or above to view binary data.\n'
-                                'Try \'pip install -U pymysql\'.')
-                        self.output(message)
-                    else:
-                        raise e
-                except KeyboardInterrupt:
-                    # Restart connection to the database
-                    sqlexecute.connect()
-                    logger.debug("cancelled query, sql: %r", document.text)
-                    self.output("cancelled query", err=True, fg='red')
-                except NotImplementedError:
-                    self.output('Not Yet Implemented.', fg="yellow")
-                except OperationalError as e:
-                    logger.debug("Exception: %r", e)
-                    reconnect = True
-                    if (e.args[0] in (2003, 2006, 2013)):
-                        reconnect = click.prompt('Connection reset. Reconnect (Y/n)',
-                                show_default=False, type=bool, default=True)
-                        if reconnect:
-                            logger.debug('Attempting to reconnect.')
-                            try:
-                                sqlexecute.connect()
-                                logger.debug('Reconnected successfully.')
-                                self.output('Reconnected!\nTry the command again.', fg='green')
-                            except OperationalError as e:
-                                logger.debug('Reconnect failed. e: %r', e)
-                                self.output(str(e), err=True, fg='red')
-                                continue  # If reconnection failed, don't proceed further.
-                        else:  # If user chooses not to reconnect, don't proceed further.
-                            continue
-                    else:
-                        logger.error("sql: %r, error: %r", document.text, e)
-                        logger.error("traceback: %r", traceback.format_exc())
-                        self.output(str(e), err=True, fg='red')
-                except Exception as e:
-                    logger.error("sql: %r, error: %r", document.text, e)
-                    logger.error("traceback: %r", traceback.format_exc())
-                    self.output(str(e), err=True, fg='red')
-                else:
-                    try:
-                        if special.is_pager_enabled():
-                            self.output_via_pager('\n'.join(output))
-                        else:
-                            self.output('\n'.join(output))
-                    except KeyboardInterrupt:
-                        pass
-                    if special.is_timing_enabled():
-                        self.output('Time: %0.03fs' % total)
-
-                    # Refresh the table names and column names if necessary.
-                    if need_completion_refresh(document.text):
-                        self.refresh_completions(
-                                reset=need_completion_reset(document.text))
-                finally:
-                    if self.logfile is False:
-                        self.output("Warning: This query was not logged.", err=True, fg='red')
-                query = Query(document.text, successful, mutating)
-                self.query_history.append(query)
-
+                one_iteration()
         except EOFError:
+            special.close_tee()
             if not self.less_chatty:
                 self.output('Goodbye!')
 
     def output(self, text, **kwargs):
+        special.write_tee(text)
         if self.logfile:
             self.logfile.write(utf8tounicode(text))
             self.logfile.write('\n')
         click.secho(text, **kwargs)
 
     def output_via_pager(self, text):
         if self.logfile:
             self.logfile.write(text)
             self.logfile.write('\n')
         click.echo_via_pager(text)
 
     def configure_pager(self):
-        # Provide sane defaults for less.
-        os.environ['LESS'] = '-RXF'
+        # Provide sane defaults for less if they are empty.
+        if not os.environ.get('LESS'):
+            os.environ['LESS'] = '-RXF'
 
         cnf = self.read_my_cnf_files(self.cnf_files, ['pager', 'skip-pager'])
         if cnf['pager']:
             special.set_pager(cnf['pager'])
         if cnf['skip-pager']:
             special.disable_pager()
 
@@ -689,25 +713,27 @@
         sqlexecute = self.sqlexecute
         host = self.login_path if self.login_path and self.login_path_as_host else sqlexecute.host
         string = string.replace('\\u', sqlexecute.user or '(none)')
         string = string.replace('\\h', host or '(none)')
         string = string.replace('\\d', sqlexecute.dbname or '(none)')
         string = string.replace('\\t', sqlexecute.server_type()[0] or 'mycli')
         string = string.replace('\\n', "\n")
+        string = string.replace('\\D', datetime.now().strftime('%a %b %d %H:%M:%S %Y'))
+        string = string.replace('\\p', str(sqlexecute.port))
+        string = string.replace('\\_', ' ')
         return string
 
-    def run_query(self, query, table_format=None):
+    def run_query(self, query, table_format=None, new_line=True):
         """Runs query"""
         results = self.sqlexecute.run(query)
         for result in results:
             title, cur, headers, status = result
-            table_format = self.table_format if table_format else None
             output = format_output(title, cur, headers, None, table_format)
             for line in output:
-                click.echo(line)
+                click.echo(line, nl=new_line)
 
 @click.command()
 @click.option('-h', '--host', envvar='MYSQL_HOST', help='Host address of the database.')
 @click.option('-P', '--port', envvar='MYSQL_TCP_PORT', type=int, help='Port number to use for connection. Honors '
               '$MYSQL_TCP_PORT')
 @click.option('-u', '--user', help='User name to connect to the database.')
 @click.option('-S', '--socket', envvar='MYSQL_UNIX_PORT', help='The socket file to use for connection.')
@@ -740,28 +766,30 @@
               help='Read config group with the specified suffix.')
 @click.option('--defaults-file', type=click.Path(),
               help='Only read default options from the given file')
 @click.option('--auto-vertical-output', is_flag=True,
               help='Automatically switch to vertical output mode if the result is wider than the terminal width.')
 @click.option('-t', '--table', is_flag=True,
               help='Display batch output in table format.')
+@click.option('--csv', is_flag=True,
+              help='Display batch output in CSV format.')
 @click.option('--warn/--no-warn', default=None,
               help='Warn before running a destructive query.')
 @click.option('--local-infile', type=bool,
               help='Enable/disable LOAD DATA LOCAL INFILE.')
 @click.option('--login-path', type=str,
               help='Read this path from the login file.')
 @click.option('-e', '--execute',  type=str,
               help='Execute query to the database.')
 @click.argument('database', default='', nargs=1)
 def cli(database, user, host, port, socket, password, dbname,
         version, prompt, logfile, defaults_group_suffix, defaults_file,
         login_path, auto_vertical_output, local_infile, ssl_ca, ssl_capath,
-        ssl_cert, ssl_key, ssl_cipher, ssl_verify_server_cert, table, warn,
-        execute):
+        ssl_cert, ssl_key, ssl_cipher, ssl_verify_server_cert, table, csv,
+        warn, execute):
 
     if version:
         print('Version:', __version__)
         sys.exit(0)
 
     mycli = MyCli(prompt=prompt, logfile=logfile,
                   defaults_suffix=defaults_group_suffix,
@@ -777,15 +805,15 @@
             'key': ssl_key and os.path.expanduser(ssl_key),
             'capath': ssl_capath,
             'cipher': ssl_cipher,
             'check_hostname': ssl_verify_server_cert,
             }
 
     # remove empty ssl options
-    ssl = dict((k, v) for (k, v) in ssl.items() if v is not None)
+    ssl = {k: v for k, v in ssl.items() if v is not None}
     if database and '://' in database:
         mycli.connect_uri(database, local_infile, ssl)
     else:
         mycli.connect(database, user, password, host, port, socket,
                       local_infile=local_infile, ssl=ssl)
 
     mycli.logger.debug('Launch Params: \n'
@@ -793,15 +821,20 @@
             '\tuser: %r'
             '\thost: %r'
             '\tport: %r', database, user, host, port)
 
     #  --execute argument
     if execute:
         try:
-            mycli.run_query(execute, table_format=table)
+            table_format = None
+            if table:
+                table_format = mycli.table_format
+            elif csv:
+                table_format = 'csv'
+            mycli.run_query(execute, table_format=table_format)
             exit(0)
         except Exception as e:
             click.secho(str(e), err=True, fg='red')
             exit(1)
 
     if sys.stdin.isatty():
         mycli.run_cli()
@@ -814,44 +847,64 @@
         except FileNotFoundError:
             mycli.logger.warning('Unable to open TTY as stdin.')
 
         if (mycli.destructive_warning and
                 confirm_destructive_query(stdin_text) is False):
             exit(0)
         try:
-            mycli.run_query(stdin_text, table_format=table)
+            table_format = None
+            new_line = True
+
+            if csv:
+                table_format = 'csv'
+                new_line = False
+            elif table:
+                table_format = mycli.table_format
+
+            mycli.run_query(stdin_text, table_format=table_format, new_line=new_line)
+            exit(0)
         except Exception as e:
             click.secho(str(e), err=True, fg='red')
             exit(1)
 
 
 def format_output(title, cur, headers, status, table_format, expanded=False, max_width=None):
     output = []
     if title:  # Only print the title if it's not None.
         output.append(title)
     if cur:
         headers = [utf8tounicode(x) for x in headers]
+        table_format = 'tsv' if table_format is None else table_format
+
         if expanded:
             output.append(expanded_table(cur, headers))
-        elif table_format is not None:
+        elif table_format == 'csv':
+            content = StringIO()
+            writer = csv.writer(content)
+            writer.writerow(headers)
+
+            for row in cur:
+                row = ['null' if val is None else str(val) for val in row]
+                writer.writerow(row)
+
+            output.append(content.getvalue())
+            content.close()
+        else:
             rows = list(cur)
             tabulated, frows = tabulate(rows, headers, tablefmt=table_format,
                                         missingval='<null>')
             if (max_width and rows and
                     content_exceeds_width(frows[0], max_width) and
                     headers):
                 output.append(expanded_table(rows, headers))
             else:
                 output.append(tabulated)
-        else:
-            output.append('\t'.join(headers))
-            for row in cur:
-                output.append('\t'.join([str(r) for r in row]))
     if status:  # Only print the status if it's not None.
         output.append(status)
+
     return output
 
 def content_exceeds_width(row, width):
     # Account for 3 characters between each column
     separator_space = (len(row)*3)
     # Add 2 columns for a bit of buffer
     line_len = sum([len(str(x)) for x in row]) + separator_space + 2
@@ -898,15 +951,15 @@
         return False
     return status.split(None, 1)[0].lower() == 'select'
 
 def query_starts_with(query, prefixes):
     """Check if the query starts with any item from *prefixes*."""
     prefixes = [prefix.lower() for prefix in prefixes]
     formatted_sql = sqlparse.format(query.lower(), strip_comments=True)
-    return formatted_sql.split()[0] in prefixes
+    return bool(formatted_sql) and formatted_sql.split()[0] in prefixes
 
 def queries_start_with(queries, prefixes):
     """Check if any queries start with any item from *prefixes*."""
     for query in sqlparse.split(queries):
         if query and query_starts_with(query, prefixes) is True:
             return True
     return False
```

### Comparing `mycli-1.8.1/mycli/myclirc` & `mycli-1.9.0/mycli/myclirc`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
 # Skip intro info on startup and outro info on exit
 less_chatty = False
 
 # Use alias from --login-path instead of host name in prompt
 login_path_as_host = False
 
+# Cause result sets to be displayed vertically if they are too wide for the current window,
+# and using normal tabular format otherwise. (This applies to statements terminated by ; or \G.) 
+auto_vertical_output = False
+
 # Custom colors for the completion menu, toolbar, etc.
 [colors]
 # Completion menus.
 Token.Menu.Completions.Completion.Current = 'bg:#00aaaa #000000'
 Token.Menu.Completions.Completion = 'bg:#008888 #ffffff'
 Token.Menu.Completions.MultiColumnMeta = 'bg:#aaffff #000000'
 Token.Menu.Completions.ProgressButton = 'bg:#003333'
```

### Comparing `mycli-1.8.1/mycli/packages/completion_engine.py` & `mycli-1.9.0/mycli/packages/completion_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,17 @@
         elif p.token_first().value.lower() == 'show':
             return [{'type': 'show'}]
 
         # We're probably in a function argument list
         return [{'type': 'column', 'tables': extract_tables(full_text)}]
     elif token_v in ('set', 'by', 'distinct'):
         return [{'type': 'column', 'tables': extract_tables(full_text)}]
+    elif token_v == 'as':
+        # Don't suggest anything for an alias
+        return []
     elif token_v in ('show'):
         return [{'type': 'show'}]
     elif token_v in ('to',):
         p = sqlparse.parse(text_before_cursor)[0]
         if p.token_first().value.lower() == 'change':
             return [{'type': 'change'}]
         else:
```

### Comparing `mycli-1.8.1/mycli/packages/connection.py` & `mycli-1.9.0/mycli/packages/connection.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/expanded.py` & `mycli-1.9.0/mycli/packages/expanded.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/parseutils.py` & `mycli-1.9.0/mycli/packages/parseutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         else:
             return ''
 
 
 # This code is borrowed from sqlparse example script.
 # <url>
 def is_subselect(parsed):
-    if not parsed.is_group():
+    if not parsed.is_group:
         return False
     for item in parsed.tokens:
         if item.ttype is DML and item.value.upper() in ('SELECT', 'INSERT',
                 'UPDATE', 'CREATE', 'DELETE'):
             return True
     return False
```

### Comparing `mycli-1.8.1/mycli/packages/special/dbcommands.py` & `mycli-1.9.0/mycli/packages/special/dbcommands.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/special/favoritequeries.py` & `mycli-1.9.0/mycli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/special/iocommands.py` & `mycli-1.9.0/mycli/packages/special/iocommands.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .main import special_command, NO_QUERY, PARSED_QUERY
 from .favoritequeries import favoritequeries
 from .utils import handle_cd_command
 
 TIMING_ENABLED = False
 use_expanded_output = False
 PAGER_ENABLED = True
+tee_file = None
 
 @export
 def set_timing_enabled(val):
     global TIMING_ENABLED
     TIMING_ENABLED = val
 
 @export
@@ -236,7 +237,48 @@
         if isinstance(response, bytes):
             encoding = locale.getpreferredencoding(False)
             response = response.decode(encoding)
 
         return [(None, None, None, response)]
     except OSError as e:
         return [(None, None, None, 'OSError: %s' % e.strerror)]
+
+@special_command('tee', 'tee [-o] filename',
+                 'write to an output file (optionally overwrite using -o)')
+def set_tee(arg, **_):
+    global tee_file
+    if arg.startswith('-o '):
+        mode = "w"
+        filename = arg[3:]
+    else:
+        mode = 'a'
+        filename = arg
+
+    if not filename:
+        raise TypeError('You must provide a filename.')
+
+    try:
+        tee_file = open(filename, mode)
+    except (IOError, OSError) as e:
+        raise OSError("Cannot write to file '{}': {}".format(e.filename, e.strerror))
+
+    return [(None, None, None, "")]
+
+@export
+def close_tee():
+    global tee_file
+    if tee_file:
+        tee_file.close()
+        tee_file = None
+
+@special_command('notee', 'notee', 'stop writing to an output file')
+def no_tee(arg, **_):
+    close_tee()
+    return [(None, None, None, "")]
+
+@export
+def write_tee(output):
+    global tee_file
+    if tee_file:
+        tee_file.write(output)
+        tee_file.write(u"\n")
+        tee_file.flush()
```

### Comparing `mycli-1.8.1/mycli/packages/special/main.py` & `mycli-1.9.0/mycli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/special/utils.py` & `mycli-1.9.0/mycli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `mycli-1.8.1/mycli/packages/tabulate.py` & `mycli-1.9.0/mycli/packages/tabulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 #
 #   - either None, to display all table elements unconditionally,
 #   - or a list of elements not to be displayed if the table has column headers.
 #
 TableFormat = namedtuple("TableFormat", ["lineabove", "linebelowheader",
                                          "linebetweenrows", "linebelow",
                                          "headerrow", "datarow",
-                                         "padding", "with_header_hide"])
+                                         "padding", "with_header_hide", "with_align"])
 
 
 def _pipe_segment_with_colons(align, colwidth):
     """Return a segment of a horizontal line with optional colons which
     indicate column's alignment (as in `pipe` output format)."""
     w = colwidth
     if align in ["right", "decimal"]:
@@ -158,130 +158,131 @@
                   TableFormat(lineabove=Line("", "-", "  ", ""),
                               linebelowheader=Line("", "-", "  ", ""),
                               linebetweenrows=None,
                               linebelow=Line("", "-", "  ", ""),
                               headerrow=DataRow("", "  ", ""),
                               datarow=DataRow("", "  ", ""),
                               padding=0,
-                              with_header_hide=["lineabove", "linebelow"]),
+                              with_header_hide=["lineabove", "linebelow"], with_align=True),
                   "plain":
                   TableFormat(lineabove=None, linebelowheader=None,
                               linebetweenrows=None, linebelow=None,
                               headerrow=DataRow("", "  ", ""),
                               datarow=DataRow("", "  ", ""),
-                              padding=0, with_header_hide=None),
+                              padding=0, with_header_hide=None, with_align=True),
                   "grid":
                   TableFormat(lineabove=Line("+", "-", "+", "+"),
                               linebelowheader=Line("+", "=", "+", "+"),
                               linebetweenrows=Line("+", "-", "+", "+"),
                               linebelow=Line("+", "-", "+", "+"),
                               headerrow=DataRow("|", "|", "|"),
                               datarow=DataRow("|", "|", "|"),
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=True),
                   "fancy_grid":
                   TableFormat(lineabove=Line("╒", "═", "╤", "╕"),
                               linebelowheader=Line("╞", "═", "╪", "╡"),
                               linebetweenrows=Line("├", "─", "┼", "┤"),
                               linebelow=Line("╘", "═", "╧", "╛"),
                               headerrow=DataRow("│", "│", "│"),
                               datarow=DataRow("│", "│", "│"),
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=True),
                   "pipe":
                   TableFormat(lineabove=_pipe_line_with_colons,
                               linebelowheader=_pipe_line_with_colons,
                               linebetweenrows=None,
                               linebelow=None,
                               headerrow=DataRow("|", "|", "|"),
                               datarow=DataRow("|", "|", "|"),
                               padding=1,
-                              with_header_hide=["lineabove"]),
+                              with_header_hide=["lineabove"], with_align=True),
                   "orgtbl":
                   TableFormat(lineabove=None,
                               linebelowheader=Line("|", "-", "+", "|"),
                               linebetweenrows=None,
                               linebelow=None,
                               headerrow=DataRow("|", "|", "|"),
                               datarow=DataRow("|", "|", "|"),
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=True),
                   "psql":
                   TableFormat(lineabove=Line("+", "-", "+", "+"),
                               linebelowheader=Line("|", "-", "+", "|"),
                               linebetweenrows=None,
                               linebelow=Line("+", "-", "+", "+"),
                               headerrow=DataRow("|", "|", "|"),
                               datarow=DataRow("|", "|", "|"),
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=True),
                   "rst":
                   TableFormat(lineabove=Line("", "=", "  ", ""),
                               linebelowheader=Line("", "=", "  ", ""),
                               linebetweenrows=None,
                               linebelow=Line("", "=", "  ", ""),
                               headerrow=DataRow("", "  ", ""),
                               datarow=DataRow("", "  ", ""),
-                              padding=0, with_header_hide=None),
+                              padding=0, with_header_hide=None, with_align=True),
                   "mediawiki":
                   TableFormat(lineabove=Line("{| class=\"wikitable\" style=\"text-align: left;\"",
                                              "", "", "\n|+ <!-- caption -->\n|-"),
                               linebelowheader=Line("|-", "", "", ""),
                               linebetweenrows=Line("|-", "", "", ""),
                               linebelow=Line("|}", "", "", ""),
                               headerrow=partial(_mediawiki_row_with_attrs, "!"),
                               datarow=partial(_mediawiki_row_with_attrs, "|"),
-                              padding=0, with_header_hide=None),
+                              padding=0, with_header_hide=None, with_align=True),
                   "html":
                   TableFormat(lineabove=Line("<table>", "", "", ""),
                               linebelowheader=None,
                               linebetweenrows=None,
                               linebelow=Line("</table>", "", "", ""),
                               headerrow=partial(_html_row_with_attrs, "th"),
                               datarow=partial(_html_row_with_attrs, "td"),
-                              padding=0, with_header_hide=None),
+                              padding=0, with_header_hide=None, with_align=False),
                   "latex":
                   TableFormat(lineabove=_latex_line_begin_tabular,
                               linebelowheader=Line("\\hline", "", "", ""),
                               linebetweenrows=None,
                               linebelow=Line("\\hline\n\\end{tabular}", "", "", ""),
                               headerrow=_latex_row,
                               datarow=_latex_row,
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=False),
                   "latex_booktabs":
                   TableFormat(lineabove=partial(_latex_line_begin_tabular, booktabs=True),
                               linebelowheader=Line("\\midrule", "", "", ""),
                               linebetweenrows=None,
                               linebelow=Line("\\bottomrule\n\\end{tabular}", "", "", ""),
                               headerrow=_latex_row,
                               datarow=_latex_row,
-                              padding=1, with_header_hide=None),
+                              padding=1, with_header_hide=None, with_align=False),
                   "tsv":
                   TableFormat(lineabove=None, linebelowheader=None,
                               linebetweenrows=None, linebelow=None,
                               headerrow=DataRow("", "\t", ""),
                               datarow=DataRow("", "\t", ""),
-                              padding=0, with_header_hide=None)}
+                              padding=0, with_header_hide=None, with_align=False)}
 
 
 tabulate_formats = list(sorted(_table_formats.keys()))
 
 
 _invisible_codes = re.compile(r"\x1b\[\d*m|\x1b\[\d*\;\d*\;\d*m")  # ANSI color codes
 _invisible_codes_bytes = re.compile(b"\x1b\[\d*m|\x1b\[\d*\;\d*\;\d*m")  # ANSI color codes
 
 
 def simple_separated_format(separator):
     """Construct a simple TableFormat with columns separated by a separator.
 
     >>> tsv = simple_separated_format("\\t") ; \
-        tabulate([["foo", 1], ["spam", 23]], tablefmt=tsv) == 'foo \\t 1\\nspam\\t23'
-    True
-
+        print(tabulate([["foo", 1], ["spam", 23]], tablefmt=tsv)[0].replace('\\t', r'\\t'))
+    foo\\t1
+    spam\\t23
     """
     return TableFormat(None, None, None, None,
                        headerrow=DataRow('', separator, ''),
                        datarow=DataRow('', separator, ''),
-                       padding=0, with_header_hide=None)
+                       padding=0, with_header_hide=None,
+                       with_align=False)
 
 
 def _isconvertible(conv, string):
     try:
         n = conv(string)
         return True
     except (ValueError, TypeError):
@@ -494,24 +495,25 @@
 
     """
     types = [_type(s, has_invisible) for s in strings ]
     return reduce(_more_generic, types, int)
 
 
 def _format(val, valtype, floatfmt, missingval=""):
-    """Format a value accoding to its type.
+    u"""Format a value accoding to its type.
 
     Unicode is supported:
 
     >>> hrow = ['\u0431\u0443\u043a\u0432\u0430', '\u0446\u0438\u0444\u0440\u0430'] ; \
         tbl = [['\u0430\u0437', 2], ['\u0431\u0443\u043a\u0438', 4]] ; \
-        good_result = '\\u0431\\u0443\\u043a\\u0432\\u0430      \\u0446\\u0438\\u0444\\u0440\\u0430\\n-------  -------\\n\\u0430\\u0437             2\\n\\u0431\\u0443\\u043a\\u0438           4' ; \
-        tabulate(tbl, headers=hrow) == good_result
-    True
-
+        print(tabulate(tbl, headers=hrow)[0])
+    буква      цифра
+    -------  -------
+    аз             2
+    буки           4
     """
     if val is None:
         return missingval
 
     if valtype in [int, _text_type]:
         return "{0}".format(val)
     elif valtype is _binary_type:
@@ -652,15 +654,15 @@
     return _table_formats.keys()
 
 def tabulate(tabular_data, headers=[], tablefmt="simple",
              floatfmt="g", numalign="decimal", stralign="left",
              missingval=""):
     """Format a fixed width table for pretty printing.
 
-    >>> print(tabulate([[1, 2.34], [-56, "8.999"], ["2", "10001"]]))
+    >>> print(tabulate([[1, 2.34], [-56, "8.999"], ["2", "10001"]])[0])
     ---  ---------
       1      2.34
     -56      8.999
       2  10001
     ---  ---------
 
     The first required argument (`tabular_data`) can be a
@@ -682,15 +684,15 @@
     Otherwise a headerless table is produced.
 
     If the number of headers is less than the number of columns, they
     are supposed to be names of the last columns. This is consistent
     with the plain-text format of R and Pandas' dataframes.
 
     >>> print(tabulate([["sex","age"],["Alice","F",24],["Bob","M",19]],
-    ...       headers="firstrow"))
+    ...       headers="firstrow")[0])
            sex      age
     -----  -----  -----
     Alice  F         24
     Bob    M         19
 
 
     Column alignment
@@ -710,15 +712,15 @@
     `floatfmt` is a format specification used for columns which
     contain numeric data with a decimal point.
 
     `None` values are replaced with a `missingval` string:
 
     >>> print(tabulate([["spam", 1, None],
     ...                 ["eggs", 42, 3.14],
-    ...                 ["other", None, 2.7]], missingval="?"))
+    ...                 ["other", None, 2.7]], missingval="?")[0])
     -----  --  ----
     spam    1  ?
     eggs   42  3.14
     other   ?  2.7
     -----  --  ----
 
     Various plain-text table formats (`tablefmt`) are supported:
@@ -726,163 +728,163 @@
      'latex', and 'latex_booktabs'. Variable `tabulate_formats` contains the list of
     currently supported formats.
 
     "plain" format doesn't use any pseudographics to draw tables,
     it separates columns with a double space:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                 ["strings", "numbers"], "plain"))
+    ...                 ["strings", "numbers"], "plain")[0])
     strings      numbers
     spam         41.9999
     eggs        451
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="plain"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="plain")[0])
     spam   41.9999
     eggs  451
 
     "simple" format is like Pandoc simple_tables:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                 ["strings", "numbers"], "simple"))
+    ...                 ["strings", "numbers"], "simple")[0])
     strings      numbers
     ---------  ---------
     spam         41.9999
     eggs        451
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="simple"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="simple")[0])
     ----  --------
     spam   41.9999
     eggs  451
     ----  --------
 
     "grid" is similar to tables produced by Emacs table.el package or
     Pandoc grid_tables:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "grid"))
+    ...                ["strings", "numbers"], "grid")[0])
     +-----------+-----------+
     | strings   |   numbers |
     +===========+===========+
     | spam      |   41.9999 |
     +-----------+-----------+
     | eggs      |  451      |
     +-----------+-----------+
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="grid"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="grid")[0])
     +------+----------+
     | spam |  41.9999 |
     +------+----------+
     | eggs | 451      |
     +------+----------+
 
     "fancy_grid" draws a grid using box-drawing characters:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "fancy_grid"))
+    ...                ["strings", "numbers"], "fancy_grid")[0])
     ╒═══════════╤═══════════╕
     │ strings   │   numbers │
     ╞═══════════╪═══════════╡
     │ spam      │   41.9999 │
     ├───────────┼───────────┤
     │ eggs      │  451      │
     ╘═══════════╧═══════════╛
 
     "pipe" is like tables in PHP Markdown Extra extension or Pandoc
     pipe_tables:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "pipe"))
+    ...                ["strings", "numbers"], "pipe")[0])
     | strings   |   numbers |
     |:----------|----------:|
     | spam      |   41.9999 |
     | eggs      |  451      |
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="pipe"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="pipe")[0])
     |:-----|---------:|
     | spam |  41.9999 |
     | eggs | 451      |
 
     "orgtbl" is like tables in Emacs org-mode and orgtbl-mode. They
     are slightly different from "pipe" format by not using colons to
     define column alignment, and using a "+" sign to indicate line
     intersections:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "orgtbl"))
+    ...                ["strings", "numbers"], "orgtbl")[0])
     | strings   |   numbers |
     |-----------+-----------|
     | spam      |   41.9999 |
     | eggs      |  451      |
 
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="orgtbl"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="orgtbl")[0])
     | spam |  41.9999 |
     | eggs | 451      |
 
     "rst" is like a simple table format from reStructuredText; please
     note that reStructuredText accepts also "grid" tables:
 
     >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "rst"))
+    ...                ["strings", "numbers"], "rst")[0])
     =========  =========
     strings      numbers
     =========  =========
     spam         41.9999
     eggs        451
     =========  =========
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="rst"))
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="rst")[0])
     ====  ========
     spam   41.9999
     eggs  451
     ====  ========
 
     "mediawiki" produces a table markup used in Wikipedia and on other
     MediaWiki-based sites:
 
     >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
-    ...                headers="firstrow", tablefmt="mediawiki"))
+    ...                headers="firstrow", tablefmt="mediawiki")[0])
     {| class="wikitable" style="text-align: left;"
     |+ <!-- caption -->
     |-
     ! strings   !! align="right"|   numbers
     |-
     | spam      || align="right"|   41.9999
     |-
     | eggs      || align="right"|  451
     |}
 
     "html" produces HTML markup:
 
     >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
-    ...                headers="firstrow", tablefmt="html"))
+    ...                headers="firstrow", tablefmt="html")[0])
     <table>
-    <tr><th>strings  </th><th style="text-align: right;">  numbers</th></tr>
-    <tr><td>spam     </td><td style="text-align: right;">  41.9999</td></tr>
-    <tr><td>eggs     </td><td style="text-align: right;"> 451     </td></tr>
+    <tr><th>strings</th><th>numbers</th></tr>
+    <tr><td>spam</td><td>41.9999</td></tr>
+    <tr><td>eggs</td><td>451</td></tr>
     </table>
 
     "latex" produces a tabular environment of LaTeX document markup:
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex"))
-    \\begin{tabular}{lr}
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex")[0])
+    \\begin{tabular}{ll}
     \\hline
-     spam &  41.9999 \\\\
-     eggs & 451      \\\\
+     spam & 41.9999 \\\\
+     eggs & 451 \\\\
     \\hline
     \\end{tabular}
 
     "latex_booktabs" produces a tabular environment of LaTeX document markup
     using the booktabs.sty package:
 
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_booktabs"))
-    \\begin{tabular}{lr}
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_booktabs")[0])
+    \\begin{tabular}{ll}
     \\toprule
-     spam &  41.9999 \\\\
-     eggs & 451      \\\\
+     spam & 41.9999 \\\\
+     eggs & 451 \\\\
     \\bottomrule
     \end{tabular}
 
     Also returns a tuple of the raw rows pulled from tabular_data
     """
     if tabular_data is None:
         tabular_data = []
@@ -900,35 +902,41 @@
                             ['\t'.join(map(_text_type, row)) for row in cols])
     has_invisible = re.search(_invisible_codes, plain_text)
     if has_invisible:
         width_fn = _visible_width
     else:
         width_fn = wcswidth
 
-    # align columns
-    aligns = [numalign if ct in [int,float] else stralign for ct in coltypes]
+    if not isinstance(tablefmt, TableFormat):
+        tablefmt = _table_formats.get(tablefmt, _table_formats["simple"])
+
+    if tablefmt.with_align:
+        # align columns
+        aligns = [numalign if ct in [int,float] else stralign for ct in coltypes]
+    else:
+        aligns = [False for ct in coltypes]
     minwidths = [width_fn(h) + MIN_PADDING for h in headers] if headers else [0]*len(cols)
     cols = [_align_column(c, a, minw, has_invisible)
             for c, a, minw in zip(cols, aligns, minwidths)]
 
     if headers:
         # align headers and add headers
         t_cols = cols or [['']] * len(headers)
-        t_aligns = aligns or [stralign] * len(headers)
+        if tablefmt.with_align:
+            t_aligns = aligns or [stralign] * len(headers)
+        else:
+            t_aligns = [False for ct in coltypes]
         minwidths = [max(minw, width_fn(c[0])) for minw, c in zip(minwidths, t_cols)]
         headers = [_align_header(h, a, minw)
                    for h, a, minw in zip(headers, t_aligns, minwidths)]
         rows = list(zip(*cols))
     else:
         minwidths = [width_fn(c[0]) for c in cols]
         rows = list(zip(*cols))
 
-    if not isinstance(tablefmt, TableFormat):
-        tablefmt = _table_formats.get(tablefmt, _table_formats["simple"])
-
     return _format_table(tablefmt, headers, rows, minwidths, aligns), rows
 
 
 def _build_simple_row(padded_cells, rowfmt):
     "Format row according to DataRow format without padding."
     begin, sep, end = rowfmt
     return (begin + sep.join(padded_cells) + end).rstrip()
```

### Comparing `mycli-1.8.1/mycli/sqlcompleter.py` & `mycli-1.9.0/mycli/sqlcompleter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,36 @@
 import logging
 from prompt_toolkit.completion import Completer, Completion
 from .packages.completion_engine import suggest_type
 from .packages.parseutils import last_word
 from .packages.special.favoritequeries import favoritequeries
 from re import compile, escape
 from .packages.tabulate import table_formats
-
-try:
-    from collections import Counter
-except ImportError:
-    # python 2.6
-    from .packages.counter import Counter
+from collections import Counter
 
 _logger = logging.getLogger(__name__)
 
 
 class SQLCompleter(Completer):
     keywords = ['ACCESS', 'ADD', 'ALL', 'ALTER TABLE', 'AND', 'ANY', 'AS',
-                'ASC', 'BEFORE', 'BEGIN', 'BETWEEN', 'BINARY', 'BY',
-                'CASE', 'CHAR', 'CHECK', 'COLUMN', 'COMMENT', 'COMMIT',
-                'CHANGE MASTER TO', 'CREATE', 'CURRENT', 'DATABASE', 'DATE',
+                'ASC', 'AUTO_INCREMENT', 'BEFORE', 'BEGIN', 'BETWEEN', 'BINARY', 'BY',
+                'CASE', 'CHAR', 'CHECK', 'COLUMN', 'COMMENT', 'COMMIT', 'CONSTRAINT',
+                'CHANGE MASTER TO', 'CHARACTER SET', 'COLLATE', 'CREATE', 'CURRENT', 'CURRENT_TIMESTAMP', 'DATABASE', 'DATE',
                 'DECIMAL', 'DEFAULT', 'DELETE FROM', 'DELIMITER', 'DESC',
-                'DESCRIBE', 'DROP', 'ELSE', 'END', 'ESCAPE', 'EXISTS',
-                'FILE', 'FLOAT', 'FOR', 'FORMAT', 'FROM', 'FULL', 'FUNCTION', 'GRANT',
+                'DESCRIBE', 'DROP', 'ELSE', 'END', 'ENGINE', 'ESCAPE', 'EXISTS',
+                'FILE', 'FLOAT', 'FOR', 'FOREIGN KEY', 'FORMAT', 'FROM', 'FULL', 'FUNCTION', 'GRANT',
                 'GROUP BY', 'HAVING', 'HOST', 'IDENTIFIED', 'IN', 'INCREMENT', 'INDEX',
-                'INSERT INTO', 'INTEGER', 'INTO', 'INTERVAL', 'IS', 'JOIN', 'LEFT',
+                'INSERT INTO', 'INTEGER', 'INTO', 'INTERVAL', 'IS', 'JOIN', 'KEY', 'LEFT',
                 'LEVEL', 'LIKE', 'LIMIT', 'LOCK', 'LOGS', 'LONG', 'MASTER', 'MODE',
                 'MODIFY', 'NOT', 'NULL', 'NUMBER', 'OFFSET', 'ON', 'OPTION', 'OR',
                 'ORDER BY', 'OUTER', 'OWNER', 'PASSWORD', 'PORT', 'PRIMARY',
-                'PRIVILEGES', 'PROCESSLIST', 'PURGE', 'RENAME', 'REPAIR', 'RESET',
-                'REVOKE', 'RIGHT', 'ROLLBACK','ROW', 'ROWS', 'SELECT', 'SESSION', 'SET',
+                'PRIVILEGES', 'PROCESSLIST', 'PURGE', 'REFERENCES', 'REGEXP', 'RENAME', 'REPAIR', 'RESET',
+                'REVOKE', 'RIGHT', 'ROLLBACK','ROW', 'ROWS', 'ROW_FORMAT', 'SELECT', 'SESSION', 'SET',
                 'SHARE', 'SHOW', 'SLAVE', 'SMALLINT', 'START', 'STOP', 'TABLE', 'THEN',
-                'TO', 'TRANSACTION', 'TRIGGER', 'TRUNCATE', 'UNION', 'UNIQUE', 'UPDATE',
+                'TO', 'TRANSACTION', 'TRIGGER', 'TRUNCATE', 'UNION', 'UNIQUE', 'UNSIGNED', 'UPDATE',
                 'USE', 'USER', 'USING', 'VALUES', 'VARCHAR', 'VIEW', 'WHEN', 'WHERE',
                 'WITH']
 
     functions = ['AVG', 'COUNT', 'DISTINCT', 'FIRST', 'FORMAT', 'LAST',
                  'LCASE', 'LEN', 'MAX', 'MIN', 'MID', 'NOW', 'ROUND', 'SUM',
                  'TOP', 'UCASE']
 
@@ -188,14 +183,15 @@
             self.all_completions.add(func[0])
 
     def set_dbname(self, dbname):
         self.dbname = dbname
 
     def reset_completions(self):
         self.databases = []
+        self.users = []
         self.show_items = []
         self.dbname = ''
         self.dbmetadata = {'tables': {}, 'views': {}, 'functions': {}}
         self.all_completions = set(self.keywords + self.functions)
 
     @staticmethod
     def find_matches(text, collection, start_only=False, fuzzy=True):
```

### Comparing `mycli-1.8.1/mycli/sqlexecute.py` & `mycli-1.9.0/mycli/sqlexecute.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         self.host = host
         self.port = port
         self.socket = socket
         self.charset = charset
         self.local_infile = local_infile
         self.ssl = ssl
         self._server_type = None
+        self.connection_id = None
         self.connect()
 
     def connect(self, database=None, user=None, password=None, host=None,
             port=None, socket=None, charset=None, local_infile=None, ssl=None):
         db = (database or self.dbname)
         user = (user or self.user)
         password = (password or self.password)
@@ -86,14 +87,16 @@
         self.user = user
         self.password = password
         self.host = host
         self.port = port
         self.socket = socket
         self.charset = charset
         self.ssl = ssl
+        # retrieve connection id
+        self.reset_connection_id()
 
     def run(self, statement):
         """Execute the sql in the database and return the results. The results
         are a list of tuples. Each tuple has 4 values
         (title, rows, headers, status).
         """
 
@@ -217,7 +220,20 @@
         elif 'percona' in version_comment:
             product_type = 'percona'
         else:
             product_type = 'mysql'
 
         self._server_type = (product_type, version)
         return self._server_type
+
+    def get_connection_id(self):
+        if not self.connection_id:
+            self.reset_connection_id()
+        return self.connection_id
+
+    def reset_connection_id(self):
+        # Remember current connection id
+        _logger.debug('Get current connection id')
+        res = self.run('select connection_id()')
+        for title, cur, headers, status in res:
+            self.connection_id = cur.fetchone()[0]
+        _logger.debug('Current connection id: %s', self.connection_id)
```

### Comparing `mycli-1.8.1/mycli.egg-info/PKG-INFO` & `mycli-1.9.0/mycli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.1
 Name: mycli
-Version: 1.8.1
+Version: 1.9.0
 Summary: CLI for MySQL Database. With auto-completion and syntax highlighting.
 Home-page: http://mycli.net
 Author: Amjith Ramanujam
 Author-email: amjith[dot]r[at]gmail.com
 License: UNKNOWN
 Description: CLI for MySQL Database. With auto-completion and syntax highlighting.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mycli-1.8.1/mycli.egg-info/SOURCES.txt` & `mycli-1.9.0/mycli.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,25 +19,22 @@
 mycli/myclirc
 mycli/sqlcompleter.py
 mycli/sqlexecute.py
 mycli.egg-info/PKG-INFO
 mycli.egg-info/SOURCES.txt
 mycli.egg-info/dependency_links.txt
 mycli.egg-info/entry_points.txt
-mycli.egg-info/pbr.json
 mycli.egg-info/requires.txt
 mycli.egg-info/top_level.txt
 mycli/../AUTHORS
 mycli/../SPONSORS
 mycli/packages/__init__.py
 mycli/packages/completion_engine.py
 mycli/packages/connection.py
-mycli/packages/counter.py
 mycli/packages/expanded.py
-mycli/packages/ordereddict.py
 mycli/packages/parseutils.py
 mycli/packages/tabulate.py
 mycli/packages/special/__init__.py
 mycli/packages/special/dbcommands.py
 mycli/packages/special/favoritequeries.py
 mycli/packages/special/iocommands.py
 mycli/packages/special/main.py
```

### Comparing `mycli-1.8.1/PKG-INFO` & `mycli-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.1
 Name: mycli
-Version: 1.8.1
+Version: 1.9.0
 Summary: CLI for MySQL Database. With auto-completion and syntax highlighting.
 Home-page: http://mycli.net
 Author: Amjith Ramanujam
 Author-email: amjith[dot]r[at]gmail.com
 License: UNKNOWN
 Description: CLI for MySQL Database. With auto-completion and syntax highlighting.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mycli-1.8.1/README.md` & `mycli-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 -----------
 
 If you already know how to install python packages, then you can install it via pip:
 
 You might need sudo on linux.
 
 ```
-$ pip install mycli
+$ pip install -U mycli
 ```
 
 or
 
 ```
 $ brew update && brew install mycli  # Only on OS X
 ```
@@ -112,17 +112,25 @@
 
 My email: amjith.r@gmail.com
 
 Twitter: [@amjithr](http://twitter.com/amjithr)
 
 ## Detailed Install Instructions:
 
-### RHEL, Centos, Fedora:
+### Fedora
 
-I haven't built an RPM package for mycli yet. So please use `pip` to install `mycli`. You can install pip on your system using:
+Fedora has a package available for mycli, install it using dnf:
+
+```
+$ sudo dnf install mycli
+```
+
+### RHEL, Centos
+
+I haven't built an RPM package for mycli for RHEL or Centos yet. So please use `pip` to install `mycli`. You can install pip on your system using:
 
 ```
 $ sudo yum install python-pip
 ```
 
 Once that is installed, you can install mycli as follows:
 
@@ -139,15 +147,15 @@
 which is quite literally the backbone library, that made this app possible.
 Jonathan has also provided valuable feedback and support during the development
 of this app.
 
 [Click](http://click.pocoo.org/3/) is used for command line option parsing
 and printing error messages.
 
-Thanks to [PyMysql](http://www.pymysql.org/) for a pure python adapter to MySQL database.
+Thanks to [PyMysql](https://github.com/PyMySQL/PyMySQL) for a pure python adapter to MySQL database.
 
 [Tabulate](https://pypi.python.org/pypi/tabulate) library is used for pretty printing the output of tables.
 
 
 ### Compatibility
 
 Tests have been run on OS X and Linux.
```

### Comparing `mycli-1.8.1/setup.py` & `mycli-1.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,24 +12,19 @@
 description = 'CLI for MySQL Database. With auto-completion and syntax highlighting.'
 
 install_requirements = [
     'click >= 4.1',
     'Pygments >= 2.0',  # Pygments has to be Capitalcased. WTF?
     'prompt_toolkit>=1.0.0,<1.1.0',
     'PyMySQL >= 0.6.2',
-    'sqlparse>=0.2.0,<0.2.2',
+    'sqlparse>=0.2.2,<0.3.0',
     'configobj >= 5.0.6',
+    'pycryptodome',
 ]
 
-# pycrypto is a hard package to install on Windows, so we make it an optional
-# dependency. When it's installed, we can read mylogin.cnf, when it is not
-# available, we skip reading mylogin.cnf and print a warning message.
-if platform.system() != 'Windows':
-    install_requirements.append('pycrypto >= 2.6.1')
-
 setup(
         name='mycli',
         author='Amjith Ramanujam',
         author_email='amjith[dot]r[at]gmail.com',
         version=version,
         url='http://mycli.net',
         packages=find_packages(),
@@ -42,20 +37,20 @@
             mycli=mycli.main:cli
         ''',
         classifiers=[
             'Intended Audience :: Developers',
             'License :: OSI Approved :: BSD License',
             'Operating System :: Unix',
             'Programming Language :: Python',
-            'Programming Language :: Python :: 2.6',
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.3',
             'Programming Language :: Python :: 3.4',
             'Programming Language :: Python :: 3.5',
+            'Programming Language :: Python :: 3.6',
             'Programming Language :: SQL',
             'Topic :: Database',
             'Topic :: Database :: Front-Ends',
             'Topic :: Software Development',
             'Topic :: Software Development :: Libraries :: Python Modules',
             ],
         )
```

