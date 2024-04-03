# Comparing `tmp/pycorrector-1.0.3.tar.gz` & `tmp/pycorrector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycorrector-1.0.3.tar", last modified: Mon Feb 19 07:06:49 2024, max compression
+gzip compressed data, was "pycorrector-1.0.4.tar", last modified: Wed Apr  3 03:35:23 2024, max compression
```

## Comparing `pycorrector-1.0.3.tar` & `pycorrector-1.0.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.240254 pycorrector-1.0.3/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-04 13:23:48.000000 pycorrector-1.0.3/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    32809 2024-02-19 07:06:49.239914 pycorrector-1.0.3/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    31950 2024-01-15 04:09:57.000000 pycorrector-1.0.3/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.114900 pycorrector-1.0.3/pycorrector/
--rw-r--r--   0 xuming     (501) staff       (20)     1237 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     2053 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/__main__.py
--rw-r--r--   0 xuming     (501) staff       (20)     2804 2024-02-03 12:41:18.000000 pycorrector-1.0.3/pycorrector/confusion_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    12151 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.154986 pycorrector-1.0.3/pycorrector/data/
--rw-r--r--   0 xuming     (501) staff       (20)    14008 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/common_char_set.txt
--rw-r--r--   0 xuming     (501) staff       (20)   588917 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/data/en.json.gz
--rw-r--r--   0 xuming     (501) staff       (20)   163162 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/person_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)   640666 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/place_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)      162 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/data/proper_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)   197815 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/same_pinyin.txt
--rw-r--r--   0 xuming     (501) staff       (20)    14636 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/same_stroke.txt
--rwxr-xr-x   0 xuming     (501) staff       (20)   204700 2023-11-07 05:11:23.000000 pycorrector-1.0.3/pycorrector/data/sighan2015_test.tsv
--rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/data/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)   202746 2022-11-22 07:22:06.000000 pycorrector-1.0.3/pycorrector/data/stroke.txt
--rwxr-xr-x   0 xuming     (501) staff       (20)  8583143 2023-09-13 09:50:34.000000 pycorrector-1.0.3/pycorrector/data/word_freq.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.188495 pycorrector-1.0.3/pycorrector/deepcontext/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/deepcontext/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3975 2023-11-08 07:43:40.000000 pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     9723 2023-11-08 07:23:58.000000 pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    15186 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    18606 2024-02-03 12:40:07.000000 pycorrector-1.0.3/pycorrector/detector.py
--rw-r--r--   0 xuming     (501) staff       (20)     6692 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/en_spell_corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.197297 pycorrector-1.0.3/pycorrector/ernie_csc/
--rw-r--r--   0 xuming     (501) staff       (20)       81 2023-10-29 14:38:15.000000 pycorrector-1.0.3/pycorrector/ernie_csc/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1585 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/ernie_csc/ernie_csc_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     6253 2023-10-29 14:38:15.000000 pycorrector-1.0.3/pycorrector/ernie_csc/model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6455 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/ernie_csc/predict.py
--rw-r--r--   0 xuming     (501) staff       (20)     4662 2023-10-29 14:38:33.000000 pycorrector-1.0.3/pycorrector/ernie_csc/sighan_evaluate.py
--rw-r--r--   0 xuming     (501) staff       (20)     5147 2023-10-29 14:38:15.000000 pycorrector-1.0.3/pycorrector/ernie_csc/utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.206477 pycorrector-1.0.3/pycorrector/gpt/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/gpt/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3574 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/gpt/gpt_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    30620 2024-02-18 10:41:54.000000 pycorrector-1.0.3/pycorrector/gpt/gpt_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    19381 2023-11-28 06:46:20.000000 pycorrector-1.0.3/pycorrector/gpt/gpt_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     3254 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/gpt/merge_peft_adapter.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.218707 pycorrector-1.0.3/pycorrector/macbert/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-11-22 13:24:05.000000 pycorrector-1.0.3/pycorrector/macbert/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     7197 2024-01-15 07:01:25.000000 pycorrector-1.0.3/pycorrector/macbert/base_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     3565 2021-10-31 04:24:05.000000 pycorrector-1.0.3/pycorrector/macbert/defaults.py
--rw-r--r--   0 xuming     (501) staff       (20)     9012 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/macbert/evaluate_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     6636 2021-10-31 04:24:05.000000 pycorrector-1.0.3/pycorrector/macbert/lr_scheduler.py
--rw-r--r--   0 xuming     (501) staff       (20)     2101 2021-12-28 03:36:23.000000 pycorrector-1.0.3/pycorrector/macbert/macbert4csc.py
--rw-r--r--   0 xuming     (501) staff       (20)     4871 2024-01-15 04:25:57.000000 pycorrector-1.0.3/pycorrector/macbert/macbert_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)     2502 2024-01-15 04:25:57.000000 pycorrector-1.0.3/pycorrector/macbert/reader.py
--rw-r--r--   0 xuming     (501) staff       (20)     6375 2021-11-22 11:54:21.000000 pycorrector-1.0.3/pycorrector/macbert/softmaskedbert4csc.py
--rw-r--r--   0 xuming     (501) staff       (20)     9237 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/proper_corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.223934 pycorrector-1.0.3/pycorrector/seq2seq/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-03 12:20:07.000000 pycorrector-1.0.3/pycorrector/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3774 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_corrector.py
--rw-r--r--   0 xuming     (501) staff       (20)    23598 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5045 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.226029 pycorrector-1.0.3/pycorrector/t5/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-03 12:05:43.000000 pycorrector-1.0.3/pycorrector/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     4044 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/t5/t5_corrector.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.237300 pycorrector-1.0.3/pycorrector/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     5274 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/utils/error_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     4918 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/utils/evaluate_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    12583 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)     1132 2021-12-02 13:22:02.000000 pycorrector-1.0.3/pycorrector/utils/io_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     8081 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/utils/langconv.py
--rw-r--r--   0 xuming     (501) staff       (20)     3214 2022-03-22 06:45:40.000000 pycorrector-1.0.3/pycorrector/utils/math_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     6234 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/utils/ngram_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     4904 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/utils/text_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     6157 2023-11-07 05:11:24.000000 pycorrector-1.0.3/pycorrector/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)   143019 2021-08-04 13:23:48.000000 pycorrector-1.0.3/pycorrector/utils/zh_wiki.py
--rw-r--r--   0 xuming     (501) staff       (20)       22 2024-02-18 10:43:37.000000 pycorrector-1.0.3/pycorrector/version.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-02-19 07:06:49.120167 pycorrector-1.0.3/pycorrector.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    32809 2024-02-19 07:06:48.000000 pycorrector-1.0.3/pycorrector.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     2242 2024-02-19 07:06:49.000000 pycorrector-1.0.3/pycorrector.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2024-02-19 07:06:48.000000 pycorrector-1.0.3/pycorrector.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-06-17 09:04:59.000000 pycorrector-1.0.3/pycorrector.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       32 2024-02-19 07:06:48.000000 pycorrector-1.0.3/pycorrector.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       12 2024-02-19 07:06:48.000000 pycorrector-1.0.3/pycorrector.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)       38 2024-02-19 07:06:49.240386 pycorrector-1.0.3/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1611 2024-02-19 07:05:38.000000 pycorrector-1.0.3/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.976775 pycorrector-1.0.4/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-04 13:23:48.000000 pycorrector-1.0.4/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    32569 2024-04-03 03:35:23.976133 pycorrector-1.0.4/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    31712 2024-03-20 04:46:44.000000 pycorrector-1.0.4/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.826276 pycorrector-1.0.4/pycorrector/
+-rw-r--r--   0 xuming     (501) staff       (20)     1237 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2053 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/__main__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2804 2024-02-03 12:41:18.000000 pycorrector-1.0.4/pycorrector/confusion_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12151 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.864138 pycorrector-1.0.4/pycorrector/data/
+-rw-r--r--   0 xuming     (501) staff       (20)    14008 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/common_char_set.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   588917 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/data/en.json.gz
+-rw-r--r--   0 xuming     (501) staff       (20)   163162 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/person_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   640666 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/place_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      162 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/data/proper_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   197815 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/same_pinyin.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    14636 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/same_stroke.txt
+-rwxr-xr-x   0 xuming     (501) staff       (20)   204700 2023-11-07 05:11:23.000000 pycorrector-1.0.4/pycorrector/data/sighan2015_test.tsv
+-rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/data/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   202746 2022-11-22 07:22:06.000000 pycorrector-1.0.4/pycorrector/data/stroke.txt
+-rwxr-xr-x   0 xuming     (501) staff       (20)  8583143 2023-09-13 09:50:34.000000 pycorrector-1.0.4/pycorrector/data/word_freq.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.916477 pycorrector-1.0.4/pycorrector/deepcontext/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/deepcontext/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3975 2023-11-08 07:43:40.000000 pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9723 2023-11-08 07:23:58.000000 pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15186 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18645 2024-03-20 05:03:32.000000 pycorrector-1.0.4/pycorrector/detector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6692 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/en_spell_corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.926321 pycorrector-1.0.4/pycorrector/ernie_csc/
+-rw-r--r--   0 xuming     (501) staff       (20)       81 2023-10-29 14:38:15.000000 pycorrector-1.0.4/pycorrector/ernie_csc/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1585 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/ernie_csc/ernie_csc_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6253 2023-10-29 14:38:15.000000 pycorrector-1.0.4/pycorrector/ernie_csc/model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6455 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/ernie_csc/predict.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4662 2023-10-29 14:38:33.000000 pycorrector-1.0.4/pycorrector/ernie_csc/sighan_evaluate.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5147 2023-10-29 14:38:15.000000 pycorrector-1.0.4/pycorrector/ernie_csc/utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.934648 pycorrector-1.0.4/pycorrector/gpt/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/gpt/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3574 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/gpt/gpt_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    30620 2024-02-18 10:41:54.000000 pycorrector-1.0.4/pycorrector/gpt/gpt_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19381 2023-11-28 06:46:20.000000 pycorrector-1.0.4/pycorrector/gpt/gpt_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3254 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/gpt/merge_peft_adapter.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.950624 pycorrector-1.0.4/pycorrector/macbert/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-11-22 13:24:05.000000 pycorrector-1.0.4/pycorrector/macbert/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7197 2024-01-15 07:01:25.000000 pycorrector-1.0.4/pycorrector/macbert/base_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3565 2021-10-31 04:24:05.000000 pycorrector-1.0.4/pycorrector/macbert/defaults.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9012 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/macbert/evaluate_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6636 2021-10-31 04:24:05.000000 pycorrector-1.0.4/pycorrector/macbert/lr_scheduler.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2101 2021-12-28 03:36:23.000000 pycorrector-1.0.4/pycorrector/macbert/macbert4csc.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4871 2024-01-15 04:25:57.000000 pycorrector-1.0.4/pycorrector/macbert/macbert_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2502 2024-01-15 04:25:57.000000 pycorrector-1.0.4/pycorrector/macbert/reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6375 2021-11-22 11:54:21.000000 pycorrector-1.0.4/pycorrector/macbert/softmaskedbert4csc.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9237 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/proper_corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.957523 pycorrector-1.0.4/pycorrector/seq2seq/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-03 12:20:07.000000 pycorrector-1.0.4/pycorrector/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3774 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_corrector.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23598 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5045 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.960781 pycorrector-1.0.4/pycorrector/t5/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-11-03 12:05:43.000000 pycorrector-1.0.4/pycorrector/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4044 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/t5/t5_corrector.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.971853 pycorrector-1.0.4/pycorrector/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5274 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/utils/error_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4918 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/utils/evaluate_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12583 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1132 2021-12-02 13:22:02.000000 pycorrector-1.0.4/pycorrector/utils/io_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8081 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/utils/langconv.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3214 2022-03-22 06:45:40.000000 pycorrector-1.0.4/pycorrector/utils/math_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6234 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/utils/ngram_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4904 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/utils/text_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6157 2023-11-07 05:11:24.000000 pycorrector-1.0.4/pycorrector/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)   143019 2021-08-04 13:23:48.000000 pycorrector-1.0.4/pycorrector/utils/zh_wiki.py
+-rw-r--r--   0 xuming     (501) staff       (20)       22 2024-04-03 03:02:22.000000 pycorrector-1.0.4/pycorrector/version.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-04-03 03:35:23.829572 pycorrector-1.0.4/pycorrector.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    32569 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     2242 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       61 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       12 2024-04-03 03:35:23.000000 pycorrector-1.0.4/pycorrector.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2024-04-03 03:35:23.977017 pycorrector-1.0.4/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1673 2024-04-03 03:01:11.000000 pycorrector-1.0.4/setup.py
```

### Comparing `pycorrector-1.0.3/LICENSE` & `pycorrector-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/PKG-INFO` & `pycorrector-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorrector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chinese Text Error Corrector
 Home-page: https://github.com/shibing624/pycorrector
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Keywords: pycorrector,correction,Chinese error correction,NLP
 Platform: Windows
