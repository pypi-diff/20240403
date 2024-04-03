# Comparing `tmp/dinopy-2.2.1.tar.gz` & `tmp/dinopy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinopy-2.2.1.tar", last modified: Sun Mar 27 17:37:37 2022, max compression
+gzip compressed data, was "dinopy-3.0.0.tar", last modified: Wed Apr  3 11:42:13 2024, max compression
```

## Comparing `dinopy-2.2.1.tar` & `dinopy-3.0.0.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.991814 dinopy-2.2.1/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      135 2020-12-23 12:06:10.000000 dinopy-2.2.1/.gitignore
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      438 2020-12-23 12:06:10.000000 dinopy-2.2.1/AUTHORS.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     8289 2022-03-27 17:33:59.000000 dinopy-2.2.1/CHANGELOG.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1079 2020-12-23 12:06:10.000000 dinopy-2.2.1/LICENSE.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       48 2020-12-23 12:06:10.000000 dinopy-2.2.1/MANIFEST.in
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     5385 2022-03-27 17:37:37.991814 dinopy-2.2.1/PKG-INFO
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4121 2022-03-22 08:11:07.000000 dinopy-2.2.1/README.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      294 2022-03-27 17:22:30.000000 dinopy-2.2.1/bitbucket-pipelines.yml
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.967814 dinopy-2.2.1/dinopy/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      493 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/__init__.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1177 2022-03-27 17:22:30.000000 dinopy-2.2.1/dinopy/__init__.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      167 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/auxiliary.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2146 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/auxiliary.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2244 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/conversion.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    28944 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/conversion.pyx
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.967814 dinopy-2.2.1/dinopy/cpp/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4313 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/cpp/sais.cpp
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      826 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/creader.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     9093 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/creader.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     3968 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/definitions.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    28630 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/definitions.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1703 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/exceptions.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     8998 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fai_io.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      463 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fasta_reader.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    26663 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fasta_reader.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1371 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fasta_writer.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    19843 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fasta_writer.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      588 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fastq_reader.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    18275 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fastq_reader.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      623 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fastq_writer.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     9662 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/fastq_writer.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      273 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/input_opener.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4400 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/input_opener.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1767 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/nameline_parser.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    17829 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/nameline_parser.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      456 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/output_opener.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     7062 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/output_opener.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      923 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/processors.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    35583 2022-03-27 17:22:30.000000 dinopy-2.2.1/dinopy/processors.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      510 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sam_reader.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     7863 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sam_reader.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      510 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sam_writer.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     7432 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sam_writer.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1825 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sambam.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    23624 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/sambam.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      624 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/shape.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     9542 2022-03-27 17:22:30.000000 dinopy-2.2.1/dinopy/shape.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      583 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/shaping.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    15503 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/shaping.pyx
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       38 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/wrap_sais.pxd
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      780 2020-12-23 12:06:10.000000 dinopy-2.2.1/dinopy/wrap_sais.pyx
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.967814 dinopy-2.2.1/dinopy.egg-info/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     5385 2022-03-27 17:37:37.000000 dinopy-2.2.1/dinopy.egg-info/PKG-INFO
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     3978 2022-03-27 17:37:37.000000 dinopy-2.2.1/dinopy.egg-info/SOURCES.txt
--rw-rw-r--   0 m00am     (1000) m00am     (1000)        1 2022-03-27 17:37:37.000000 dinopy-2.2.1/dinopy.egg-info/dependency_links.txt
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       25 2022-03-27 17:37:37.000000 dinopy-2.2.1/dinopy.egg-info/requires.txt
--rw-rw-r--   0 m00am     (1000) m00am     (1000)        7 2022-03-27 17:37:37.000000 dinopy-2.2.1/dinopy.egg-info/top_level.txt
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.967814 dinopy-2.2.1/docs/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     6774 2022-03-27 17:22:30.000000 dinopy-2.2.1/docs/Makefile
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     6710 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/make.bat
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       37 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/requirements.txt
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.967814 dinopy-2.2.1/docs/source/
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.971814 dinopy-2.2.1/docs/source/_static/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/_static/hide.css
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.975814 dinopy-2.2.1/docs/source/autodoc/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      116 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/auxiliary.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      149 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/conversion.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      137 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/creader.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      251 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/definitions.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      310 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/dinopy.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      129 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/exceptions.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      133 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/fai_io.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/fasta_reader.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/fasta_writer.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/fastq_reader.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/fastq_writer.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/input_opener.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       55 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/modules.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      134 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/nameline_parser.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      149 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/processors.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      119 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/sam_reader.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      119 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/sam_writer.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      107 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/sambam.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      123 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/shape.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      133 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/autodoc/shaping.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       49 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/changelog.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     8846 2022-03-27 17:22:30.000000 dinopy-2.2.1/docs/source/conf.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1770 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/cython_integration.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2601 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/encoding.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    10000 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/faq.rst
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.975814 dinopy-2.2.1/docs/source/getting-started/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     3996 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/getting-started/examples.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4314 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/getting-started/first-steps.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      167 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/getting-started/index.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4259 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/getting-started/introduction.rst
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/hide.css
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      255 2020-12-23 12:06:10.000000 dinopy-2.2.1/docs/source/index.rst
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.983814 dinopy-2.2.1/files/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       26 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/broken.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)        0 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/empty.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      371 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/example.sam
--rw-rw-r--   0 m00am     (1000) m00am     (1000)   607756 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/phix.small.fastq.gz
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      439 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome.fasta.fai
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       87 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome.fasta.gz
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      241 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_IUPAC.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      439 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_no_fai.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      433 2022-03-22 10:22:35.000000 dinopy-2.2.1/files/testgenome_verify.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2022-03-22 10:22:35.000000 dinopy-2.2.1/files/testgenome_verify.fasta.fai
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      433 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_verify2.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_verify2.fasta.fai
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      442 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_verify2_win.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_verify2_win.fasta.fai
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      454 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_win.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       85 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testgenome_win.fasta.fai
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      219 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      110 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads.fastq.gz
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      101 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_big.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      226 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_double_name.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      221 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_double_plus.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      236 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_double_qvs.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      236 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_double_seq.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      220 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_empty_line.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      212 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_missing_name.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      217 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_missing_plus.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      202 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_missing_qvs.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      202 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_missing_seq.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       97 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_error_npc.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       95 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_illumina_1.3.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       89 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_illumina_1.5.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       97 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_illumina_1.8.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    40219 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_long.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       95 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_sanger.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      105 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/testreads_solexa.fastq
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       42 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/tiny_testgenome_1chr.fasta
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/tiny_testgenome_1chr.fasta.gz
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       65 2020-12-23 12:06:10.000000 dinopy-2.2.1/files/tiny_testgenome_2chr_nrseq.fasta.fai
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.983814 dinopy-2.2.1/images/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)   175768 2020-12-23 12:06:10.000000 dinopy-2.2.1/images/dinopy_overview.svg
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       53 2022-03-27 17:22:30.000000 dinopy-2.2.1/nose2.cfg
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      171 2022-03-27 17:22:30.000000 dinopy-2.2.1/pyproject.toml
--rw-rw-r--   0 m00am     (1000) m00am     (1000)       38 2022-03-27 17:37:37.991814 dinopy-2.2.1/setup.cfg
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2631 2022-03-27 17:22:30.000000 dinopy-2.2.1/setup.py
-drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2022-03-27 17:37:37.991814 dinopy-2.2.1/test/
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1624 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/aux_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    23124 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/conversion_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2818 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/creader_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     5952 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fai_io_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    25187 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fasta_reader_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1203 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fasta_sources.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    27103 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fasta_writer_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    96405 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fastq_reader_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    13550 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/fastq_writer_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     1939 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/init_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     2046 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/input_opener_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     3372 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/output_opener_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)    33198 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/processors_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4052 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/read_write_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     4136 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/sam_reader_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     8708 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/sam_writer_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)     8623 2020-12-23 12:06:10.000000 dinopy-2.2.1/test/shaping_test.py
--rw-rw-r--   0 m00am     (1000) m00am     (1000)      221 2022-03-27 17:22:30.000000 dinopy-2.2.1/tox.ini
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.893251 dinopy-3.0.0/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      135 2020-12-23 12:06:10.000000 dinopy-3.0.0/.gitignore
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      438 2020-12-23 12:06:10.000000 dinopy-3.0.0/AUTHORS.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8660 2024-04-02 20:03:01.000000 dinopy-3.0.0/CHANGELOG.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1079 2020-12-23 12:06:10.000000 dinopy-3.0.0/LICENSE.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       48 2020-12-23 12:06:10.000000 dinopy-3.0.0/MANIFEST.in
+-rw-r--r--   0 m00am     (1000) m00am     (1000)     5386 2024-04-03 11:42:13.893251 dinopy-3.0.0/PKG-INFO
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4134 2024-04-02 20:44:20.000000 dinopy-3.0.0/README.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      302 2024-04-02 20:03:01.000000 dinopy-3.0.0/bitbucket-pipelines.yml
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.885251 dinopy-3.0.0/dinopy/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      493 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/__init__.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1177 2024-04-02 21:01:08.000000 dinopy-3.0.0/dinopy/__init__.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      167 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/auxiliary.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2146 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/auxiliary.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2244 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/conversion.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    28944 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/conversion.pyx
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.885251 dinopy-3.0.0/dinopy/cpp/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4313 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/cpp/sais.cpp
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      826 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/creader.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9080 2024-04-02 20:03:01.000000 dinopy-3.0.0/dinopy/creader.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3967 2024-03-23 20:06:52.000000 dinopy-3.0.0/dinopy/definitions.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    28629 2024-03-23 20:06:52.000000 dinopy-3.0.0/dinopy/definitions.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1703 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/exceptions.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8998 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fai_io.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      463 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fasta_reader.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    26663 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fasta_reader.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1371 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fasta_writer.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    19843 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fasta_writer.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      588 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fastq_reader.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    18275 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fastq_reader.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      623 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fastq_writer.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9662 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/fastq_writer.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      273 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/input_opener.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4400 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/input_opener.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1767 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/nameline_parser.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    17829 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/nameline_parser.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      456 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/output_opener.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     7062 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/output_opener.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      923 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/processors.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    35583 2022-03-27 17:22:30.000000 dinopy-3.0.0/dinopy/processors.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      510 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/sam_reader.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     7860 2024-04-02 20:03:01.000000 dinopy-3.0.0/dinopy/sam_reader.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      510 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/sam_writer.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     7432 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/sam_writer.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1825 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/sambam.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    23621 2024-04-02 20:03:01.000000 dinopy-3.0.0/dinopy/sambam.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      624 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/shape.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9533 2024-03-23 20:06:52.000000 dinopy-3.0.0/dinopy/shape.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      583 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/shaping.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    15503 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/shaping.pyx
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       38 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/wrap_sais.pxd
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      780 2020-12-23 12:06:10.000000 dinopy-3.0.0/dinopy/wrap_sais.pyx
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.893251 dinopy-3.0.0/dinopy.egg-info/
+-rw-r--r--   0 m00am     (1000) m00am     (1000)     5386 2024-04-03 11:42:13.000000 dinopy-3.0.0/dinopy.egg-info/PKG-INFO
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3978 2024-04-03 11:42:13.000000 dinopy-3.0.0/dinopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        1 2024-04-03 11:42:13.000000 dinopy-3.0.0/dinopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       26 2024-04-03 11:42:13.000000 dinopy-3.0.0/dinopy.egg-info/requires.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        7 2024-04-03 11:42:13.000000 dinopy-3.0.0/dinopy.egg-info/top_level.txt
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.885251 dinopy-3.0.0/docs/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     6774 2022-03-27 17:22:30.000000 dinopy-3.0.0/docs/Makefile
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     6710 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/make.bat
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       55 2024-04-02 20:32:35.000000 dinopy-3.0.0/docs/requirements.txt
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.885251 dinopy-3.0.0/docs/source/
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.885251 dinopy-3.0.0/docs/source/_static/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/_static/hide.css
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.889251 dinopy-3.0.0/docs/source/autodoc/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      116 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/auxiliary.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      149 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/conversion.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      137 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/creader.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      251 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/definitions.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      310 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/dinopy.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      129 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/exceptions.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      133 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/fai_io.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/fasta_reader.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/fasta_writer.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/fastq_reader.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/fastq_writer.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      157 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/input_opener.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       55 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/modules.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      134 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/nameline_parser.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      149 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/processors.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      119 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/sam_reader.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      119 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/sam_writer.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      107 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/sambam.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      123 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/shape.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      133 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/autodoc/shaping.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       49 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/changelog.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8914 2024-04-02 20:37:02.000000 dinopy-3.0.0/docs/source/conf.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1770 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/cython_integration.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2601 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/encoding.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    10000 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/faq.rst
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.889251 dinopy-3.0.0/docs/source/getting-started/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3996 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/getting-started/examples.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4314 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/getting-started/first-steps.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      167 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/getting-started/index.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4259 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/getting-started/introduction.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/hide.css
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      255 2020-12-23 12:06:10.000000 dinopy-3.0.0/docs/source/index.rst
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.889251 dinopy-3.0.0/files/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       26 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/broken.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        0 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/empty.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      371 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/example.sam
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   607756 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/phix.small.fastq.gz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      439 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome.fasta.fai
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       87 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome.fasta.gz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      241 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_IUPAC.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      439 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_no_fai.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      433 2024-03-23 20:56:33.000000 dinopy-3.0.0/files/testgenome_verify.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2024-03-23 20:56:33.000000 dinopy-3.0.0/files/testgenome_verify.fasta.fai
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      433 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_verify2.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_verify2.fasta.fai
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      442 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_verify2_win.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_verify2_win.fasta.fai
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      454 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_win.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       85 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testgenome_win.fasta.fai
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      219 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      110 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads.fastq.gz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      101 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_big.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      226 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_double_name.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      221 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_double_plus.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      236 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_double_qvs.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      236 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_double_seq.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      220 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_empty_line.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      212 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_missing_name.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      217 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_missing_plus.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      202 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_missing_qvs.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      202 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_missing_seq.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       97 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_error_npc.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       95 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_illumina_1.3.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       89 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_illumina_1.5.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       97 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_illumina_1.8.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    40219 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_long.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       95 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_sanger.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      105 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/testreads_solexa.fastq
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       42 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/tiny_testgenome_1chr.fasta
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       76 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/tiny_testgenome_1chr.fasta.gz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       65 2020-12-23 12:06:10.000000 dinopy-3.0.0/files/tiny_testgenome_2chr_nrseq.fasta.fai
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.889251 dinopy-3.0.0/images/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   175768 2020-12-23 12:06:10.000000 dinopy-3.0.0/images/dinopy_overview.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       53 2022-03-27 17:22:30.000000 dinopy-3.0.0/nose2.cfg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      172 2024-04-02 20:03:01.000000 dinopy-3.0.0/pyproject.toml
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       38 2024-04-03 11:42:13.893251 dinopy-3.0.0/setup.cfg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2585 2024-04-03 11:41:54.000000 dinopy-3.0.0/setup.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-03 11:42:13.893251 dinopy-3.0.0/test/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1624 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/aux_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    23124 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/conversion_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2818 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/creader_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     5952 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fai_io_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    25187 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fasta_reader_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1203 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fasta_sources.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    27103 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fasta_writer_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    96405 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fastq_reader_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    13550 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/fastq_writer_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1939 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/init_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2046 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/input_opener_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3372 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/output_opener_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    33198 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/processors_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4052 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/read_write_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4136 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/sam_reader_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8708 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/sam_writer_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8623 2020-12-23 12:06:10.000000 dinopy-3.0.0/test/shaping_test.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      234 2024-04-02 20:03:01.000000 dinopy-3.0.0/tox.ini
```

### Comparing `dinopy-2.2.1/CHANGELOG.rst` & `dinopy-3.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+Version 3.0.0 (2024-04-03)
+--------------------------
+
+- Added Cython 3 compatibility. Thanks to @galaxy001 for the contribution!
+  Since this means dinopy is no longer compatible with Cython 2, this 
+  requires a major version change.
+- Deprecated compatibility for Python 3.5 to 3.7.
+- Added compatibility with Python 3.11 and 3.12.
+- Added readthedocs config file.
+
+
+
 Version 2.2.1 (2022-03-22)
 --------------------------
 
 - Added ``pyproject.toml`` to correctly handle build dependencies
   (see `Issue #11 <https://bitbucket.org/HenningTimm/dinopy/issues/11>`__).
   Thanks to Sanjay Kumar Srikakulam for the input!
 - Added compatibility with Python 3.10
