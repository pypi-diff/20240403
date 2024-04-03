# Comparing `tmp/eons-3.1.4.tar.gz` & `tmp/eons-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-3.1.4.tar", last modified: Wed Mar 13 05:15:33 2024, max compression
+gzip compressed data, was "eons-3.1.5.tar", last modified: Wed Apr  3 14:40:58 2024, max compression
```

## Comparing `eons-3.1.4.tar` & `eons-3.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.218891 eons-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-03-13 05:15:33.218891 eons-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25801 2024-03-13 05:15:23.000000 eons-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.214891 eons-3.1.4/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.214891 eons-3.1.4/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-13 05:15:30.000000 eons-3.1.4/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   128835 2024-03-13 05:15:30.000000 eons-3.1.4/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.214891 eons-3.1.4/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 05:15:30.000000 eons-3.1.4/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.218891 eons-3.1.4/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 05:15:30.000000 eons-3.1.4/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_install_with_pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-13 05:15:17.000000 eons-3.1.4/pkg/eons/resolve/resolve_namespace_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:15:33.218891 eons-3.1.4/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-03-13 05:15:33.000000 eons-3.1.4/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-13 05:15:33.000000 eons-3.1.4/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 05:15:33.000000 eons-3.1.4/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-13 05:15:33.000000 eons-3.1.4/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-13 05:15:33.000000 eons-3.1.4/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-13 05:15:30.000000 eons-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-13 05:15:33.218891 eons-3.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.454152 eons-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-04-03 14:40:58.454152 eons-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25801 2024-04-03 14:40:49.000000 eons-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.446152 eons-3.1.5/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.450152 eons-3.1.5/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 14:40:56.000000 eons-3.1.5/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128868 2024-04-03 14:40:56.000000 eons-3.1.5/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.450152 eons-3.1.5/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:40:56.000000 eons-3.1.5/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.454152 eons-3.1.5/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:40:56.000000 eons-3.1.5/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_install_with_pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-03 14:40:42.000000 eons-3.1.5/pkg/eons/resolve/resolve_namespace_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:40:58.454152 eons-3.1.5/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-04-03 14:40:58.000000 eons-3.1.5/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 14:40:58.000000 eons-3.1.5/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:40:58.000000 eons-3.1.5/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 14:40:58.000000 eons-3.1.5/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 14:40:58.000000 eons-3.1.5/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 14:40:56.000000 eons-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-03 14:40:58.454152 eons-3.1.5/setup.cfg
```

### Comparing `eons-3.1.4/PKG-INFO` & `eons-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 3.1.4
+Version: 3.1.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: eot
+Requires-Dist: pyyaml
+Requires-Dist: requests_futures
 Requires-Dist: jsonpickle
+Requires-Dist: eot
 Requires-Dist: requests
 Requires-Dist: tqdm
-Requires-Dist: requests_futures
-Requires-Dist: pyyaml
 
 # Eons Python Framework
 
 The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
```

### Comparing `eons-3.1.4/README.md` & `eons-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons/eons.py` & `eons-3.1.5/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 import logging
-import os
-import shutil
-import dis
+import sys
+import traceback
+import jsonpickle
 import inspect
-import types
+import gc
 from copy import deepcopy
-from copy import copy
-import builtins
-import sys
+import operator
+import os
 import pkgutil
 import importlib.machinery
 import importlib.util
-import traceback
-import jsonpickle
-import gc
-from pathlib import Path
-from subprocess import Popen
-from subprocess import PIPE
-from subprocess import STDOUT
-import re
+import types
+import shutil
+import dis
+from copy import copy
+import builtins
 import argparse
 import requests
 import importlib
 import yaml
 from requests_futures.sessions import FuturesSession
+from pathlib import Path
 from tqdm import tqdm
 from zipfile import ZipFile
 from eot import EOT
-import operator
+from subprocess import Popen
+from subprocess import PIPE
+from subprocess import STDOUT
+import re
 
 ######## START CONTENT ########
-def INVALID_NAME():
-	return "INVALID_NAME"
-
+#from .Executor import Executor # don't import this, it'll be circular!
 class ActualType(type):
 	def __repr__(self):
 		return self.__name__
 
 class GlobalError(Exception, metaclass=ActualType): pass
 
 class NotInstantiableError(Exception, metaclass=ActualType): pass
@@ -65,14 +63,265 @@
 
 class PackageError(Exception, metaclass=ActualType): pass
 
 class MethodPendingPopulation(Exception, metaclass=ActualType): pass
 
 class ConstellatusError(Exception, metaclass=ActualType): pass
 
