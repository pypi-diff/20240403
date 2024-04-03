# Comparing `tmp/FactScoreLite-0.1.0.tar.gz` & `tmp/FactScoreLite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FactScoreLite-0.1.0.tar", last modified: Sat Mar 30 18:02:31 2024, max compression
+gzip compressed data, was "FactScoreLite-0.2.0.tar", last modified: Tue Apr  2 18:51:50 2024, max compression
```

## Comparing `FactScoreLite-0.1.0.tar` & `FactScoreLite-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 18:02:31.328579 FactScoreLite-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:02:31.291677 FactScoreLite-0.1.0/FactScoreLite/
--rw-rw-rw-   0        0        0        0 2024-03-28 17:32:35.000000 FactScoreLite-0.1.0/FactScoreLite/__init__.py
--rw-rw-rw-   0        0        0     4799 2024-03-30 17:17:03.000000 FactScoreLite-0.1.0/FactScoreLite/atomic_facts.py
--rw-rw-rw-   0        0        0      152 2024-03-30 17:11:34.000000 FactScoreLite-0.1.0/FactScoreLite/configs.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:02:31.325588 FactScoreLite-0.1.0/FactScoreLite/data/
--rw-rw-rw-   0        0        0     5560 2024-03-28 23:07:04.000000 FactScoreLite-0.1.0/FactScoreLite/data/demons.json
--rw-rw-rw-   0        0        0     2764 2024-03-30 16:37:05.000000 FactScoreLite-0.1.0/FactScoreLite/data/demons_generation_prompt.txt
--rw-rw-rw-   0        0        0      547 2024-03-30 14:43:16.000000 FactScoreLite-0.1.0/FactScoreLite/openai_agent.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:02:31.321598 FactScoreLite-0.1.0/FactScoreLite.egg-info/
--rw-rw-rw-   0        0        0      490 2024-03-30 18:02:31.000000 FactScoreLite-0.1.0/FactScoreLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-03-30 18:02:31.000000 FactScoreLite-0.1.0/FactScoreLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 18:02:31.000000 FactScoreLite-0.1.0/FactScoreLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-30 18:02:31.000000 FactScoreLite-0.1.0/FactScoreLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-30 18:02:31.000000 FactScoreLite-0.1.0/FactScoreLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-03-26 22:42:51.000000 FactScoreLite-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      490 2024-03-30 18:02:31.327581 FactScoreLite-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       62 2024-03-26 22:42:51.000000 FactScoreLite-0.1.0/README.md
--rw-rw-rw-   0        0        0      523 2024-03-30 18:02:31.331572 FactScoreLite-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-03-30 17:43:43.000000 FactScoreLite-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/FactScoreLite/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/FactScoreLite/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/data/demons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/data/demons_generation_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/FactScoreLite/openai_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/FactScoreLite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 18:51:50.000000 FactScoreLite-0.2.0/FactScoreLite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-02 18:51:50.000000 FactScoreLite-0.2.0/FactScoreLite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:51:50.000000 FactScoreLite-0.2.0/FactScoreLite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 18:51:50.000000 FactScoreLite-0.2.0/FactScoreLite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 18:51:50.000000 FactScoreLite-0.2.0/FactScoreLite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:50.126337 FactScoreLite-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/tests/test_atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-02 18:51:44.000000 FactScoreLite-0.2.0/tests/test_openai_agent.py
```

### Comparing `FactScoreLite-0.1.0/FactScoreLite/atomic_facts.py` & `FactScoreLite-0.2.0/FactScoreLite/atomic_facts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,143 +1,140 @@
-import re
-import numpy as np
-from nltk.tokenize import sent_tokenize
-from openai_agent import OpenAIAgent
-import configs
-import json
-
-# next steps
-# 1. remove refs in data
-
-
-class AtomicFactGenerator:
-    def __init__(self):
-        self.demons = self.load_demons()
-        self.openai_lm = OpenAIAgent()
-
-    def run(self, text):
-        sentences = []
-
-        initials = self.detect_initials(text)
-        sentences = sent_tokenize(text)
-        sentences = self.fix_sentence_splitter(sentences, initials)
-
-        atoms = []
-        for sent in sentences:
-            atom = self.get_sentence_af(sent)
-            atoms.append((sent, atom))
-
-        return atoms
-
-    def load_demons(self):
-        with open(configs.demons_path, "r") as file:
-            demons = json.load(file)
-
-        return demons
-
-    def get_instructions(self):
-        # n = 8
-        instructions = (
-            "Please breakdown the following sentence into independent facts:\n\n"
-        )
-
-        for demon in self.demons:
-            sentence = demon["Sentence"]
-            facts = demon["Independent Facts"]
-
-            instructions += f"Sentence:\n{sentence}\n"
-
-            instructions += "Independent Facts:\n"
-
-            for fact in facts:
-                instructions += "- {}\n".format(fact)
-
-            instructions += "\n\n"
-
-        return instructions
-
-    def get_sentence_af(self, sent):
-        atoms = None
-        instructions = self.get_instructions()
-
-        prompt = instructions + f"Sentence: {sent}\nIndependent Facts:"
-
-        output = self.openai_lm.generate(prompt)
-        atoms = self.text_to_sentences(output)
-
-        return atoms
-
-    def text_to_sentences(self, text):
-        sentences = text.split("- ")[1:]
-        sentences = [
-            sent.strip()[:-1] if sent.strip()[-1] == "\n" else sent.strip()
-            for sent in sentences
-        ]
-        if len(sentences) > 0:
-            if sentences[-1][-1] != ".":
-                sentences[-1] = sentences[-1] + "."
-        else:
-            sentences = []
-
-        return sentences
-
-    def detect_initials(self, text):
-        pattern = r"[A-Z]\. ?[A-Z]\."
-        match = re.findall(pattern, text)
-        return [m for m in match]
-
-    def fix_sentence_splitter(self, sentences, initials):
-        for initial in initials:
-            if not np.any([initial in sent for sent in sentences]):
-                alpha1, alpha2 = [
-                    t.strip() for t in initial.split(".") if len(t.strip()) > 0
-                ]
-                for i, (sent1, sent2) in enumerate(zip(sentences, sentences[1:])):
-                    if sent1.endswith(alpha1 + ".") and sent2.startswith(alpha2 + "."):
-                        # merge sentence i and i+1
-                        sentences = (
-                            sentences[:i]
-                            + [sentences[i] + " " + sentences[i + 1]]
-                            + sentences[i + 2 :]
-                        )
-                        break
-
-        results = []
-        combine_with_previous = None
-
-        for sent_idx, sent in enumerate(sentences):
-            if len(sent.split()) <= 1 and sent_idx == 0:
-                assert not combine_with_previous
-                combine_with_previous = True
-                results.append(sent)
-            elif len(sent.split()) <= 1:
-                assert sent_idx > 0
-                results[-1] += " " + sent
-                combined_with_previous = False
-            elif sent[0].isalpha() and not sent[0].isupper() and sent_idx > 0:
-                assert sent_idx > 0, results
-                results[-1] += " " + sent
-                combine_with_previous = False
-            elif combine_with_previous:
-                assert sent_idx > 0
-                results[-1] += " " + sent
-                combine_with_previous = False
-            else:
-                assert not combine_with_previous
-                results.append(sent)
-        return results
-
-
-if __name__ == "__main__":
-    generator = AtomicFactGenerator()
-    text = """
-To winterize your battery and prevent damage:
- 
- 1. **For the Li-ion battery**:
-  - Avoid storing the vehicle in temperatures below -13°F (-25°C) for more than seven days to prevent the Li-ion battery from freezing.
-  - Move the vehicle to a warm location if the outside temperature is -13°F (-25°C) or below, as it may freeze and be unable to charge or power the vehicle.
- 
- 2. **For the 12-volt battery**:
-  - Ensure it is fully charged during extremely cold weather conditions to prevent the battery fluid from freezing and possibly causing damage to the battery.
-""".strip()
-
-    print(generator.run(text))
+import re
+import numpy as np
+from nltk.tokenize import sent_tokenize
+from .openai_agent import OpenAIAgent
+from . import configs
+import json
+
+
+class AtomicFactGenerator:
+    def __init__(self):
+        self.demons = self.load_demons()
+        self.openai_agent = OpenAIAgent()
+
+    def run(self, text):
+        sentences = []
+
+        initials = self.detect_initials(text)
+        sentences = sent_tokenize(text)
+        sentences = self.fix_sentence_splitter(sentences, initials)
+
+        atoms = []
+        for sent in sentences:
+            atom = self.get_sentence_af(sent)
+            atoms.append((sent, atom))
+
+        return atoms
+
+    def load_demons(self):
+        with open(configs.demons_path, "r") as file:
+            demons = json.load(file)
+
+        return demons
+
+    def get_instructions(self):
+        # n = 8
+        instructions = (
+            "Please breakdown the following sentence into independent facts:\n\n"
+        )
+
+        for demon in self.demons:
+            sentence = demon["Sentence"]
+            facts = demon["Independent Facts"]
+
+            instructions += f"Sentence:\n{sentence}\n"
+
+            instructions += "Independent Facts:\n"
+
+            for fact in facts:
+                instructions += "- {}\n".format(fact)
+
+            instructions += "\n\n"
+
+        return instructions
+
+    def get_sentence_af(self, sent):
+        atoms = None
+        instructions = self.get_instructions()
+
+        prompt = instructions + f"Sentence: {sent}\nIndependent Facts:"
+
+        output = self.openai_agent.generate(prompt)
+        atoms = self.gpt_output_to_sentences(output)
+
+        return atoms
+
+    def gpt_output_to_sentences(self, text):
+        sentences = text.split("- ")[1:]
+        sentences = [
+            sent.strip()[:-1] if sent.strip()[-1] == "\n" else sent.strip()
+            for sent in sentences
+        ]
+        if len(sentences) > 0:
+            if sentences[-1][-1] != ".":
+                sentences[-1] = sentences[-1] + "."
+        else:
+            sentences = []
+
+        return sentences
+
+    def detect_initials(self, text):
+        pattern = r"[A-Z]\. ?[A-Z]\."
+        return re.findall(pattern, text)
+
+    def fix_sentence_splitter(self, sentences, initials):
+        for initial in initials:
+            if not np.any([initial in sent for sent in sentences]):
+                alpha1, alpha2 = [
+                    t.strip() for t in initial.split(".") if len(t.strip()) > 0
+                ]
+                for i, (sent1, sent2) in enumerate(zip(sentences, sentences[1:])):
+                    if sent1.endswith(alpha1 + ".") and sent2.startswith(alpha2 + "."):
+                        # merge sentence i and i+1
+                        sentences = (
+                            sentences[:i]
+                            + [sentences[i] + " " + sentences[i + 1]]
+                            + sentences[i + 2 :]
+                        )
+                        break
+
+        results = []
+        combine_with_previous = None
+
+        for sent_idx, sent in enumerate(sentences):
+            if len(sent.split()) <= 1 and sent_idx == 0:
+                assert not combine_with_previous
+                combine_with_previous = True
+                results.append(sent)
+            elif len(sent.split()) <= 1:
+                assert sent_idx > 0
+                results[-1] += " " + sent
+                combined_with_previous = False
+            elif sent[0].isalpha() and not sent[0].isupper() and sent_idx > 0:
+                assert sent_idx > 0, results
+                results[-1] += " " + sent
+                combine_with_previous = False
+            elif combine_with_previous:
+                assert sent_idx > 0
+                results[-1] += " " + sent
+                combine_with_previous = False
+            else:
+                assert not combine_with_previous
+                results.append(sent)
+
+        return results
+
+
+if __name__ == "__main__":
+    generator = AtomicFactGenerator()
+    text = """
+To winterize your battery and prevent damage:
+ 
+ 1. **For the Li-ion battery**:
+  - Avoid storing the vehicle in temperatures below -13°F (-25°C) for more than seven days to prevent the Li-ion battery from freezing.
+  - Move the vehicle to a warm location if the outside temperature is -13°F (-25°C) or below, as it may freeze and be unable to charge or power the vehicle.
+ 
+ 2. **For the 12-volt battery**:
+  - Ensure it is fully charged during extremely cold weather conditions to prevent the battery fluid from freezing and possibly causing damage to the battery.
+""".strip()
+
+    print(generator.run(text))
```

### Comparing `FactScoreLite-0.1.0/FactScoreLite/data/demons.json` & `FactScoreLite-0.2.0/FactScoreLite/data/demons.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 15% similar despite different names*