```

### Comparing `dinopy-2.2.1/LICENSE.rst` & `dinopy-3.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/PKG-INFO` & `dinopy-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dinopy
-Version: 2.2.1
+Version: 3.0.0
 Summary: DNA input and output library for Python and Cython. Includes reader and writer for FASTA and FASTQ files, support for samtools faidx files, and generators for solid and gapped q-grams (k-mers).
 Home-page: https://bitbucket.org/HenningTimm/dinopy
 Author: Henning Timm, Till Hartmann
 Author-email: henning.timm@tu-dortmund.de, till.hartmann@tu-dortmund.de
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
+Requires-Dist: numpy>=1.17
+Requires-Dist: Cython>=3.0.0
 
 .. image:: https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat
    :target: https://bioconda.github.io/recipes/dinopy/README.html
 
 .. image:: https://img.shields.io/pypi/v/dinopy.svg?style=flat
    :target: https://pypi.python.org/pypi/dinopy
 
@@ -63,30 +63,30 @@
 
 Features
 ~~~~~~~~
 
 -  Easy to use reader and writer for FASTA-, FASTQ-, and SAM-files.
 -  Specifiable data type and representation for return values (bytes,
    bytearrays, strings and integers see
-   `dtype <https://dinopy.readthedocs.org/en/latest/encoding/>`__ for
+   `dtype <https://dinopy.readthedocs.org/en/latest/encoding.html>`__ for
    more information).
 -  Implemented in `Cython <http://cython.org/>`__ for additional speedup.