+# util is a namespace for any miscellaneous utilities.
+# You cannot create a util.
+class util:
+	def __init__(this):
+		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
+
+	#dot.notation access to dictionary attributes
+	class DotDict(dict):
+		__getattr__ = dict.get
+		__setattr__ = dict.__setitem__
+		__delattr__ = dict.__delitem__
+
+		def __deepcopy__(this, memo=None):
+			return util.DotDict(deepcopy(dict(this), memo=memo))
+
+	# DotDict doesn't pickle right, since it's a class and not a native dict.
+	class DotDictPickler(jsonpickle.handlers.BaseHandler):
+		def flatten(this, dotdict, data):
+			return dict(dotdict)
+
+	@staticmethod
+	def RecursiveAttrFunc(func, obj, attrList):
+		attr = attrList.pop(0)
+		if (not attrList):
+			return eval(f"{func}attr(obj, attr)")
+		if (not hasattr(obj, attr)):
+			raise AttributeError(f"{obj} has not attribute '{attr}'")
+		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
+
+	@staticmethod
+	def HasAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
+
+	@staticmethod
+	def GetAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
+
+	@staticmethod
+	def SetAttr(obj, attrStr):
+		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
+
+
+	@staticmethod
+	def LogStack():
+		logging.debug(traceback.format_exc())
+
+
+	class console:
+
+		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
+
+		saturationCode = {
+			'dark': 3,
+			'light': 9
+		}
+
+		foregroundCodes = {
+			'black': 0,
+			'red': 1,
+			'green': 2,
+			'yellow': 3,
+			'blue': 4,
+			'magenta': 5,
+			'cyan': 6,
+			'white': 7
+		}
+
+		backgroundCodes = {
+			'none': 0,
+			'black': 40,
+			'red': 41,
+			'green': 42,
+			'yellow': 43,
+			'blue': 44,
+			'magenta': 45,
+			'cyan': 46,
+			'white': 47,
+		}
+
+		styleCodes = {
+			'none': 0,
+			'bold': 1,
+			'faint': 2, # Not widely supported.
+			'italic': 3, # Not widely supported.
+			'underline': 4,
+			'blink_slow': 5,
+			'blink_fast': 6, # Not widely supported.
+			'invert': 7,
+			'conceal': 8, # Not widely supported.
+			'strikethrough': 9, # Not widely supported.
+			'frame': 51,
+			'encircle': 52,
+			'overline': 53
+		}
+
+		@classmethod
+		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
+			if (styles is None):
+				styles = []
+			#\x1b may also work.
+			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
+			if (background != 'none'):
+				compiledCode += f";{cls.backgroundCodes[background]}"
+			if (styles):
+				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
+			compiledCode += 'm'
+			return compiledCode
+
+		resetStyle = "\033[0m"
+
+
+	# Add a logging level
+	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
+	@staticmethod
+	def AddLoggingLevel(level, value):
+		levelName = level.upper()
+		methodName = level.lower()
+
+		if hasattr(logging, levelName):
+			raise AttributeError('{} already defined in logging module'.format(levelName))
+		if hasattr(logging, methodName):
+			raise AttributeError('{} already defined in logging module'.format(methodName))
+		if hasattr(logging.getLogger(), methodName):
+			raise AttributeError('{} already defined in logger class'.format(methodName))
+
+		# This method was inspired by the answers to Stack Overflow post
+		# http://stackoverflow.com/q/2183233/2988730, especially
+		# http://stackoverflow.com/a/13638084/2988730
+		def logForLevel(this, message, *args, **kwargs):
+			if this.isEnabledFor(value):
+				this._log(value, message, args, **kwargs)
+		def logToRoot(message, *args, **kwargs):
+			logging.log(value, message, *args, **kwargs)
+
+		logging.addLevelName(value, levelName)
+		setattr(logging, levelName, value)
+		setattr(logging.getLogger(), methodName, logForLevel)
+		setattr(logging, methodName, logToRoot)
+
+	@staticmethod
+	def forerunner(forerunner, *forerunnerArgs, **forerunnerKwargs):
+		def WrapperFactory(function):
+			def Wrapper(*functionArgs, **functionKwargs):
+				forerunner(*forerunnerArgs, **forerunnerKwargs)
+				return function(*functionArgs, **functionKwargs)
+			return Wrapper
+		return WrapperFactory
+	
+
+	class BlackMagick:
+
+		@staticmethod
+		def InjectIntoModule(source, name, value):
+			moduleToHack = inspect.getmodule(source)
+			setattr(moduleToHack, name, value)
+
+		# Identify the current function object, without any inputs.
+		# TODO: This is slow and implementation dependent. There should be a more optimized way to do this.
+		@staticmethod
+		def GetCurrentFunction():
+			code = inspect.currentframe().f_back.f_code
+			functype = type(lambda: None)
+			for func in gc.get_referrers(code):
+				if type(func) is functype and getattr(func, "__code__", None) is code:
+					return func
+			return None
+
+jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
+
+
+# @recoverable
+# Decorating another function with this method will engage the error recovery system provided by *this.
+# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
+# For more info, see Executor.ResolveError and the README.md
+def recoverable(function):
+	def RecoverableDecorator(obj, *args, **kwargs):
+		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
+	return RecoverableDecorator
+
+
+# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
+def RecoverableImplementation(obj, executor, function, *args, **kwargs):
+	try:
+		return function(obj, *args, **kwargs)
+	except FailedErrorResolution as fatal:
+		raise fatal
+	except Exception as e:
+		if (not executor.error.resolve):
+			raise e
+		return Recover(e, obj, executor, function, *args, **kwargs)
+
+
+def Recover(error, obj, executor, function, *args, **kwargs):
+	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
+	util.LogStack()
+
+	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
+	if (str(error) not in executor.error.resolution.stack.keys()):
+		executor.error.resolution.stack.update({str(error):[]})
+
+	# The executor.error.resolution.stack grows each time we invoke *this or (indirectly) executor.ResolveError().
+	# ResolveError is itself @recoverable.
+	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
+	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
+	executor.error.depth = executor.error.depth + 1
+
+	if (executor.error.depth > len(executor.error.resolution.stack.keys())+1):
+		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.error.depth}; STACK: {executor.error.resolution.stack}.")
+
+	successfullyRecovered = False
+	ret = None
+	resolvedBy = None
+	for i, res in enumerate(executor.error.resolvers):
+
+		logging.debug(f"Checking if {res} can fix '{error}'.")
+		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
+			# if no resolution was attempted, there's no need to re-run the function.
+			continue
+		try:
+			logging.debug(f"Trying function ({function}) again after applying {res}.")
+			resolvedBy = res
+			ret = function(obj, *args, **kwargs)
+			successfullyRecovered = True
+			break
+
+		except Exception as e2:
+			if (str(error) == str(e2)):
+				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
+				# Resolution failed. That's okay. Let's try the next.
+				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+				continue
+			else:
+				# The error changed, maybe we're making progress.
+				ret = Recover(e2, obj, executor, function, *args, **kwargs)
+				successfullyRecovered = True
+				break
+
+	if (successfullyRecovered):
+		executor.ClearErrorResolutionStack(str(error)) # success!
+		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
+		logging.debug(f"Error stack is now: {executor.error.resolution.stack}")
+		return ret
+
+	#  We failed to resolve the error. Die
+	sys.tracebacklimit = 0 # traceback is NOT helpful here.
+	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.error.resolution.stack}. See earlier logs (in debug) for traceback.")
+
+def INVALID_NAME():
+	return "INVALID_NAME"
+
+
 # The Eons way of tracking logical & extensible groupings.
 class Namespace:
 
 	def __init__(this, namespaces = None):
 		this.namespaces = []
 
 		if (isinstance(namespaces, str)):