```diff
@@ -1,348 +1,342 @@
-00000000: 0d0a 5b0d 0a20 207b 0d0a 2020 2020 2253  ..[..  {..    "S
-00000010: 656e 7465 6e63 6522 3a20 2254 6865 2054  entence": "The T
-00000020: 7572 626f 2056 3620 656e 6769 6e65 2062  urbo V6 engine b
-00000030: 6f61 7374 7320 616e 2069 6d70 7265 7373  oasts an impress
-00000040: 6976 6520 686f 7273 6570 6f77 6572 206f  ive horsepower o
-00000050: 6620 3435 3020 616e 6420 6120 7065 616b  f 450 and a peak
-00000060: 2074 6f72 7175 6520 6f66 2035 3130 206c   torque of 510 l
-00000070: 622d 6674 2c20 6163 6869 6576 6564 2062  b-ft, achieved b
-00000080: 6574 7765 656e 2032 2c35 3030 2061 6e64  etween 2,500 and
-00000090: 2035 2c35 3030 2072 706d 2c20 6571 7569   5,500 rpm, equi
-000000a0: 7070 6564 2077 6974 6820 6120 3130 2d73  pped with a 10-s
-000000b0: 7065 6564 2061 7574 6f6d 6174 6963 2074  peed automatic t
-000000c0: 7261 6e73 6d69 7373 696f 6e20 616e 6420  ransmission and 
-000000d0: 6120 6475 616c 2d65 7868 6175 7374 2073  a dual-exhaust s
-000000e0: 7973 7465 6d2c 2065 6e68 616e 6369 6e67  ystem, enhancing
-000000f0: 2062 6f74 6820 7065 7266 6f72 6d61 6e63   both performanc
-00000100: 6520 616e 6420 736f 756e 642e 222c 0d0a  e and sound.",..
-00000110: 2020 2020 2249 6e64 6570 656e 6465 6e74      "Independent
-00000120: 2046 6163 7473 223a 205b 0d0a 2020 2020   Facts": [..    
-00000130: 2020 2249 7420 6861 7320 6120 5475 7262    "It has a Turb
-00000140: 6f20 5636 2065 6e67 696e 652e 222c 0d0a  o V6 engine.",..
-00000150: 2020 2020 2020 2254 6865 2068 6f72 7365        "The horse
-00000160: 706f 7765 7220 6973 2034 3530 2e22 2c0d  power is 450.",.
-00000170: 0a20 2020 2020 2022 5468 6520 7065 616b  .      "The peak
-00000180: 2074 6f72 7175 6520 6973 2035 3130 206c   torque is 510 l
-00000190: 622d 6674 2e22 2c0d 0a20 2020 2020 2022  b-ft.",..      "
-000001a0: 5065 616b 2074 6f72 7175 6520 6f63 6375  Peak torque occu
-000001b0: 7273 2062 6574 7765 656e 2032 2c35 3030  rs between 2,500
-000001c0: 2061 6e64 2035 2c35 3030 2072 706d 2e22   and 5,500 rpm."
-000001d0: 2c0d 0a20 2020 2020 2022 5468 6520 7665  ,..      "The ve
-000001e0: 6869 636c 6520 6861 7320 6120 3130 2d73  hicle has a 10-s
-000001f0: 7065 6564 2061 7574 6f6d 6174 6963 2074  peed automatic t
-00000200: 7261 6e73 6d69 7373 696f 6e2e 222c 0d0a  ransmission.",..
-00000210: 2020 2020 2020 2249 7420 6665 6174 7572        "It featur
-00000220: 6573 2061 2064 7561 6c2d 6578 6861 7573  es a dual-exhaus
-00000230: 7420 7379 7374 656d 2e22 2c0d 0a20 2020  t system.",..   
-00000240: 2020 2022 5468 6520 6475 616c 2d65 7868     "The dual-exh
-00000250: 6175 7374 2073 7973 7465 6d20 656e 6861  aust system enha
-00000260: 6e63 6573 2070 6572 666f 726d 616e 6365  nces performance
-00000270: 2e22 2c0d 0a20 2020 2020 2022 5468 6520  .",..      "The 
-00000280: 6475 616c 2d65 7868 6175 7374 2073 7973  dual-exhaust sys
-00000290: 7465 6d20 656e 6861 6e63 6573 2073 6f75  tem enhances sou
-000002a0: 6e64 2e22 0d0a 2020 2020 5d0d 0a20 207d  nd."..    ]..  }
-000002b0: 2c0d 0a20 207b 0d0a 2020 2020 2253 656e  ,..  {..    "Sen
-000002c0: 7465 6e63 6522 3a20 2241 6363 6f72 6469  tence": "Accordi
-000002d0: 6e67 2074 6f20 7468 6520 6d61 696e 7465  ng to the mainte
-000002e0: 6e61 6e63 6520 7363 6865 6475 6c65 2069  nance schedule i
-000002f0: 6e20 7468 6520 6f77 6e65 7227 7320 6d61  n the owner's ma
-00000300: 6e75 616c 2c20 7468 6520 636f 6f6c 616e  nual, the coolan
-00000310: 7420 666c 7569 6420 7368 6f75 6c64 2062  t fluid should b
-00000320: 6520 7265 706c 6163 6564 2065 7665 7279  e replaced every
-00000330: 2034 302c 3030 3020 6d69 6c65 7320 6f72   40,000 miles or
-00000340: 2034 2079 6561 7273 2c20 7768 6963 6865   4 years, whiche
-00000350: 7665 7220 636f 6d65 7320 6669 7273 742c  ver comes first,
-00000360: 2074 6f20 656e 7375 7265 206f 7074 696d   to ensure optim
-00000370: 616c 2065 6e67 696e 6520 7065 7266 6f72  al engine perfor
-00000380: 6d61 6e63 6520 616e 6420 7072 6576 656e  mance and preven
-00000390: 7420 6f76 6572 6865 6174 696e 672e 222c  t overheating.",
-000003a0: 0d0a 2020 2020 2249 6e64 6570 656e 6465  ..    "Independe
-000003b0: 6e74 2046 6163 7473 223a 205b 0d0a 2020  nt Facts": [..  
-000003c0: 2020 2020 2254 6865 2063 6f6f 6c61 6e74      "The coolant
-000003d0: 2066 6c75 6964 2072 6570 6c61 6365 6d65   fluid replaceme
-000003e0: 6e74 2069 7320 6d65 6e74 696f 6e65 6420  nt is mentioned 
-000003f0: 696e 2074 6865 206d 6169 6e74 656e 616e  in the maintenan
-00000400: 6365 2073 6368 6564 756c 652e 222c 0d0a  ce schedule.",..
-00000410: 2020 2020 2020 2254 6865 206f 776e 6572        "The owner
-00000420: 2773 206d 616e 7561 6c20 636f 6e74 6169  's manual contai
-00000430: 6e73 2074 6865 206d 6169 6e74 656e 616e  ns the maintenan
-00000440: 6365 2073 6368 6564 756c 652e 222c 0d0a  ce schedule.",..
-00000450: 2020 2020 2020 2243 6f6f 6c61 6e74 2066        "Coolant f
-00000460: 6c75 6964 2073 686f 756c 6420 6265 2072  luid should be r
-00000470: 6570 6c61 6365 6420 6576 6572 7920 3430  eplaced every 40
-00000480: 2c30 3030 206d 696c 6573 2e22 2c0d 0a20  ,000 miles.",.. 
-00000490: 2020 2020 2022 416c 7465 726e 6174 6976       "Alternativ
-000004a0: 656c 792c 2063 6f6f 6c61 6e74 2066 6c75  ely, coolant flu
-000004b0: 6964 2073 686f 756c 6420 6265 2072 6570  id should be rep
-000004c0: 6c61 6365 6420 6576 6572 7920 3420 7965  laced every 4 ye
-000004d0: 6172 732e 222c 0d0a 2020 2020 2020 2252  ars.",..      "R
-000004e0: 6570 6c61 6365 6d65 6e74 2069 7320 6261  eplacement is ba
-000004f0: 7365 6420 6f6e 2077 6869 6368 6576 6572  sed on whichever
-00000500: 206d 696c 6573 746f 6e65 2069 7320 7265   milestone is re
-00000510: 6163 6865 6420 6669 7273 742e 222c 0d0a  ached first.",..
-00000520: 2020 2020 2020 2254 6865 2070 7572 706f        "The purpo
-00000530: 7365 2069 7320 746f 2065 6e73 7572 6520  se is to ensure 
-00000540: 6f70 7469 6d61 6c20 656e 6769 6e65 2070  optimal engine p
-00000550: 6572 666f 726d 616e 6365 2e22 2c0d 0a20  erformance.",.. 
-00000560: 2020 2020 2022 416e 6f74 6865 7220 7075       "Another pu
-00000570: 7270 6f73 6520 6973 2074 6f20 7072 6576  rpose is to prev
-00000580: 656e 7420 6f76 6572 6865 6174 696e 672e  ent overheating.
-00000590: 220d 0a20 2020 205d 0d0a 2020 7d2c 0d0a  "..    ]..  },..
-000005a0: 2020 7b0d 0a20 2020 2022 5365 6e74 656e    {..    "Senten
-000005b0: 6365 223a 2022 4665 6174 7572 696e 6720  ce": "Featuring 
-000005c0: 6164 7661 6e63 6564 2073 6166 6574 7920  advanced safety 
-000005d0: 7465 6368 6e6f 6c6f 6779 2c20 7468 6520  technology, the 
-000005e0: 3230 3232 2056 6972 7475 6520 5365 6461  2022 Virtue Seda
-000005f0: 6e20 696e 636f 7270 6f72 6174 6573 2061  n incorporates a
-00000600: 6e20 6175 746f 6d61 7469 6320 656d 6572  n automatic emer
-00000610: 6765 6e63 7920 6272 616b 696e 6720 7379  gency braking sy
-00000620: 7374 656d 2c20 6120 6c61 6e65 2d6b 6565  stem, a lane-kee
-00000630: 7069 6e67 2061 7373 6973 7420 6665 6174  ping assist feat
-00000640: 7572 652c 2061 6e64 2061 6461 7074 6976  ure, and adaptiv
-00000650: 6520 6372 7569 7365 2063 6f6e 7472 6f6c  e cruise control
-00000660: 2c20 616c 6c20 6465 7369 676e 6564 2074  , all designed t
-00000670: 6f20 636f 6d70 6c79 2077 6974 6820 7468  o comply with th
-00000680: 6520 6c61 7465 7374 2045 7572 6f20 4e43  e latest Euro NC
-00000690: 4150 2073 6166 6574 7920 7374 616e 6461  AP safety standa
-000006a0: 7264 732e 222c 0d0a 2020 2020 2249 6e64  rds.",..    "Ind
-000006b0: 6570 656e 6465 6e74 2046 6163 7473 223a  ependent Facts":
-000006c0: 205b 0d0a 2020 2020 2020 2254 6865 206d   [..      "The m
-000006d0: 6f64 656c 2079 6561 7220 6973 2032 3032  odel year is 202
-000006e0: 322e 222c 0d0a 2020 2020 2020 2254 6865  2.",..      "The
-000006f0: 206d 6f64 656c 2069 7320 7468 6520 5669   model is the Vi
-00000700: 7274 7565 2053 6564 616e 2e22 2c0d 0a20  rtue Sedan.",.. 
-00000710: 2020 2020 2022 4974 2066 6561 7475 7265       "It feature
-00000720: 7320 6164 7661 6e63 6564 2073 6166 6574  s advanced safet
-00000730: 7920 7465 6368 6e6f 6c6f 6779 2e22 2c0d  y technology.",.
-00000740: 0a20 2020 2020 2022 5468 6520 7465 6368  .      "The tech
-00000750: 6e6f 6c6f 6779 2069 6e63 6c75 6465 7320  nology includes 
-00000760: 616e 2061 7574 6f6d 6174 6963 2065 6d65  an automatic eme
-00000770: 7267 656e 6379 2062 7261 6b69 6e67 2073  rgency braking s
-00000780: 7973 7465 6d2e 222c 0d0a 2020 2020 2020  ystem.",..      
-00000790: 2249 7420 616c 736f 2069 6e63 6c75 6465  "It also include
-000007a0: 7320 6120 6c61 6e65 2d6b 6565 7069 6e67  s a lane-keeping
-000007b0: 2061 7373 6973 7420 6665 6174 7572 652e   assist feature.
-000007c0: 222c 0d0a 2020 2020 2020 2241 6461 7074  ",..      "Adapt
-000007d0: 6976 6520 6372 7569 7365 2063 6f6e 7472  ive cruise contr
-000007e0: 6f6c 2069 7320 616e 6f74 6865 7220 696e  ol is another in
-000007f0: 636c 7564 6564 2074 6563 686e 6f6c 6f67  cluded technolog
-00000800: 792e 222c 0d0a 2020 2020 2020 2241 6c6c  y.",..      "All
-00000810: 2074 6563 686e 6f6c 6f67 6965 7320 6172   technologies ar
-00000820: 6520 6465 7369 676e 6564 2074 6f20 636f  e designed to co
-00000830: 6d70 6c79 2077 6974 6820 4575 726f 204e  mply with Euro N
-00000840: 4341 5020 7361 6665 7479 2073 7461 6e64  CAP safety stand
-00000850: 6172 6473 2e22 0d0a 2020 2020 5d0d 0a20  ards."..    ].. 
-00000860: 207d 2c0d 0a20 207b 0d0a 2020 2020 2253   },..  {..    "S
-00000870: 656e 7465 6e63 6522 3a20 2254 6865 2047  entence": "The G
-00000880: 5420 4861 776b 2043 6f75 7065 2773 204c  T Hawk Coupe's L
-00000890: 4544 2068 6561 646c 6967 6874 7320 6172  ED headlights ar
-000008a0: 6520 7072 6f67 7261 6d6d 6162 6c65 2066  e programmable f
-000008b0: 6f72 2061 7574 6f6d 6174 6963 2061 646a  or automatic adj
-000008c0: 7573 746d 656e 7420 6261 7365 6420 6f6e  ustment based on
-000008d0: 2065 7874 6572 696f 7220 6c69 6768 7420   exterior light 
-000008e0: 636f 6e64 6974 696f 6e73 2c20 6665 6174  conditions, feat
-000008f0: 7572 696e 6720 6479 6e61 6d69 6320 6265  uring dynamic be
-00000900: 6e64 696e 6720 6c69 6768 7420 7465 6368  nding light tech
-00000910: 6e6f 6c6f 6779 2074 6861 7420 6164 6a75  nology that adju
-00000920: 7374 7320 7468 6520 6265 616d 2064 6972  sts the beam dir
-00000930: 6563 7469 6f6e 2064 7572 696e 6720 7475  ection during tu
-00000940: 726e 7320 746f 2065 6e68 616e 6365 2076  rns to enhance v
-00000950: 6973 6962 696c 6974 792e 222c 0d0a 2020  isibility.",..  
-00000960: 2020 2249 6e64 6570 656e 6465 6e74 2046    "Independent F
-00000970: 6163 7473 223a 205b 0d0a 2020 2020 2020  acts": [..      
-00000980: 2254 6865 206d 6f64 656c 2069 7320 7468  "The model is th
-00000990: 6520 4754 2048 6177 6b20 436f 7570 652e  e GT Hawk Coupe.
-000009a0: 222c 0d0a 2020 2020 2020 2249 7420 6861  ",..      "It ha
-000009b0: 7320 4c45 4420 6865 6164 6c69 6768 7473  s LED headlights
-000009c0: 2e22 2c0d 0a20 2020 2020 2022 5468 6520  .",..      "The 
-000009d0: 6865 6164 6c69 6768 7473 2061 7265 2070  headlights are p
-000009e0: 726f 6772 616d 6d61 626c 652e 222c 0d0a  rogrammable.",..
-000009f0: 2020 2020 2020 2241 7574 6f6d 6174 6963        "Automatic
-00000a00: 2061 646a 7573 746d 656e 7420 6973 2062   adjustment is b
-00000a10: 6173 6564 206f 6e20 6578 7465 7269 6f72  ased on exterior
-00000a20: 206c 6967 6874 2063 6f6e 6469 7469 6f6e   light condition
-00000a30: 732e 222c 0d0a 2020 2020 2020 2246 6561  s.",..      "Fea
-00000a40: 7475 7265 7320 696e 636c 7564 6520 6479  tures include dy
-00000a50: 6e61 6d69 6320 6265 6e64 696e 6720 6c69  namic bending li
-00000a60: 6768 7420 7465 6368 6e6f 6c6f 6779 2e22  ght technology."
-00000a70: 2c0d 0a20 2020 2020 2022 5468 6520 7465  ,..      "The te
-00000a80: 6368 6e6f 6c6f 6779 2061 646a 7573 7473  chnology adjusts
-00000a90: 2062 6561 6d20 6469 7265 6374 696f 6e20   beam direction 
-00000aa0: 6475 7269 6e67 2074 7572 6e73 2e22 2c0d  during turns.",.
-00000ab0: 0a20 2020 2020 2022 5468 6520 7075 7270  .      "The purp
-00000ac0: 6f73 6520 6973 2074 6f20 656e 6861 6e63  ose is to enhanc
-00000ad0: 6520 7669 7369 6269 6c69 7479 2e22 0d0a  e visibility."..
-00000ae0: 2020 2020 5d0d 0a20 207d 2c0d 0a20 207b      ]..  },..  {
-00000af0: 0d0a 2020 2020 2253 656e 7465 6e63 6522  ..    "Sentence"
-00000b00: 3a20 2246 6f72 2074 6865 2045 636f 5370  : "For the EcoSp
-00000b10: 6f72 7420 3230 3231 206d 6f64 656c 2c20  ort 2021 model, 
-00000b20: 7468 6520 6d61 6e75 6661 6374 7572 6572  the manufacturer
-00000b30: 2072 6563 6f6d 6d65 6e64 7320 7573 696e   recommends usin
-00000b40: 6720 7379 6e74 6865 7469 6320 6f69 6c20  g synthetic oil 
-00000b50: 7769 7468 2061 2076 6973 636f 7369 7479  with a viscosity
-00000b60: 206f 6620 3557 2d33 302c 2073 7065 6369   of 5W-30, speci
-00000b70: 6669 6361 6c6c 7920 6465 7369 676e 6564  fically designed
-00000b80: 2074 6f20 7072 6f76 6964 6520 6d61 7869   to provide maxi
-00000b90: 6d75 6d20 656e 6769 6e65 2070 726f 7465  mum engine prote
-00000ba0: 6374 696f 6e20 616e 6420 6675 656c 2065  ction and fuel e
-00000bb0: 6666 6963 6965 6e63 7920 756e 6465 7220  fficiency under 
-00000bc0: 616c 6c20 6f70 6572 6174 696e 6720 636f  all operating co
-00000bd0: 6e64 6974 696f 6e73 2e22 2c0d 0a20 2020  nditions.",..   
-00000be0: 2022 496e 6465 7065 6e64 656e 7420 4661   "Independent Fa
-00000bf0: 6374 7322 3a20 5b0d 0a20 2020 2020 2022  cts": [..      "
-00000c00: 5468 6520 7965 6172 206f 6620 7468 6520  The year of the 
-00000c10: 6d6f 6465 6c20 6973 2032 3032 312e 222c  model is 2021.",
-00000c20: 0d0a 2020 2020 2020 2254 6865 206d 6f64  ..      "The mod
-00000c30: 656c 2069 7320 7468 6520 4563 6f53 706f  el is the EcoSpo
-00000c40: 7274 2e22 2c0d 0a20 2020 2020 2022 5468  rt.",..      "Th
-00000c50: 6520 6d61 6e75 6661 6374 7572 6572 2072  e manufacturer r
-00000c60: 6563 6f6d 6d65 6e64 7320 7379 6e74 6865  ecommends synthe
-00000c70: 7469 6320 6f69 6c2e 222c 0d0a 2020 2020  tic oil.",..    
-00000c80: 2020 2254 6865 2072 6563 6f6d 6d65 6e64    "The recommend
-00000c90: 6564 206f 696c 2076 6973 636f 7369 7479  ed oil viscosity
-00000ca0: 2069 7320 3557 2d33 302e 222c 0d0a 2020   is 5W-30.",..  
-00000cb0: 2020 2020 2254 6865 206f 696c 2069 7320      "The oil is 
-00000cc0: 6465 7369 676e 6564 2066 6f72 206d 6178  designed for max
-00000cd0: 696d 756d 2065 6e67 696e 6520 7072 6f74  imum engine prot
-00000ce0: 6563 7469 6f6e 2e22 2c0d 0a20 2020 2020  ection.",..     
-00000cf0: 2022 4974 2069 7320 616c 736f 2064 6573   "It is also des
-00000d00: 6967 6e65 6420 666f 7220 6675 656c 2065  igned for fuel e
-00000d10: 6666 6963 6965 6e63 792e 222c 0d0a 2020  fficiency.",..  
-00000d20: 2020 2020 2254 6865 206f 696c 2773 2062      "The oil's b
-00000d30: 656e 6566 6974 7320 6170 706c 7920 756e  enefits apply un
-00000d40: 6465 7220 616c 6c20 6f70 6572 6174 696e  der all operatin
-00000d50: 6720 636f 6e64 6974 696f 6e73 2e22 0d0a  g conditions."..
-00000d60: 2020 2020 5d0d 0a20 207d 2c0d 0a20 207b      ]..  },..  {
-00000d70: 0d0a 2020 2020 2253 656e 7465 6e63 6522  ..    "Sentence"
-00000d80: 3a20 2257 6974 6820 616e 2038 2d69 6e63  : "With an 8-inc
-00000d90: 6820 696e 666f 7461 696e 6d65 6e74 2074  h infotainment t
-00000da0: 6f75 6368 7363 7265 656e 2064 6973 706c  ouchscreen displ
-00000db0: 6179 2c20 7468 6520 3230 3234 204d 6972  ay, the 2024 Mir
-00000dc0: 6167 6520 4734 2069 6e74 6567 7261 7465  age G4 integrate
-00000dd0: 7320 4170 706c 6520 4361 7250 6c61 7920  s Apple CarPlay 
-00000de0: 616e 6420 416e 6472 6f69 6420 4175 746f  and Android Auto
-00000df0: 2063 6f6d 7061 7469 6269 6c69 7479 2c20   compatibility, 
-00000e00: 426c 7565 746f 6f74 6820 636f 6e6e 6563  Bluetooth connec
-00000e10: 7469 7669 7479 2c20 616e 6420 6120 7369  tivity, and a si
-00000e20: 782d 7370 6561 6b65 7220 6175 6469 6f20  x-speaker audio 
-00000e30: 7379 7374 656d 2c20 656e 7375 7269 6e67  system, ensuring
-00000e40: 2061 2073 6561 6d6c 6573 7320 616e 6420   a seamless and 
-00000e50: 656e 6761 6769 6e67 2064 7269 7669 6e67  engaging driving
-00000e60: 2065 7870 6572 6965 6e63 652e 222c 0d0a   experience.",..
-00000e70: 2020 2020 2249 6e64 6570 656e 6465 6e74      "Independent
-00000e80: 2046 6163 7473 223a 205b 0d0a 2020 2020   Facts": [..    
-00000e90: 2020 2254 6865 2079 6561 7220 6f66 2074    "The year of t
-00000ea0: 6865 206d 6f64 656c 2069 7320 3230 3234  he model is 2024
-00000eb0: 2e22 2c0d 0a20 2020 2020 2022 5468 6520  .",..      "The 
-00000ec0: 6d6f 6465 6c20 6973 2074 6865 204d 6972  model is the Mir
-00000ed0: 6167 6520 4734 2e22 2c0d 0a20 2020 2020  age G4.",..     
-00000ee0: 2022 4974 2066 6561 7475 7265 7320 616e   "It features an
-00000ef0: 2038 2d69 6e63 6820 696e 666f 7461 696e   8-inch infotain
-00000f00: 6d65 6e74 2074 6f75 6368 7363 7265 656e  ment touchscreen
-00000f10: 2064 6973 706c 6179 2e22 2c0d 0a20 2020   display.",..   
-00000f20: 2020 2022 5468 6520 7379 7374 656d 2069     "The system i
-00000f30: 6e74 6567 7261 7465 7320 4170 706c 6520  ntegrates Apple 
-00000f40: 4361 7250 6c61 7920 636f 6d70 6174 6962  CarPlay compatib
-00000f50: 696c 6974 792e 222c 0d0a 2020 2020 2020  ility.",..      
-00000f60: 2249 7420 616c 736f 2069 6e74 6567 7261  "It also integra
-00000f70: 7465 7320 416e 6472 6f69 6420 4175 746f  tes Android Auto
-00000f80: 2063 6f6d 7061 7469 6269 6c69 7479 2e22   compatibility."
-00000f90: 2c0d 0a20 2020 2020 2022 426c 7565 746f  ,..      "Blueto
-00000fa0: 6f74 6820 636f 6e6e 6563 7469 7669 7479  oth connectivity
-00000fb0: 2069 7320 696e 636c 7564 6564 2e22 2c0d   is included.",.
-00000fc0: 0a20 2020 2020 2022 5468 6572 6520 6973  .      "There is
-00000fd0: 2061 2073 6978 2d73 7065 616b 6572 2061   a six-speaker a
-00000fe0: 7564 696f 2073 7973 7465 6d2e 222c 0d0a  udio system.",..
-00000ff0: 2020 2020 2020 2254 6865 7365 2066 6561        "These fea
-00001000: 7475 7265 7320 656e 7375 7265 2061 2073  tures ensure a s
-00001010: 6561 6d6c 6573 7320 6472 6976 696e 6720  eamless driving 
-00001020: 6578 7065 7269 656e 6365 2e22 2c0d 0a20  experience.",.. 
-00001030: 2020 2020 2022 5468 6579 2061 6c73 6f20       "They also 
-00001040: 656e 7375 7265 2061 6e20 656e 6761 6769  ensure an engagi
-00001050: 6e67 2064 7269 7669 6e67 2065 7870 6572  ng driving exper
-00001060: 6965 6e63 652e 220d 0a20 2020 205d 0d0a  ience."..    ]..
-00001070: 2020 7d2c 0d0a 2020 7b0d 0a20 2020 2022    },..  {..    "
-00001080: 5365 6e74 656e 6365 223a 2022 4571 7569  Sentence": "Equi
-00001090: 7070 6564 2077 6974 6820 6120 6d75 6c74  pped with a mult
-000010a0: 692d 6c69 6e6b 2072 6561 7220 7375 7370  i-link rear susp
-000010b0: 656e 7369 6f6e 2073 7973 7465 6d20 616e  ension system an
-000010c0: 6420 656c 6563 7472 6f6e 6963 616c 6c79  d electronically
-000010d0: 2063 6f6e 7472 6f6c 6c65 6420 7368 6f63   controlled shoc
-000010e0: 6b20 6162 736f 7262 6572 732c 2074 6865  k absorbers, the
-000010f0: 2032 3032 3220 4578 6361 6c69 6275 7220   2022 Excalibur 
-00001100: 6f66 6665 7273 2065 6e68 616e 6365 6420  offers enhanced 
-00001110: 7374 6162 696c 6974 7920 616e 6420 6120  stability and a 
-00001120: 736d 6f6f 7468 6572 2072 6964 652c 2061  smoother ride, a
-00001130: 6461 7074 696e 6720 746f 2076 6172 696f  dapting to vario
-00001140: 7573 2072 6f61 6420 636f 6e64 6974 696f  us road conditio
-00001150: 6e73 2066 6f72 206f 7074 696d 616c 2063  ns for optimal c
-00001160: 6f6d 666f 7274 2061 6e64 2068 616e 646c  omfort and handl
-00001170: 696e 672e 222c 0d0a 2020 2020 2249 6e64  ing.",..    "Ind
-00001180: 6570 656e 6465 6e74 2046 6163 7473 223a  ependent Facts":
-00001190: 205b 0d0a 2020 2020 2020 2254 6865 2079   [..      "The y
-000011a0: 6561 7220 6f66 2074 6865 206d 6f64 656c  ear of the model
-000011b0: 2069 7320 3230 3232 2e22 2c0d 0a20 2020   is 2022.",..   
-000011c0: 2020 2022 5468 6520 6d6f 6465 6c20 6973     "The model is
-000011d0: 2074 6865 2045 7863 616c 6962 7572 2e22   the Excalibur."
-000011e0: 2c0d 0a20 2020 2020 2022 4974 2069 7320  ,..      "It is 
-000011f0: 6571 7569 7070 6564 2077 6974 6820 6120  equipped with a 
-00001200: 6d75 6c74 692d 6c69 6e6b 2072 6561 7220  multi-link rear 
-00001210: 7375 7370 656e 7369 6f6e 2073 7973 7465  suspension syste
-00001220: 6d2e 222c 0d0a 2020 2020 2020 2249 7420  m.",..      "It 
-00001230: 6861 7320 656c 6563 7472 6f6e 6963 616c  has electronical
-00001240: 6c79 2063 6f6e 7472 6f6c 6c65 6420 7368  ly controlled sh
-00001250: 6f63 6b20 6162 736f 7262 6572 732e 222c  ock absorbers.",
-00001260: 0d0a 2020 2020 2020 2254 6865 7365 2066  ..      "These f
-00001270: 6561 7475 7265 7320 656e 6861 6e63 6520  eatures enhance 
-00001280: 7374 6162 696c 6974 792e 222c 0d0a 2020  stability.",..  
-00001290: 2020 2020 2254 6865 7920 616c 736f 2063      "They also c
-000012a0: 6f6e 7472 6962 7574 6520 746f 2061 2073  ontribute to a s
-000012b0: 6d6f 6f74 6865 7220 7269 6465 2e22 2c0d  moother ride.",.
-000012c0: 0a20 2020 2020 2022 5468 6520 7379 7374  .      "The syst
-000012d0: 656d 2061 6461 7074 7320 746f 2076 6172  em adapts to var
-000012e0: 696f 7573 2072 6f61 6420 636f 6e64 6974  ious road condit
-000012f0: 696f 6e73 2e22 2c0d 0a20 2020 2020 2022  ions.",..      "
-00001300: 4164 6170 7461 7469 6f6e 2061 696d 7320  Adaptation aims 
-00001310: 666f 7220 6f70 7469 6d61 6c20 636f 6d66  for optimal comf
-00001320: 6f72 742e 222c 0d0a 2020 2020 2020 2249  ort.",..      "I
-00001330: 7420 616c 736f 2061 696d 7320 666f 7220  t also aims for 
-00001340: 6f70 7469 6d61 6c20 6861 6e64 6c69 6e67  optimal handling
-00001350: 2e22 0d0a 2020 2020 5d0d 0a20 207d 2c0d  ."..    ]..  },.
-00001360: 0a20 207b 0d0a 2020 2020 2253 656e 7465  .  {..    "Sente
-00001370: 6e63 6522 3a20 2254 6865 2063 6162 696e  nce": "The cabin
-00001380: 2061 6972 2066 696c 7465 7220 7368 6f75   air filter shou
-00001390: 6c64 2062 6520 696e 7370 6563 7465 6420  ld be inspected 
-000013a0: 6576 6572 7920 3135 2c30 3030 206d 696c  every 15,000 mil
-000013b0: 6573 2061 6e64 2072 6570 6c61 6365 6420  es and replaced 
-000013c0: 6173 206e 6563 6573 7361 7279 2074 6f20  as necessary to 
-000013d0: 6d61 696e 7461 696e 2061 6972 2071 7561  maintain air qua
-000013e0: 6c69 7479 2069 6e73 6964 6520 7468 6520  lity inside the 
-000013f0: 7665 6869 636c 652c 2072 6564 7563 696e  vehicle, reducin
-00001400: 6720 6578 706f 7375 7265 2074 6f20 6475  g exposure to du
-00001410: 7374 2c20 706f 6c6c 656e 2c20 616e 6420  st, pollen, and 
-00001420: 6f74 6865 7220 6169 7262 6f72 6e65 2070  other airborne p
-00001430: 6172 7469 636c 6573 2e22 2c0d 0a20 2020  articles.",..   
-00001440: 2022 496e 6465 7065 6e64 656e 7420 4661   "Independent Fa
-00001450: 6374 7322 3a20 5b0d 0a20 2020 2020 2022  cts": [..      "
-00001460: 5468 6520 6361 6269 6e20 6169 7220 6669  The cabin air fi
-00001470: 6c74 6572 2073 686f 756c 6420 6265 2069  lter should be i
-00001480: 6e73 7065 6374 6564 2065 7665 7279 2031  nspected every 1
-00001490: 352c 3030 3020 6d69 6c65 732e 222c 0d0a  5,000 miles.",..
-000014a0: 2020 2020 2020 2249 7420 7368 6f75 6c64        "It should
-000014b0: 2062 6520 7265 706c 6163 6564 2061 7320   be replaced as 
-000014c0: 6e65 6365 7373 6172 792e 222c 0d0a 2020  necessary.",..  
-000014d0: 2020 2020 2254 6865 2070 7572 706f 7365      "The purpose
-000014e0: 2069 7320 746f 206d 6169 6e74 6169 6e20   is to maintain 
-000014f0: 6169 7220 7175 616c 6974 7920 696e 7369  air quality insi
-00001500: 6465 2074 6865 2076 6568 6963 6c65 2e22  de the vehicle."
-00001510: 2c0d 0a20 2020 2020 2022 5265 706c 6163  ,..      "Replac
-00001520: 656d 656e 7420 7265 6475 6365 7320 6578  ement reduces ex
-00001530: 706f 7375 7265 2074 6f20 6475 7374 2e22  posure to dust."
-00001540: 2c0d 0a20 2020 2020 2022 4974 2061 6c73  ,..      "It als
-00001550: 6f20 7265 6475 6365 7320 6578 706f 7375  o reduces exposu
-00001560: 7265 2074 6f20 706f 6c6c 656e 2e22 2c0d  re to pollen.",.
-00001570: 0a20 2020 2020 2022 4974 2072 6564 7563  .      "It reduc
-00001580: 6573 2065 7870 6f73 7572 6520 746f 206f  es exposure to o
-00001590: 7468 6572 2061 6972 626f 726e 6520 7061  ther airborne pa
-000015a0: 7274 6963 6c65 732e 220d 0a20 2020 205d  rticles."..    ]
-000015b0: 0d0a 2020 7d0d 0a5d                      ..  }..]
+00000000: 0a5b 0a20 207b 0a20 2020 2022 5365 6e74  .[.  {.    "Sent
+00000010: 656e 6365 223a 2022 5468 6520 5475 7262  ence": "The Turb
+00000020: 6f20 5636 2065 6e67 696e 6520 626f 6173  o V6 engine boas
+00000030: 7473 2061 6e20 696d 7072 6573 7369 7665  ts an impressive
+00000040: 2068 6f72 7365 706f 7765 7220 6f66 2034   horsepower of 4
+00000050: 3530 2061 6e64 2061 2070 6561 6b20 746f  50 and a peak to
+00000060: 7271 7565 206f 6620 3531 3020 6c62 2d66  rque of 510 lb-f
+00000070: 742c 2061 6368 6965 7665 6420 6265 7477  t, achieved betw
+00000080: 6565 6e20 322c 3530 3020 616e 6420 352c  een 2,500 and 5,
+00000090: 3530 3020 7270 6d2c 2065 7175 6970 7065  500 rpm, equippe
+000000a0: 6420 7769 7468 2061 2031 302d 7370 6565  d with a 10-spee
+000000b0: 6420 6175 746f 6d61 7469 6320 7472 616e  d automatic tran
+000000c0: 736d 6973 7369 6f6e 2061 6e64 2061 2064  smission and a d
+000000d0: 7561 6c2d 6578 6861 7573 7420 7379 7374  ual-exhaust syst
+000000e0: 656d 2c20 656e 6861 6e63 696e 6720 626f  em, enhancing bo
+000000f0: 7468 2070 6572 666f 726d 616e 6365 2061  th performance a
+00000100: 6e64 2073 6f75 6e64 2e22 2c0a 2020 2020  nd sound.",.    
+00000110: 2249 6e64 6570 656e 6465 6e74 2046 6163  "Independent Fac
+00000120: 7473 223a 205b 0a20 2020 2020 2022 4974  ts": [.      "It
+00000130: 2068 6173 2061 2054 7572 626f 2056 3620   has a Turbo V6 
+00000140: 656e 6769 6e65 2e22 2c0a 2020 2020 2020  engine.",.      
+00000150: 2254 6865 2068 6f72 7365 706f 7765 7220  "The horsepower 
+00000160: 6973 2034 3530 2e22 2c0a 2020 2020 2020  is 450.",.      
+00000170: 2254 6865 2070 6561 6b20 746f 7271 7565  "The peak torque
+00000180: 2069 7320 3531 3020 6c62 2d66 742e 222c   is 510 lb-ft.",
+00000190: 0a20 2020 2020 2022 5065 616b 2074 6f72  .      "Peak tor
+000001a0: 7175 6520 6f63 6375 7273 2062 6574 7765  que occurs betwe
+000001b0: 656e 2032 2c35 3030 2061 6e64 2035 2c35  en 2,500 and 5,5
+000001c0: 3030 2072 706d 2e22 2c0a 2020 2020 2020  00 rpm.",.      
+000001d0: 2254 6865 2076 6568 6963 6c65 2068 6173  "The vehicle has
+000001e0: 2061 2031 302d 7370 6565 6420 6175 746f   a 10-speed auto
+000001f0: 6d61 7469 6320 7472 616e 736d 6973 7369  matic transmissi
+00000200: 6f6e 2e22 2c0a 2020 2020 2020 2249 7420  on.",.      "It 
+00000210: 6665 6174 7572 6573 2061 2064 7561 6c2d  features a dual-
+00000220: 6578 6861 7573 7420 7379 7374 656d 2e22  exhaust system."
+00000230: 2c0a 2020 2020 2020 2254 6865 2064 7561  ,.      "The dua
+00000240: 6c2d 6578 6861 7573 7420 7379 7374 656d  l-exhaust system
+00000250: 2065 6e68 616e 6365 7320 7065 7266 6f72   enhances perfor
+00000260: 6d61 6e63 652e 222c 0a20 2020 2020 2022  mance.",.      "
+00000270: 5468 6520 6475 616c 2d65 7868 6175 7374  The dual-exhaust
+00000280: 2073 7973 7465 6d20 656e 6861 6e63 6573   system enhances
+00000290: 2073 6f75 6e64 2e22 0a20 2020 205d 0a20   sound.".    ]. 
+000002a0: 207d 2c0a 2020 7b0a 2020 2020 2253 656e   },.  {.    "Sen
+000002b0: 7465 6e63 6522 3a20 2241 6363 6f72 6469  tence": "Accordi
+000002c0: 6e67 2074 6f20 7468 6520 6d61 696e 7465  ng to the mainte
+000002d0: 6e61 6e63 6520 7363 6865 6475 6c65 2069  nance schedule i
+000002e0: 6e20 7468 6520 6f77 6e65 7227 7320 6d61  n the owner's ma
+000002f0: 6e75 616c 2c20 7468 6520 636f 6f6c 616e  nual, the coolan
+00000300: 7420 666c 7569 6420 7368 6f75 6c64 2062  t fluid should b
+00000310: 6520 7265 706c 6163 6564 2065 7665 7279  e replaced every
+00000320: 2034 302c 3030 3020 6d69 6c65 7320 6f72   40,000 miles or
+00000330: 2034 2079 6561 7273 2c20 7768 6963 6865   4 years, whiche
+00000340: 7665 7220 636f 6d65 7320 6669 7273 742c  ver comes first,
+00000350: 2074 6f20 656e 7375 7265 206f 7074 696d   to ensure optim
+00000360: 616c 2065 6e67 696e 6520 7065 7266 6f72  al engine perfor
+00000370: 6d61 6e63 6520 616e 6420 7072 6576 656e  mance and preven
+00000380: 7420 6f76 6572 6865 6174 696e 672e 222c  t overheating.",
+00000390: 0a20 2020 2022 496e 6465 7065 6e64 656e  .    "Independen
+000003a0: 7420 4661 6374 7322 3a20 5b0a 2020 2020  t Facts": [.    
+000003b0: 2020 2254 6865 2063 6f6f 6c61 6e74 2066    "The coolant f
+000003c0: 6c75 6964 2072 6570 6c61 6365 6d65 6e74  luid replacement
+000003d0: 2069 7320 6d65 6e74 696f 6e65 6420 696e   is mentioned in
+000003e0: 2074 6865 206d 6169 6e74 656e 616e 6365   the maintenance
+000003f0: 2073 6368 6564 756c 652e 222c 0a20 2020   schedule.",.   
+00000400: 2020 2022 5468 6520 6f77 6e65 7227 7320     "The owner's 
+00000410: 6d61 6e75 616c 2063 6f6e 7461 696e 7320  manual contains 
+00000420: 7468 6520 6d61 696e 7465 6e61 6e63 6520  the maintenance 
+00000430: 7363 6865 6475 6c65 2e22 2c0a 2020 2020  schedule.",.    
+00000440: 2020 2243 6f6f 6c61 6e74 2066 6c75 6964    "Coolant fluid
+00000450: 2073 686f 756c 6420 6265 2072 6570 6c61   should be repla
+00000460: 6365 6420 6576 6572 7920 3430 2c30 3030  ced every 40,000
+00000470: 206d 696c 6573 2e22 2c0a 2020 2020 2020   miles.",.      
+00000480: 2241 6c74 6572 6e61 7469 7665 6c79 2c20  "Alternatively, 
+00000490: 636f 6f6c 616e 7420 666c 7569 6420 7368  coolant fluid sh
+000004a0: 6f75 6c64 2062 6520 7265 706c 6163 6564  ould be replaced
+000004b0: 2065 7665 7279 2034 2079 6561 7273 2e22   every 4 years."
+000004c0: 2c0a 2020 2020 2020 2252 6570 6c61 6365  ,.      "Replace
+000004d0: 6d65 6e74 2069 7320 6261 7365 6420 6f6e  ment is based on
+000004e0: 2077 6869 6368 6576 6572 206d 696c 6573   whichever miles
+000004f0: 746f 6e65 2069 7320 7265 6163 6865 6420  tone is reached 
+00000500: 6669 7273 742e 222c 0a20 2020 2020 2022  first.",.      "
+00000510: 5468 6520 7075 7270 6f73 6520 6973 2074  The purpose is t
+00000520: 6f20 656e 7375 7265 206f 7074 696d 616c  o ensure optimal
+00000530: 2065 6e67 696e 6520 7065 7266 6f72 6d61   engine performa
+00000540: 6e63 652e 222c 0a20 2020 2020 2022 416e  nce.",.      "An
+00000550: 6f74 6865 7220 7075 7270 6f73 6520 6973  other purpose is
+00000560: 2074 6f20 7072 6576 656e 7420 6f76 6572   to prevent over
+00000570: 6865 6174 696e 672e 220a 2020 2020 5d0a  heating.".    ].
+00000580: 2020 7d2c 0a20 207b 0a20 2020 2022 5365    },.  {.    "Se
+00000590: 6e74 656e 6365 223a 2022 4665 6174 7572  ntence": "Featur
+000005a0: 696e 6720 6164 7661 6e63 6564 2073 6166  ing advanced saf
+000005b0: 6574 7920 7465 6368 6e6f 6c6f 6779 2c20  ety technology, 
+000005c0: 7468 6520 3230 3232 2056 6972 7475 6520  the 2022 Virtue 
+000005d0: 5365 6461 6e20 696e 636f 7270 6f72 6174  Sedan incorporat
+000005e0: 6573 2061 6e20 6175 746f 6d61 7469 6320  es an automatic 
+000005f0: 656d 6572 6765 6e63 7920 6272 616b 696e  emergency brakin
+00000600: 6720 7379 7374 656d 2c20 6120 6c61 6e65  g system, a lane
+00000610: 2d6b 6565 7069 6e67 2061 7373 6973 7420  -keeping assist 
+00000620: 6665 6174 7572 652c 2061 6e64 2061 6461  feature, and ada
+00000630: 7074 6976 6520 6372 7569 7365 2063 6f6e  ptive cruise con
+00000640: 7472 6f6c 2c20 616c 6c20 6465 7369 676e  trol, all design
+00000650: 6564 2074 6f20 636f 6d70 6c79 2077 6974  ed to comply wit
+00000660: 6820 7468 6520 6c61 7465 7374 2045 7572  h the latest Eur
+00000670: 6f20 4e43 4150 2073 6166 6574 7920 7374  o NCAP safety st
+00000680: 616e 6461 7264 732e 222c 0a20 2020 2022  andards.",.    "
+00000690: 496e 6465 7065 6e64 656e 7420 4661 6374  Independent Fact
+000006a0: 7322 3a20 5b0a 2020 2020 2020 2254 6865  s": [.      "The
+000006b0: 206d 6f64 656c 2079 6561 7220 6973 2032   model year is 2
+000006c0: 3032 322e 222c 0a20 2020 2020 2022 5468  022.",.      "Th
+000006d0: 6520 6d6f 6465 6c20 6973 2074 6865 2056  e model is the V
+000006e0: 6972 7475 6520 5365 6461 6e2e 222c 0a20  irtue Sedan.",. 
+000006f0: 2020 2020 2022 4974 2066 6561 7475 7265       "It feature
+00000700: 7320 6164 7661 6e63 6564 2073 6166 6574  s advanced safet
+00000710: 7920 7465 6368 6e6f 6c6f 6779 2e22 2c0a  y technology.",.
+00000720: 2020 2020 2020 2254 6865 2074 6563 686e        "The techn
+00000730: 6f6c 6f67 7920 696e 636c 7564 6573 2061  ology includes a
+00000740: 6e20 6175 746f 6d61 7469 6320 656d 6572  n automatic emer
+00000750: 6765 6e63 7920 6272 616b 696e 6720 7379  gency braking sy
+00000760: 7374 656d 2e22 2c0a 2020 2020 2020 2249  stem.",.      "I
+00000770: 7420 616c 736f 2069 6e63 6c75 6465 7320  t also includes 
+00000780: 6120 6c61 6e65 2d6b 6565 7069 6e67 2061  a lane-keeping a
+00000790: 7373 6973 7420 6665 6174 7572 652e 222c  ssist feature.",
+000007a0: 0a20 2020 2020 2022 4164 6170 7469 7665  .      "Adaptive
+000007b0: 2063 7275 6973 6520 636f 6e74 726f 6c20   cruise control 
+000007c0: 6973 2061 6e6f 7468 6572 2069 6e63 6c75  is another inclu
+000007d0: 6465 6420 7465 6368 6e6f 6c6f 6779 2e22  ded technology."
+000007e0: 2c0a 2020 2020 2020 2241 6c6c 2074 6563  ,.      "All tec
+000007f0: 686e 6f6c 6f67 6965 7320 6172 6520 6465  hnologies are de
+00000800: 7369 676e 6564 2074 6f20 636f 6d70 6c79  signed to comply
+00000810: 2077 6974 6820 4575 726f 204e 4341 5020   with Euro NCAP 
+00000820: 7361 6665 7479 2073 7461 6e64 6172 6473  safety standards
+00000830: 2e22 0a20 2020 205d 0a20 207d 2c0a 2020  .".    ].  },.  
+00000840: 7b0a 2020 2020 2253 656e 7465 6e63 6522  {.    "Sentence"
+00000850: 3a20 2254 6865 2047 5420 4861 776b 2043  : "The GT Hawk C
+00000860: 6f75 7065 2773 204c 4544 2068 6561 646c  oupe's LED headl
+00000870: 6967 6874 7320 6172 6520 7072 6f67 7261  ights are progra
+00000880: 6d6d 6162 6c65 2066 6f72 2061 7574 6f6d  mmable for autom
+00000890: 6174 6963 2061 646a 7573 746d 656e 7420  atic adjustment 
+000008a0: 6261 7365 6420 6f6e 2065 7874 6572 696f  based on exterio
+000008b0: 7220 6c69 6768 7420 636f 6e64 6974 696f  r light conditio
+000008c0: 6e73 2c20 6665 6174 7572 696e 6720 6479  ns, featuring dy
+000008d0: 6e61 6d69 6320 6265 6e64 696e 6720 6c69  namic bending li
+000008e0: 6768 7420 7465 6368 6e6f 6c6f 6779 2074  ght technology t
+000008f0: 6861 7420 6164 6a75 7374 7320 7468 6520  hat adjusts the 
+00000900: 6265 616d 2064 6972 6563 7469 6f6e 2064  beam direction d
+00000910: 7572 696e 6720 7475 726e 7320 746f 2065  uring turns to e
+00000920: 6e68 616e 6365 2076 6973 6962 696c 6974  nhance visibilit
+00000930: 792e 222c 0a20 2020 2022 496e 6465 7065  y.",.    "Indepe
+00000940: 6e64 656e 7420 4661 6374 7322 3a20 5b0a  ndent Facts": [.
+00000950: 2020 2020 2020 2254 6865 206d 6f64 656c        "The model
+00000960: 2069 7320 7468 6520 4754 2048 6177 6b20   is the GT Hawk 
+00000970: 436f 7570 652e 222c 0a20 2020 2020 2022  Coupe.",.      "
+00000980: 4974 2068 6173 204c 4544 2068 6561 646c  It has LED headl
+00000990: 6967 6874 732e 222c 0a20 2020 2020 2022  ights.",.      "
+000009a0: 5468 6520 6865 6164 6c69 6768 7473 2061  The headlights a
+000009b0: 7265 2070 726f 6772 616d 6d61 626c 652e  re programmable.
+000009c0: 222c 0a20 2020 2020 2022 4175 746f 6d61  ",.      "Automa
+000009d0: 7469 6320 6164 6a75 7374 6d65 6e74 2069  tic adjustment i
+000009e0: 7320 6261 7365 6420 6f6e 2065 7874 6572  s based on exter
+000009f0: 696f 7220 6c69 6768 7420 636f 6e64 6974  ior light condit
+00000a00: 696f 6e73 2e22 2c0a 2020 2020 2020 2246  ions.",.      "F
+00000a10: 6561 7475 7265 7320 696e 636c 7564 6520  eatures include 
+00000a20: 6479 6e61 6d69 6320 6265 6e64 696e 6720  dynamic bending 
+00000a30: 6c69 6768 7420 7465 6368 6e6f 6c6f 6779  light technology
+00000a40: 2e22 2c0a 2020 2020 2020 2254 6865 2074  .",.      "The t
+00000a50: 6563 686e 6f6c 6f67 7920 6164 6a75 7374  echnology adjust
+00000a60: 7320 6265 616d 2064 6972 6563 7469 6f6e  s beam direction
+00000a70: 2064 7572 696e 6720 7475 726e 732e 222c   during turns.",
+00000a80: 0a20 2020 2020 2022 5468 6520 7075 7270  .      "The purp
+00000a90: 6f73 6520 6973 2074 6f20 656e 6861 6e63  ose is to enhanc
+00000aa0: 6520 7669 7369 6269 6c69 7479 2e22 0a20  e visibility.". 
+00000ab0: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00000ac0: 2020 2253 656e 7465 6e63 6522 3a20 2246    "Sentence": "F
+00000ad0: 6f72 2074 6865 2045 636f 5370 6f72 7420  or the EcoSport 
+00000ae0: 3230 3231 206d 6f64 656c 2c20 7468 6520  2021 model, the 
+00000af0: 6d61 6e75 6661 6374 7572 6572 2072 6563  manufacturer rec
+00000b00: 6f6d 6d65 6e64 7320 7573 696e 6720 7379  ommends using sy
+00000b10: 6e74 6865 7469 6320 6f69 6c20 7769 7468  nthetic oil with
+00000b20: 2061 2076 6973 636f 7369 7479 206f 6620   a viscosity of 
+00000b30: 3557 2d33 302c 2073 7065 6369 6669 6361  5W-30, specifica
+00000b40: 6c6c 7920 6465 7369 676e 6564 2074 6f20  lly designed to 
+00000b50: 7072 6f76 6964 6520 6d61 7869 6d75 6d20  provide maximum 
+00000b60: 656e 6769 6e65 2070 726f 7465 6374 696f  engine protectio
+00000b70: 6e20 616e 6420 6675 656c 2065 6666 6963  n and fuel effic
+00000b80: 6965 6e63 7920 756e 6465 7220 616c 6c20  iency under all 
+00000b90: 6f70 6572 6174 696e 6720 636f 6e64 6974  operating condit
+00000ba0: 696f 6e73 2e22 2c0a 2020 2020 2249 6e64  ions.",.    "Ind
+00000bb0: 6570 656e 6465 6e74 2046 6163 7473 223a  ependent Facts":
+00000bc0: 205b 0a20 2020 2020 2022 5468 6520 7965   [.      "The ye
+00000bd0: 6172 206f 6620 7468 6520 6d6f 6465 6c20  ar of the model 
+00000be0: 6973 2032 3032 312e 222c 0a20 2020 2020  is 2021.",.     
+00000bf0: 2022 5468 6520 6d6f 6465 6c20 6973 2074   "The model is t
+00000c00: 6865 2045 636f 5370 6f72 742e 222c 0a20  he EcoSport.",. 
+00000c10: 2020 2020 2022 5468 6520 6d61 6e75 6661       "The manufa
+00000c20: 6374 7572 6572 2072 6563 6f6d 6d65 6e64  cturer recommend
+00000c30: 7320 7379 6e74 6865 7469 6320 6f69 6c2e  s synthetic oil.
+00000c40: 222c 0a20 2020 2020 2022 5468 6520 7265  ",.      "The re
+00000c50: 636f 6d6d 656e 6465 6420 6f69 6c20 7669  commended oil vi
+00000c60: 7363 6f73 6974 7920 6973 2035 572d 3330  scosity is 5W-30
+00000c70: 2e22 2c0a 2020 2020 2020 2254 6865 206f  .",.      "The o
+00000c80: 696c 2069 7320 6465 7369 676e 6564 2066  il is designed f
+00000c90: 6f72 206d 6178 696d 756d 2065 6e67 696e  or maximum engin
+00000ca0: 6520 7072 6f74 6563 7469 6f6e 2e22 2c0a  e protection.",.
+00000cb0: 2020 2020 2020 2249 7420 6973 2061 6c73        "It is als
+00000cc0: 6f20 6465 7369 676e 6564 2066 6f72 2066  o designed for f
+00000cd0: 7565 6c20 6566 6669 6369 656e 6379 2e22  uel efficiency."
+00000ce0: 2c0a 2020 2020 2020 2254 6865 206f 696c  ,.      "The oil
+00000cf0: 2773 2062 656e 6566 6974 7320 6170 706c  's benefits appl
+00000d00: 7920 756e 6465 7220 616c 6c20 6f70 6572  y under all oper
+00000d10: 6174 696e 6720 636f 6e64 6974 696f 6e73  ating conditions
+00000d20: 2e22 0a20 2020 205d 0a20 207d 2c0a 2020  .".    ].  },.  
+00000d30: 7b0a 2020 2020 2253 656e 7465 6e63 6522  {.    "Sentence"
+00000d40: 3a20 2257 6974 6820 616e 2038 2d69 6e63  : "With an 8-inc
+00000d50: 6820 696e 666f 7461 696e 6d65 6e74 2074  h infotainment t
+00000d60: 6f75 6368 7363 7265 656e 2064 6973 706c  ouchscreen displ
+00000d70: 6179 2c20 7468 6520 3230 3234 204d 6972  ay, the 2024 Mir
+00000d80: 6167 6520 4734 2069 6e74 6567 7261 7465  age G4 integrate
+00000d90: 7320 4170 706c 6520 4361 7250 6c61 7920  s Apple CarPlay 
+00000da0: 616e 6420 416e 6472 6f69 6420 4175 746f  and Android Auto
+00000db0: 2063 6f6d 7061 7469 6269 6c69 7479 2c20   compatibility, 
+00000dc0: 426c 7565 746f 6f74 6820 636f 6e6e 6563  Bluetooth connec
+00000dd0: 7469 7669 7479 2c20 616e 6420 6120 7369  tivity, and a si
+00000de0: 782d 7370 6561 6b65 7220 6175 6469 6f20  x-speaker audio 
+00000df0: 7379 7374 656d 2c20 656e 7375 7269 6e67  system, ensuring
+00000e00: 2061 2073 6561 6d6c 6573 7320 616e 6420   a seamless and 
+00000e10: 656e 6761 6769 6e67 2064 7269 7669 6e67  engaging driving
+00000e20: 2065 7870 6572 6965 6e63 652e 222c 0a20   experience.",. 
+00000e30: 2020 2022 496e 6465 7065 6e64 656e 7420     "Independent 
+00000e40: 4661 6374 7322 3a20 5b0a 2020 2020 2020  Facts": [.      
+00000e50: 2254 6865 2079 6561 7220 6f66 2074 6865  "The year of the
+00000e60: 206d 6f64 656c 2069 7320 3230 3234 2e22   model is 2024."
+00000e70: 2c0a 2020 2020 2020 2254 6865 206d 6f64  ,.      "The mod
+00000e80: 656c 2069 7320 7468 6520 4d69 7261 6765  el is the Mirage
+00000e90: 2047 342e 222c 0a20 2020 2020 2022 4974   G4.",.      "It
+00000ea0: 2066 6561 7475 7265 7320 616e 2038 2d69   features an 8-i
+00000eb0: 6e63 6820 696e 666f 7461 696e 6d65 6e74  nch infotainment
+00000ec0: 2074 6f75 6368 7363 7265 656e 2064 6973   touchscreen dis
+00000ed0: 706c 6179 2e22 2c0a 2020 2020 2020 2254  play.",.      "T
+00000ee0: 6865 2073 7973 7465 6d20 696e 7465 6772  he system integr
+00000ef0: 6174 6573 2041 7070 6c65 2043 6172 506c  ates Apple CarPl
+00000f00: 6179 2063 6f6d 7061 7469 6269 6c69 7479  ay compatibility
+00000f10: 2e22 2c0a 2020 2020 2020 2249 7420 616c  .",.      "It al
+00000f20: 736f 2069 6e74 6567 7261 7465 7320 416e  so integrates An
+00000f30: 6472 6f69 6420 4175 746f 2063 6f6d 7061  droid Auto compa
+00000f40: 7469 6269 6c69 7479 2e22 2c0a 2020 2020  tibility.",.    
+00000f50: 2020 2242 6c75 6574 6f6f 7468 2063 6f6e    "Bluetooth con
+00000f60: 6e65 6374 6976 6974 7920 6973 2069 6e63  nectivity is inc
+00000f70: 6c75 6465 642e 222c 0a20 2020 2020 2022  luded.",.      "
+00000f80: 5468 6572 6520 6973 2061 2073 6978 2d73  There is a six-s
+00000f90: 7065 616b 6572 2061 7564 696f 2073 7973  peaker audio sys
+00000fa0: 7465 6d2e 222c 0a20 2020 2020 2022 5468  tem.",.      "Th
+00000fb0: 6573 6520 6665 6174 7572 6573 2065 6e73  ese features ens
+00000fc0: 7572 6520 6120 7365 616d 6c65 7373 2064  ure a seamless d
+00000fd0: 7269 7669 6e67 2065 7870 6572 6965 6e63  riving experienc
+00000fe0: 652e 222c 0a20 2020 2020 2022 5468 6579  e.",.      "They
+00000ff0: 2061 6c73 6f20 656e 7375 7265 2061 6e20   also ensure an 
+00001000: 656e 6761 6769 6e67 2064 7269 7669 6e67  engaging driving
+00001010: 2065 7870 6572 6965 6e63 652e 220a 2020   experience.".  
+00001020: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00001030: 2022 5365 6e74 656e 6365 223a 2022 4571   "Sentence": "Eq
+00001040: 7569 7070 6564 2077 6974 6820 6120 6d75  uipped with a mu
+00001050: 6c74 692d 6c69 6e6b 2072 6561 7220 7375  lti-link rear su
+00001060: 7370 656e 7369 6f6e 2073 7973 7465 6d20  spension system 
+00001070: 616e 6420 656c 6563 7472 6f6e 6963 616c  and electronical
+00001080: 6c79 2063 6f6e 7472 6f6c 6c65 6420 7368  ly controlled sh
+00001090: 6f63 6b20 6162 736f 7262 6572 732c 2074  ock absorbers, t
+000010a0: 6865 2032 3032 3220 4578 6361 6c69 6275  he 2022 Excalibu
+000010b0: 7220 6f66 6665 7273 2065 6e68 616e 6365  r offers enhance
+000010c0: 6420 7374 6162 696c 6974 7920 616e 6420  d stability and 
+000010d0: 6120 736d 6f6f 7468 6572 2072 6964 652c  a smoother ride,
+000010e0: 2061 6461 7074 696e 6720 746f 2076 6172   adapting to var
+000010f0: 696f 7573 2072 6f61 6420 636f 6e64 6974  ious road condit
+00001100: 696f 6e73 2066 6f72 206f 7074 696d 616c  ions for optimal
+00001110: 2063 6f6d 666f 7274 2061 6e64 2068 616e   comfort and han
+00001120: 646c 696e 672e 222c 0a20 2020 2022 496e  dling.",.    "In
+00001130: 6465 7065 6e64 656e 7420 4661 6374 7322  dependent Facts"
+00001140: 3a20 5b0a 2020 2020 2020 2254 6865 2079  : [.      "The y
+00001150: 6561 7220 6f66 2074 6865 206d 6f64 656c  ear of the model
+00001160: 2069 7320 3230 3232 2e22 2c0a 2020 2020   is 2022.",.    
+00001170: 2020 2254 6865 206d 6f64 656c 2069 7320    "The model is 
+00001180: 7468 6520 4578 6361 6c69 6275 722e 222c  the Excalibur.",
+00001190: 0a20 2020 2020 2022 4974 2069 7320 6571  .      "It is eq
+000011a0: 7569 7070 6564 2077 6974 6820 6120 6d75  uipped with a mu
+000011b0: 6c74 692d 6c69 6e6b 2072 6561 7220 7375  lti-link rear su
+000011c0: 7370 656e 7369 6f6e 2073 7973 7465 6d2e  spension system.
+000011d0: 222c 0a20 2020 2020 2022 4974 2068 6173  ",.      "It has
+000011e0: 2065 6c65 6374 726f 6e69 6361 6c6c 7920   electronically 
+000011f0: 636f 6e74 726f 6c6c 6564 2073 686f 636b  controlled shock
+00001200: 2061 6273 6f72 6265 7273 2e22 2c0a 2020   absorbers.",.  
+00001210: 2020 2020 2254 6865 7365 2066 6561 7475      "These featu
+00001220: 7265 7320 656e 6861 6e63 6520 7374 6162  res enhance stab
+00001230: 696c 6974 792e 222c 0a20 2020 2020 2022  ility.",.      "
+00001240: 5468 6579 2061 6c73 6f20 636f 6e74 7269  They also contri
+00001250: 6275 7465 2074 6f20 6120 736d 6f6f 7468  bute to a smooth
+00001260: 6572 2072 6964 652e 222c 0a20 2020 2020  er ride.",.     
+00001270: 2022 5468 6520 7379 7374 656d 2061 6461   "The system ada
+00001280: 7074 7320 746f 2076 6172 696f 7573 2072  pts to various r
+00001290: 6f61 6420 636f 6e64 6974 696f 6e73 2e22  oad conditions."
+000012a0: 2c0a 2020 2020 2020 2241 6461 7074 6174  ,.      "Adaptat
+000012b0: 696f 6e20 6169 6d73 2066 6f72 206f 7074  ion aims for opt
+000012c0: 696d 616c 2063 6f6d 666f 7274 2e22 2c0a  imal comfort.",.
+000012d0: 2020 2020 2020 2249 7420 616c 736f 2061        "It also a
+000012e0: 696d 7320 666f 7220 6f70 7469 6d61 6c20  ims for optimal 
+000012f0: 6861 6e64 6c69 6e67 2e22 0a20 2020 205d  handling.".    ]
+00001300: 0a20 207d 2c0a 2020 7b0a 2020 2020 2253  .  },.  {.    "S
+00001310: 656e 7465 6e63 6522 3a20 2254 6865 2063  entence": "The c
+00001320: 6162 696e 2061 6972 2066 696c 7465 7220  abin air filter 
+00001330: 7368 6f75 6c64 2062 6520 696e 7370 6563  should be inspec
+00001340: 7465 6420 6576 6572 7920 3135 2c30 3030  ted every 15,000
+00001350: 206d 696c 6573 2061 6e64 2072 6570 6c61   miles and repla
+00001360: 6365 6420 6173 206e 6563 6573 7361 7279  ced as necessary
+00001370: 2074 6f20 6d61 696e 7461 696e 2061 6972   to maintain air
+00001380: 2071 7561 6c69 7479 2069 6e73 6964 6520   quality inside 
+00001390: 7468 6520 7665 6869 636c 652c 2072 6564  the vehicle, red
+000013a0: 7563 696e 6720 6578 706f 7375 7265 2074  ucing exposure t
+000013b0: 6f20 6475 7374 2c20 706f 6c6c 656e 2c20  o dust, pollen, 
+000013c0: 616e 6420 6f74 6865 7220 6169 7262 6f72  and other airbor
+000013d0: 6e65 2070 6172 7469 636c 6573 2e22 2c0a  ne particles.",.
+000013e0: 2020 2020 2249 6e64 6570 656e 6465 6e74      "Independent
+000013f0: 2046 6163 7473 223a 205b 0a20 2020 2020   Facts": [.     
+00001400: 2022 5468 6520 6361 6269 6e20 6169 7220   "The cabin air 
+00001410: 6669 6c74 6572 2073 686f 756c 6420 6265  filter should be
+00001420: 2069 6e73 7065 6374 6564 2065 7665 7279   inspected every
+00001430: 2031 352c 3030 3020 6d69 6c65 732e 222c   15,000 miles.",
+00001440: 0a20 2020 2020 2022 4974 2073 686f 756c  .      "It shoul
+00001450: 6420 6265 2072 6570 6c61 6365 6420 6173  d be replaced as
+00001460: 206e 6563 6573 7361 7279 2e22 2c0a 2020   necessary.",.  
+00001470: 2020 2020 2254 6865 2070 7572 706f 7365      "The purpose
+00001480: 2069 7320 746f 206d 6169 6e74 6169 6e20   is to maintain 
+00001490: 6169 7220 7175 616c 6974 7920 696e 7369  air quality insi
+000014a0: 6465 2074 6865 2076 6568 6963 6c65 2e22  de the vehicle."
+000014b0: 2c0a 2020 2020 2020 2252 6570 6c61 6365  ,.      "Replace
+000014c0: 6d65 6e74 2072 6564 7563 6573 2065 7870  ment reduces exp
+000014d0: 6f73 7572 6520 746f 2064 7573 742e 222c  osure to dust.",
+000014e0: 0a20 2020 2020 2022 4974 2061 6c73 6f20  .      "It also 
+000014f0: 7265 6475 6365 7320 6578 706f 7375 7265  reduces exposure
+00001500: 2074 6f20 706f 6c6c 656e 2e22 2c0a 2020   to pollen.",.  
+00001510: 2020 2020 2249 7420 7265 6475 6365 7320      "It reduces 
+00001520: 6578 706f 7375 7265 2074 6f20 6f74 6865  exposure to othe
+00001530: 7220 6169 7262 6f72 6e65 2070 6172 7469  r airborne parti
+00001540: 636c 6573 2e22 0a20 2020 205d 0a20 207d  cles.".    ].  }
+00001550: 0a5d                                     .]
```