--  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration/>`__ to avoid introducing Python code into Cython projects.
+-  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration.html>`__ to avoid introducing Python code into Cython projects.
 -  Works directly on gzipped files.
 -  Iterators for q-grams of a sequence (also allowing shaped q-grams).
 -  (Reverse) complement.
 -  Chromosome selection from FASTA files.
 
 
 Getting Started
 ~~~~~~~~~~~~~~~
 
 -  If you are new to dinopy you can get started by following the
    first-steps
-   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction/>`__.
+   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction.html>`__.
 -  A full list of features, as well as the documentation, can be found
    `here <https://dinopy.readthedocs.org/en/latest/>`__.
 
 Installation
 ~~~~~~~~~~~~
 
 Dinopy can be installed with pip:
@@ -125,17 +125,17 @@
        $ python
 
        >>> import dinopy
 
 Installation requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
--  `python <https://www.python.org/>`__ >= 3.5
+-  `python <https://www.python.org/>`__ >= 3.8
 -  `numpy <http://www.numpy.org/>`__ >= 1.17
--  `cython <http://cython.org/>`__ >= 0.22
+-  `cython <http://cython.org/>`__ >= 3.0.0
 -  C and C++ compilers, for example from ``build-essentials`` (Linux) or ``Xcode`` (OSX)
 
 We recommend using
 `anaconda <https://www.continuum.io/downloads>`__
 and the
 `bioconda channel <https://github.com/bioconda/bioconda-recipes>`__.
 
