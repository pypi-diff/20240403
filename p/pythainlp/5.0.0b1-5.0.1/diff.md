# Comparing `tmp/pythainlp-5.0.0b1.tar.gz` & `tmp/pythainlp-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-5.0.0b1.tar", last modified: Mon Feb  5 05:37:49 2024, max compression
+gzip compressed data, was "pythainlp-5.0.1.tar", last modified: Sat Feb 10 15:11:39 2024, max compression
```

## Comparing `pythainlp-5.0.0b1.tar` & `pythainlp-5.0.1.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.223456 pythainlp-5.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-05 05:37:49.223456 pythainlp-5.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17925 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/README_TH.md
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.195456 pythainlp-5.0.0b1/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/ancient/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/ancient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/ancient/aksonhan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/lm/phayathaibert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/chat/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/chat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/classify/param_free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp/cls/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/cls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/coref/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/coref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/coref/_fastcoref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/coref/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/coref/han_coref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-05 05:37:38.000000 pythainlp-5.0.0b1/pythainlp/corpus/icu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/volubilis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/el/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/el/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/el/_multiel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/el/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/generate/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/generate/wangchanglm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25056 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.203456 pythainlp-5.0.0b1/pythainlp/morpheme/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/morpheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/morpheme/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/morpheme/word_formation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.207456 pythainlp-5.0.0b1/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.207456 pythainlp-5.0.0b1/pythainlp/phayathaibert/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/phayathaibert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/phayathaibert/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.207456 pythainlp-5.0.0b1/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.207456 pythainlp-5.0.0b1/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/spell/wanchanberta_thai_grammarly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.207456 pythainlp-5.0.0b1/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.211456 pythainlp-5.0.0b1/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.211456 pythainlp-5.0.0b1/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (127)    31393 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/han_solo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (127)    20614 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tokenize/wtsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.215456 pythainlp-5.0.0b1/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.215456 pythainlp-5.0.0b1/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/small100.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/tokenization_small100.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.215456 pythainlp-5.0.0b1/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.215456 pythainlp-5.0.0b1/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.219456 pythainlp-5.0.0b1/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/abbreviation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (127)    93468 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/morse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/pronounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/remove_trailing_repeat_consonants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/spell_words.py
--rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.219456 pythainlp-5.0.0b1/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.219456 pythainlp-5.0.0b1/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.219456 pythainlp-5.0.0b1/pythainlp/wsd/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/wsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/pythainlp/wsd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.199456 pythainlp-5.0.0b1/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-02-05 05:37:49.000000 pythainlp-5.0.0b1/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 05:37:48.000000 pythainlp-5.0.0b1/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-05 05:37:49.223456 pythainlp-5.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.223456 pythainlp-5.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 05:37:49.223456 pythainlp-5.0.0b1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_ancient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_coref.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_el.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_morpheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    58164 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (127)    38798 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_word_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-05 05:37:39.000000 pythainlp-5.0.0b1/tests/test_wsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.162659 pythainlp-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-02-10 15:11:27.000000 pythainlp-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-10 15:11:27.000000 pythainlp-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-10 15:11:27.000000 pythainlp-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-02-10 15:11:39.162659 pythainlp-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-02-10 15:11:27.000000 pythainlp-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17925 2024-02-10 15:11:27.000000 pythainlp-5.0.1/README_TH.md
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp/ancient/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ancient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ancient/aksonhan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/lm/phayathaibert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/chat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/classify/param_free.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/cls/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/cls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/coref/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/coref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/coref/_fastcoref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/coref/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/coref/han_coref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.126659 pythainlp-5.0.1/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/icu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/volubilis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/el/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/el/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/el/_multiel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/el/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/generate/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/generate/wangchanglm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25056 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/morpheme/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/morpheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/morpheme/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/morpheme/word_formation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/phayathaibert/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/phayathaibert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/phayathaibert/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.130659 pythainlp-5.0.1/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.134659 pythainlp-5.0.1/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/spell/wanchanberta_thai_grammarly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.134659 pythainlp-5.0.1/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.134659 pythainlp-5.0.1/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.146659 pythainlp-5.0.1/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31393 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/han_solo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20614 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tokenize/wtsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.146659 pythainlp-5.0.1/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.146659 pythainlp-5.0.1/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/small100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/tokenization_small100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.150658 pythainlp-5.0.1/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.150658 pythainlp-5.0.1/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.154659 pythainlp-5.0.1/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/abbreviation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93468 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/morse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/pronounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/remove_trailing_repeat_consonants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/spell_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.154659 pythainlp-5.0.1/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.154659 pythainlp-5.0.1/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.154659 pythainlp-5.0.1/pythainlp/wsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/wsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-02-10 15:11:27.000000 pythainlp-5.0.1/pythainlp/wsd/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.122659 pythainlp-5.0.1/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-02-10 15:11:39.000000 pythainlp-5.0.1/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-10 15:11:38.000000 pythainlp-5.0.1/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-10 15:11:39.162659 pythainlp-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-02-10 15:11:27.000000 pythainlp-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.162659 pythainlp-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 15:11:39.162659 pythainlp-5.0.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_coref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_el.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_morpheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58164 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38798 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_word_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-10 15:11:27.000000 pythainlp-5.0.1/tests/test_wsd.py
```

### Comparing `pythainlp-5.0.0b1/CONTRIBUTING.md` & `pythainlp-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/LICENSE` & `pythainlp-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/PKG-INFO` & `pythainlp-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 5.0.0b1
+Version: 5.0.1
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
-Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
+Project-URL: Documentation, https://pythainlp.github.io/docs/5.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
 Project-URL: Source Code, https://github.com/PyThaiNLP/pythainlp
 Project-URL: Bug Tracker, https://github.com/PyThaiNLP/pythainlp/issues
 Description: 
         ![PyThaiNLP Logo](https://avatars0.githubusercontent.com/u/32934255?s=200&v=4)
         
         PyThaiNLP is a Python library for Thai natural language processing.
```

### Comparing `pythainlp-5.0.0b1/README.md` & `pythainlp-5.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 **News**
 
 > Now, You can contact with or ask any questions of the PyThaiNLP team. <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | Version | Description | Status |
 |:------:|:--:|:------:|
-| [4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
-| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.0 | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [5.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1 | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/900) |
 
 
 ## Getting Started
 
 - PyThaiNLP 2 requires Python 3.7+. Python 2.7 users can use PyThaiNLP 1.6. See [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) | [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/pythainlp/wiki/Upgrade-ThaiNER-from-PyThaiNLP-1.7-to-PyThaiNLP-2.0)
 - [PyThaiNLP Get Started notebook](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) | [API document](https://pythainlp.github.io/docs) | [Tutorials](https://pythainlp.github.io/tutorials)
 - [Official website](https://pythainlp.github.io/) | [PyPI](https://pypi.org/project/pythainlp/) | [Facebook page](https://www.facebook.com/pythainlp/)
```

#### html2text {}

```diff
@@ -10,18 +10,18 @@
 PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¸à¸¥à¹à¸²à¸¢à¸à¸±à¸ NLTK à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢
 [à¸à¸¹à¸£à¸²à¸¢à¸¥à¸°à¹à¸­à¸µà¸¢à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢à¹à¸à¹à¸à¸µà¹
 README_TH.MD](https://github.com/PyThaiNLP/pythainlp/blob/dev/README_TH.md)
 **News** > Now, You can contact with or ask any questions of the PyThaiNLP
 team. _[_C_h_a_t_ _o_n_ _M_a_t_r_i_x_]| Version | Description | Status | |:------:|:--:|:-----
--:| | [4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change
-Log](https://github.com/PyThaiNLP/pythainlp/issues/714) | | [`dev`](https://
-github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.0 | [Change
-Log](https://github.com/PyThaiNLP/pythainlp/issues/788) | ## Getting Started -
+-:| | [5.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change
+Log](https://github.com/PyThaiNLP/pythainlp/issues/788) | | [`dev`](https://
+github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1 | [Change
+Log](https://github.com/PyThaiNLP/pythainlp/issues/900) | ## Getting Started -
 PyThaiNLP 2 requires Python 3.7+. Python 2.7 users can use PyThaiNLP 1.6. See
 [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) |
 [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-
 2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/
 pythainlp/wiki/Upgrade-ThaiNER-from-PyThaiNLP-1.7-to-PyThaiNLP-2.0) -
 [PyThaiNLP Get Started notebook](https://pythainlp.github.io/tutorials/
 notebooks/pythainlp_get_started.html) | [API document](https://
```

### Comparing `pythainlp-5.0.0b1/README_TH.md` & `pythainlp-5.0.1/README_TH.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 **ข่าวสาร**
 
 > คุณสามารถพูดคุยหรือแชทกับทีม PyThaiNLP หรือผู้สนับสนุนคนอื่น ๆ ได้ที่ <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | รุ่น | คำอธิบาย | สถานะ |
 |:------:|:--:|:------:|
-| [4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
-| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.0  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [5.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/900) |
 
 ติดตามพวกเราบน [PyThaiNLP Facebook page](https://www.facebook.com/pythainlp/) เพื่อรับข่าวสารเพิ่มเติม
 
 
 ## เริ่มต้นกับ PyThaiNLP
 
 พวกเราได้จัดทำ [PyThaiNLP Get Started Tutorial](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) สำหรับสำรวจความสามารถของ PyThaiNLP; พวกเรามีเอกสารสอนใช้งาน สามารถศึกษาได้ที่ [หน้า tutorial](https://pythainlp.github.io/tutorials).
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
                  _B_a_d_g_e_]_[_F_O_S_S_A_ _S_t_a_t_u_s_]_[_G_o_o_g_l_e_ _C_o_l_a_b_ _B_a_d_g_e_]_[_D_O_I_]
 PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢ **à¸à¹à¸²à¸§à¸ªà¸²à¸£** >
 à¸à¸¸à¸à¸ªà¸²à¸¡à¸²à¸£à¸à¸à¸¹à¸à¸à¸¸à¸¢à¸«à¸£à¸·à¸­à¹à¸à¸à¸à¸±à¸à¸à¸µà¸¡
 PyThaiNLP à¸«à¸£à¸·à¸­à¸à¸¹à¹à¸ªà¸à¸±à¸à¸ªà¸à¸¸à¸à¸à¸à¸­à¸·à¹à¸ à¹
 à¹à¸à¹à¸à¸µà¹ _[_C_h_a_t_ _o_n_ _M_a_t_r_i_x_]| à¸£à¸¸à¹à¸ | à¸à¸³à¸­à¸à¸´à¸à¸²à¸¢ |
-à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [4.0](https://github.com/
+à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [5.0](https://github.com/
 PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/
-PyThaiNLP/pythainlp/issues/714) | | [`dev`](https://github.com/PyThaiNLP/
-pythainlp/tree/dev) | Release Candidate for 5.0 | [Change Log](https://
-github.com/PyThaiNLP/pythainlp/issues/788) |
+PyThaiNLP/pythainlp/issues/788) | | [`dev`](https://github.com/PyThaiNLP/
+pythainlp/tree/dev) | Release Candidate for 5.1 | [Change Log](https://
+github.com/PyThaiNLP/pythainlp/issues/900) |
 à¸à¸´à¸à¸à¸²à¸¡à¸à¸§à¸à¹à¸£à¸²à¸à¸ [PyThaiNLP Facebook page](https://
 www.facebook.com/pythainlp/
 ) à¹à¸à¸·à¹à¸­à¸£à¸±à¸à¸à¹à¸²à¸§à¸ªà¸²à¸£à¹à¸à¸´à¹à¸¡à¹à¸à¸´à¸¡ ##
 à¹à¸£à¸´à¹à¸¡à¸à¹à¸à¸à¸±à¸ PyThaiNLP
 à¸à¸§à¸à¹à¸£à¸²à¹à¸à¹à¸à¸±à¸à¸à¸³ [PyThaiNLP Get Started Tutorial]
 (https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html)
 à¸ªà¸³à¸«à¸£à¸±à¸à¸ªà¸³à¸£à¸§à¸à¸à¸§à¸²à¸¡à¸ªà¸²à¸¡à¸²à¸£à¸à¸à¸­à¸
```

### Comparing `pythainlp-5.0.0b1/pythainlp/__init__.py` & `pythainlp-5.0.1/pythainlp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: Copyright 2016-2024 PyThaiNLP Project
 # SPDX-License-Identifier: Apache-2.0
-__version__ = "5.0.0beta1"
+__version__ = "5.0.1"
 
 thai_consonants = "กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรลวศษสหฬอฮ"  # 44 chars
 
 thai_vowels = (
     "\u0e24\u0e26\u0e30\u0e31\u0e32\u0e33\u0e34\u0e35\u0e36\u0e37"
     + "\u0e38\u0e39\u0e40\u0e41\u0e42\u0e43\u0e44\u0e45\u0e4d\u0e47"
 )  # 20
```

### Comparing `pythainlp-5.0.0b1/pythainlp/__main__.py` & `pythainlp-5.0.1/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/ancient/aksonhan.py` & `pythainlp-5.0.1/pythainlp/ancient/aksonhan.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/lm/fasttext.py` & `pythainlp-5.0.1/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/lm/phayathaibert.py` & `pythainlp-5.0.1/pythainlp/augment/lm/phayathaibert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-5.0.1/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-5.0.1/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/word2vec/core.py` & `pythainlp-5.0.1/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-5.0.1/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-5.0.1/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/augment/wordnet.py` & `pythainlp-5.0.1/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-5.0.1/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/chat/core.py` & `pythainlp-5.0.1/pythainlp/chat/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/classify/param_free.py` & `pythainlp-5.0.1/pythainlp/classify/param_free.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/__init__.py` & `pythainlp-5.0.1/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/benchmark.py` & `pythainlp-5.0.1/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/data.py` & `pythainlp-5.0.1/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/soundex.py` & `pythainlp-5.0.1/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/tag.py` & `pythainlp-5.0.1/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/cli/tokenize.py` & `pythainlp-5.0.1/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/coref/_fastcoref.py` & `pythainlp-5.0.1/pythainlp/coref/_fastcoref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/coref/core.py` & `pythainlp-5.0.1/pythainlp/coref/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/__init__.py` & `pythainlp-5.0.1/pythainlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/common.py` & `pythainlp-5.0.1/pythainlp/corpus/common.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/conceptnet.py` & `pythainlp-5.0.1/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/core.py` & `pythainlp-5.0.1/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/icu.py` & `pythainlp-5.0.1/pythainlp/corpus/icu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/oscar.py` & `pythainlp-5.0.1/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/th_en_translit.py` & `pythainlp-5.0.1/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/tnc.py` & `pythainlp-5.0.1/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/ttc.py` & `pythainlp-5.0.1/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/util.py` & `pythainlp-5.0.1/pythainlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/volubilis.py` & `pythainlp-5.0.1/pythainlp/corpus/volubilis.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/wikipedia.py` & `pythainlp-5.0.1/pythainlp/corpus/wikipedia.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/corpus/wordnet.py` & `pythainlp-5.0.1/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/el/_multiel.py` & `pythainlp-5.0.1/pythainlp/el/_multiel.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/el/core.py` & `pythainlp-5.0.1/pythainlp/el/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/generate/core.py` & `pythainlp-5.0.1/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/generate/thai2fit.py` & `pythainlp-5.0.1/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/generate/wangchanglm.py` & `pythainlp-5.0.1/pythainlp/generate/wangchanglm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/khavee/core.py` & `pythainlp-5.0.1/pythainlp/khavee/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/khavee/example.py` & `pythainlp-5.0.1/pythainlp/khavee/example.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/morpheme/thaiwordcheck.py` & `pythainlp-5.0.1/pythainlp/morpheme/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/morpheme/word_formation.py` & `pythainlp-5.0.1/pythainlp/morpheme/word_formation.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     Read more: https://www.trueplookpanya.com/learning/detail/1180
 
     :param str w1: A Thai word that has a nighit.
     :param str w2: A Thai word.
     :return: Thai word.
     :rtype: str
     :Example:
+
     ::
+
         from pythainlp.morpheme import nighit
 
         assert nighit("สํ","คีต")=="สังคีต"
         assert nighit("สํ","จร")=="สัญจร"
         assert nighit("สํ","ฐาน")=="สัณฐาน"
         assert nighit("สํ","นิษฐาน")=="สันนิษฐาน"
         assert nighit("สํ","ปทา")=="สัมปทา"
```

### Comparing `pythainlp-5.0.0b1/pythainlp/parse/core.py` & `pythainlp-5.0.1/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/parse/esupar_engine.py` & `pythainlp-5.0.1/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-5.0.1/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/parse/transformers_ud.py` & `pythainlp-5.0.1/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/parse/ud_goeswith.py` & `pythainlp-5.0.1/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/phayathaibert/core.py` & `pythainlp-5.0.1/pythainlp/phayathaibert/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/__init__.py` & `pythainlp-5.0.1/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/core.py` & `pythainlp-5.0.1/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/lk82.py` & `pythainlp-5.0.1/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/metasound.py` & `pythainlp-5.0.1/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-5.0.1/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/sound.py` & `pythainlp-5.0.1/pythainlp/soundex/sound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/soundex/udom83.py` & `pythainlp-5.0.1/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/spell/core.py` & `pythainlp-5.0.1/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/spell/pn.py` & `pythainlp-5.0.1/pythainlp/spell/pn.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/spell/symspellpy.py` & `pythainlp-5.0.1/pythainlp/spell/symspellpy.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/spell/wanchanberta_thai_grammarly.py` & `pythainlp-5.0.1/pythainlp/spell/wanchanberta_thai_grammarly.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/summarize/core.py` & `pythainlp-5.0.1/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/summarize/freq.py` & `pythainlp-5.0.1/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/summarize/keybert.py` & `pythainlp-5.0.1/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/summarize/mt5.py` & `pythainlp-5.0.1/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/__init__.py` & `pythainlp-5.0.1/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/_tag_perceptron.py` & `pythainlp-5.0.1/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/blackboard.py` & `pythainlp-5.0.1/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/chunk.py` & `pythainlp-5.0.1/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/crfchunk.py` & `pythainlp-5.0.1/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/locations.py` & `pythainlp-5.0.1/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/named_entity.py` & `pythainlp-5.0.1/pythainlp/tag/named_entity.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/orchid.py` & `pythainlp-5.0.1/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/perceptron.py` & `pythainlp-5.0.1/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/pos_tag.py` & `pythainlp-5.0.1/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/thainer.py` & `pythainlp-5.0.1/pythainlp/tag/thainer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/tltk.py` & `pythainlp-5.0.1/pythainlp/tag/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/unigram.py` & `pythainlp-5.0.1/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-5.0.1/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/__init__.py` & `pythainlp-5.0.1/pythainlp/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/_utils.py` & `pythainlp-5.0.1/pythainlp/tokenize/_utils.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/attacut.py` & `pythainlp-5.0.1/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/core.py` & `pythainlp-5.0.1/pythainlp/tokenize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/crfcls.py` & `pythainlp-5.0.1/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/crfcut.py` & `pythainlp-5.0.1/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/deepcut.py` & `pythainlp-5.0.1/pythainlp/tokenize/deepcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/etcc.py` & `pythainlp-5.0.1/pythainlp/tokenize/etcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/han_solo.py` & `pythainlp-5.0.1/pythainlp/tokenize/han_solo.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/longest.py` & `pythainlp-5.0.1/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/multi_cut.py` & `pythainlp-5.0.1/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/nercut.py` & `pythainlp-5.0.1/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/newmm.py` & `pythainlp-5.0.1/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/nlpo3.py` & `pythainlp-5.0.1/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/oskut.py` & `pythainlp-5.0.1/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/pyicu.py` & `pythainlp-5.0.1/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/sefr_cut.py` & `pythainlp-5.0.1/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/tcc.py` & `pythainlp-5.0.1/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/tcc_p.py` & `pythainlp-5.0.1/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/thaisumcut.py` & `pythainlp-5.0.1/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/tltk.py` & `pythainlp-5.0.1/pythainlp/tokenize/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tokenize/wtsplit.py` & `pythainlp-5.0.1/pythainlp/tokenize/wtsplit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tools/misspell.py` & `pythainlp-5.0.1/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/tools/path.py` & `pythainlp-5.0.1/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/core.py` & `pythainlp-5.0.1/pythainlp/translate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/en_th.py` & `pythainlp-5.0.1/pythainlp/translate/en_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/small100.py` & `pythainlp-5.0.1/pythainlp/translate/small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/th_fr.py` & `pythainlp-5.0.1/pythainlp/translate/th_fr.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/tokenization_small100.py` & `pythainlp-5.0.1/pythainlp/translate/tokenization_small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/translate/zh_th.py` & `pythainlp-5.0.1/pythainlp/translate/zh_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/core.py` & `pythainlp-5.0.1/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/ipa.py` & `pythainlp-5.0.1/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/iso_11940.py` & `pythainlp-5.0.1/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/lookup.py` & `pythainlp-5.0.1/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/pyicu.py` & `pythainlp-5.0.1/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/royin.py` & `pythainlp-5.0.1/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/spoonerism.py` & `pythainlp-5.0.1/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/thai2rom.py` & `pythainlp-5.0.1/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-5.0.1/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/thaig2p.py` & `pythainlp-5.0.1/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/tltk.py` & `pythainlp-5.0.1/pythainlp/transliterate/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/w2p.py` & `pythainlp-5.0.1/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/transliterate/wunsen.py` & `pythainlp-5.0.1/pythainlp/transliterate/wunsen.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/ulmfit/__init__.py` & `pythainlp-5.0.1/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/ulmfit/core.py` & `pythainlp-5.0.1/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/ulmfit/preprocess.py` & `pythainlp-5.0.1/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/ulmfit/tokenizer.py` & `pythainlp-5.0.1/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/__init__.py` & `pythainlp-5.0.1/pythainlp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/abbreviation.py` & `pythainlp-5.0.1/pythainlp/util/abbreviation.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/collate.py` & `pythainlp-5.0.1/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/date.py` & `pythainlp-5.0.1/pythainlp/util/date.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/digitconv.py` & `pythainlp-5.0.1/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/emojiconv.py` & `pythainlp-5.0.1/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/encoding.py` & `pythainlp-5.0.1/pythainlp/util/encoding.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/keyboard.py` & `pythainlp-5.0.1/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/keywords.py` & `pythainlp-5.0.1/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/morse.py` & `pythainlp-5.0.1/pythainlp/util/morse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/normalize.py` & `pythainlp-5.0.1/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/numtoword.py` & `pythainlp-5.0.1/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/phoneme.py` & `pythainlp-5.0.1/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/pronounce.py` & `pythainlp-5.0.1/pythainlp/util/pronounce.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 from pythainlp.corpus import thai_words
 from pythainlp.tokenize import syllable_tokenize
 from pythainlp.khavee import KhaveeVerifier
 
 
 kv = KhaveeVerifier()
-all_thai_words_dict = [
-    i for i in list(thai_words()) if len(syllable_tokenize(i)) == 1
-]
+all_thai_words_dict = None
 
 
 def rhyme(word: str) -> List[str]:
     """
     Find Thai rhyme
 
     :param str word: A Thai word
@@ -25,12 +23,17 @@
     :Example:
     ::
         from pythainlp.util import rhyme
 
         print(rhyme("จีบ"))
         # output: ['กลีบ', 'กีบ', 'ครีบ', ...]
     """
+    global all_thai_words_dict
     list_sumpus = []
+    if all_thai_words_dict == None:
+        all_thai_words_dict = [
+            i for i in list(thai_words()) if len(syllable_tokenize(i)) == 1
+        ]
     for i in all_thai_words_dict:
         if kv.is_sumpus(word, i) and i != word:
             list_sumpus.append(i)
     return sorted(list_sumpus)
```

### Comparing `pythainlp-5.0.0b1/pythainlp/util/remove_trailing_repeat_consonants.py` & `pythainlp-5.0.1/pythainlp/util/remove_trailing_repeat_consonants.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/spell_words.py` & `pythainlp-5.0.1/pythainlp/util/spell_words.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/strftime.py` & `pythainlp-5.0.1/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/syllable.py` & `pythainlp-5.0.1/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/thai.py` & `pythainlp-5.0.1/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/time.py` & `pythainlp-5.0.1/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/trie.py` & `pythainlp-5.0.1/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/util/wordtonum.py` & `pythainlp-5.0.1/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/wangchanberta/core.py` & `pythainlp-5.0.1/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/word_vector/core.py` & `pythainlp-5.0.1/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp/wsd/core.py` & `pythainlp-5.0.1/pythainlp/wsd/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp.egg-info/PKG-INFO` & `pythainlp-5.0.1/pythainlp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 5.0.0b1
+Version: 5.0.1
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
-Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
+Project-URL: Documentation, https://pythainlp.github.io/docs/5.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
 Project-URL: Source Code, https://github.com/PyThaiNLP/pythainlp
 Project-URL: Bug Tracker, https://github.com/PyThaiNLP/pythainlp/issues
 Description: 
         ![PyThaiNLP Logo](https://avatars0.githubusercontent.com/u/32934255?s=200&v=4)
         
         PyThaiNLP is a Python library for Thai natural language processing.
```

### Comparing `pythainlp-5.0.0b1/pythainlp.egg-info/SOURCES.txt` & `pythainlp-5.0.1/pythainlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/pythainlp.egg-info/requires.txt` & `pythainlp-5.0.1/pythainlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/setup.cfg` & `pythainlp-5.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 5.0.0beta1
+current_version = 5.0.1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `pythainlp-5.0.0b1/setup.py` & `pythainlp-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         "sentence-transformers>=2.2.2",
         "khamyo>=0.2.0",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="5.0.0beta1",
+    version="5.0.1",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
@@ -206,15 +206,15 @@
     ],
     entry_points={
         "console_scripts": [
             "thainlp = pythainlp.__main__:main",
         ],
     },
     project_urls={
-        "Documentation": "https://pythainlp.github.io/docs/4.0/",
+        "Documentation": "https://pythainlp.github.io/docs/5.0/",
         "Tutorials": "https://pythainlp.github.io/tutorials/",
         "Source Code": "https://github.com/PyThaiNLP/pythainlp",
         "Bug Tracker": "https://github.com/PyThaiNLP/pythainlp/issues",
     },
 )
 
 # TODO: Check extras and decide whether or not additional data, like model files, should be downloaded
```

### Comparing `pythainlp-5.0.0b1/tests/data/eval-details-input.json` & `pythainlp-5.0.1/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/data/sentences.yml` & `pythainlp-5.0.1/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_ancient.py` & `pythainlp-5.0.1/tests/test_ancient.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_augment.py` & `pythainlp-5.0.1/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_benchmarks.py` & `pythainlp-5.0.1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_classify.py` & `pythainlp-5.0.1/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_cli.py` & `pythainlp-5.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_coref.py` & `pythainlp-5.0.1/tests/test_coref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_corpus.py` & `pythainlp-5.0.1/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_generate.py` & `pythainlp-5.0.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_khavee.py` & `pythainlp-5.0.1/tests/test_khavee.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_misspell.py` & `pythainlp-5.0.1/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_morpheme.py` & `pythainlp-5.0.1/tests/test_morpheme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_parse.py` & `pythainlp-5.0.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_soundex.py` & `pythainlp-5.0.1/tests/test_soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_spell.py` & `pythainlp-5.0.1/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_summarize.py` & `pythainlp-5.0.1/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_tag.py` & `pythainlp-5.0.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_tokenize.py` & `pythainlp-5.0.1/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_tools.py` & `pythainlp-5.0.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_translate.py` & `pythainlp-5.0.1/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_transliterate.py` & `pythainlp-5.0.1/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_ulmfit.py` & `pythainlp-5.0.1/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_util.py` & `pythainlp-5.0.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_wangchanberta.py` & `pythainlp-5.0.1/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_word_vector.py` & `pythainlp-5.0.1/tests/test_word_vector.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.0b1/tests/test_wsd.py` & `pythainlp-5.0.1/tests/test_wsd.py`

 * *Files identical despite different names*