@@ -256,182 +505,171 @@
 
 
 	# Sets valid to false.
 	def Invalidate(this):
 		this.valid = False
 
 
-# util is a namespace for any miscellaneous utilities.
-# You cannot create a util.
-class util:
-	def __init__(this):
-		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
 
-	#dot.notation access to dictionary attributes
-	class DotDict(dict):
-		__getattr__ = dict.get
-		__setattr__ = dict.__setitem__
-		__delattr__ = dict.__delitem__
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
 
-		def __deepcopy__(this, memo=None):
-			return util.DotDict(deepcopy(dict(this), memo=memo))
+		# The data *this contains.
+		this.data = []
 
-	# DotDict doesn't pickle right, since it's a class and not a native dict.
-	class DotDictPickler(jsonpickle.handlers.BaseHandler):
-		def flatten(this, dotdict, data):
-			return dict(dotdict)
 
-	@staticmethod
-	def RecursiveAttrFunc(func, obj, attrList):
-		attr = attrList.pop(0)
-		if (not attrList):
-			return eval(f"{func}attr(obj, attr)")
-		if (not hasattr(obj, attr)):
-			raise AttributeError(f"{obj} has not attribute '{attr}'")
-		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
 
-	@staticmethod
-	def HasAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
 
-	@staticmethod
-	def GetAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
 
-	@staticmethod
-	def SetAttr(obj, attrStr):
-		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
 
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
 
-	@staticmethod
-	def LogStack():
-		logging.debug(traceback.format_exc())
 
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
 
-	class console:
 
-		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
 
-		saturationCode = {
-			'dark': 3,
-			'light': 9
-		}
 
-		foregroundCodes = {
-			'black': 0,
-			'red': 1,
-			'green': 2,
-			'yellow': 3,
-			'blue': 4,
-			'magenta': 5,
-			'cyan': 6,
-			'white': 7
-		}
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
 
-		backgroundCodes = {
-			'none': 0,
-			'black': 40,
-			'red': 41,
-			'green': 42,
-			'yellow': 43,
-			'blue': 44,
-			'magenta': 45,
-			'cyan': 46,
-			'white': 47,
-		}
 
-		styleCodes = {
-			'none': 0,
-			'bold': 1,
-			'faint': 2, # Not widely supported.
-			'italic': 3, # Not widely supported.
-			'underline': 4,
-			'blink_slow': 5,
-			'blink_fast': 6, # Not widely supported.
-			'invert': 7,
-			'conceal': 8, # Not widely supported.
-			'strikethrough': 9, # Not widely supported.
-			'frame': 51,
-			'encircle': 52,
-			'overline': 53
-		}
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
 
-		@classmethod
-		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
-			if (styles is None):
-				styles = []
-			#\x1b may also work.
-			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
-			if (background != 'none'):
-				compiledCode += f";{cls.backgroundCodes[background]}"
-			if (styles):
-				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
-			compiledCode += 'm'
-			return compiledCode
 
-		resetStyle = "\033[0m"
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
 
 
-	# Add a logging level
-	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
-	@staticmethod
-	def AddLoggingLevel(level, value):
-		levelName = level.upper()
-		methodName = level.lower()
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
 
-		if hasattr(logging, levelName):
-			raise AttributeError('{} already defined in logging module'.format(levelName))
-		if hasattr(logging, methodName):
-			raise AttributeError('{} already defined in logging module'.format(methodName))
-		if hasattr(logging.getLogger(), methodName):
-			raise AttributeError('{} already defined in logger class'.format(methodName))
 
-		# This method was inspired by the answers to Stack Overflow post
-		# http://stackoverflow.com/q/2183233/2988730, especially
-		# http://stackoverflow.com/a/13638084/2988730
-		def logForLevel(this, message, *args, **kwargs):
-			if this.isEnabledFor(value):
-				this._log(value, message, args, **kwargs)
-		def logToRoot(message, *args, **kwargs):
-			logging.log(value, message, *args, **kwargs)
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
 
-		logging.addLevelName(value, levelName)
-		setattr(logging, levelName, value)
-		setattr(logging.getLogger(), methodName, logForLevel)
-		setattr(logging, methodName, logToRoot)
 
-	@staticmethod
-	def forerunner(forerunner, *forerunnerArgs, **forerunnerKwargs):
-		def WrapperFactory(function):
-			def Wrapper(*functionArgs, **functionKwargs):
-				forerunner(*forerunnerArgs, **forerunnerKwargs)
-				return function(*functionArgs, **functionKwargs)
-			return Wrapper
-		return WrapperFactory
-	
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
 
-	class BlackMagick:
 