@@ -169,9 +169,7 @@
 
 
 License
 ~~~~~~~
 
 Dinopy is Open Source and licensed under the `MIT
 License <http://opensource.org/licenses/MIT>`__.
-
-
```

### Comparing `dinopy-2.2.1/README.rst` & `dinopy-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,30 @@
 
 Features
 ~~~~~~~~
 
 -  Easy to use reader and writer for FASTA-, FASTQ-, and SAM-files.
 -  Specifiable data type and representation for return values (bytes,
    bytearrays, strings and integers see
-   `dtype <https://dinopy.readthedocs.org/en/latest/encoding/>`__ for
+   `dtype <https://dinopy.readthedocs.org/en/latest/encoding.html>`__ for
    more information).
 -  Implemented in `Cython <http://cython.org/>`__ for additional speedup.
--  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration/>`__ to avoid introducing Python code into Cython projects.
+-  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration.html>`__ to avoid introducing Python code into Cython projects.
 -  Works directly on gzipped files.
 -  Iterators for q-grams of a sequence (also allowing shaped q-grams).
 -  (Reverse) complement.
 -  Chromosome selection from FASTA files.
 
 
 Getting Started
 ~~~~~~~~~~~~~~~
 
 -  If you are new to dinopy you can get started by following the
    first-steps
