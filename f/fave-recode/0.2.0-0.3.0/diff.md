# Comparing `tmp/fave_recode-0.2.0.tar.gz` & `tmp/fave_recode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fave_recode-0.2.0.tar", max compression
+gzip compressed data, was "fave_recode-0.3.0.tar", max compression
```

## Comparing `fave_recode-0.2.0.tar` & `fave_recode-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-11-08 22:53:37.529813 fave_recode-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2630 2023-11-22 01:49:16.314987 fave_recode-0.2.0/README.md
--rw-r--r--   0        0        0     1188 2023-11-22 01:49:16.320388 fave_recode-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-22 01:49:16.320504 fave_recode-0.2.0/src/fave_recode/__init__.py
--rw-r--r--   0        0        0     8325 2023-11-22 01:49:16.320607 fave_recode-0.2.0/src/fave_recode/fave_recode.py
--rw-r--r--   0        0        0     3601 2023-11-22 01:49:16.320742 fave_recode-0.2.0/src/fave_recode/relations.py
--rw-r--r--   0        0        0     4667 2023-11-22 01:49:16.320850 fave_recode-0.2.0/src/fave_recode/resources/cmu2labov.yml
--rw-r--r--   0        0        0    10543 2023-11-22 01:49:16.320941 fave_recode-0.2.0/src/fave_recode/resources/cmu2phila.yml
--rw-r--r--   0        0        0     5762 2023-11-22 01:49:16.321020 fave_recode-0.2.0/src/fave_recode/rule_classes.py
--rw-r--r--   0        0        0     1301 2023-11-22 01:49:16.321090 fave_recode-0.2.0/src/fave_recode/ruleschema.py
--rw-r--r--   0        0        0      303 2023-11-22 01:49:16.321148 fave_recode-0.2.0/src/fave_recode/schemes.py
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 fave_recode-0.2.0/setup.py
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 fave_recode-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-08 22:53:37.529813 fave_recode-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2878 2024-04-03 18:31:30.492756 fave_recode-0.3.0/README.md
+-rw-r--r--   0        0        0     1219 2024-04-03 18:31:30.494857 fave_recode-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-22 01:49:16.320504 fave_recode-0.3.0/src/fave_recode/__init__.py
+-rw-r--r--   0        0        0     9305 2024-04-03 18:31:30.495060 fave_recode-0.3.0/src/fave_recode/fave_recode.py
+-rw-r--r--   0        0        0     3922 2024-04-03 18:31:30.495182 fave_recode-0.3.0/src/fave_recode/labelset_parser.py
+-rw-r--r--   0        0        0     3601 2023-11-22 01:49:16.320742 fave_recode-0.3.0/src/fave_recode/relations.py
+-rw-r--r--   0        0        0     4919 2024-04-03 18:31:30.495412 fave_recode-0.3.0/src/fave_recode/resources/cmu2labov.yml
+-rw-r--r--   0        0        0    10933 2024-04-03 18:31:30.495655 fave_recode-0.3.0/src/fave_recode/resources/cmu2phila.yml
+-rw-r--r--   0        0        0      900 2024-04-03 18:31:30.495778 fave_recode-0.3.0/src/fave_recode/resources/cmu_parser.yml
+-rw-r--r--   0        0        0     6257 2024-04-03 18:31:30.496001 fave_recode-0.3.0/src/fave_recode/rule_classes.py
+-rw-r--r--   0        0        0     2013 2024-04-03 18:31:30.496151 fave_recode-0.3.0/src/fave_recode/ruleschema.py
+-rw-r--r--   0        0        0      422 2024-04-03 18:31:30.496294 fave_recode-0.3.0/src/fave_recode/schemes.py
+-rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 fave_recode-0.3.0/setup.py
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 fave_recode-0.3.0/PKG-INFO
```

### Comparing `fave_recode-0.2.0/LICENSE.md` & `fave_recode-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fave_recode-0.2.0/README.md` & `fave_recode-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Getting started with `fave-recode`
 
