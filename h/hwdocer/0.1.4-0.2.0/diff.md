# Comparing `tmp/hwdocer-0.1.4.tar.gz` & `tmp/hwdocer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdocer-0.1.4.tar", max compression
+gzip compressed data, was "hwdocer-0.2.0.tar", max compression
```

## Comparing `hwdocer-0.1.4.tar` & `hwdocer-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2583 2024-04-02 23:58:32.435476 hwdocer-0.1.4/doc/release.md
--rw-r--r--   0        0        0     1986 2024-04-03 00:04:57.802531 hwdocer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2845 2024-04-02 17:25:55.333825 hwdocer-0.1.4/readme.md
--rw-r--r--   0        0        0       22 2024-04-03 00:04:57.806531 hwdocer-0.1.4/src/hwdocer/__init__.py
--rw-r--r--   0        0        0      139 2024-03-26 14:58:45.867365 hwdocer-0.1.4/src/hwdocer/__main__.py
--rw-r--r--   0        0        0    16648 2024-04-03 00:00:14.658370 hwdocer-0.1.4/src/hwdocer/hwdocer.py
--rw-r--r--   0        0        0     4593 1970-01-01 00:00:00.000000 hwdocer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3134 2024-04-03 19:29:01.034792 hwdocer-0.2.0/doc/release.md
+-rw-r--r--   0        0        0     1986 2024-04-03 19:30:08.088584 hwdocer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2845 2024-04-03 19:29:01.034792 hwdocer-0.2.0/readme.md
+-rw-r--r--   0        0        0       22 2024-04-03 19:30:08.088584 hwdocer-0.2.0/src/hwdocer/__init__.py
+-rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.2.0/src/hwdocer/__main__.py
+-rw-r--r--   0        0        0    17957 2024-04-03 19:29:01.034792 hwdocer-0.2.0/src/hwdocer/hwdocer.py
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 hwdocer-0.2.0/PKG-INFO
```

### Comparing `hwdocer-0.1.4/doc/release.md` & `hwdocer-0.2.0/doc/release.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # HWDOCER releases
 
 See what is planned in the [roadmap][roadmap_file]
 
+## 0.2.0
+
+Release date: _2024-04-03_
+
+**Features:**
+
+- Automatic removal of undesired file format (wireviz) in output folder (multiple can be kept via `--hrs` args)
+
+**Fix:**
+
+- Wrapped wireviz and drawio call in silent subprocess to handle console pollution (unknown exception will still be raised)
+
 ## 0.1.4
 
 Release date: _2024-04-02_
 
 **Features:**
 
 - source files are now copied in output folder
@@ -17,30 +29,30 @@
 
 **Fix:**
 
 - image from harnesses are now correctly copied into a similar folder structure inside output folder
 
 **Known problems:**
 
-- drawio calls throws some error in console and logs
-- wireviz bad syntax throws stacktrace in console and logs
+- **[corrected in 0.2.0]** drawio calls throws some error in console and logs
+- **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - leave a lot of undesired generated files in input and output folders
 
 ## 0.1.3
 
 Release date: _2024-03-27_
 
 **Features:**
 
 - copy all images defined in harness with tag `image`.`src` to output path (for html correct render)
 
 **Known problems:**
 
-- drawio calls throws some error in console and logs
-- wireviz bad syntax throws stacktrace in console and logs
+- **[corrected in 0.2.0]** drawio calls throws some error in console and logs
+- **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - **[corrected in 0.1.4]** image copy doesn't recreate sub-folder structure into output destination
 - leave a lot of undesired generated files in input and output folders
 
 ## 0.1.2
 
 Release date: _2024-03-27_
 
@@ -51,30 +63,30 @@
 
 **Change:**
 
 - Changed input file search to use glob instead of os.walk
 
 **Known problems:**
 
-- drawio calls throws some error in console and logs
-- wireviz bad syntax throws stacktrace in console and logs
+- **[corrected in 0.2.0]** drawio calls throws some error in console and logs
+- **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - leave a lot of undesired generated files in input and output folders
 
 ## 0.1.1
 
 Release date: _2024-03-26_
 
 **Fix:**
 
 - Project publishing metadata added/corrected
 
 **Known problems:**
 
-- drawio calls throws some error in console and logs
-- wireviz bad syntax throws stacktrace in console and logs
+- **[corrected in 0.2.0]** drawio calls throws some error in console and logs
+- **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - leave a lot of undesired generated files in input and output folders
 
 ## 0.1.0
 
 Release date: _2024-03-26_
 
 **Features:**