-		@staticmethod
-		def InjectIntoModule(source, name, value):
-			moduleToHack = inspect.getmodule(source)
-			setattr(moduleToHack, name, value)
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
 
-		# Identify the current function object, without any inputs.
-		# TODO: This is slow and implementation dependent. There should be a more optimized way to do this.
-		@staticmethod
-		def GetCurrentFunction():
-			code = inspect.currentframe().f_back.f_code
-			functype = type(lambda: None)
-			for func in gc.get_referrers(code):
-				if type(func) is functype and getattr(func, "__code__", None) is code:
-					return func
-			return None
 
-jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
+
 
 
 # BackwardsCompatible classes simply map old names to new names.
 # The more compatible an object, the slower it is to access.
 # Compatibility can be adjusted by changing the compatibility member variable.
 # Compatibility values are versions in accordance with the eons versioning convention: https://eons.llc/convention/versioning
 class BackwardsCompatible:
@@ -607,93 +845,14 @@
 		except:
 			pass
 
 	@staticmethod
 	def GetLatest():
 		return ExecutorTracker.Instance().executors[-1]
 
-#from .Executor import Executor # don't import this, it'll be circular!
-
-# @recoverable
-# Decorating another function with this method will engage the error recovery system provided by *this.
-# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
-# For more info, see Executor.ResolveError and the README.md
-def recoverable(function):
-	def RecoverableDecorator(obj, *args, **kwargs):
-		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
-	return RecoverableDecorator
-
-
-# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
-def RecoverableImplementation(obj, executor, function, *args, **kwargs):
-	try:
-		return function(obj, *args, **kwargs)
-	except FailedErrorResolution as fatal:
-		raise fatal
-	except Exception as e:
-		if (not executor.error.resolve):
-			raise e
-		return Recover(e, obj, executor, function, *args, **kwargs)
-
-
-def Recover(error, obj, executor, function, *args, **kwargs):
-	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
-	util.LogStack()
-
-	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
-	if (str(error) not in executor.error.resolution.stack.keys()):
-		executor.error.resolution.stack.update({str(error):[]})
-
-	# The executor.error.resolution.stack grows each time we invoke *this or (indirectly) executor.ResolveError().
-	# ResolveError is itself @recoverable.
-	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
-	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
-	executor.error.depth = executor.error.depth + 1
-
-	if (executor.error.depth > len(executor.error.resolution.stack.keys())+1):
-		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.error.depth}; STACK: {executor.error.resolution.stack}.")
-
-	successfullyRecovered = False
-	ret = None
-	resolvedBy = None
-	for i, res in enumerate(executor.error.resolvers):
-
-		logging.debug(f"Checking if {res} can fix '{error}'.")
-		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
-			# if no resolution was attempted, there's no need to re-run the function.
-			continue
-		try:
-			logging.debug(f"Trying function ({function}) again after applying {res}.")
-			resolvedBy = res
-			ret = function(obj, *args, **kwargs)
-			successfullyRecovered = True
-			break
-
-		except Exception as e2:
-			if (str(error) == str(e2)):
-				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
-				# Resolution failed. That's okay. Let's try the next.
-				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
-				continue
-			else:
-				# The error changed, maybe we're making progress.
-				ret = Recover(e2, obj, executor, function, *args, **kwargs)
-				successfullyRecovered = True
-				break
-
-	if (successfullyRecovered):
-		executor.ClearErrorResolutionStack(str(error)) # success!
-		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
-		logging.debug(f"Error stack is now: {executor.error.resolution.stack}")
-		return ret
-
-	#  We failed to resolve the error. Die
-	sys.tracebacklimit = 0 # traceback is NOT helpful here.
-	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.error.resolution.stack}. See earlier logs (in debug) for traceback.")
-
 
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
@@ -2047,136 +2206,14 @@
 		if (not this.next):
 			return None
 
 		for next in this.next:
 			next(precursor=this)
 
 
