# Comparing `tmp/regmapGen-1.0.1.tar.gz` & `tmp/regmapGen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regmapGen-1.0.1.tar", last modified: Wed Mar 27 18:13:35 2024, max compression
+gzip compressed data, was "regmapGen-1.0.2.tar", last modified: Wed Apr  3 19:40:34 2024, max compression
```

## Comparing `regmapGen-1.0.1.tar` & `regmapGen-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-03-27 18:13:35.751416 regmapGen-1.0.1/
--rw-r--r--   0 paul      (1000) paul      (1000)     1081 2024-03-19 12:13:26.000000 regmapGen-1.0.1/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     7587 2024-03-27 18:13:35.751416 regmapGen-1.0.1/PKG-INFO
--rwxr-xr-x   0 paul      (1000) paul      (1000)     7045 2024-03-27 18:05:57.000000 regmapGen-1.0.1/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-03-27 18:13:35.741416 regmapGen-1.0.1/regmapGen/
--rwxr-xr-x   0 paul      (1000) paul      (1000)      684 2024-03-19 12:32:41.000000 regmapGen-1.0.1/regmapGen/__init__.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     8133 2024-03-26 18:19:54.000000 regmapGen-1.0.1/regmapGen/__main__.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)    11204 2024-03-19 12:30:11.000000 regmapGen-1.0.1/regmapGen/bitfield.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     4452 2024-03-26 19:57:39.000000 regmapGen-1.0.1/regmapGen/config.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2877 2024-03-19 12:30:11.000000 regmapGen-1.0.1/regmapGen/enum.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)    26649 2024-03-26 19:35:58.000000 regmapGen-1.0.1/regmapGen/generators.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     7975 2024-03-19 12:45:29.000000 regmapGen-1.0.1/regmapGen/reg.py
--rwxr-xr-x   0 paul      (1000) paul      (1000)     9074 2024-03-19 12:45:04.000000 regmapGen-1.0.1/regmapGen/regmap.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-03-27 18:13:35.741416 regmapGen-1.0.1/regmapGen/templates/
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2085 2024-03-23 10:32:06.000000 regmapGen-1.0.1/regmapGen/templates/amm2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1618 2024-03-23 10:30:08.000000 regmapGen-1.0.1/regmapGen/templates/apb2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     5259 2024-03-23 10:30:44.000000 regmapGen-1.0.1/regmapGen/templates/axil2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     3764 2024-03-23 10:18:16.000000 regmapGen-1.0.1/regmapGen/templates/c_header.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2943 2024-03-26 19:41:45.000000 regmapGen-1.0.1/regmapGen/templates/regmap_asciidoc.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     3227 2024-03-26 19:42:25.000000 regmapGen-1.0.1/regmapGen/templates/regmap_md.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     2544 2024-03-19 12:51:37.000000 regmapGen-1.0.1/regmapGen/templates/regmap_py.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)    15879 2024-03-26 19:10:36.000000 regmapGen-1.0.1/regmapGen/templates/regmap_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     9730 2024-03-23 10:33:02.000000 regmapGen-1.0.1/regmapGen/templates/spi2lb_sv.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1656 2024-03-26 16:16:54.000000 regmapGen-1.0.1/regmapGen/templates/sv_header.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     1900 2024-03-23 10:10:08.000000 regmapGen-1.0.1/regmapGen/templates/sv_package.j2
--rwxr-xr-x   0 paul      (1000) paul      (1000)     5878 2024-03-19 12:30:11.000000 regmapGen-1.0.1/regmapGen/utils.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-03-27 18:13:35.741416 regmapGen-1.0.1/regmapGen.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     7587 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)      780 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       55 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/entry_points.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      124 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       10 2024-03-27 18:13:35.000000 regmapGen-1.0.1/regmapGen.egg-info/top_level.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2024-03-27 18:13:35.751416 regmapGen-1.0.1/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1251 2024-03-27 18:13:33.000000 regmapGen-1.0.1/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1081 2024-03-19 12:13:26.000000 regmapGen-1.0.2/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-03 19:40:34.009918 regmapGen-1.0.2/PKG-INFO
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     7145 2024-04-03 19:40:02.000000 regmapGen-1.0.2/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen/
+-rwxr-xr-x   0 paul      (1000) paul      (1000)      684 2024-03-19 12:32:41.000000 regmapGen-1.0.2/regmapGen/__init__.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     8438 2024-04-02 20:34:28.000000 regmapGen-1.0.2/regmapGen/__main__.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)    11204 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/bitfield.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     5087 2024-04-01 19:31:56.000000 regmapGen-1.0.2/regmapGen/config.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     2877 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/enum.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)    37017 2024-04-03 19:33:06.000000 regmapGen-1.0.2/regmapGen/generators.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     7975 2024-03-19 12:45:29.000000 regmapGen-1.0.2/regmapGen/reg.py
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     9242 2024-04-03 19:33:51.000000 regmapGen-1.0.2/regmapGen/regmap.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen/templates/
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     2085 2024-03-23 10:32:06.000000 regmapGen-1.0.2/regmapGen/templates/amm2lb_sv.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     1618 2024-03-23 10:30:08.000000 regmapGen-1.0.2/regmapGen/templates/apb2lb_sv.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     5259 2024-03-23 10:30:44.000000 regmapGen-1.0.2/regmapGen/templates/axil2lb_sv.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     3764 2024-03-23 10:18:16.000000 regmapGen-1.0.2/regmapGen/templates/c_header.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3267 2024-04-02 18:39:12.000000 regmapGen-1.0.2/regmapGen/templates/cmsis_svd.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3526 2024-04-02 19:39:18.000000 regmapGen-1.0.2/regmapGen/templates/ipxact_xml.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     2943 2024-03-26 19:41:45.000000 regmapGen-1.0.2/regmapGen/templates/regmap_asciidoc.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     3227 2024-03-26 19:42:25.000000 regmapGen-1.0.2/regmapGen/templates/regmap_md.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     2544 2024-03-19 12:51:37.000000 regmapGen-1.0.2/regmapGen/templates/regmap_py.j2
+-rw-r--r--   0 paul      (1000) paul      (1000)     3637 2024-04-02 20:53:31.000000 regmapGen-1.0.2/regmapGen/templates/regmap_rst.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)    15879 2024-03-26 19:10:36.000000 regmapGen-1.0.2/regmapGen/templates/regmap_sv.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     9730 2024-03-23 10:33:02.000000 regmapGen-1.0.2/regmapGen/templates/spi2lb_sv.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     1656 2024-03-26 16:16:54.000000 regmapGen-1.0.2/regmapGen/templates/sv_header.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     1900 2024-03-23 10:10:08.000000 regmapGen-1.0.2/regmapGen/templates/sv_package.j2
+-rwxr-xr-x   0 paul      (1000) paul      (1000)     5878 2024-03-19 12:30:11.000000 regmapGen-1.0.2/regmapGen/utils.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-04-03 19:40:34.009918 regmapGen-1.0.2/regmapGen.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     7687 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)      881 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       55 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/entry_points.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      124 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       10 2024-04-03 19:40:33.000000 regmapGen-1.0.2/regmapGen.egg-info/top_level.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2024-04-03 19:40:34.009918 regmapGen-1.0.2/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1251 2024-04-02 20:23:34.000000 regmapGen-1.0.2/setup.py
```

### Comparing `regmapGen-1.0.1/LICENSE` & `regmapGen-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/PKG-INFO` & `regmapGen-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regmapGen
-Version: 1.0.1
+Version: 1.0.2
 Summary: Генератор Регистровой Карты
 Home-page: https://github.com/paulmsv/regmapGen
 Author: paulmsv
 Author-email: bobkovpg@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://regmapGen.readthedocs.io
 Platform: UNKNOWN