### Comparing `FactScoreLite-0.1.0/FactScoreLite/data/demons_generation_prompt.txt` & `FactScoreLite-0.2.0/FactScoreLite/data/demons_generation_prompt.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Objective:
-Develop a comprehensive dataset containing 8 detailed examples from the automotive domain, focusing on sentences extracted from car manuals. This dataset should train GPT to adeptly break down complex sentences into their constituent, independent facts, enhancing its capability to process and understand intricate information.
-
-Dataset Specifications:
-
-    Source Material: Select sentences from a diverse array of sections within car manuals, including, but not limited to, technical specifications, maintenance guidelines, safety protocols, and feature explanations.
-    Complexity and Variety: Ensure the dataset represents:
-        A wide range of sentence complexities, from straightforward to multifaceted.
-        Sentences that incorporate a significant number of facts (aim for more than 10 per sentence where feasible).
-        Variations in sentence length and structure to include both concise and elaborate examples.
-        The inclusion of numerical data, symbols, and technical terminology.
-
-Dataset Format:
-
-    Format Requirement: Present the dataset in JSON format, with each entry comprising a sentence from a car manual and its breakdown into separate, independent facts.
-    Detailed Breakdown: Each fact should be a standalone piece of information that contributes to the full understanding of the original sentence.
-
-Example Dataset Entry:
-
-json
-
-[
-  {
-    "Sentence": "In 2020, the Model X received a firmware update that improved battery efficiency by 5%, allowing for an extended range of up to 350 miles on a single charge.",
-    "Independent Facts": [
-      "The event occurred in 2020.",
-      "The subject of the event is the Model X.",
-      "The Model X received a firmware update.",
-      "The firmware update was aimed at improving battery efficiency.",
-      "Battery efficiency was improved by 5%.",
-      "The improvement in battery efficiency contributed to an extended range.",
-      "The extended range allows for travel of up to 350 miles.",
-      "The travel range is achievable on a single charge."
-    ]
-  }
-]
-
-Instructional Goal:
-By dissecting sentences into smaller, independent facts, this dataset aims to:
-
-    Enhance GPT's ability to analyze, understand, and generate information from complex texts.
-    Prepare GPT for efficient processing and comprehension of technical documentation, specifically automotive manuals, by familiarizing it with the structure and content of such documents.
-
-Usage:
+Objective:
+Develop a comprehensive dataset containing 8 detailed examples from the automotive domain, focusing on sentences extracted from car manuals. This dataset should train GPT to adeptly break down complex sentences into their constituent, independent facts, enhancing its capability to process and understand intricate information.
+
+Dataset Specifications:
+
+    Source Material: Select sentences from a diverse array of sections within car manuals, including, but not limited to, technical specifications, maintenance guidelines, safety protocols, and feature explanations.
+    Complexity and Variety: Ensure the dataset represents:
+        A wide range of sentence complexities, from straightforward to multifaceted.
+        Sentences that incorporate a significant number of facts (aim for more than 10 per sentence where feasible).
+        Variations in sentence length and structure to include both concise and elaborate examples.
+        The inclusion of numerical data, symbols, and technical terminology.
+
+Dataset Format:
+
+    Format Requirement: Present the dataset in JSON format, with each entry comprising a sentence from a car manual and its breakdown into separate, independent facts.
+    Detailed Breakdown: Each fact should be a standalone piece of information that contributes to the full understanding of the original sentence.
+
+Example Dataset Entry:
+
+json
+
+[
+  {
+    "Sentence": "In 2020, the Model X received a firmware update that improved battery efficiency by 5%, allowing for an extended range of up to 350 miles on a single charge.",
+    "Independent Facts": [
+      "The event occurred in 2020.",
+      "The subject of the event is the Model X.",
+      "The Model X received a firmware update.",
+      "The firmware update was aimed at improving battery efficiency.",
+      "Battery efficiency was improved by 5%.",
+      "The improvement in battery efficiency contributed to an extended range.",
+      "The extended range allows for travel of up to 350 miles.",
+      "The travel range is achievable on a single charge."
+    ]
+  }
+]
+
+Instructional Goal:
+By dissecting sentences into smaller, independent facts, this dataset aims to:
+
+    Enhance GPT's ability to analyze, understand, and generate information from complex texts.
+    Prepare GPT for efficient processing and comprehension of technical documentation, specifically automotive manuals, by familiarizing it with the structure and content of such documents.
+
+Usage:
 This dataset will serve as a foundational tool in training GPT models to navigate and interpret the dense, technical information typically found in automotive manuals, ensuring they can provide accurate, detailed, and user-friendly responses and explanations.
```

### Comparing `FactScoreLite-0.1.0/LICENSE` & `FactScoreLite-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 armin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 armin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