+
+![PyPI](https://img.shields.io/pypi/v/fave-recode.png)
 [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode/graph/badge.svg?token=C23B1H3DAX)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode)
 [![Maintainability](https://api.codeclimate.com/v1/badges/2375ddfef5d77ba1681d/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/fave-recode/maintainability)
 [![FAVE Python
 CI](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml/badge.svg?branch=dev)](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml)
 [![Build
 Docs](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/fave-recode/)
+[![DOI](https://zenodo.org/badge/605740158.svg)](https://zenodo.org/badge/latestdoi/605740158)
 
 The idea behind `fave-recode` is that no matter how much you may adjust
 the dictionary of a forced-aligner, you may still want to make
 programmatic changes to the output.
 
 ## Installation
 
@@ -37,14 +40,15 @@
       -p, --input_path PATH      Path to a set of files
 
     Outputs:
       -o, --output_file TEXT     An output file name
       -d, --output_dest PATH     An output directory
 
     Other options:
+      -a, --parser TEXT          Label set parser. Built in options are cmu_parser
       -s, --scheme TEXT          Recoding scheme. Built in options are cmu2labov
                                  and cmu2phila  [required]
       -r, --recode_stem TEXT     Stem to append to recoded TextGrid file names
       -t, --target_tier TEXT     Target tier to recode
       --help                     Show this message and exit.
 
 To recode a single file, you need to provide `fave_recode` with,
@@ -55,15 +59,15 @@
 ``` bash
 ls data
 ```
 
     KY25A_1.TextGrid                 josef-fruehwald_speaker.TextGrid
 
 ``` bash
-fave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila
+fave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila -a cmu_parser
 
 ls data
 ```
 
     KY25A_1.TextGrid
     josef-fruehwald_speaker.TextGrid
     josef-fruehwald_speaker_recoded.TextGrid
```

### Comparing `fave_recode-0.2.0/pyproject.toml` & `fave_recode-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fave-recode"
-version = "0.2.0"
+version = "0.3.0"
 description = "A package for recoding Praat TextGrids"
 authors = ["JoFrhwld <JoFrhwld@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "fave_recode", from="src"}]
 exclude = [
     ".github/",
@@ -12,15 +12,15 @@
     "doc_src/"
 ]
 homepage = "https://forced-alignment-and-vowel-extraction.github.io/fave-recode"
 repository = "https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aligned-textgrid = "^v0.4.1"
+aligned-textgrid = "^0.6.4"
 pyyaml = "^6.0"
 cerberus = "^1.3.5"
 click = "^8.1.7"
 cloup = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
@@ -37,15 +37,16 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--cov-config=.coveragerc",
-    "--cov"
+    "--cov",
+    "--cov-report=xml:cov.xml"
 ]
 filterwarnings =[
     "ignore::UserWarning"
 ]
 pythonpath = "src"
 testpaths = "tests"
```

### Comparing `fave_recode-0.2.0/src/fave_recode/fave_recode.py` & `fave_recode-0.3.0/src/fave_recode/fave_recode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from aligned_textgrid import AlignedTextGrid, custom_classes, Word, Phone
 from fave_recode.rule_classes import RuleSet
+from fave_recode.labelset_parser import LabelSetParser
 from fave_recode.schemes import all_schemes
 from pathlib import Path
 from typing import Union
 import click
 import cloup
 import io
 
@@ -38,14 +39,18 @@
     cloup.constraints.mutually_exclusive,
     ["input_file", "output_dest"]
 )
 @cloup.constraint(
     cloup.constraints.mutually_exclusive,
     ["input_path", "output_file"]
 )
+@click.option("-a","--parser",
+              type = click.STRING,
+              help = "Label set parser."\
+                " Built in options are cmu_parser")
 @click.option("-s", "--scheme",
               type=click.STRING,
               help = "Recoding scheme."\
                 " Built in options are cmu2labov and cmu2phila",
             required = True)
 @click.option("-r", "--recode_stem",
               type = click.STRING,
@@ -56,33 +61,37 @@
               help = "Target tier to recode",
               default = "Phone")
 def fave_recode(
     input_file = None,
     input_path = None,
     output_file = None,
     output_dest = None,
+    parser = None,
     scheme = None,
     save_recode = True,
     recode_stem = "_recoded",
     target_tier = "Phone"
 )->Union[AlignedTextGrid,list]:
+    parser = get_parser(parser)
     rules = get_rules(scheme)
     if input_file:
         input_p = Path(input_file.name)
         ratg = process_file(
             input_path=input_p, 
             output_file=output_file, 
+            parser = parser,
             scheme = rules, 
             recode_stem = recode_stem,
             save_recode = save_recode,
             target_tier = target_tier)
     if input_path:
         ratg = process_directory(
             input_path = input_path,
             output_dest = output_dest,
+            parser = parser,
             scheme = rules,
             recode_stem = recode_stem,
             target_tier = target_tier,
             save_recode = save_recode
         )
     return ratg
     
@@ -93,49 +102,67 @@
     if scheme in all_schemes:
         return RuleSet(rule_path = all_schemes[scheme])
     scheme_path = Path(scheme)
     if scheme_path.is_file():
         return RuleSet(rule_path = str(scheme_path))
     raise Exception(f"Cannot find rule schema file: {scheme}")
 
+def get_parser(
+        parser: str
+    ) -> LabelSetParser:
+    if not parser:
+        return LabelSetParser()
+    if parser in all_schemes:
+        return LabelSetParser(parser_path = Path(all_schemes[parser]))
+    scheme_path = Path(parser)
+    if scheme_path.is_file():
+        return LabelSetParser(parser_path = scheme_path)
+    raise Exception(f"Cannot find rule schema file: {parser}")
+
+
 def process_directory(
        input_path: str,
        scheme: RuleSet,
        save_recode: bool, 
+       parser: LabelSetParser = None,
        output_dest: Union[str,None] = None,
        recode_stem: str = "_recoded",
        target_tier: str = "Phone"
 ):
     input_path = Path(input_path)
     text_grids = get_target_list(input_path)
     ratg_list = []
     for tg in text_grids:
 
         ratg = process_file(
             input_path = tg,
+            parser = parser,
             scheme = scheme,
             save_recode = save_recode,
             output_file = output_dest,
             recode_stem=recode_stem,
             target_tier=target_tier
         )
         ratg_list.append(ratg)
     
     return ratg_list
 
 def process_file(
         input_path: Path, 
         scheme: RuleSet,
         save_recode: bool,
+        parser: LabelSetParser = None,
         output_file: str = None,
         recode_stem:str = "_recoded",
         target_tier: str = "Phone"
     ):
     atg = validate_input_file(input_path)
-    run_recode(atg, scheme, target_tier)
+    if not parser:
+        parser = LabelSetParser()
+    run_recode(atg, parser, scheme, target_tier)
 
     if output_file and save_recode:
         output_path = make_output_path(
             input_path=input_path,
             recode_stem=recode_stem,
             output_path=Path(output_file)
         )
@@ -223,21 +250,24 @@
         new_name = input_path.with_stem(input_stem+recode_stem).name
         return output_path.joinpath(new_name)
     
     return output_path
          
 def run_recode(
         atg: AlignedTextGrid, 
+        parser: LabelSetParser,
         scheme: RuleSet, 
         target_tier: str
     ):
     all_targets = [t for tgr in atg 
                    for t in tgr 
                    if t.entry_class.__name__ == target_tier]
     for tier in all_targets:
+        parser.map_parser(tier)
+    for tier in all_targets:
         scheme.map_ruleset(tier)
 
 def validate_input_file(
         input_path: Path
     ) -> AlignedTextGrid:
     try:
         atg = AlignedTextGrid(textgrid_path=str(input_path),
```

### Comparing `fave_recode-0.2.0/src/fave_recode/relations.py` & `fave_recode-0.3.0/src/fave_recode/relations.py`

 * *Files identical despite different names*

### Comparing `fave_recode-0.2.0/src/fave_recode/resources/cmu2labov.yml` & `fave_recode-0.3.0/src/fave_recode/resources/cmu2labov.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 - rule: schwa
   conditions:
     - attribute: label
       relation: ==
       set: AH0
-  return: "@"
+  return: "@_{stress}"
 - rule: eyf
   conditions: 
     - attribute: label
       relation: contains
       set: EY
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: eyF
+  return: eyF_{stress}
 - rule: iyF
   conditions: 
     - attribute: label
       relation: contains
       set: IY
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: iyF
+  return: iyF_{stress}
 - rule: owF
   conditions: 
     - attribute: label
       relation: contains
       set: OW
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: owF
+  return: owF_{stress}
 - rule: ay0
   conditions:
     - attribute: label
       relation: contains
       set: AY
     - attribute: fol.label
       relation: in
@@ -44,15 +44,15 @@
         - HH
         - K
         - P
         - S
         - SH
         - T
         - TH
-  return: ay0
+  return: ay0_{stress}
 - rule: ah
   conditions:
     - attribute: label
       relation: contains
       set: AA
     - attribute: inword.label
       relation: in
@@ -93,15 +93,15 @@
         - ALMOND
         - ALMONDS
         - LAGER
         - SALAMI
         - NIRVANA
         - KARATE
         - AH
-  return: ah
+  return: ah_{stress}
 - rule: Tuw
   conditions:
     - attribute: label
       relation: contains
       set: UW
     - attribute: prev.label
       relation: in
@@ -113,15 +113,15 @@
         - EN
         - L
         - N
         - R
         - S
         - T 
         - Z
-  return: Tuw
+  return: Tuw_{stress}
 - rule: iyr
   conditions:
     - attribute: label
       relation: in
       set: 
         - IH0
         - IH1
@@ -130,37 +130,37 @@
         - IY1
         - IY2
     - attribute: fol.label
       relation: in
       set: 
         - AXR
         - R
-  return: iyr
+  return: iyr_{stress}
 - rule: eyr
   conditions: 
     - attribute: label
       relation: contains
       set: EY
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: eyr
+  return: eyr_{stress}
 - rule: ahr
   conditions:
     - attribute: label
       relation: contains
       set: AA
     - attribute: fol.label
       relation: in
       set: 
         - AXR
         - R
-  return: ahr
+  return: ahr_{stress}
 - rule: owr
   conditions:
     - attribute: label
       relation: in
       set: 
         - AO0
         - AO1
@@ -169,15 +169,15 @@
         - OW1
         - OW2
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: owr
+  return: owr_{stress}
 - rule: uwr
   conditions: 
     - attribute: label
       relation: in
       set: 
         - UH0
         - UH1
@@ -186,100 +186,100 @@
         - UW1
         - UW2
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: uwr
+  return: uwr_{stress}
 - rule: o
   conditions:
     - attribute: label
       relation: contains
       set: AA
-  return: o
+  return: o_{stress}
 - rule: ae
   conditions: 
     - attribute: label
       relation: contains
       set: AE
-  return: ae
+  return: ae_{stress}
 - rule: wedge
   conditions:
     - attribute: label
       relation: in
       set:
         - AH1
         - AH2
-  return: uh
+  return: uh_{stress}
 - rule: oh
   conditions:
     - attribute: label
       relation: contains
       set: AO
-  return: oh
+  return: oh_{stress}
 - rule: aw
   conditions:
     - attribute: label
       relation: contains
       set: AW
-  return: aw
+  return: aw_{stress}
 - rule: ay
   conditions:
     - attribute: label
       relation: contains
       set: AY
-  return: ay
+  return: ay_{stress}
 - rule: e
   conditions:
     - attribute: label
       relation: contains
       set: "EH"
-  return: e
-- rule: "*hr"
+  return: e_{stress}
+- rule: "*hr_{stress}"
   conditions:
     - attribute: label
       relation: contains
       set: ER
-  return: "*hr"
+  return: "*hr_{stress}"
 - rule: ey
   conditions:
     - attribute: label
       relation: contains
       set: EY
-  return: ey
+  return: ey_{stress}
 - rule: i
   conditions:
     - attribute: label
       relation: contains
       set: IH
-  return: i
+  return: i_{stress}
 - rule: iy
   conditions:
     - attribute: label
       relation: contains
       set: IY
-  return: iy
+  return: iy_{stress}
 - rule: ow
   conditions:
     - attribute: label
       relation: contains
       set: OW
-  return: ow
+  return: ow_{stress}
 - rule: oy
   conditions: 
     - attribute: label
       relation: contains
       set: OY
-  return: oy
+  return: oy_{stress}
 - rule: u
   conditions: 
     - attribute: label
       relation: contains
       set: UH
-  return: u
+  return: u_{stress}
 - rule: uw
   conditions:
     - attribute: label
       relation: contains
       set: UW
-  return: uw
+  return: uw_{stress}
```

### Comparing `fave_recode-0.2.0/src/fave_recode/resources/cmu2phila.yml` & `fave_recode-0.3.0/src/fave_recode/resources/cmu2phila.yml`

 * *Files 11% similar despite different names*

```diff
@@ -4,58 +4,58 @@
       relation: rematches
       set: "[AEIOU]"
     - attribute: inword.label
       relation: in
       set:
         - KEPT
         - CATCH
-  return: e
+  return: e_{stress}
 
 - rule: a-foreign-a
   conditions:
     - attribute: label
       relation: ==
       set: AE1
     - attribute: inword.label
       relation: contains
       set: LANZA
-  return: o
+  return: o_{stress}
 
 # foriegn A-ae
 - rule: a-foreign-ae
   conditions:
     - attribute: label
       relation: ==
       set: AA1
     - attribute: inword.label
       relation: contains
       set: MARIO
-  return: ae
+  return: ae_{stress}
 
 # marry class
 - rule: marry
   conditions:
     - attribute: label
       relation: contains
       set: EH
     - attribute: inword.label
       relation: rematches
       set: "ARRY$"
-  return: ae
+  return: ae_{stress}
 
 # tense lexical exceptions
 - rule: aeh-lex
   conditions:
     - attribute: label
       relation: ==
       set: AE1
     - attribute: inword.label
       relation: rematches
       set: "(MAD|BAD|GLAD)(LY|DER|DEST|NESS)?$"
-  return: aeh
+  return: aeh_{stress}
 
 # lax lexical exceptions
 - rule: ae-lex
   conditions:
     - attribute: label
       relation: ==
       set: AE1
@@ -88,15 +88,15 @@
         - CAMERA 
         - AN'
         - AM
         - THAN
         - MATH
         - EXAM       
         - AND      
-  return: aeBR
+  return: aeBR_{stress}
 
 # SKV words
 - rule: ae-skv
   conditions:
     - attribute: label
       relation: ==
       set: AE1
@@ -111,26 +111,26 @@
         - K
     - attribute: fol.fol.fol.label
       relation: rematches
       set: "[AEIUO]"
     - attribute: inword.label
       relation: reunmatches
       set: "ING?$"
-  return: aeBR
+  return: aeBR_{stress}
 
 # aeL
 - rule: aeL
   conditions:
     - attribute: label
       relation: ==
       set: AE1
     - attribute: fol.label
       relation: ==
       set: L
-  return: aeBR
+  return: aeBR_{stress}
 
 # ae followed by trigger followed by end of word
 - rule: aeh-c-endword
   conditions:
     - attribute: label
       relation: ==
       set: AE1
@@ -141,15 +141,15 @@
         - N
         - S
         - TH
         - F
     - attribute: fol.fol.label
       relation: ==
       set: "#"
-  return: aeh
+  return: aeh_{stress}
 
 # ae followed by trigger followed by consonant
 - rule: aeh-c-X
   conditions:
     - attribute: label
       relation: ==
       set: AE1
@@ -183,15 +183,15 @@
         - SH
         - T
         - TH
         - V
         - W
         - Z
         - ZH
-  return: aeh
+  return: aeh_{stress}
 
 # ae followed by trigger and inflection
 - rule: aeh-ing-or-es
   conditions: 
     - attribute: label
       relation: ==
       set: AE1
@@ -216,15 +216,15 @@
         - Z
     - attribute: fol.fol.fol.fol.label
       relation: ==
       set: "#"
     - attribute: inword.label
       relation: rematches
       set: "(ING?|ES)$"      
-  return: "aeh"
+  return: aeh_{stress}
 
 # oh-fix
 - rule: oh-fix
   conditions:
     - attribute: label
       relation: contains
       set: AA
@@ -268,15 +268,15 @@
         - AWKWARDNESS
         - AWESOME
         - AUGUST
         - COUGH
         - COUGHS
         - COUGHED
         - COUGHING
-  return: oh
+  return: oh_{stress}
 
 # o-fix
 - rule: o-fix
   conditions:
     - attribute: label
       relation: contains
       set: AO
@@ -305,78 +305,78 @@
         - PONG
         - GONG
         - KONG
         - FLORIDA
         - ORANGE
         - HORRIBLE
         - MAJORITY
-  return: o
+  return: o_{stress}
 
 # iw
 - rule: iw-1
   conditions:
     - attribute: label
       relation: ==
       set: UW1
     - attribute: prev.label
       relation: == 
       set: Y
-  return: "iw"
+  return: iw_{stress}
 - rule: iw-2
   conditions:
     - attribute: label
       relation: ==
       set: UW1
     - attribute: inword.label
       relation: contains
       set: EW
-  return: "iw"
+  return: iw_{stress}
 - rule: iw-2
   conditions:
     - attribute: label
       relation: ==
       set: UW1
     - attribute: inword.label
       relation: rematches
       set: "[TDNLS]U"
-  return: iw
+  return: iw_{stress}
 
 - rule: schwa
   conditions:
     - attribute: label
       relation: ==
       set: AH0
-  return: "@"
+  return: "@_{stress}"
 - rule: eyf
   conditions: 
     - attribute: label
       relation: contains
       set: EY
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: eyF
+  return: eyF_{stress}
 - rule: iyF
   conditions: 
     - attribute: label
       relation: contains
       set: IY
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: iyF
+  return: iyF_{stress}
 - rule: owF
   conditions: 
     - attribute: label
       relation: contains
       set: OW
     - attribute: fol.label
       relation: ==
       set: "#"
-  return: owF
+  return: owF_{stress}
 - rule: ay0
   conditions:
     - attribute: label
       relation: contains
       set: AY
     - attribute: fol.label
       relation: in
@@ -386,15 +386,15 @@
         - HH
         - K
         - P
         - S
         - SH
         - T
         - TH
-  return: ay0
+  return: ay0_{stress}
 - rule: ah
   conditions:
     - attribute: label
       relation: contains
       set: AA
     - attribute: inword.label
       relation: in
@@ -435,15 +435,15 @@
         - ALMOND
         - ALMONDS
         - LAGER
         - SALAMI
         - NIRVANA
         - KARATE
         - AH
-  return: ah
+  return: ah_{stress}
 - rule: Tuw
   conditions:
     - attribute: label
       relation: contains
       set: UW
     - attribute: prev.label
       relation: in
@@ -455,15 +455,15 @@
         - EN
         - L
         - N
         - R
         - S
         - T 
         - Z
-  return: Tuw
+  return: Tuw_{stress}
 - rule: iyr
   conditions:
     - attribute: label
       relation: in
       set: 
         - IH0
         - IH1
@@ -472,37 +472,37 @@
         - IY1
         - IY2
     - attribute: fol.label
       relation: in
       set: 
         - AXR
         - R
-  return: iyr
+  return: iyr_{stress}
 - rule: eyr
   conditions: 
     - attribute: label
       relation: contains
       set: EY
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: eyr
+  return: eyr_{stress}
 - rule: ahr
   conditions:
     - attribute: label
       relation: contains
       set: AA
     - attribute: fol.label
       relation: in
       set: 
         - AXR
         - R
-  return: ahr
+  return: ahr_{stress}
 - rule: owr
   conditions:
     - attribute: label
       relation: in
       set: 
         - AO0
         - AO1
@@ -511,15 +511,15 @@
         - OW1
         - OW2
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: owr
+  return: owr_{stress}
 - rule: uwr
   conditions: 
     - attribute: label
       relation: in
       set: 
         - UH0
         - UH1
@@ -528,100 +528,100 @@
         - UW1
         - UW2
     - attribute: fol.label
       relation: in
       set:
         - AXR
         - R
-  return: uwr
+  return: uwr_{stress}
 - rule: o
   conditions:
     - attribute: label
       relation: contains
       set: AA
-  return: o
+  return: o_{stress}
 - rule: ae
   conditions: 
     - attribute: label
       relation: contains
       set: AE
-  return: ae
+  return: ae_{stress}
 - rule: wedge
   conditions:
     - attribute: label
       relation: in
       set:
         - AH1
         - AH2
-  return: uh
+  return: uh_{stress}
 - rule: oh
   conditions:
     - attribute: label
       relation: contains
       set: AO
-  return: oh
+  return: oh_{stress}
 - rule: aw
   conditions:
     - attribute: label
       relation: contains
       set: AW
-  return: aw
+  return: aw_{stress}
 - rule: ay
   conditions:
     - attribute: label
       relation: contains
       set: AY
-  return: ay
+  return: ay_{stress}
 - rule: e
   conditions:
     - attribute: label
       relation: contains
       set: "EH"
-  return: e
-- rule: "*hr"
+  return: e_{stress}
+- rule: "*hr_{stress}"
   conditions:
     - attribute: label
       relation: contains
       set: ER
-  return: "*hr"
+  return: "*hr_{stress}"
 - rule: ey
   conditions:
     - attribute: label
       relation: contains
       set: EY
-  return: ey
+  return: ey_{stress}
 - rule: i
   conditions:
     - attribute: label
       relation: contains
       set: IH
-  return: i
+  return: i_{stress}
 - rule: iy
   conditions:
     - attribute: label
       relation: contains
       set: IY
-  return: iy
+  return: iy_{stress}
 - rule: ow
   conditions:
     - attribute: label
       relation: contains
       set: OW
-  return: ow
+  return: ow_{stress}
 - rule: oy
   conditions: 
     - attribute: label
       relation: contains
       set: OY
-  return: oy
+  return: oy_{stress}
 - rule: u
   conditions: 
     - attribute: label
       relation: contains
       set: UH
-  return: u
+  return: u_{stress}
 - rule: uw
   conditions:
     - attribute: label
       relation: contains
       set: UW
-  return: uw
+  return: uw_{stress}
```

### Comparing `fave_recode-0.2.0/src/fave_recode/rule_classes.py` & `fave_recode-0.3.0/src/fave_recode/rule_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from aligned_textgrid.sequences.sequences import SequenceInterval
 from aligned_textgrid.sequences.tiers import SequenceTier
 from fave_recode.ruleschema import rule_validator, condition_validator
 from fave_recode.relations import relation_dict
 from collections.abc import Callable
 import functools
 import yaml
+import re
 
 def rgetattr(obj: SequenceInterval, 
              attr : str, 
              *args):
     """_gets object attribute from string_
 
     Args:
@@ -84,14 +85,18 @@
             rule: dict
     ):
         self.validate_rule(rule)
         self.conditions = [Condition(x) for x in rule["conditions"]]
         self.rule = rule["rule"]
         self.name = self.rule
         self.output = rule["return"]
+        if "updates" in rule:
+            self.updates = rule["updates"]
+        else:
+            self.updates = "label"
     
     def __repr__(self):
         return f"rule: {self.rule} with {len(self.conditions)} conditions. returns {self.output}"
     
     def validate_rule(
             self,
             rule:dict
@@ -125,16 +130,26 @@
         """
         try:
             cond_met = [c.check_condition(obj) for c in self.conditions]
         except:
             raise Exception
         
         if all(cond_met):
-            obj.label = self.output
+            output = self.parse_output(obj)
+            obj.set_feature(self.updates, output)
             return True
+        
+    def parse_output(self, obj):
+        get_features = re.findall(r"\{(.*?)\}", self.output)
+        feature_dict = {
+            f:rgetattr(obj, f)
+            for f in get_features
+        }
+        output = self.output.format(**feature_dict)
+        return output
 
 class RuleSet:
     """A rule set class
 
     Pass `RuleSet` either a rules dictionary, or a path 
     to a rules yaml file
 
@@ -173,14 +188,15 @@
             obj (SequenceInterval): The SequenceInterval undergoing rule application
         """
         for rule in self.rules:
             application = rule.apply_rule(obj)
             ## Crucial! 
             ## First rule wins
             if application:
+                return True
                 break
     
     def map_ruleset(
             self,
             obj: SequenceTier
     ):
         """_Apply the ruleset to all sequences_
```

### Comparing `fave_recode-0.2.0/setup.py` & `fave_recode-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 packages = \
 ['fave_recode']
 
 package_data = \
 {'': ['*'], 'fave_recode': ['resources/*']}
 
 install_requires = \
-['aligned-textgrid>=v0.4.1,<0.5.0',
+['aligned-textgrid>=0.6.4,<0.7.0',
  'cerberus>=1.3.5,<2.0.0',
  'click>=8.1.7,<9.0.0',
  'cloup>=3.0.2,<4.0.0',
  'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['fave_recode = fave_recode.fave_recode:fave_recode']}
 
 setup_kwargs = {
     'name': 'fave-recode',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A package for recoding Praat TextGrids',
-    'long_description': '# Getting started with `fave-recode`\n\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode/graph/badge.svg?token=C23B1H3DAX)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2375ddfef5d77ba1681d/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/fave-recode/maintainability)\n[![FAVE Python\nCI](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml/badge.svg?branch=dev)](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml)\n[![Build\nDocs](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/fave-recode/)\n\nThe idea behind `fave-recode` is that no matter how much you may adjust\nthe dictionary of a forced-aligner, you may still want to make\nprogrammatic changes to the output.\n\n## Installation\n\nYou can install `fave-recode` at your system’s command line with `pip`.\n\n``` bash\npip install fave-recode\n```\n\n## Basic usage\n\nInstallation of the `fave-recode` python package makes the `fave_recode`\nexecutable, which can also be run at the command line. You can get help\nwith `--help`\n\n``` bash\nfave_recode --help\n```\n\n    Usage: fave_recode [OPTIONS]\n\n    Inputs: [at least 1 required]\n      File inputs. Either a single file with -i or a path with -p. Not both.\n      -i, --input_file FILENAME  single input file\n      -p, --input_path PATH      Path to a set of files\n\n    Outputs:\n      -o, --output_file TEXT     An output file name\n      -d, --output_dest PATH     An output directory\n\n    Other options:\n      -s, --scheme TEXT          Recoding scheme. Built in options are cmu2labov\n                                 and cmu2phila  [required]\n      -r, --recode_stem TEXT     Stem to append to recoded TextGrid file names\n      -t, --target_tier TEXT     Target tier to recode\n      --help                     Show this message and exit.\n\nTo recode a single file, you need to provide `fave_recode` with,\nminimally, the input file (the `-i` flag), and the recoding scheme (with\nthe `-s` flag). There are a few default recoding schemes that come with\n`fave_recode`.\n\n``` bash\nls data\n```\n\n    KY25A_1.TextGrid                 josef-fruehwald_speaker.TextGrid\n\n``` bash\nfave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila\n\nls data\n```\n\n    KY25A_1.TextGrid\n    josef-fruehwald_speaker.TextGrid\n    josef-fruehwald_speaker_recoded.TextGrid\n',
+    'long_description': '# Getting started with `fave-recode`\n\n\n![PyPI](https://img.shields.io/pypi/v/fave-recode.png)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode/graph/badge.svg?token=C23B1H3DAX)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2375ddfef5d77ba1681d/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/fave-recode/maintainability)\n[![FAVE Python\nCI](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml/badge.svg?branch=dev)](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml)\n[![Build\nDocs](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/fave-recode/)\n[![DOI](https://zenodo.org/badge/605740158.svg)](https://zenodo.org/badge/latestdoi/605740158)\n\nThe idea behind `fave-recode` is that no matter how much you may adjust\nthe dictionary of a forced-aligner, you may still want to make\nprogrammatic changes to the output.\n\n## Installation\n\nYou can install `fave-recode` at your system’s command line with `pip`.\n\n``` bash\npip install fave-recode\n```\n\n## Basic usage\n\nInstallation of the `fave-recode` python package makes the `fave_recode`\nexecutable, which can also be run at the command line. You can get help\nwith `--help`\n\n``` bash\nfave_recode --help\n```\n\n    Usage: fave_recode [OPTIONS]\n\n    Inputs: [at least 1 required]\n      File inputs. Either a single file with -i or a path with -p. Not both.\n      -i, --input_file FILENAME  single input file\n      -p, --input_path PATH      Path to a set of files\n\n    Outputs:\n      -o, --output_file TEXT     An output file name\n      -d, --output_dest PATH     An output directory\n\n    Other options:\n      -a, --parser TEXT          Label set parser. Built in options are cmu_parser\n      -s, --scheme TEXT          Recoding scheme. Built in options are cmu2labov\n                                 and cmu2phila  [required]\n      -r, --recode_stem TEXT     Stem to append to recoded TextGrid file names\n      -t, --target_tier TEXT     Target tier to recode\n      --help                     Show this message and exit.\n\nTo recode a single file, you need to provide `fave_recode` with,\nminimally, the input file (the `-i` flag), and the recoding scheme (with\nthe `-s` flag). There are a few default recoding schemes that come with\n`fave_recode`.\n\n``` bash\nls data\n```\n\n    KY25A_1.TextGrid                 josef-fruehwald_speaker.TextGrid\n\n``` bash\nfave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila -a cmu_parser\n\nls data\n```\n\n    KY25A_1.TextGrid\n    josef-fruehwald_speaker.TextGrid\n    josef-fruehwald_speaker_recoded.TextGrid\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://forced-alignment-and-vowel-extraction.github.io/fave-recode',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fave_recode-0.2.0/PKG-INFO` & `fave_recode-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: fave-recode
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package for recoding Praat TextGrids
 Home-page: https://forced-alignment-and-vowel-extraction.github.io/fave-recode
 License: GPLv3
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aligned-textgrid (>=v0.4.1,<0.5.0)
+Requires-Dist: aligned-textgrid (>=0.6.4,<0.7.0)
 Requires-Dist: cerberus (>=1.3.5,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloup (>=3.0.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode
 Description-Content-Type: text/markdown
 
 # Getting started with `fave-recode`
 
+
+![PyPI](https://img.shields.io/pypi/v/fave-recode.png)
 [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode/graph/badge.svg?token=C23B1H3DAX)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-recode)
 [![Maintainability](https://api.codeclimate.com/v1/badges/2375ddfef5d77ba1681d/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/fave-recode/maintainability)
 [![FAVE Python
 CI](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml/badge.svg?branch=dev)](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/test-and-run.yml)
 [![Build
 Docs](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-recode/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/fave-recode/)
+[![DOI](https://zenodo.org/badge/605740158.svg)](https://zenodo.org/badge/latestdoi/605740158)
 
 The idea behind `fave-recode` is that no matter how much you may adjust
 the dictionary of a forced-aligner, you may still want to make
 programmatic changes to the output.
 
 ## Installation
 
@@ -58,14 +61,15 @@
       -p, --input_path PATH      Path to a set of files
 
     Outputs:
       -o, --output_file TEXT     An output file name
       -d, --output_dest PATH     An output directory
 
     Other options:
+      -a, --parser TEXT          Label set parser. Built in options are cmu_parser
       -s, --scheme TEXT          Recoding scheme. Built in options are cmu2labov
                                  and cmu2phila  [required]
       -r, --recode_stem TEXT     Stem to append to recoded TextGrid file names
       -t, --target_tier TEXT     Target tier to recode
       --help                     Show this message and exit.
 
 To recode a single file, you need to provide `fave_recode` with,
@@ -76,15 +80,15 @@
 ``` bash
 ls data
 ```
 
     KY25A_1.TextGrid                 josef-fruehwald_speaker.TextGrid
 
 ``` bash
-fave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila
+fave_recode -i data/josef-fruehwald_speaker.TextGrid -s cmu2phila -a cmu_parser
 
 ls data
 ```
 
     KY25A_1.TextGrid
     josef-fruehwald_speaker.TextGrid
     josef-fruehwald_speaker_recoded.TextGrid
```