-   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction/>`__.
+   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction.html>`__.
 -  A full list of features, as well as the documentation, can be found
    `here <https://dinopy.readthedocs.org/en/latest/>`__.
 
 Installation
 ~~~~~~~~~~~~
 
 Dinopy can be installed with pip:
@@ -98,17 +98,17 @@
        $ python
 
        >>> import dinopy
 
 Installation requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
--  `python <https://www.python.org/>`__ >= 3.5
+-  `python <https://www.python.org/>`__ >= 3.8
 -  `numpy <http://www.numpy.org/>`__ >= 1.17
--  `cython <http://cython.org/>`__ >= 0.22
+-  `cython <http://cython.org/>`__ >= 3.0.0
 -  C and C++ compilers, for example from ``build-essentials`` (Linux) or ``Xcode`` (OSX)
 
 We recommend using
 `anaconda <https://www.continuum.io/downloads>`__
 and the
 `bioconda channel <https://github.com/bioconda/bioconda-recipes>`__.
```

### Comparing `dinopy-2.2.1/dinopy/__init__.py` & `dinopy-3.0.0/dinopy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 For documentation please visit https://dinopy.readthedocs.org or use the 
 python help-function.
 You can also build the help files yourself after checking out the code
 from https://bitbucket.org/HenningTimm/dinopy .
 """
 
-__version__ = '2.2.1'
+__version__ = '3.0.0'
 
 __all__ = ['fasta_reader', 'fasta_writer', 'fastq_reader', 'fastq_writer', 'auxiliary', 'shaping', 'shape',
            'processors', 'definitions', 'exceptions', 'output_opener', 'nameline_parser', 'sam_reader', 'sam_writer',
            'sambam']
 from .output_opener import OutputOpener
 from .fastq_reader import FastqReader
 from .fasta_reader import FastaReader
```

### Comparing `dinopy-2.2.1/dinopy/auxiliary.pyx` & `dinopy-3.0.0/dinopy/auxiliary.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/conversion.pxd` & `dinopy-3.0.0/dinopy/conversion.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/conversion.pyx` & `dinopy-3.0.0/dinopy/conversion.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/cpp/sais.cpp` & `dinopy-3.0.0/dinopy/cpp/sais.cpp`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/creader.pxd` & `dinopy-3.0.0/dinopy/creader.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/creader.pyx` & `dinopy-3.0.0/dinopy/creader.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -277,9 +277,9 @@
         cdef char *line = NULL
         cdef size_t l = 0
         cdef ssize_t read
 
         while True:
             read = getline(&line, &l, self.cfile)
             if read == -1:
-                raise StopIteration
+                return
             yield line
```

### Comparing `dinopy-2.2.1/dinopy/definitions.pxd` & `dinopy-3.0.0/dinopy/definitions.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     dict linetype_as_str
 
 cdef set valid_dtypes
 
 cdef class IUPACRandomReplacementDict(dict):
     cdef dict __dict__
 
-cpdef IUPACRandomReplacementDict _2bit_from_any_with_iupac_replacement
+cdef IUPACRandomReplacementDict _2bit_from_any_with_iupac_replacement
 
 # Dummy classes to specify data types of sequences
 cdef class basenumbers(object):
     """Basenumbers type for dtype parameters.
 
     - A → 0
     - C → 1