-# The standard Functor extends Functor to add a set of standard members and methods.
-# This is similar to the standard library in C and C++
-# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
-class StandardFunctor(Functor):
-	def __init__(this, name="Standard Functor"):
-		super().__init__(name)
-
-	# Override this and do whatever!
-	# This is purposefully vague.
-	def Function(this):
-		pass
-
-
-	# Undo any changes made by UserFunction.
-	# Please override this too!
-	def Rollback(this):
-		pass
-
-
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
-	def DidFunctionSucceed(this):
-		return this.functionSucceeded
-
-
-	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
-	def DidRollbackSucceed(this):
-		return this.rollbackSucceeded
-
-
-	######## START: UTILITIES ########
-
-	# RETURNS: an opened file object for writing.
-	# Creates the path if it does not exist.
-	@method()
-	def CreateFile(this, file, mode="w+"):
-		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
-		return open(file, mode)
-
-	# Copy a file or folder from source to destination.
-	# This really shouldn't be so hard...
-	# root allows us to interpret '/' as something other than the top of the filesystem.
-	@method()
-	def Copy(this, source, destination, root='/'):
-		if (source.startswith('/')):
-			source = str(Path(root).joinpath(source[1:]).resolve())
-		else:
-			source = str(Path(source).resolve())
-		
-		destination = str(Path(destination).resolve())
-		
-		Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-		if (os.path.isfile(source)):
-			logging.debug(f"Copying file {source} to {destination}")
-			try:
-				shutil.copy(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		elif (os.path.isdir(source)):
-			logging.debug(f"Copying directory {source} to {destination}")
-			try:
-				shutil.copytree(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		else:
-			logging.error(f"Could not find source to copy: {source}")
-
-	# Delete a file or folder
-	@method()
-	def Delete(this, target):
-		if (not os.path.exists(target)):
-			logging.debug(f"Unable to delete nonexistent target: {target}")
-			return
-		if (os.path.isfile(target)):
-			logging.debug(f"Deleting file {target}")
-			os.remove(target)
-		elif (os.path.isdir(target)):
-			logging.debug(f"Deleting directory {target}")
-			try:
-				shutil.rmtree(target)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-
-	# Run whatever.
-	# DANGEROUS!!!!!
-	# RETURN: Return value and, optionally, the output as a list of lines.
-	@method()
-	def RunCommand(this, command, saveout=False, raiseExceptions=True):
-		logging.debug(f"================ Running command: {command} ================")
-		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
-		output = []
-		while process.poll() is None:
-			line = process.stdout.readline().decode('utf8')[:-1]
-			if (saveout):
-				output.append(line)
-			if (line):
-				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
-
-		message = f"Command returned {process.returncode}: {command}"
-		logging.debug(message)
-		if (raiseExceptions and process.returncode is not None and process.returncode):
-			raise CommandUnsuccessful(message)
-		
-		logging.debug(f"================ Completed command: {command} ================")
-		if (saveout):
-			return process.returncode, output
-		
-		return process.returncode
-	######## END: UTILITIES ########
-
-
 # Invoke the External Method machinery to fetch a Functor & return it.
 # This should be used with other eons.kinds
 class Inject(Functor):
 	def __init__(this, name = "Inject"):
 		super().__init__(name)
 		this.arg.kw.required.append('target')
 		this.arg.kw.optional['impl'] = 'External'
@@ -2236,352 +2273,22 @@
 				'default': inject(source)
 			})
 
 def public_methods(*args, **kwargs):
 	[kwargs.update({arg: arg}) for arg in args]
 	return PublicMethods()(**kwargs)
 
-def kind(
-	base = StandardFunctor,
-	**kwargs
-):
-	def ParseParameters(functor, args, source, ctor, strongType = False):
-		# Code duplicated from Method.PopulateFrom. See that class for more info.
-		for arg in args.values():
-			if (arg.name == 'constructor' or arg.name == '__init__'):
-				ctor.additions += f"{arg.default}\n"
-				continue
-
-			replaceWith = arg.name
-
-			# *args
-			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
-				replaceWith = 'this.args'
-
-			# **kwargs
-			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
-				replaceWith = 'this.kwargs'
-
-			# Normal argument
-			else:
-				replaceWith = f'this.{arg.name}'
-				shouldMapArg = arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]
-
-				if (arg.default != inspect.Parameter.empty):
-					if (isinstance(arg.default, Method)):
-						arg.default.name = arg.name # Rename the Functor to match what was requested
-						PrepareClassMethod(functor, arg.name, arg.default)
-						shouldMapArg = False
-					elif (isinstance(arg.default, AccessControl)):
-						# NOTE: arg.name is discarded.
-						functor, source, ctor = ParseParameters(
-							functor,
-							arg.default.parameters,
-							source,
-							ctor,
-							strongType=strongType
-						)
-						shouldMapArg = False
-					else:
-						defaultValue = arg.default
-						if (isinstance(arg.default, str)):
-							defaultValue = f"'{arg.default}'"
-						ctor.source.append(f"this.arg.kw.optional['{arg.name}'] = {defaultValue}")
-				else:
-					ctor.source.append(f"this.arg.kw.required.append('{arg.name}')")
-
-				if (strongType and hasattr(arg, 'type')):
-					ctor.source.append(f"""
-	try:
-		this.arg.type['{arg.name}'] = {arg.type.__name__}
-	except:
-		this.arg.type['{arg.name}'] = eons.SelfRegistering('{arg.type.__name__}')
-""")
-
-				if (shouldMapArg):
-					ctor.source.append(f"this.arg.mapping.append('{arg.name}')")
-
-			# Source mangling
-			# TODO: Expand as we have more solid test cases.
-			source = re.sub(fr"{arg.name}([\s\[\]\.\(\)\}}\*\+/-=%,]|$)", fr"{replaceWith}\1", source)
-			
-		return functor, source, ctor
-
-	def FunctionToFunctor(function, functorName=None, args=None, source=None, strongType=False):
-		executor = ExecutorTracker.GetLatest()
-		shouldLog = executor and executor.verbosity > 3
-		
-		destinedModule = inspect.getmodule(function)
-		destinedModuleName = INVALID_NAME()
-		if (destinedModule):
-			destinedModuleName = destinedModule.__name__
-		pivotModule = None
-		if (not destinedModule):
-			pivotModule = inspect.currentframe().f_back
-			if (not str(pivotModule).endswith('<module>>')):
-				pivotModule = None
-
-		bases = base
-		if (isinstance(bases, type)):
-			bases = [bases]
-		
-		primaryFunctionName = bases[0].primaryFunctionName
-
-		if (functorName is None):
-			functorName = function.__name__
-
-		logging.debug(f"Creating '{functorName}' from {bases} in module '{destinedModuleName if destinedModule else 'eons'}'")
-
-		functor = type(
-			functorName,
-			(*bases,),
-			{}
-		)
-
-		if ('name' not in kwargs):
-			kwargs['name'] = functorName
-
-		if (args is None):
-			args = inspect.signature(function).parameters
-		if (source is None):
-			source = inspect.getsource(function)
-
-		source = source[source.find(':\n')+1:].strip() # Will fail if an arg has ':\n' in it
-		source = re.sub(r'(^|[\s\[\(\{\*\+/-=%\^,])epidef([\s\[\]\.\(\)\}\*\+/-=%\^,]|$)', r'\1this.epidef\2', source)
-
-		ctor = util.DotDict()
-		ctor.source = []
-		ctor.additions = ""
-
-		functor, source, ctor = ParseParameters(functor, args, source, ctor, strongType=strongType)
-
-		# Constructor creation
-		constructorName = f"_eons_constructor_{kwargs['name']}"
-		constructorSource = f"def {constructorName}(this, name='{functorName}', **kwargs):"
-		constructorSource += "\n\timport sys"
-		constructorSource += "\n\timport eons"
-		constructorSource += f'''
-	this.name = name # For debugging
-	try:
-		{functor.__name__} = importedAs = eons.util.BlackMagick.GetCurrentFunction().__source_class__
-		if (not isinstance(this, {functor.__name__})):
-			raise Exception('{functor.__name__} not in source class')
-	except Exception as e1:
-		try:
-			importedAs = eons.util.BlackMagick.GetCurrentFunction().__pivot_module__.f_locals['__imported_as__']
-			{functor.__name__} = sys.modules[importedAs].{functor.__name__}
-			if (not isinstance(this, {functor.__name__})):
-				raise Exception('{functor.__name__} not in {{importedAs}}')
-		except Exception as e2:
-			try:
-				{functor.__name__} = sys.modules[{destinedModuleName}].{functor.__name__}
-				if (not isinstance(this, {functor.__name__})):
-					raise Exception('{functor.__name__} not in {destinedModuleName}')
-			except Exception as e3:
-				logging.warning(f"Failed to initialize {functor.__name__}: \\n{{e1}}\\n{{e2}}\\n{{e3}}")
-				# Catch all. This will cause an infinite loop if this != {functor.__name__}
-				{functor.__name__} = this.__class__
-	this.parent = type(this).mro()[1]
-	super({functor.__name__}, this).__init__(**kwargs)
-	this.name = name # For use
-'''
-		constructorSource += '\n\t' + '\n\t'.join(ctor.source)
-		if (len(ctor.additions)):
-			re.sub(r'^\s+', '\n', ctor.additions)
-			constructorSource += '\n\t' + ('\n\t'.join(ctor.additions.split('\n'))).replace('self', 'this')
-		if (shouldLog):
-			logging.debug(f"Constructor source for {kwargs['name']}:\n{constructorSource}")
-		code = compile(constructorSource, '', 'exec')
-		exec(code)
-		exec(f'functor.__init__ = {constructorName}')
-		functor.__init__.__source_class__ = functor
-		functor.__init__.__pivot_module__ = pivotModule
-
-		wrappedPrimaryFunction = f"_eons_method_{kwargs['name']}"
-		completeSource = f'''\
-def {wrappedPrimaryFunction}(this):
-	{source}
-'''
-		if (shouldLog):
-			logging.debug(f"Primary function source for {kwargs['name']}:\n{completeSource}")
-		code = compile(completeSource, '', 'exec')
-		exec(code)
-		exec(f'functor.{primaryFunctionName} = {wrappedPrimaryFunction}')
-
-		if (not destinedModule):
-			destinedModuleName = 'eons.eons'
-
-		try:
-			setattr(sys.modules[destinedModuleName], functorName, functor)
-		except Exception as e:
-			logging.warning(f"Failed to set {functorName} in {destinedModuleName}: {e}")
-
-		return functor
-
-	return FunctionToFunctor
-
-
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
-
-
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
-
-
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
-
-
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
-
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
 
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
 
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
 #			super().__init__()