@@ -86,14 +98,14 @@
 - wireviz automatic drawing
 - basic functional test for diagram and harness
 - selectable verbosity in console and log (one argument for both)
 - buildable & deployable with poetry
 
 **Known problems:**
 
-- drawio calls throws some error in console and logs
-- wireviz bad syntax throws stacktrace in console and logs
+- **[corrected in 0.2.0]** drawio calls throws some error in console and logs
+- **[corrected in 0.2.0]** wireviz bad syntax throws stacktrace in console and logs
 - leave a lot of undesired generated files in input and output folders
 
 ---
 
 [roadmap_file]: roadmap.md
```

### Comparing `hwdocer-0.1.4/pyproject.toml` & `hwdocer-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwdocer"
-version = "0.1.4"
+version = "0.2.0"
 description = "Wireviz, drawio and other documentation build tool"
 authors = ["Laurence DV <laurencedv@realee.tech>"]
 homepage = "https://gitlab.com/real-ee/public/hwdocer"
 repository = "https://gitlab.com/real-ee/public/hwdocer"
 documentation = "https://gitlab.com/real-ee/public/hwdocer/-/tree/master/doc"
 readme = "readme.md"
 license = "GPL-3.0-or-later"
@@ -39,15 +39,15 @@
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 bumpver = "^2023.1129"
 pytest = "^7.4.0"
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Version increase {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `hwdocer-0.1.4/readme.md` & `hwdocer-0.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `hwdocer-0.1.4/src/hwdocer/hwdocer.py` & `hwdocer-0.2.0/src/hwdocer/hwdocer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
+import errno
 import sys
 import glob
 import shutil
 import argparse
 import pathlib
 import time
 import yaml
+from subprocess import DEVNULL, check_call
 
 # logging
 from multiprocessing import Process, Queue, current_process, Pool
 from logging.handlers import TimedRotatingFileHandler, QueueHandler
 import logging
 
 
@@ -25,14 +27,16 @@
     __search_folder__ = '/**/'
     __suffix_hrs__ = '.yml'
     __suffix_dia__ = '.drawio'
     __search_hrs__ = '*' + __suffix_hrs__
     __search_dia__ = '*' + __suffix_dia__
     __def_dia_format__ = 'png'
     __def_hrs_format__ = 'html'
+    __dia_format_choices__ = ['png', 'pdf', 'jpg', 'svg', 'vsdx', 'xml']
+    __hrs_format_choices__ = ['png', 'html', 'pdf(NOT IMPLEMENTED)', 'gv', 'svg', 'bom']
     __verb_levels__ = [logging.CRITICAL, logging.ERROR, logging.WARNING, logging.INFO, logging.DEBUG]
 
     """automatic drawing of drawio diagrams and wireviz harnesses tool"""
 
     def __init__(self, arg):
         super(HwDocer, self).__init__()
         self.time_start = time.time()
@@ -41,29 +45,30 @@
         # Arguments
         argParse = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
         argParse.add_argument("-v", "--verbose", help="Increase the verbosity level (can be used upto 4 times)", action='count', default=0)
         argParse.add_argument("-i", "--input", help="input directory to search for docs to build", default=self.__def_input__, type=pathlib.Path)
         argParse.add_argument("-o", "--output", help="output build directory", default=self.__def_output__, type=pathlib.Path)
         argParse.add_argument("-w", "--worker", help="maximum number of worker process to spawn", default=self.__def_worker_nb__, type=int)
         argParse.add_argument("-t", "--timeout", help="maximum execution time allowed (in sec)", default=self.__def_timeout__, type=int)
-        argParse.add_argument("--dia-format", help="diagram output file format", choices=['png', 'pdf', 'jpg', 'svg', 'vsdx', 'xml'], default=self.__def_dia_format__, type=str)
-        argParse.add_argument("--hrs-format", help="harness output files to keep (many can be choosen)", choices=['png', 'html', 'pdf(NOT IMPLEMENTED)', 'gv', 'svg', 'bom'], default=self.__def_hrs_format__, action='append', type=str)
+        argParse.add_argument("--dia", help="diagram output file format", choices=self.__dia_format_choices__, default=self.__def_dia_format__, type=str)
+        argParse.add_argument("--hrs", help="harness output files to keep (many can be choosen)", choices=self.__hrs_format_choices__, default=self.__def_hrs_format__, nargs='*', type=str)
         self.args = argParse.parse_args()  # Parse & save all arguments
 
         # region Logger
         self.verbosity = self.__verb_levels__[min(self.args.verbose, len(self.__verb_levels__) - 1)]
         self.log_q = Queue()
 
         # main object logger
         self.logger = logging.getLogger('hwdocer')
         self.logger.setLevel(self.verbosity)
         self.logger.addHandler(QueueHandler(self.log_q))
 
         logger_p = Process(target=self.logger_process, args=(self.log_q,))
         logger_p.start()
+        self.logger.debug(f'log queue: {id(self.log_q)}')
         # endregion
 
         # param - input files
         current_directory = os.getcwd()
         if not os.path.isabs(self.args.input):
             self.src_path = os.path.normpath(os.path.join(current_directory, self.args.input))
         else:
@@ -86,20 +91,25 @@
         if self.args.timeout < 0:
             self.exec_timeout = self.__def_timeout__
         else:
             self.exec_timeout = self.args.timeout
         self.logger.debug(f'args - timeout: {self.exec_timeout} sec')
 
         # param - diagram format
-        self.dia_format = self.args.dia_format
+        self.dia_format = self.args.dia
         self.logger.debug(f'args - dia format: {self.dia_format}')
 
+        # arg - harness format
+        self.hrs_format = self.args.hrs
+        self.logger.debug(f'args - hrs format: {self.hrs_format}')
+
         # start with empty work queues
         self.work_q = Queue()
-        self.built_q = Queue()
+        self.done_q = Queue()
+        self.logger.debug(f'work queue: {id(self.work_q)}, done queue: {id(self.done_q)}')
 
         self.time_creation = time.time()
         self.logger.debug(f'{__name__} created successfully in {self.time_creation - self.time_start:.6f} sec')
 
     def _search_and_copy_files(self):
         self.logger.debug(f'searching in \'{self.src_path}\' for {self.__search_folder__}')     # first search all subfolder to known the complete structure
 
@@ -109,24 +119,24 @@
 
             # searching for harnesses
             self.logger.debug(f'searching in \'{folder}\' for {self.__search_hrs__}')
             for file in glob.iglob(folder + self.__search_hrs__):
                 self.logger.debug(f'harness found: \'{os.path.basename(file)}\'')
                 copied_file = self._copy_src_files(file)
                 if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.info(f'work added: \'{os.path.basename(copied_file)}\'')
+                    self.logger.debug(f'work added: \'{os.path.basename(copied_file)}\'')
                     self.work_q.put(copied_file)
 
             # searching for diagrams
             self.logger.debug(f'searching in \'{folder}\' for {self.__search_dia__}')
             for file in glob.iglob(folder + self.__search_dia__):
                 self.logger.debug(f'diagram found: \'{os.path.basename(file)}\'')
                 copied_file = self._copy_src_files(file)
                 if os.path.basename(copied_file) == os.path.basename(file):     # ensure the copied file atleast as the same name as original
-                    self.logger.info(f'work added: \'{os.path.basename(copied_file)}\'')
+                    self.logger.debug(f'work added: \'{os.path.basename(copied_file)}\'')
                     self.work_q.put(copied_file)
 
         self.time_search = time.time()
         self.logger.info(f'found {self.work_q.qsize()} buildable files in {self.time_search - self.time_creation:.6f} sec')
 
     def _prep_output(self):
         self.logger.debug(f'outut folder preparation')
@@ -139,75 +149,76 @@
                 os.makedirs(self.dst_path)
             else:
                 self.logger.debug(f'output folder: \'{self.dst_path}\' already existed')
         except Exception as e:
             self.logger.error(f'failed to create output folder \'{self.dst_path}\'')
             raise e
 
+    def _silentremove(self, file):
+        try:
+            os.remove(file)
+        except OSError as e:
+            self.logger.debug(f'tried to delete \'{file}\' but wasn\'t present')
+            if e.errno != errno.ENOENT:
+                raise
+
     def build_hrs(self, hrs) -> int:
         self.logger.info(f'hrs building: \'{os.path.basename(hrs)}\'')
         exec_status = -1
 
         # Building
         try:
-            exec_status = os.system(f'wireviz {hrs}')
+            exec_status = check_call(['wireviz', hrs], stdout=DEVNULL, stderr=DEVNULL)
         except Exception as e:
-            raise e
+            self.logger.error(f'wireviz failed: \'{e}\'')
 
         # Cleanup unwanted output
-        # TODO: implement the cleanup phase
+        for hrsformat in self.__hrs_format_choices__:   # delete all files that weren't mentionned to be kept
+            if hrsformat not in self.hrs_format:
+                # handle special cases
+                if hrsformat == 'bom':
+                    hrsformat = 'bom.tsv'   # extension of bom file is special
+                elif hrsformat == 'pdf(NOT IMPLEMENTED)':
+                    hrsformat = 'pdf'
+                # delete the file with absolute path
+                file2del = os.path.dirname(hrs) + '/' + pathlib.Path(hrs).stem + '.' + hrsformat
+                self.logger.debug(f'deleting file \'{file2del}\'')
+                self._silentremove(file2del)
 
-        #     # move to build folder and cleanup
-        #     try:
-        #         name, extension = os.path.basename(hrs).split('.')
-        #         os.chdir(os.path.dirname(hrs))
-        #         shutil.copy(name + '.bom.tsv', outPath)
-        #         os.remove(name + '.bom.tsv')
-        #         shutil.copy(name + '.gv', outPath)
-        #         os.remove(name + '.gv')
-        #         shutil.copy(name + '.html', outPath)
-        #         os.remove(name + '.html')
-        #         shutil.copy(name + '.png', outPath)
-        #         os.remove(name + '.png')
-        #         shutil.copy(name + '.svg', outPath)
-        #         os.remove(name + '.svg')
-        #     except Exception as e:
-        #         print(e)
-        #         pass
         self.logger.debug(f'hrs built: \'{hrs}\'')
         return exec_status
 
     def build_dia(self, dia) -> int:
         self.logger.info(f'dia building: \'{os.path.basename(dia)}\'')
         exec_status = -1
 
         # Building
         try:
-            exec_status = os.system(f'drawio -x -t -f {self.dia_format} {dia}')
+            exec_status = check_call(['drawio', '-x', '-t', '-f', self.dia_format, dia], stdout=DEVNULL, stderr=DEVNULL)
         except Exception as e:
-            raise e
+            self.logger.error(f'drawio failed: \'{e}\'')
 
         self.logger.debug(f'dia built \'{dia}\'')
         return exec_status
 
-    def _get_diffpath(self, basepath: pathlib.Path, filepath: pathlib.Path) -> str:
+    def _get_diffpath(self, basepath: pathlib.Path, filepath: pathlib.Path) -> pathlib.Path:
         subpath = '.'
         if basepath is not None and filepath is not None:
             commonpath = os.path.commonpath([basepath, filepath])
             subpath = os.path.dirname(filepath).replace(commonpath, '')
-        return str(subpath)
+        return subpath
 
     def _copy_src_files(self, file: pathlib.Path) -> pathlib.Path:
         if file is not None:
             file = pathlib.Path(file)  # ensure the file is a valid path
             resulting_file = pathlib.Path()
             # 1. Create subfolder in destination
             try:
                 subfolder = self._get_diffpath(self.src_path, file)
-                destination = str(self.dst_path) + str(subfolder)
+                destination = pathlib.Path(str(self.dst_path) + str(subfolder))
                 if not os.path.exists(destination):
                     self.logger.info(f'creating folder: \'{destination}\'')
                     os.makedirs(destination)
                 else:
                     self.logger.debug(f'folder: \'{destination}\' already existed')
             except Exception as e:
                 self.logger.error(f'failed to create folder: \'{destination}\'')
@@ -223,28 +234,32 @@
             # 3. If harness, also copy images
             try:
                 if file.suffix == self.__suffix_hrs__:
                     img_list = self._get_all_img_path_from_hrs(file)
                     if len(img_list) > 0:
                         self.logger.info(f'copying {len(img_list)} image(s) linked in \'{file}\'')
                     for image in img_list:
-                        destination = self._get_diffpath(self.src_path, image)
-                        destination = str(self.dst_path) + destination
+                        # compute the complete destination path
+                        subfolder = self._get_diffpath(self.src_path, image)
+                        destination = pathlib.Path(str(self.dst_path) + str(subfolder) + '/' + os.path.basename(image))
                         self.logger.debug(f'copying image: \'{image}\' to \'{destination}\'')
+                        # make sure directory exist at destination
+                        os.makedirs(os.path.dirname(destination), exist_ok=True)
+
                         if not os.path.exists(os.path.join(destination, os.path.basename(image))):
                             shutil.copy2(image, destination)
                         else:
                             self.logger.debug(f'\'{image}\' already exist')
             except Exception as e:
                 self.logger.warning(f'failed to copy image: \'{destination}\'')
 
             self.logger.debug(f'successfully copied: \'{resulting_file}\'')
             return resulting_file
 
-    def _get_all_img_path_from_hrs(self, hrs_path):
+    def _get_all_img_path_from_hrs(self, hrs_path: pathlib.Path) -> list:
         image_list = []
 
         try:
             with open(hrs_path, 'r') as file:
                 yaml_content = yaml.safe_load(file)
                 for key, val in yaml_content.items():
                     if key == 'connectors' or key == 'cables':      # top level
@@ -274,47 +289,56 @@
 
         # 3. Start workers
         nb_of_file = self.work_q.qsize()
         self.worker_nb = min(self.worker_nb, nb_of_file)   # worker number is the lowest of: number of file or argument passed
         self.logger.info(f'starting {self.worker_nb} workers')
         processes = []
         for i in range(self.worker_nb):
-            processes.append(Process(target=self.worker_process, args=(self.log_q, self.work_q, self.built_q), daemon=True))
+            processes.append(Process(target=self.worker_process, args=(self.log_q, self.work_q, self.done_q), daemon=True))
             processes[i].start()
 
         # 4. Wait for results
         while True:
-            if self.built_q.qsize() >= nb_of_file:
+            if self.done_q.qsize() >= nb_of_file:
                 self.time_done = time.time()
                 self.logger.info(f'all file built in {self.time_done - self.time_search:.3f} sec')
                 break
             waited = time.time() - self.time_search
             if waited >= self.exec_timeout:
                 self.time_done = time.time()
                 self.logger.warning(f'timeout reached after {waited:.3f} sec')
+                for i in range(len(processes)):
+                    # TODO: send explicit stop signal to workers
+                    pass
                 break
             time.sleep(0.1)
 
         # graceful end of exec
         self.logger.info(f'P execution, pid: {current_process().pid}, total time: {self.time_done - self.time_start:.6f} sec')
         self.log_q.put(None)
         return status
 
-    def worker_process(self, log_q, q_in, q_out):
+    def worker_process(self, log_q: Queue, q_in: Queue, q_out: Queue) -> int:
         """worker isolated process to generate output files from input file
 
         Args:
             file (pathlib.Path): input source file
         """
         self.logger = logging.getLogger(f'worker {current_process().pid}')
         self.logger.setLevel(self.verbosity)
         self.logger.addHandler(QueueHandler(log_q))
-        self.logger.debug(f'started with in: {q_in} out: {q_out}')
+        self.logger.debug(f'started with in: {id(q_in)} out: {id(q_out)}')
 
         while True:
+            # X. handle special message to kill worker
+            # if work == 'STOP':
+            #     self.logger.debug(f'received explicit stop')
+            #     break
+            # TODO: add rx signal to break execution
+
             # 1. take one file to build
             work = pathlib.Path(q_in.get())
             self.logger.debug(f'working on {work}')
 
             # 2. build the file
             exec_status = 0
             if work.suffix == self.__suffix_hrs__:
@@ -322,31 +346,28 @@
             elif work.suffix == self.__suffix_dia__:
                 exec_status = self.build_dia(work)
             else:
                 self.logger.error(f'work given is not valid: {work}')
             if exec_status != 0:
                 self.logger.error(f'{work} did not complete correctly with code: {exec_status}')
 
-            # 3. cleanup
-            # TODO: cleanup the copied source file in output folder
+            # 3. cleanup src file
+            self._silentremove(work)
 
             # 4. put the file on the build list
             q_out.put(work)
 
             # X. stop when we are at the end of the queue
             if q_in.qsize() <= 0:
                 break
 
-        # logger.debug(f'file: {file}')
-        # self._copy_src_files(file)
-
         self.logger.info(f'done')
         return 0
 
-    def logger_process(self, queue):
+    def logger_process(self, queue: Queue) -> int:
         """ logging isolated process
 
         Args:
             queue (Queue): logging queue receiving all logs to be saved
         """
 
         logger = logging.getLogger('logger')
```

### Comparing `hwdocer-0.1.4/PKG-INFO` & `hwdocer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdocer
-Version: 0.1.4
+Version: 0.2.0
 Summary: Wireviz, drawio and other documentation build tool
 Home-page: https://gitlab.com/real-ee/public/hwdocer
 License: GPL-3.0-or-later
 Keywords: drawio,wireviz,toolchain,automation,documentation
 Author: Laurence DV
 Author-email: laurencedv@realee.tech
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Requires-Dist: drawio (>=0.0.10,<0.0.11)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
```