@@ -35,20 +35,20 @@
 -----------------
 
 # pycorrector: useful python text correction toolkit
 [![PyPI version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/pycorrector)
 [![Downloads](https://static.pepy.tech/badge/pycorrector)](https://pepy.tech/project/pycorrector)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
-[![python_vesion](https://img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt)
+[![python_vesion](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/issues)
-[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 
 
-**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3开发。
+**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3.8开发。
 
 **pycorrector**实现了Kenlm、ConvSeq2Seq、BERT、MacBERT、ELECTRA、ERNIE、Transformer等多种模型的文本纠错，并在SigHAN数据集评估各模型的效果。
 
 **Guide**
 
 - [Features](#Features)
 - [Evaluation](#Evaluation)
@@ -146,20 +146,14 @@
 
 * docker使用
 
 ```shell
 docker run -it -v ~/.pycorrector:/root/.pycorrector shibing624/pycorrector:0.0.2
 ```
 
-后续调用python使用即可，该镜像已经安装好kenlm、pycorrector等包，具体参见[Dockerfile](Dockerfile)。
-
-使用示例：
-
-![docker](https://github.com/shibing624/pycorrector/blob/master/docs/git_image/docker.png)
-
 ## Usage
 本项目的初衷之一是比对、调研各种中文文本纠错方法，抛砖引玉。
 
 项目实现了kenlm、macbert、seq2seq、 ernie_csc、T5、deepcontext、LLaMA等模型应用于文本纠错任务，各模型均可基于已经训练好的纠错模型快速预测，也可使用自有数据训练、预测。
 
 
 ### kenlm模型（统计模型）
@@ -619,9 +613,7 @@
 * [Neural Abstractive Text Summarization with Sequence-to-Sequence Models[Tian Shi, 2018]](https://arxiv.org/abs/1812.02303)
 * [基于深度学习的中文文本自动校对研究与实现[杨宗霖, 2019]](https://github.com/shibing624/pycorrector/blob/master/docs/基于深度学习的中文文本自动校对研究与实现.pdf)
 * [A Sequence to Sequence Learning for Chinese Grammatical Error Correction[Hongkai Ren, 2018]](https://link.springer.com/chapter/10.1007/978-3-319-99501-4_36)
 * [ELECTRA: Pre-training Text Encoders as Discriminators Rather Than Generators](https://openreview.net/pdf?id=r1xMH1BtvB)
 * [Revisiting Pre-trained Models for Chinese Natural Language Processing](https://arxiv.org/abs/2004.13922)
 * Ruiqing Zhang, Chao Pang et al. "Correcting Chinese Spelling Errors with Phonetic Pre-training", ACL, 2021
 * DingminWang et al. "A Hybrid Approach to Automatic Corpus Generation for Chinese Spelling Check", EMNLP, 2018
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycorrector Version: 1.0.3 Summary: Chinese Text
+Metadata-Version: 2.1 Name: pycorrector Version: 1.0.4 Summary: Chinese Text
 Error Corrector Home-page: https://github.com/shibing624/pycorrector Author:
 XuMing Author-email: xuming624@qq.com License: Apache 2.0 Keywords:
 pycorrector,correction,Chinese error correction,NLP Platform: Windows Platform:
 Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified) Classifier: Natural
 Language :: Chinese (Traditional) Classifier: Programming Language :: Python
@@ -18,20 +18,20 @@
 ----------------- # pycorrector: useful python text correction toolkit [![PyPI
 version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/
 pycorrector) [![Downloads](https://static.pepy.tech/badge/pycorrector)](https:/
 /pepy.tech/project/pycorrector) [![GitHub contributors](https://img.shields.io/
 github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/
 pycorrector/graphs/contributors) [![License Apache 2.0](https://img.shields.io/
 badge/license-Apache%202.0-blue.svg)](LICENSE) [![python_vesion](https://
-img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt) [![GitHub
+img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt) [![GitHub
 issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)]
 (https://github.com/shibing624/pycorrector/issues) [![Wechat Group](https://
-img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 **pycorrector**:
-ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3å¼åã
+ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3.8å¼åã
 **pycorrector**å®ç°äºKenlmãConvSeq2SeqãBERTãMacBERTãELECTRAãERNIEãTransformerç­å¤ç§æ¨¡åçææ¬çº éï¼å¹¶å¨SigHANæ°æ®éè¯ä¼°åæ¨¡åçææã
 **Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Usage](#usage)
 - [Dataset](#Dataset) - [Contact](#Contact) - [References](#references) ##
 Introduction ä¸­æææ¬çº éä»»å¡ï¼å¸¸è§éè¯¯ç±»åï¼ [https://
 github.com/shibing624/pycorrector/blob/master/docs/git_image/
 error_type.png]å½ç¶ï¼éå¯¹ä¸åä¸å¡åºæ¯ï¼è¿äºé®é¢å¹¶ä¸ä¸å®å¨é¨å­å¨ï¼æ¯å¦æ¼é³è¾å¥æ³ãè¯­é³è¯å«æ ¡å¯¹å³æ³¨é³ä¼¼éè¯¯ï¼äºç¬è¾å¥æ³ãOCRæ ¡å¯¹å³æ³¨å½¢ä¼¼éè¯¯ï¼
 æç´¢å¼æqueryçº éå³æ³¨ææéè¯¯ç±»åã
@@ -106,18 +106,15 @@
 CSC**ï¼æ¨¡ååç§°æ¯*shibing624/mengzi-t5-base-chinese-
 correction*ï¼huggingface modelï¼https://huggingface.co/shibing624/mengzi-t5-
 base-chinese-correction ## Install ```shell pip install -U pycorrector ``` or
 ```shell pip install -r requirements.txt git clone https://github.com/
 shibing624/pycorrector.git cd pycorrector pip install --no-deps . ```
 éè¿ä»¥ä¸ä¸¤ç§æ¹æ³çä»»ä½ä¸ç§å®æå®è£é½å¯ä»¥ãå¦æä¸æ³å®è£ä¾èµåï¼å¯ä»¥ædockerç¯å¢ã
 * dockerä½¿ç¨ ```shell docker run -it -v ~/.pycorrector:/root/.pycorrector
-shibing624/pycorrector:0.0.2 ```
-åç»­è°ç¨pythonä½¿ç¨å³å¯ï¼è¯¥éåå·²ç»å®è£å¥½kenlmãpycorrectorç­åï¼å·ä½åè§
-[Dockerfile](Dockerfile)ã ä½¿ç¨ç¤ºä¾ï¼ ![docker](https://github.com/
-shibing624/pycorrector/blob/master/docs/git_image/docker.png) ## Usage
+shibing624/pycorrector:0.0.2 ``` ## Usage
 æ¬é¡¹ç®çåè¡·ä¹ä¸æ¯æ¯å¯¹ãè°ç åç§ä¸­æææ¬çº éæ¹æ³ï¼æç å¼çã
 é¡¹ç®å®ç°äºkenlmãmacbertãseq2seqã
 ernie_cscãT5ãdeepcontextãLLaMAç­æ¨¡ååºç¨äºææ¬çº éä»»å¡ï¼åæ¨¡ååå¯åºäºå·²ç»è®­ç»å¥½ççº éæ¨¡åå¿«éé¢æµï¼ä¹å¯ä½¿ç¨èªææ°æ®è®­ç»ãé¢æµã
 ### kenlmæ¨¡åï¼ç»è®¡æ¨¡åï¼ #### ä¸­ææ¼åçº é example: [examples/
 kenlm/demo.py](https://github.com/shibing624/pycorrector/blob/master/examples/
 kenlm/demo.py) ```python from pycorrector import Corrector m = Corrector()
 print(m.correct_batch(['å°åéåå è¯¥ä¸ºèäººè®©å',
```

### Comparing `pycorrector-1.0.3/README.md` & `pycorrector-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 -----------------
 
 # pycorrector: useful python text correction toolkit
 [![PyPI version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/pycorrector)
 [![Downloads](https://static.pepy.tech/badge/pycorrector)](https://pepy.tech/project/pycorrector)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
-[![python_vesion](https://img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt)
+[![python_vesion](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/issues)
-[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 
 
-**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3开发。
+**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3.8开发。
 
 **pycorrector**实现了Kenlm、ConvSeq2Seq、BERT、MacBERT、ELECTRA、ERNIE、Transformer等多种模型的文本纠错，并在SigHAN数据集评估各模型的效果。
 
 **Guide**
 
 - [Features](#Features)
 - [Evaluation](#Evaluation)
@@ -120,20 +120,14 @@
 
 * docker使用
 
 ```shell
 docker run -it -v ~/.pycorrector:/root/.pycorrector shibing624/pycorrector:0.0.2
 ```
 
-后续调用python使用即可，该镜像已经安装好kenlm、pycorrector等包，具体参见[Dockerfile](Dockerfile)。
-
-使用示例：
-
-![docker](https://github.com/shibing624/pycorrector/blob/master/docs/git_image/docker.png)
-
 ## Usage
 本项目的初衷之一是比对、调研各种中文文本纠错方法，抛砖引玉。
 
 项目实现了kenlm、macbert、seq2seq、 ernie_csc、T5、deepcontext、LLaMA等模型应用于文本纠错任务，各模型均可基于已经训练好的纠错模型快速预测，也可使用自有数据训练、预测。
 
 
 ### kenlm模型（统计模型）
```

#### html2text {}

```diff
@@ -6,20 +6,20 @@
 ----------------- # pycorrector: useful python text correction toolkit [![PyPI
 version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/
 pycorrector) [![Downloads](https://static.pepy.tech/badge/pycorrector)](https:/
 /pepy.tech/project/pycorrector) [![GitHub contributors](https://img.shields.io/
 github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/
 pycorrector/graphs/contributors) [![License Apache 2.0](https://img.shields.io/
 badge/license-Apache%202.0-blue.svg)](LICENSE) [![python_vesion](https://
-img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt) [![GitHub
+img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt) [![GitHub
 issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)]
 (https://github.com/shibing624/pycorrector/issues) [![Wechat Group](https://
-img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 **pycorrector**:
-ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3å¼åã
+ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3.8å¼åã
 **pycorrector**å®ç°äºKenlmãConvSeq2SeqãBERTãMacBERTãELECTRAãERNIEãTransformerç­å¤ç§æ¨¡åçææ¬çº éï¼å¹¶å¨SigHANæ°æ®éè¯ä¼°åæ¨¡åçææã
 **Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Usage](#usage)
 - [Dataset](#Dataset) - [Contact](#Contact) - [References](#references) ##
 Introduction ä¸­æææ¬çº éä»»å¡ï¼å¸¸è§éè¯¯ç±»åï¼ [https://
 github.com/shibing624/pycorrector/blob/master/docs/git_image/
 error_type.png]å½ç¶ï¼éå¯¹ä¸åä¸å¡åºæ¯ï¼è¿äºé®é¢å¹¶ä¸ä¸å®å¨é¨å­å¨ï¼æ¯å¦æ¼é³è¾å¥æ³ãè¯­é³è¯å«æ ¡å¯¹å³æ³¨é³ä¼¼éè¯¯ï¼äºç¬è¾å¥æ³ãOCRæ ¡å¯¹å³æ³¨å½¢ä¼¼éè¯¯ï¼
 æç´¢å¼æqueryçº éå³æ³¨ææéè¯¯ç±»åã
@@ -94,18 +94,15 @@
 CSC**ï¼æ¨¡ååç§°æ¯*shibing624/mengzi-t5-base-chinese-
 correction*ï¼huggingface modelï¼https://huggingface.co/shibing624/mengzi-t5-
 base-chinese-correction ## Install ```shell pip install -U pycorrector ``` or
 ```shell pip install -r requirements.txt git clone https://github.com/
 shibing624/pycorrector.git cd pycorrector pip install --no-deps . ```
 éè¿ä»¥ä¸ä¸¤ç§æ¹æ³çä»»ä½ä¸ç§å®æå®è£é½å¯ä»¥ãå¦æä¸æ³å®è£ä¾èµåï¼å¯ä»¥ædockerç¯å¢ã
 * dockerä½¿ç¨ ```shell docker run -it -v ~/.pycorrector:/root/.pycorrector
-shibing624/pycorrector:0.0.2 ```
-åç»­è°ç¨pythonä½¿ç¨å³å¯ï¼è¯¥éåå·²ç»å®è£å¥½kenlmãpycorrectorç­åï¼å·ä½åè§
-[Dockerfile](Dockerfile)ã ä½¿ç¨ç¤ºä¾ï¼ ![docker](https://github.com/
-shibing624/pycorrector/blob/master/docs/git_image/docker.png) ## Usage
+shibing624/pycorrector:0.0.2 ``` ## Usage
 æ¬é¡¹ç®çåè¡·ä¹ä¸æ¯æ¯å¯¹ãè°ç åç§ä¸­æææ¬çº éæ¹æ³ï¼æç å¼çã
 é¡¹ç®å®ç°äºkenlmãmacbertãseq2seqã
 ernie_cscãT5ãdeepcontextãLLaMAç­æ¨¡ååºç¨äºææ¬çº éä»»å¡ï¼åæ¨¡ååå¯åºäºå·²ç»è®­ç»å¥½ççº éæ¨¡åå¿«éé¢æµï¼ä¹å¯ä½¿ç¨èªææ°æ®è®­ç»ãé¢æµã
 ### kenlmæ¨¡åï¼ç»è®¡æ¨¡åï¼ #### ä¸­ææ¼åçº é example: [examples/
 kenlm/demo.py](https://github.com/shibing624/pycorrector/blob/master/examples/
 kenlm/demo.py) ```python from pycorrector import Corrector m = Corrector()
 print(m.correct_batch(['å°åéåå è¯¥ä¸ºèäººè®©å',
```

### Comparing `pycorrector-1.0.3/pycorrector/__init__.py` & `pycorrector-1.0.4/pycorrector/__init__.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/__main__.py` & `pycorrector-1.0.4/pycorrector/__main__.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/confusion_corrector.py` & `pycorrector-1.0.4/pycorrector/confusion_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/corrector.py` & `pycorrector-1.0.4/pycorrector/corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/common_char_set.txt` & `pycorrector-1.0.4/pycorrector/data/common_char_set.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/en.json.gz` & `pycorrector-1.0.4/pycorrector/data/en.json.gz`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/person_name.txt` & `pycorrector-1.0.4/pycorrector/data/person_name.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/place_name.txt` & `pycorrector-1.0.4/pycorrector/data/place_name.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/same_pinyin.txt` & `pycorrector-1.0.4/pycorrector/data/same_pinyin.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/same_stroke.txt` & `pycorrector-1.0.4/pycorrector/data/same_stroke.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/sighan2015_test.tsv` & `pycorrector-1.0.4/pycorrector/data/sighan2015_test.tsv`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/stopwords.txt` & `pycorrector-1.0.4/pycorrector/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/stroke.txt` & `pycorrector-1.0.4/pycorrector/data/stroke.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/data/word_freq.txt` & `pycorrector-1.0.4/pycorrector/data/word_freq.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_corrector.py` & `pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_model.py` & `pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/deepcontext/deepcontext_utils.py` & `pycorrector-1.0.4/pycorrector/deepcontext/deepcontext_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/detector.py` & `pycorrector-1.0.4/pycorrector/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pycorrector.proper_corrector import ProperCorrector
 from pycorrector.utils.get_file import get_file
 from pycorrector.utils.text_utils import uniform, is_alphabet_string, is_chinese_string
 from pycorrector.utils.tokenizer import Tokenizer, split_text_into_sentences_by_symbol
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 # -----用户目录，存储模型文件-----
-USER_DATA_DIR = os.path.expanduser('~/.pycorrector/datasets/')
+USER_DATA_DIR = os.environ.get('PYCORRECTOR_DATA_DIR', os.path.expanduser('~/.pycorrector/datasets'))
 os.makedirs(USER_DATA_DIR, exist_ok=True)
 language_model_path = os.path.join(USER_DATA_DIR, 'zh_giga.no_cna_cmn.prune01244.klm')
 
 # -----词典文件路径-----
 # 通用分词词典文件  format: 词语 词频
 word_freq_path = os.path.join(pwd_path, 'data/word_freq.txt')
 # 五笔笔画字典
```

### Comparing `pycorrector-1.0.3/pycorrector/en_spell_corrector.py` & `pycorrector-1.0.4/pycorrector/en_spell_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/ernie_csc/ernie_csc_corrector.py` & `pycorrector-1.0.4/pycorrector/ernie_csc/ernie_csc_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/ernie_csc/model.py` & `pycorrector-1.0.4/pycorrector/ernie_csc/model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/ernie_csc/predict.py` & `pycorrector-1.0.4/pycorrector/ernie_csc/predict.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/ernie_csc/sighan_evaluate.py` & `pycorrector-1.0.4/pycorrector/ernie_csc/sighan_evaluate.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/ernie_csc/utils.py` & `pycorrector-1.0.4/pycorrector/ernie_csc/utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/gpt/gpt_corrector.py` & `pycorrector-1.0.4/pycorrector/gpt/gpt_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/gpt/gpt_model.py` & `pycorrector-1.0.4/pycorrector/gpt/gpt_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/gpt/gpt_utils.py` & `pycorrector-1.0.4/pycorrector/gpt/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/gpt/merge_peft_adapter.py` & `pycorrector-1.0.4/pycorrector/gpt/merge_peft_adapter.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/base_model.py` & `pycorrector-1.0.4/pycorrector/macbert/base_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/defaults.py` & `pycorrector-1.0.4/pycorrector/macbert/defaults.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/evaluate_util.py` & `pycorrector-1.0.4/pycorrector/macbert/evaluate_util.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/lr_scheduler.py` & `pycorrector-1.0.4/pycorrector/macbert/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/macbert4csc.py` & `pycorrector-1.0.4/pycorrector/macbert/macbert4csc.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/macbert_corrector.py` & `pycorrector-1.0.4/pycorrector/macbert/macbert_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/reader.py` & `pycorrector-1.0.4/pycorrector/macbert/reader.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/macbert/softmaskedbert4csc.py` & `pycorrector-1.0.4/pycorrector/macbert/softmaskedbert4csc.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/proper_corrector.py` & `pycorrector-1.0.4/pycorrector/proper_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_corrector.py` & `pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_model.py` & `pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/seq2seq/conv_seq2seq_utils.py` & `pycorrector-1.0.4/pycorrector/seq2seq/conv_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/t5/t5_corrector.py` & `pycorrector-1.0.4/pycorrector/t5/t5_corrector.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/error_utils.py` & `pycorrector-1.0.4/pycorrector/utils/error_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/evaluate_utils.py` & `pycorrector-1.0.4/pycorrector/utils/evaluate_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/get_file.py` & `pycorrector-1.0.4/pycorrector/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/io_utils.py` & `pycorrector-1.0.4/pycorrector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/langconv.py` & `pycorrector-1.0.4/pycorrector/utils/langconv.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/math_utils.py` & `pycorrector-1.0.4/pycorrector/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/ngram_util.py` & `pycorrector-1.0.4/pycorrector/utils/ngram_util.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/text_utils.py` & `pycorrector-1.0.4/pycorrector/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/tokenizer.py` & `pycorrector-1.0.4/pycorrector/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector/utils/zh_wiki.py` & `pycorrector-1.0.4/pycorrector/utils/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/pycorrector.egg-info/PKG-INFO` & `pycorrector-1.0.4/pycorrector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycorrector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chinese Text Error Corrector
 Home-page: https://github.com/shibing624/pycorrector
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Keywords: pycorrector,correction,Chinese error correction,NLP
 Platform: Windows
@@ -35,20 +35,20 @@
 -----------------
 
 # pycorrector: useful python text correction toolkit
 [![PyPI version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/pycorrector)
 [![Downloads](https://static.pepy.tech/badge/pycorrector)](https://pepy.tech/project/pycorrector)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
-[![python_vesion](https://img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt)
+[![python_vesion](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)](https://github.com/shibing624/pycorrector/issues)
-[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 
 
-**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3开发。
+**pycorrector**: 中文文本纠错工具。支持中文音似、形似、语法错误纠正，python3.8开发。
 
 **pycorrector**实现了Kenlm、ConvSeq2Seq、BERT、MacBERT、ELECTRA、ERNIE、Transformer等多种模型的文本纠错，并在SigHAN数据集评估各模型的效果。
 
 **Guide**
 
 - [Features](#Features)
 - [Evaluation](#Evaluation)
@@ -146,20 +146,14 @@
 
 * docker使用
 
 ```shell
 docker run -it -v ~/.pycorrector:/root/.pycorrector shibing624/pycorrector:0.0.2
 ```
 
-后续调用python使用即可，该镜像已经安装好kenlm、pycorrector等包，具体参见[Dockerfile](Dockerfile)。
-
-使用示例：
-
-![docker](https://github.com/shibing624/pycorrector/blob/master/docs/git_image/docker.png)
-
 ## Usage
 本项目的初衷之一是比对、调研各种中文文本纠错方法，抛砖引玉。
 
 项目实现了kenlm、macbert、seq2seq、 ernie_csc、T5、deepcontext、LLaMA等模型应用于文本纠错任务，各模型均可基于已经训练好的纠错模型快速预测，也可使用自有数据训练、预测。
 
 
 ### kenlm模型（统计模型）
@@ -619,9 +613,7 @@
 * [Neural Abstractive Text Summarization with Sequence-to-Sequence Models[Tian Shi, 2018]](https://arxiv.org/abs/1812.02303)
 * [基于深度学习的中文文本自动校对研究与实现[杨宗霖, 2019]](https://github.com/shibing624/pycorrector/blob/master/docs/基于深度学习的中文文本自动校对研究与实现.pdf)
 * [A Sequence to Sequence Learning for Chinese Grammatical Error Correction[Hongkai Ren, 2018]](https://link.springer.com/chapter/10.1007/978-3-319-99501-4_36)
 * [ELECTRA: Pre-training Text Encoders as Discriminators Rather Than Generators](https://openreview.net/pdf?id=r1xMH1BtvB)
 * [Revisiting Pre-trained Models for Chinese Natural Language Processing](https://arxiv.org/abs/2004.13922)
 * Ruiqing Zhang, Chao Pang et al. "Correcting Chinese Spelling Errors with Phonetic Pre-training", ACL, 2021
 * DingminWang et al. "A Hybrid Approach to Automatic Corpus Generation for Chinese Spelling Check", EMNLP, 2018
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycorrector Version: 1.0.3 Summary: Chinese Text
+Metadata-Version: 2.1 Name: pycorrector Version: 1.0.4 Summary: Chinese Text
 Error Corrector Home-page: https://github.com/shibing624/pycorrector Author:
 XuMing Author-email: xuming624@qq.com License: Apache 2.0 Keywords:
 pycorrector,correction,Chinese error correction,NLP Platform: Windows Platform:
 Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified) Classifier: Natural
 Language :: Chinese (Traditional) Classifier: Programming Language :: Python
@@ -18,20 +18,20 @@
 ----------------- # pycorrector: useful python text correction toolkit [![PyPI
 version](https://badge.fury.io/py/pycorrector.svg)](https://badge.fury.io/py/
 pycorrector) [![Downloads](https://static.pepy.tech/badge/pycorrector)](https:/
 /pepy.tech/project/pycorrector) [![GitHub contributors](https://img.shields.io/
 github/contributors/shibing624/pycorrector.svg)](https://github.com/shibing624/
 pycorrector/graphs/contributors) [![License Apache 2.0](https://img.shields.io/
 badge/license-Apache%202.0-blue.svg)](LICENSE) [![python_vesion](https://
-img.shields.io/badge/Python-3.6%2B-green.svg)](requirements.txt) [![GitHub
+img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt) [![GitHub
 issues](https://img.shields.io/github/issues/shibing624/pycorrector.svg)]
 (https://github.com/shibing624/pycorrector/issues) [![Wechat Group](https://
-img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#wechat-group)
+img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 **pycorrector**:
-ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3å¼åã
+ä¸­æææ¬çº éå·¥å·ãæ¯æä¸­æé³ä¼¼ãå½¢ä¼¼ãè¯­æ³éè¯¯çº æ­£ï¼python3.8å¼åã
 **pycorrector**å®ç°äºKenlmãConvSeq2SeqãBERTãMacBERTãELECTRAãERNIEãTransformerç­å¤ç§æ¨¡åçææ¬çº éï¼å¹¶å¨SigHANæ°æ®éè¯ä¼°åæ¨¡åçææã
 **Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Usage](#usage)
 - [Dataset](#Dataset) - [Contact](#Contact) - [References](#references) ##
 Introduction ä¸­æææ¬çº éä»»å¡ï¼å¸¸è§éè¯¯ç±»åï¼ [https://
 github.com/shibing624/pycorrector/blob/master/docs/git_image/
 error_type.png]å½ç¶ï¼éå¯¹ä¸åä¸å¡åºæ¯ï¼è¿äºé®é¢å¹¶ä¸ä¸å®å¨é¨å­å¨ï¼æ¯å¦æ¼é³è¾å¥æ³ãè¯­é³è¯å«æ ¡å¯¹å³æ³¨é³ä¼¼éè¯¯ï¼äºç¬è¾å¥æ³ãOCRæ ¡å¯¹å³æ³¨å½¢ä¼¼éè¯¯ï¼
 æç´¢å¼æqueryçº éå³æ³¨ææéè¯¯ç±»åã
@@ -106,18 +106,15 @@
 CSC**ï¼æ¨¡ååç§°æ¯*shibing624/mengzi-t5-base-chinese-
 correction*ï¼huggingface modelï¼https://huggingface.co/shibing624/mengzi-t5-
 base-chinese-correction ## Install ```shell pip install -U pycorrector ``` or
 ```shell pip install -r requirements.txt git clone https://github.com/
 shibing624/pycorrector.git cd pycorrector pip install --no-deps . ```
 éè¿ä»¥ä¸ä¸¤ç§æ¹æ³çä»»ä½ä¸ç§å®æå®è£é½å¯ä»¥ãå¦æä¸æ³å®è£ä¾èµåï¼å¯ä»¥ædockerç¯å¢ã
 * dockerä½¿ç¨ ```shell docker run -it -v ~/.pycorrector:/root/.pycorrector
-shibing624/pycorrector:0.0.2 ```
-åç»­è°ç¨pythonä½¿ç¨å³å¯ï¼è¯¥éåå·²ç»å®è£å¥½kenlmãpycorrectorç­åï¼å·ä½åè§
-[Dockerfile](Dockerfile)ã ä½¿ç¨ç¤ºä¾ï¼ ![docker](https://github.com/
-shibing624/pycorrector/blob/master/docs/git_image/docker.png) ## Usage
+shibing624/pycorrector:0.0.2 ``` ## Usage
 æ¬é¡¹ç®çåè¡·ä¹ä¸æ¯æ¯å¯¹ãè°ç åç§ä¸­æææ¬çº éæ¹æ³ï¼æç å¼çã
 é¡¹ç®å®ç°äºkenlmãmacbertãseq2seqã
 ernie_cscãT5ãdeepcontextãLLaMAç­æ¨¡ååºç¨äºææ¬çº éä»»å¡ï¼åæ¨¡ååå¯åºäºå·²ç»è®­ç»å¥½ççº éæ¨¡åå¿«éé¢æµï¼ä¹å¯ä½¿ç¨èªææ°æ®è®­ç»ãé¢æµã
 ### kenlmæ¨¡åï¼ç»è®¡æ¨¡åï¼ #### ä¸­ææ¼åçº é example: [examples/
 kenlm/demo.py](https://github.com/shibing624/pycorrector/blob/master/examples/
 kenlm/demo.py) ```python from pycorrector import Corrector m = Corrector()
 print(m.correct_batch(['å°åéåå è¯¥ä¸ºèäººè®©å',
```

### Comparing `pycorrector-1.0.3/pycorrector.egg-info/SOURCES.txt` & `pycorrector-1.0.4/pycorrector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycorrector-1.0.3/setup.py` & `pycorrector-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,18 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     platforms=["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
     keywords='pycorrector,correction,Chinese error correction,NLP',
     install_requires=[
         "jieba",
         "pypinyin",
+        "transformers",
+        "datasets",
         "numpy",
+        "pandas",
         "six",
         "loguru",
     ],
     packages=find_packages(exclude=['tests']),
     package_dir={'pycorrector': 'pycorrector'},
     package_data={'pycorrector': ['*.*', 'data/*', 'data/en.json.gz', 'data/sighan2015_test.tsv']}
 )
```