@@ -2887,14 +2594,16 @@
 
 	# Logging to stderr is easy, since it will always happen.
 	# However, we also want the user to be able to log to a file, possibly set in the config.json, which requires a Fetch().
 	# Thus, setting up the log file handler has to occur later than the initial SetupLogging call.
 	# Calling this multiple times will add multiple log handlers.
 	def SetLogFile(this):
 		this.Set('log_file', this.Fetch('log_file', None, this.fetch.useDuringSetup))
+		this.log.file = this.log_file
+
 		if (this.log.file is None):
 			return
 
 		logFilePath = Path(this.log.file).resolve()
 		if (not logFilePath.exists()):
 			logFilePath.parent.mkdir(parents=True, exist_ok=True)
 			logFilePath.touch()
@@ -3483,14 +3192,328 @@
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
+class FetchCallbackFunctor(Functor):
+
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
+
+		this.arg.kw.required.append('varName')
+		this.arg.kw.required.append('location')
+		this.arg.kw.required.append('value')
+
+		this.functionSucceeded = True
+		this.feature.rollback = False
+
+# The standard Functor extends Functor to add a set of standard members and methods.
+# This is similar to the standard library in C and C++
+# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
+class StandardFunctor(Functor):
+	def __init__(this, name="Standard Functor"):
+		super().__init__(name)
+
+	# Override this and do whatever!
+	# This is purposefully vague.
+	def Function(this):
+		pass
+
+
+	# Undo any changes made by UserFunction.
+	# Please override this too!
+	def Rollback(this):
+		pass
+
+
+	# Override this to check results of operation and report on status.
+	# Override this to perform whatever success checks are necessary.
+	def DidFunctionSucceed(this):
+		return this.functionSucceeded
+
+
+	# RETURN whether or not the Rollback was successful.
+	# Override this to perform whatever success checks are necessary.
+	def DidRollbackSucceed(this):
+		return this.rollbackSucceeded
+
+
+	######## START: UTILITIES ########
+
+	# RETURNS: an opened file object for writing.
+	# Creates the path if it does not exist.
+	@method()
+	def CreateFile(this, file, mode="w+"):
+		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
+		return open(file, mode)
+
+	# Copy a file or folder from source to destination.
+	# This really shouldn't be so hard...
+	# root allows us to interpret '/' as something other than the top of the filesystem.
+	@method()
+	def Copy(this, source, destination, root='/'):
+		if (source.startswith('/')):
+			source = str(Path(root).joinpath(source[1:]).resolve())
+		else:
+			source = str(Path(source).resolve())
+		
+		destination = str(Path(destination).resolve())
+		
+		Path(destination).parent.mkdir(parents=True, exist_ok=True)
+
+		if (os.path.isfile(source)):
+			logging.debug(f"Copying file {source} to {destination}")
+			try:
+				shutil.copy(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		elif (os.path.isdir(source)):
+			logging.debug(f"Copying directory {source} to {destination}")
+			try:
+				shutil.copytree(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		else:
+			logging.error(f"Could not find source to copy: {source}")
+
+	# Delete a file or folder
+	@method()
+	def Delete(this, target):
+		if (not os.path.exists(target)):
+			logging.debug(f"Unable to delete nonexistent target: {target}")
+			return
+		if (os.path.isfile(target)):
+			logging.debug(f"Deleting file {target}")
+			os.remove(target)
+		elif (os.path.isdir(target)):
+			logging.debug(f"Deleting directory {target}")
+			try:
+				shutil.rmtree(target)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+
+	# Run whatever.
+	# DANGEROUS!!!!!
+	# RETURN: Return value and, optionally, the output as a list of lines.
+	@method()
+	def RunCommand(this, command, saveout=False, raiseExceptions=True):
+		logging.debug(f"================ Running command: {command} ================")
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		output = []
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
+			if (saveout):
+				output.append(line)
+			if (line):
+				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
+
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
+		
+		logging.debug(f"================ Completed command: {command} ================")
+		if (saveout):
+			return process.returncode, output
+		
+		return process.returncode
+	######## END: UTILITIES ########
+
+
+def kind(
+	base = StandardFunctor,
+	**kwargs
+):
+	def ParseParameters(functor, args, source, ctor, strongType = False):
+		# Code duplicated from Method.PopulateFrom. See that class for more info.
+		for arg in args.values():
+			if (arg.name == 'constructor' or arg.name == '__init__'):
+				ctor.additions += f"{arg.default}\n"
+				continue
+
+			replaceWith = arg.name
+
+			# *args
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			# **kwargs
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			# Normal argument
+			else:
+				replaceWith = f'this.{arg.name}'
+				shouldMapArg = arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]
+
+				if (arg.default != inspect.Parameter.empty):
+					if (isinstance(arg.default, Method)):
+						arg.default.name = arg.name # Rename the Functor to match what was requested
+						PrepareClassMethod(functor, arg.name, arg.default)
+						shouldMapArg = False
+					elif (isinstance(arg.default, AccessControl)):
+						# NOTE: arg.name is discarded.
+						functor, source, ctor = ParseParameters(
+							functor,
+							arg.default.parameters,
+							source,
+							ctor,
+							strongType=strongType
+						)
+						shouldMapArg = False
+					else:
+						defaultValue = arg.default
+						if (isinstance(arg.default, str)):
+							defaultValue = f"'{arg.default}'"
+						ctor.source.append(f"this.arg.kw.optional['{arg.name}'] = {defaultValue}")
+				else:
+					ctor.source.append(f"this.arg.kw.required.append('{arg.name}')")
+
+				if (strongType and hasattr(arg, 'type')):
+					ctor.source.append(f"""
+	try:
+		this.arg.type['{arg.name}'] = {arg.type.__name__}
+	except:
+		this.arg.type['{arg.name}'] = eons.SelfRegistering('{arg.type.__name__}')
+""")
+
+				if (shouldMapArg):
+					ctor.source.append(f"this.arg.mapping.append('{arg.name}')")
+
+			# Source mangling
+			# TODO: Expand as we have more solid test cases.
+			source = re.sub(fr"{arg.name}([\s\[\]\.\(\)\}}\*\+/-=%,]|$)", fr"{replaceWith}\1", source)
+			
+		return functor, source, ctor
+
+	def FunctionToFunctor(function, functorName=None, args=None, source=None, strongType=False):
+		executor = ExecutorTracker.GetLatest()
+		shouldLog = executor and executor.verbosity > 3
+		
+		destinedModule = inspect.getmodule(function)
+		destinedModuleName = INVALID_NAME()
+		if (destinedModule):
+			destinedModuleName = destinedModule.__name__
+		pivotModule = None
+		if (not destinedModule):
+			pivotModule = inspect.currentframe().f_back
+			if (not str(pivotModule).endswith('<module>>')):
+				pivotModule = None
+
+		bases = base
+		if (isinstance(bases, type)):
+			bases = [bases]
+		
+		primaryFunctionName = bases[0].primaryFunctionName
+
+		if (functorName is None):
+			functorName = function.__name__
+
+		logging.debug(f"Creating '{functorName}' from {bases} in module '{destinedModuleName if destinedModule else 'eons'}'")
+
+		functor = type(
+			functorName,
+			(*bases,),
+			{}
+		)
+
+		if ('name' not in kwargs):
+			kwargs['name'] = functorName
+
+		if (args is None):
+			args = inspect.signature(function).parameters
+		if (source is None):
+			source = inspect.getsource(function)
+
+		source = source[source.find(':\n')+1:].strip() # Will fail if an arg has ':\n' in it
+		source = re.sub(r'(^|[\s\[\(\{\*\+/-=%\^,])epidef([\s\[\]\.\(\)\}\*\+/-=%\^,]|$)', r'\1this.epidef\2', source)
+
+		ctor = util.DotDict()
+		ctor.source = []
+		ctor.additions = ""
+
+		functor, source, ctor = ParseParameters(functor, args, source, ctor, strongType=strongType)
+
+		# Constructor creation
+		constructorName = f"_eons_constructor_{kwargs['name']}"
+		constructorSource = f"def {constructorName}(this, name='{functorName}', **kwargs):"
+		constructorSource += "\n\timport sys"
+		constructorSource += "\n\timport eons"
+		constructorSource += f'''
+	this.name = name # For debugging
+	try:
+		{functor.__name__} = importedAs = eons.util.BlackMagick.GetCurrentFunction().__source_class__
+		if (not isinstance(this, {functor.__name__})):
+			raise Exception('{functor.__name__} not in source class')
+	except Exception as e1:
+		try:
+			importedAs = eons.util.BlackMagick.GetCurrentFunction().__pivot_module__.f_locals['__imported_as__']
+			{functor.__name__} = sys.modules[importedAs].{functor.__name__}
+			if (not isinstance(this, {functor.__name__})):
+				raise Exception('{functor.__name__} not in {{importedAs}}')
+		except Exception as e2:
+			try:
+				{functor.__name__} = sys.modules[{destinedModuleName}].{functor.__name__}
+				if (not isinstance(this, {functor.__name__})):
+					raise Exception('{functor.__name__} not in {destinedModuleName}')
+			except Exception as e3:
+				logging.warning(f"Failed to initialize {functor.__name__}: \\n{{e1}}\\n{{e2}}\\n{{e3}}")
+				# Catch all. This will cause an infinite loop if this != {functor.__name__}
+				{functor.__name__} = this.__class__
+	this.parent = type(this).mro()[1]
+	super({functor.__name__}, this).__init__(**kwargs)
+	this.name = name # For use
+'''
+		constructorSource += '\n\t' + '\n\t'.join(ctor.source)
+		if (len(ctor.additions)):
+			re.sub(r'^\s+', '\n', ctor.additions)
+			constructorSource += '\n\t' + ('\n\t'.join(ctor.additions.split('\n'))).replace('self', 'this')
+		if (shouldLog):
+			logging.debug(f"Constructor source for {kwargs['name']}:\n{constructorSource}")
+		code = compile(constructorSource, '', 'exec')
+		exec(code)
+		exec(f'functor.__init__ = {constructorName}')
+		functor.__init__.__source_class__ = functor
+		functor.__init__.__pivot_module__ = pivotModule
+
+		wrappedPrimaryFunction = f"_eons_method_{kwargs['name']}"
+		completeSource = f'''\
+def {wrappedPrimaryFunction}(this):
+	{source}
+'''
+		if (shouldLog):
+			logging.debug(f"Primary function source for {kwargs['name']}:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'functor.{primaryFunctionName} = {wrappedPrimaryFunction}')
+
+		if (not destinedModule):
+			destinedModuleName = 'eons.eons'
+
+		try:
+			setattr(sys.modules[destinedModuleName], functorName, functor)
+		except Exception as e:
+			logging.warning(f"Failed to set {functorName} in {destinedModuleName}: {e}")
+
+		return functor
+
+	return FunctionToFunctor
+
+
 # Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetSubjectFromError method and create a new class for every error you want to handle.
 # ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
 # Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
 # NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
 # startPosition is always positive
 # endPosition is always negative
@@ -3637,28 +3660,7 @@
 			logging.error(f"Error resolution with {this.name} failed: {e}")
 			util.LogStack()
 			this.functionSucceeded = False
 		
 		this.error.resolution.stack[this.error.string].append(this.name)
 		return this.error.resolution.stack, this.error.resolution.successful
 
-
-class FetchCallbackFunctor(Functor):
-
-	def __init__(this, name = "FetchCallbackFunctor"):
-		super().__init__(name)
-
-		this.arg.kw.required.append('varName')
-		this.arg.kw.required.append('location')
-		this.arg.kw.required.append('value')
-
-		this.functionSucceeded = True
-		this.feature.rollback = False
-
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
```

### Comparing `eons-3.1.4/pkg/eons/method/External.py` & `eons-3.1.5/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-3.1.5/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons/resolve/resolve_import_module.py` & `eons-3.1.5/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-3.1.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons/resolve/resolve_namespace_lookup.py` & `eons-3.1.5/pkg/eons/resolve/resolve_namespace_lookup.py`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/pkg/eons.egg-info/PKG-INFO` & `eons-3.1.5/pkg/eons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 3.1.4
+Version: 3.1.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: eot
+Requires-Dist: pyyaml
+Requires-Dist: requests_futures
 Requires-Dist: jsonpickle
+Requires-Dist: eot
 Requires-Dist: requests
 Requires-Dist: tqdm
-Requires-Dist: requests_futures
-Requires-Dist: pyyaml
 
 # Eons Python Framework
 
 The Eons Python Framework provides a user-friendly Python extension to the [Develop Biology](https://develop.bio) project. This means `eons` helps you blur the lines between what it means to be, have, and do. Gone are the days of classes meaning "to be", members meaning "to have", and functions meaning "to do". With Eons and Biology, they are all one and the same. 
 
 Design in short: Self-registering, sequential functors with implicit and automatic inheritance, downloaded just-in-time for use with arbitrary data structures.
```

### Comparing `eons-3.1.4/pkg/eons.egg-info/SOURCES.txt` & `eons-3.1.5/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-3.1.4/setup.cfg` & `eons-3.1.5/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 3.1.4
+version = 3.1.5
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	eot
+	pyyaml
+	requests_futures
 	jsonpickle
+	eot
 	requests
 	tqdm
-	requests_futures
-	pyyaml
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