@@ -131,12 +131,21 @@
 
 Если вы ищете дополнительные примеры, пожалуйста, проверьте директорию `examples`.
 
 ## Разработка
 
 Пожалуйста, ознакомьтесь с [Руководством разработчика](https://regmapGen.readthedocs.io/en/latest/contributing.html).
 
+Для PyPi:
+
+```bash
+rm -rf dist
+pip3 install -e .
+python3 setup.py sdist
+twine upload dist/*
+```
+
 ## Лицензия
 
 regmapGen лицензирован под [Лицензией MIT](LICENSE).
```

### Comparing `regmapGen-1.0.1/README.md` & `regmapGen-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,10 +114,19 @@
 
 Если вы ищете дополнительные примеры, пожалуйста, проверьте директорию `examples`.
 
 ## Разработка
 
 Пожалуйста, ознакомьтесь с [Руководством разработчика](https://regmapGen.readthedocs.io/en/latest/contributing.html).
 
+Для PyPi:
+
+```bash
+rm -rf dist
+pip3 install -e .
+python3 setup.py sdist
+twine upload dist/*
+```
+
 ## Лицензия
 
 regmapGen лицензирован под [Лицензией MIT](LICENSE).
```

### Comparing `regmapGen-1.0.1/regmapGen/__init__.py` & `regmapGen-1.0.2/regmapGen/__init__.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/__main__.py` & `regmapGen-1.0.2/regmapGen/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,19 @@
     # targets
     targets = {}
     targets.update(regmapGen.generators.SystemVerilog(path="hw/regs.sv").make_target('sv_module'))
     targets.update(regmapGen.generators.SystemVerilogHeader(path="hw/regs.svh").make_target('sv_header'))
     targets.update(regmapGen.generators.SystemVerilogPackage(path="hw/regs_pkg.sv").make_target('sv_pkg'))
     targets.update(regmapGen.generators.Python(path="sw/regs.py").make_target('py'))
     targets.update(regmapGen.generators.CHeader(path="sw/regs.h").make_target('c_header'))
+    targets.update(regmapGen.generators.CmsisSvd(path="sw/regs.svd").make_target('cmsis_svd'))
+    targets.update(regmapGen.generators.IpxactXml(path="sw/regs.xml").make_target('ipxact_xml'))
     targets.update(regmapGen.generators.Markdown(path="doc/regs.md", image_dir="md_img").make_target('md_doc'))
     targets.update(regmapGen.generators.Asciidoc(path="doc/regs.adoc", image_dir="adoc_img").make_target('asciidoc_doc'))
+    targets.update(regmapGen.generators.Rst(path="doc/regs.rst", image_dir="rst_img").make_target('rst_doc'))
     targets.update(regmapGen.generators.Docx(path="doc/regs.docx").make_target('docx_doc'))
 
     # create templates
     if format == 'txt':
         rmap = regmapGen.utils.create_template_simple()
     else:
         rmap = regmapGen.utils.create_template()
```

### Comparing `regmapGen-1.0.1/regmapGen/bitfield.py` & `regmapGen-1.0.2/regmapGen/bitfield.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/config.py` & `regmapGen-1.0.2/regmapGen/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     return {
         "base_address": 0,
         "data_width": 32,
         "address_width": 16,
         "register_reset": "sync_pos",
         "address_increment": "none",
         "address_alignment": "data_width",
+        "address_duplicate": "none",
         "force_name_case": "none",
     }
 
 
 def read_config(cfgpath):
     """Parse regmapGen configuration file. Return two dictionaries: global configuration and targets."""
     # open config file
@@ -38,14 +39,18 @@
             globcfg["address_increment"] = utils.str2int(globcfg["address_increment"])
         except ValueError:
             pass
         try:
             globcfg["address_alignment"] = utils.str2int(globcfg["address_alignment"])
         except ValueError:
             pass
+        try:
+            globcfg["address_duplicate"] = utils.str2int(globcfg["address_duplicate"])
+        except ValueError:
+            pass
         validate_globcfg(globcfg)
 
     # parse targets
     targets = {}
     for target_name in [name for name in cfg.sections() if name != 'globcfg']:
         if 'generator' in dict(cfg[target_name]).keys():
             targets[target_name] = dict(cfg[target_name])
@@ -100,14 +105,25 @@
                     utils.is_non_neg_int(globcfg["address_alignment"]))
     except ValueError:
         is_valid = False
     assert is_valid, \
         "Wrong value for 'address_alignment'='%s'. Must be one of this: %s or a non negative integer." % (
             globcfg["address_alignment"], address_alignment_alowed)
 
+    # address_duplicate
+    address_duplicate_alowed = ['none', 'true']
+    try:
+        is_valid = (globcfg["address_duplicate"] in address_duplicate_alowed or
+                    utils.is_non_neg_int(globcfg["address_duplicate"]))
+    except ValueError:
+        is_valid = False
+    assert is_valid, \
+        "Wrong value for 'address_duplicate'='%s'. Must be one of this: %s." % (
+            globcfg["address_duplicate"], address_duplicate_alowed)
+
     # force_name_case
     force_name_case_allowed = ['lower', 'upper', 'none']
     assert globcfg["force_name_case"] in force_name_case_allowed, \
         "Wrong value for 'force_name_case'='%s'. Must be one of this: %s." % (globcfg["force_name_case"],
                                                                               force_name_case_allowed)
```

### Comparing `regmapGen-1.0.1/regmapGen/enum.py` & `regmapGen-1.0.2/regmapGen/enum.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/reg.py` & `regmapGen-1.0.2/regmapGen/reg.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/regmap.py` & `regmapGen-1.0.2/regmapGen/regmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,19 @@
         assert (reg.address % align_val) == 0, \
             "Register '%s' with address '%d' is not %d bytes alligned!" % (reg.name, reg.address, align_val)
 
     def _addr_check_conflicts(self, reg):
         addresses = [reg.address for reg in self]
         if reg.address in addresses:
             conflict_reg = self[addresses.index(reg.address)]
-            assert False, "Register '%s' with address '%d' conflicts with register '%s' with the same address!" % \
-                (reg.name, reg.address, conflict_reg.name)
+            if config.globcfg['address_duplicate'] == 'true':
+                return
+            else:
+                assert False, "Register '%s' with address '%d' conflicts with register '%s' with the same address!" % \
+                    (reg.name, reg.address, conflict_reg.name)
 
     @property
     def regs(self):
         """List with register objects."""
         return self._regs
 
     def add_registers(self, new_regs):
@@ -164,27 +167,27 @@
         elif ext == '.txt':
             self.read_txt(path)
         else:
             raise ValueError("Unknown extension '%s' of the file '%s'" % (ext, path))
 
     def read_json(self, path):
         """Read register map from JSON file."""
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding="utf-8") as f:
             data = json.load(f)
             self._fill_from_file_data(data['regmap'])
 
     def read_yaml(self, path):
         """Read register map from YAML file."""
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding="utf-8") as f:
             data = yaml.safe_load(f)
             self._fill_from_file_data(data['regmap'])
 
     def read_txt(self, path):
         """Read register map from text file."""
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding="utf-8") as f:
             raw_lines = f.readlines()
             data = []
             reg_start_idx = None
             for i, line in enumerate(raw_lines):
                 if '-----' in line:
                     reg_start_idx = i + 1
                 if reg_start_idx and i >= reg_start_idx:
```

### Comparing `regmapGen-1.0.1/regmapGen/templates/amm2lb_sv.j2` & `regmapGen-1.0.2/regmapGen/templates/amm2lb_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/apb2lb_sv.j2` & `regmapGen-1.0.2/regmapGen/templates/apb2lb_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/axil2lb_sv.j2` & `regmapGen-1.0.2/regmapGen/templates/axil2lb_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/c_header.j2` & `regmapGen-1.0.2/regmapGen/templates/c_header.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/regmap_asciidoc.j2` & `regmapGen-1.0.2/regmapGen/templates/regmap_asciidoc.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/regmap_md.j2` & `regmapGen-1.0.2/regmapGen/templates/regmap_md.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/regmap_py.j2` & `regmapGen-1.0.2/regmapGen/templates/regmap_py.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/regmap_sv.j2` & `regmapGen-1.0.2/regmapGen/templates/regmap_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/spi2lb_sv.j2` & `regmapGen-1.0.2/regmapGen/templates/spi2lb_sv.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/sv_header.j2` & `regmapGen-1.0.2/regmapGen/templates/sv_header.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/templates/sv_package.j2` & `regmapGen-1.0.2/regmapGen/templates/sv_package.j2`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen/utils.py` & `regmapGen-1.0.2/regmapGen/utils.py`

 * *Files identical despite different names*