```

### Comparing `dinopy-2.2.1/dinopy/definitions.pyx` & `dinopy-3.0.0/dinopy/definitions.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1176,15 +1176,15 @@
 
     def __iter__(self):
         return chain(iter(self.__dict__), iter(_iupac_mapping))
 
     def __call__(self):
         return self.__dict__
 
-cpdef IUPACRandomReplacementDict _2bit_from_any_with_iupac_replacement = IUPACRandomReplacementDict()
+cdef IUPACRandomReplacementDict _2bit_from_any_with_iupac_replacement = IUPACRandomReplacementDict()
 
 
 class two_bit(bit_base):
     """Two bit encoding **type** for encoding parameters.
     For convenience, `two_bit` behaves a lot like `int` in that it can either be used as a type
     (for example in `dinopy.processors.qgrams`, see `dtype` for more information),
     or used as a conversion function (as in ``two_bit("ACGT") == 0b00011011``) [#]_ .
```

### Comparing `dinopy-2.2.1/dinopy/exceptions.py` & `dinopy-3.0.0/dinopy/exceptions.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fai_io.py` & `dinopy-3.0.0/dinopy/fai_io.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fasta_reader.pyx` & `dinopy-3.0.0/dinopy/fasta_reader.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fasta_writer.pxd` & `dinopy-3.0.0/dinopy/fasta_writer.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fasta_writer.pyx` & `dinopy-3.0.0/dinopy/fasta_writer.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fastq_reader.pxd` & `dinopy-3.0.0/dinopy/fastq_reader.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fastq_reader.pyx` & `dinopy-3.0.0/dinopy/fastq_reader.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fastq_writer.pxd` & `dinopy-3.0.0/dinopy/fastq_writer.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/fastq_writer.pyx` & `dinopy-3.0.0/dinopy/fastq_writer.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/input_opener.pyx` & `dinopy-3.0.0/dinopy/input_opener.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/nameline_parser.pxd` & `dinopy-3.0.0/dinopy/nameline_parser.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/nameline_parser.pyx` & `dinopy-3.0.0/dinopy/nameline_parser.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/output_opener.pyx` & `dinopy-3.0.0/dinopy/output_opener.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/processors.pxd` & `dinopy-3.0.0/dinopy/processors.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/processors.pyx` & `dinopy-3.0.0/dinopy/processors.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/sam_reader.pyx` & `dinopy-3.0.0/dinopy/sam_reader.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 # s: int16_t
                 # S: uint16_t
                 # i: int32_t
                 # I: uint32_t
                 # f: float
                 num_values = ovalue.count(',') + 1
                 value_type = {'c': np.int8, 'C': np.uint8, 's': np.int16, 'S': np.uint16, 'i': np.int32, 'I': np.uint32,
-                              'f': np.float}
+                              'f': float}
                 type_char = ovalue[0]
                 arr = np.empty(num_values, dtype=value_type[type_char])  # TODO: numpy.ndarray or python list?
                 if num_values > 1:
                     str_values = ovalue[1:].split(',')
                 else:
                     str_values = ovalue[1:]
```

### Comparing `dinopy-2.2.1/dinopy/sam_writer.pyx` & `dinopy-3.0.0/dinopy/sam_writer.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/sambam.pxd` & `dinopy-3.0.0/dinopy/sambam.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/sambam.pyx` & `dinopy-3.0.0/dinopy/sambam.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             else:
                 raw_opt_list.append("{}:{}:{}".format(key, type_char_lookup[t], value))
         else:  # H, Byte array in the Hex format; B, Integer or numeric array  --  not yet supported
             if t in (bytes, bytearray):
                 raw_opt_list.append("{}:H:{}".format(key, hexlify(value).decode('ascii')))
             elif t in (list, np.ndarray):
                 type_value = {np.uint16: 'S', np.int16: 's', np.uint32: 'I', np.int32: 'i', np.uint8: 'C',
-                              np.float: 'f', np.int8: 'c', int: 'i', float: 'f'}
+                              float: 'f', np.int8: 'c', int: 'i', float: 'f'}
                 raw_opt_list.append("{}:B:{}{}".format(key, type_value[type(value[0])], ','.join(map(str, value))))
             else:
                 raise TypeError("Unsupported type {} for value {}".format(type(value), value))
     return "\t".join(raw_opt_list).rstrip()
 
 cpdef int create_flag(bint template_having_multiple_segments_in_sequencing=False,
                       bint each_segment_properly_aligned=False,
```

### Comparing `dinopy-2.2.1/dinopy/shape.pxd` & `dinopy-3.0.0/dinopy/shape.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/shape.pyx` & `dinopy-3.0.0/dinopy/shape.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -126,23 +126,23 @@
         cdef int shp_length
         cdef char index
         cdef set chars
         if isinstance(shp, int):
             shp_length = shp
         else:
             shp_length = len(shp)
-        cdef np.ndarray bshape = np.empty(shp_length, dtype=np.bool)
+        cdef np.ndarray bshape = np.empty(shp_length, dtype=bool)
 
         if isinstance(shp, Shape):
             return shp.bool_shape
         if isinstance(shp, np.ndarray):
-            if shp.dtype == np.bool:
+            if shp.dtype == bool:
                 return shp
             else:
-                return np.array(list(shp), dtype=np.bool)
+                return np.array(list(shp), dtype=bool)
         if isinstance(shp, int):
             shp = "#" * shp
         if isinstance(shp, Iterable):
             if isinstance(shp, str) or isinstance(shp, unicode):
                 try:
                     self._bshape_from_str(bshape, shp)
                 except UnknownCharactersError:
```

### Comparing `dinopy-2.2.1/dinopy/shaping.pxd` & `dinopy-3.0.0/dinopy/shaping.pxd`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/shaping.pyx` & `dinopy-3.0.0/dinopy/shaping.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy/wrap_sais.pyx` & `dinopy-3.0.0/dinopy/wrap_sais.pyx`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/dinopy.egg-info/PKG-INFO` & `dinopy-3.0.0/dinopy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dinopy
-Version: 2.2.1
+Version: 3.0.0
 Summary: DNA input and output library for Python and Cython. Includes reader and writer for FASTA and FASTQ files, support for samtools faidx files, and generators for solid and gapped q-grams (k-mers).
 Home-page: https://bitbucket.org/HenningTimm/dinopy
 Author: Henning Timm, Till Hartmann
 Author-email: henning.timm@tu-dortmund.de, till.hartmann@tu-dortmund.de
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
+Requires-Dist: numpy>=1.17
+Requires-Dist: Cython>=3.0.0
 
 .. image:: https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat
    :target: https://bioconda.github.io/recipes/dinopy/README.html
 
 .. image:: https://img.shields.io/pypi/v/dinopy.svg?style=flat
    :target: https://pypi.python.org/pypi/dinopy
 
@@ -63,30 +63,30 @@
 
 Features
 ~~~~~~~~
 
 -  Easy to use reader and writer for FASTA-, FASTQ-, and SAM-files.
 -  Specifiable data type and representation for return values (bytes,
    bytearrays, strings and integers see
-   `dtype <https://dinopy.readthedocs.org/en/latest/encoding/>`__ for
+   `dtype <https://dinopy.readthedocs.org/en/latest/encoding.html>`__ for
    more information).
 -  Implemented in `Cython <http://cython.org/>`__ for additional speedup.
--  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration/>`__ to avoid introducing Python code into Cython projects.
+-  Offers a `Cython API <https://dinopy.readthedocs.org/en/latest/cython_integration.html>`__ to avoid introducing Python code into Cython projects.
 -  Works directly on gzipped files.
 -  Iterators for q-grams of a sequence (also allowing shaped q-grams).
 -  (Reverse) complement.
 -  Chromosome selection from FASTA files.
 
 
 Getting Started
 ~~~~~~~~~~~~~~~
 
 -  If you are new to dinopy you can get started by following the
    first-steps
-   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction/>`__.
+   `tutorial <https://dinopy.readthedocs.org/en/latest/getting-started/introduction.html>`__.
 -  A full list of features, as well as the documentation, can be found
    `here <https://dinopy.readthedocs.org/en/latest/>`__.
 
 Installation
 ~~~~~~~~~~~~
 
 Dinopy can be installed with pip:
@@ -125,17 +125,17 @@
        $ python
 
        >>> import dinopy
 
 Installation requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
--  `python <https://www.python.org/>`__ >= 3.5
+-  `python <https://www.python.org/>`__ >= 3.8
 -  `numpy <http://www.numpy.org/>`__ >= 1.17
--  `cython <http://cython.org/>`__ >= 0.22
+-  `cython <http://cython.org/>`__ >= 3.0.0
 -  C and C++ compilers, for example from ``build-essentials`` (Linux) or ``Xcode`` (OSX)
 
 We recommend using
 `anaconda <https://www.continuum.io/downloads>`__
 and the
 `bioconda channel <https://github.com/bioconda/bioconda-recipes>`__.
 
@@ -169,9 +169,7 @@
 
 
 License
 ~~~~~~~
 
 Dinopy is Open Source and licensed under the `MIT
 License <http://opensource.org/licenses/MIT>`__.
-
-
```

### Comparing `dinopy-2.2.1/dinopy.egg-info/SOURCES.txt` & `dinopy-3.0.0/dinopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/Makefile` & `dinopy-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/make.bat` & `dinopy-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/conf.py` & `dinopy-3.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,41 +11,40 @@
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys
 import os
-#import sphinx_bootstrap_theme
 import sphinx_rtd_theme
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 # allow for local building of the documentation
 on_rtd = os.environ.get('READTHEDOCS') == 'True'
 if not on_rtd:
-   sys.path.insert(0, os.path.abspath('../../'))
+    sys.path.insert(0, os.path.abspath('../../'))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
     'sphinx.ext.coverage',
-    'sphinx.ext.imgmath', # this requires sphinx >= 1.4
+    'sphinx.ext.imgmath',  # this requires sphinx >= 1.4
     'sphinx.ext.viewcode',
-    'sphinx.ext.napoleon', # used for parsing numpy and google docstrings; was sphinxcontrib.napoleon before v1.3
+    'sphinx.ext.napoleon',  # used for parsing numpy and google docstrings; was sphinxcontrib.napoleon before v1.3
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -54,24 +53,24 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'dinopy'
-copyright = '2014-2022, Henning Timm, Till Hartmann'
+copyright = '2014-2024, Henning Timm, Till Hartmann'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2.2'
+version = '3.0'
 # The full version, including alpha/beta/rc tags.
-release = '2.2.1'
+release = '3.0.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -251,15 +250,15 @@
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
   ('index', 'dinopy', 'dinopy Documentation',
-   'Henning Timm, Till Hartmann', 'dinopy', 'One line description of project.',
+   'Henning Timm, Till Hartmann', 'dinopy', 'Dna INput and Output in PYthon. Python package for (dna-)sequence handling, especially reading and writing FASTA- and FASTQ-files.',
    'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
@@ -269,9 +268,9 @@
 #texinfo_show_urls = 'footnote'
 
 autoclass_content = 'both'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 def setup(app):
-   app.add_stylesheet("hide.css")
+   app.add_css_file("hide.css")
```

### Comparing `dinopy-2.2.1/docs/source/cython_integration.rst` & `dinopy-3.0.0/docs/source/cython_integration.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/encoding.rst` & `dinopy-3.0.0/docs/source/encoding.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/faq.rst` & `dinopy-3.0.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/getting-started/examples.rst` & `dinopy-3.0.0/docs/source/getting-started/examples.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/getting-started/first-steps.rst` & `dinopy-3.0.0/docs/source/getting-started/first-steps.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/docs/source/getting-started/introduction.rst` & `dinopy-3.0.0/docs/source/getting-started/introduction.rst`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/files/phix.small.fastq.gz` & `dinopy-3.0.0/files/phix.small.fastq.gz`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/files/testreads_long.fastq` & `dinopy-3.0.0/files/testreads_long.fastq`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/images/dinopy_overview.svg` & `dinopy-3.0.0/images/dinopy_overview.svg`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/setup.py` & `dinopy-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,35 +36,34 @@
 
 
 setup(
     name='dinopy',
     description="DNA input and output library for Python and Cython. Includes reader and writer for FASTA and FASTQ "
                 "files, support for samtools faidx files, and generators for solid and gapped q-grams (k-mers).",
     long_description=open("README.rst").read(),
-    version='2.2.1',
+    version='3.0.0',
     author='Henning Timm, Till Hartmann',
     author_email='henning.timm@tu-dortmund.de, till.hartmann@tu-dortmund.de',
     license="MIT",
     url="https://bitbucket.org/HenningTimm/dinopy",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Cython',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
     ],
     packages=['dinopy'],
     # Add cython and c++ files
     package_data={'dinopy': ['*.pyx', '*.pxd', 'cpp/sais.cpp', '../README.rst']},
-    install_requires=['numpy>=1.17', 'cython>=0.22'],
+    install_requires=['numpy>=1.17', 'Cython>=3.0.0'],
     ext_modules=extensions,
 )
```

### Comparing `dinopy-2.2.1/test/aux_test.py` & `dinopy-3.0.0/test/aux_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/conversion_test.py` & `dinopy-3.0.0/test/conversion_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/creader_test.py` & `dinopy-3.0.0/test/creader_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fai_io_test.py` & `dinopy-3.0.0/test/fai_io_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fasta_reader_test.py` & `dinopy-3.0.0/test/fasta_reader_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fasta_sources.py` & `dinopy-3.0.0/test/fasta_sources.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fasta_writer_test.py` & `dinopy-3.0.0/test/fasta_writer_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fastq_reader_test.py` & `dinopy-3.0.0/test/fastq_reader_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/fastq_writer_test.py` & `dinopy-3.0.0/test/fastq_writer_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/init_test.py` & `dinopy-3.0.0/test/init_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/input_opener_test.py` & `dinopy-3.0.0/test/input_opener_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/output_opener_test.py` & `dinopy-3.0.0/test/output_opener_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/processors_test.py` & `dinopy-3.0.0/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/read_write_test.py` & `dinopy-3.0.0/test/read_write_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/sam_reader_test.py` & `dinopy-3.0.0/test/sam_reader_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/sam_writer_test.py` & `dinopy-3.0.0/test/sam_writer_test.py`

 * *Files identical despite different names*

### Comparing `dinopy-2.2.1/test/shaping_test.py` & `dinopy-3.0.0/test/shaping_test.py`

 * *Files identical despite different names*