### Comparing `regmapGen-1.0.1/regmapGen.egg-info/PKG-INFO` & `regmapGen-1.0.2/regmapGen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regmapGen
-Version: 1.0.1
+Version: 1.0.2
 Summary: Генератор Регистровой Карты
 Home-page: https://github.com/paulmsv/regmapGen
 Author: paulmsv
 Author-email: bobkovpg@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://regmapGen.readthedocs.io
 Platform: UNKNOWN
@@ -131,12 +131,21 @@
 
 Если вы ищете дополнительные примеры, пожалуйста, проверьте директорию `examples`.
 
 ## Разработка
 
 Пожалуйста, ознакомьтесь с [Руководством разработчика](https://regmapGen.readthedocs.io/en/latest/contributing.html).
 
+Для PyPi:
+
+```bash
+rm -rf dist
+pip3 install -e .
+python3 setup.py sdist
+twine upload dist/*
+```
+
 ## Лицензия
 
 regmapGen лицензирован под [Лицензией MIT](LICENSE).
```

### Comparing `regmapGen-1.0.1/regmapGen.egg-info/SOURCES.txt` & `regmapGen-1.0.2/regmapGen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 regmapGen.egg-info/entry_points.txt
 regmapGen.egg-info/requires.txt
 regmapGen.egg-info/top_level.txt
 regmapGen/templates/amm2lb_sv.j2
 regmapGen/templates/apb2lb_sv.j2
 regmapGen/templates/axil2lb_sv.j2
 regmapGen/templates/c_header.j2
+regmapGen/templates/cmsis_svd.j2
+regmapGen/templates/ipxact_xml.j2
 regmapGen/templates/regmap_asciidoc.j2
 regmapGen/templates/regmap_md.j2
 regmapGen/templates/regmap_py.j2
+regmapGen/templates/regmap_rst.j2
 regmapGen/templates/regmap_sv.j2
 regmapGen/templates/spi2lb_sv.j2
 regmapGen/templates/sv_header.j2
 regmapGen/templates/sv_package.j2
```

### Comparing `regmapGen-1.0.1/setup.py` & `regmapGen-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Install package
 setuptools.setup(
     name="regmapGen",
-    version='1.0.1',
+    version='1.0.2',
     author="paulmsv",
     author_email="bobkovpg@gmail.com",
     description="Генератор Регистровой Карты",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/paulmsv/regmapGen",
     project_urls={
```

