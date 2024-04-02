# Comparing `tmp/latex-rubber-1.6.1.tar.gz` & `tmp/latex-rubber-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex-rubber-1.6.1.tar", last modified: Wed Jun  8 17:51:40 2022, max compression
+gzip compressed data, was "latex-rubber-1.6.2.tar", last modified: Tue Apr  2 23:40:48 2024, max compression
```

## Comparing `latex-rubber-1.6.1.tar` & `latex-rubber-1.6.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.869493 latex-rubber-1.6.1/
--rw-r--r--   0 safonso   (1000) safonso   (1000)    35149 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/COPYING
--rw-r--r--   0 safonso   (1000) safonso   (1000)       38 2022-06-08 17:24:26.000000 latex-rubber-1.6.1/MANIFEST.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)    14016 2022-06-08 17:48:26.000000 latex-rubber-1.6.1/NEWS
--rw-r--r--   0 safonso   (1000) safonso   (1000)      871 2022-06-08 17:51:40.869493 latex-rubber-1.6.1/PKG-INFO
--rw-r--r--   0 safonso   (1000) safonso   (1000)     6574 2022-06-08 17:45:31.000000 latex-rubber-1.6.1/README
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.859493 latex-rubber-1.6.1/bin/
--rwxr-xr-x   0 safonso   (1000) safonso   (1000)      785 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/bin/rubber
--rwxr-xr-x   0 safonso   (1000) safonso   (1000)      784 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/bin/rubber-info
--rwxr-xr-x   0 safonso   (1000) safonso   (1000)      756 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/bin/rubber-lsmod
--rwxr-xr-x   0 safonso   (1000) safonso   (1000)      784 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/bin/rubber-pipe
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.859493 latex-rubber-1.6.1/doc/
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.859493 latex-rubber-1.6.1/doc/man-en/
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2535 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/doc/man-en/rubber-info.1.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)    18437 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/doc/man-en/rubber.1.in
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.859493 latex-rubber-1.6.1/doc/man-fr/
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2930 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/doc/man-fr/rubber-info.1.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)    20999 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/doc/man-fr/rubber.1.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)    42055 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/doc/rubber.texi.in
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.859493 latex-rubber-1.6.1/latex_rubber.egg-info/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      871 2022-06-08 17:51:39.000000 latex-rubber-1.6.1/latex_rubber.egg-info/PKG-INFO
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2059 2022-06-08 17:51:40.000000 latex-rubber-1.6.1/latex_rubber.egg-info/SOURCES.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)        1 2022-06-08 17:51:39.000000 latex-rubber-1.6.1/latex_rubber.egg-info/dependency_links.txt
--rw-r--r--   0 safonso   (1000) safonso   (1000)        7 2022-06-08 17:51:40.000000 latex-rubber-1.6.1/latex_rubber.egg-info/top_level.txt
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.862826 latex-rubber-1.6.1/rubber/
--rw-r--r--   0 safonso   (1000) safonso   (1000)      305 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/__init__.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     6688 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/biblio.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    25990 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/cmdline.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     4265 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/contents.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     9270 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/convert.py
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.862826 latex-rubber-1.6.1/rubber/converters/
--rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/__init__.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      887 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/compressor.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1840 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/eps_gz.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2115 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/fig2dev.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    48050 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/latex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1025 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/literate.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     7804 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/mpost.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      761 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/converters/shell.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    11277 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/depend.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1926 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/dvip_tool.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     4782 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/environment.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     4272 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/index.py
-drwxr-xr-x   0 safonso   (1000) safonso   (1000)        0 2022-06-08 17:51:40.869493 latex-rubber-1.6.1/rubber/latex_modules/
--rw-r--r--   0 safonso   (1000) safonso   (1000)        0 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/__init__.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      233 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/aleph.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     4204 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/asymptote.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      283 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/backref.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      570 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/beamer.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     4274 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/biblatex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      863 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/bibtex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2362 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/bibtopic.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1665 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/combine.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      264 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/dvipdfm.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      262 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/dvips.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1298 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/epsfig.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      588 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/glossaries.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      212 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/gnuplottex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     7513 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/graphics.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     7513 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/graphicx.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      370 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/hyperref.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     3602 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/index.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      866 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/listings.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      620 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/ltxtable.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      317 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/lualatex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      288 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/makeidx.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1654 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/minitoc-hyper.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1654 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/minitoc.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1044 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/moreverb.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2544 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/multibib.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      492 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/nomencl.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      283 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/ntheorem.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      234 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/omega.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1069 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/pdftex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      692 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/ps2pdf.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1431 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/pythontex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      669 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/verbatim.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      907 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/vtex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)      315 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/xelatex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     1021 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/latex_modules/xr.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     3831 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/module_interface.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)     2158 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/rules.ini
--rw-r--r--   0 safonso   (1000) safonso   (1000)    14742 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/tex.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)    10336 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/util.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)       37 2022-06-08 17:18:30.000000 latex-rubber-1.6.1/rubber/version.py
--rw-r--r--   0 safonso   (1000) safonso   (1000)       22 2022-06-08 15:41:22.000000 latex-rubber-1.6.1/rubber/version.py.in
--rw-r--r--   0 safonso   (1000) safonso   (1000)       38 2022-06-08 17:51:40.869493 latex-rubber-1.6.1/setup.cfg
--rw-r--r--   0 safonso   (1000) safonso   (1000)     9814 2022-06-08 17:48:34.000000 latex-rubber-1.6.1/setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/
+-rw-r--r--   0 sping     (1000) sping     (1000)    35149 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/COPYING
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/MANIFEST.in
+-rw-r--r--   0 sping     (1000) sping     (1000)    14527 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/NEWS
+-rw-r--r--   0 sping     (1000) sping     (1000)      894 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     6574 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/README
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.348085 latex-rubber-1.6.2/bin/
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      785 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      784 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-info
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      756 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-lsmod
+-rwxr-xr-x   0 sping     (1000) sping     (1000)      784 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-pipe
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/man-en/
+-rw-r--r--   0 sping     (1000) sping     (1000)     2535 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-en/rubber-info.1.in
+-rw-r--r--   0 sping     (1000) sping     (1000)    18437 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-en/rubber.1.in
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/man-fr/
+-rw-r--r--   0 sping     (1000) sping     (1000)     2930 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-fr/rubber-info.1.in
+-rw-r--r--   0 sping     (1000) sping     (1000)    20999 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-fr/rubber.1.in
+-rw-r--r--   0 sping     (1000) sping     (1000)    42055 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/rubber.texi.in
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/latex_rubber.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)      894 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     2059 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        7 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/top_level.txt
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.352086 latex-rubber-1.6.2/rubber/
+-rw-r--r--   0 sping     (1000) sping     (1000)      305 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6688 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/biblio.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    26003 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/cmdline.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4265 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/contents.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     9270 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/convert.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.353086 latex-rubber-1.6.2/rubber/converters/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      887 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/compressor.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1840 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/eps_gz.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2115 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/fig2dev.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    48052 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/latex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1025 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/literate.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7804 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/mpost.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      761 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/shell.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    11277 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/depend.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1926 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/dvip_tool.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4782 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/environment.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4272 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/index.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/rubber/latex_modules/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      233 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/aleph.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4204 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/asymptote.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      283 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/backref.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      570 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/beamer.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     4274 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/biblatex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      863 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/bibtex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2362 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/bibtopic.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1665 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/combine.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      264 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/dvipdfm.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      262 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/dvips.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1298 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/epsfig.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      588 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/glossaries.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      212 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/gnuplottex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7513 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/graphics.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7513 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/graphicx.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      370 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/hyperref.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3602 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/index.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      866 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/listings.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      620 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ltxtable.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      317 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/lualatex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      288 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/makeidx.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1654 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/minitoc-hyper.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1654 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/minitoc.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1044 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/moreverb.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2544 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/multibib.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      492 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/nomencl.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      283 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ntheorem.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      234 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/omega.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1069 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/pdftex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      692 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ps2pdf.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1431 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/pythontex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      669 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/verbatim.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      907 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/vtex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      315 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/xelatex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1021 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/xr.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     3831 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/module_interface.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2158 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/rules.ini
+-rw-r--r--   0 sping     (1000) sping     (1000)    14742 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/tex.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    10336 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/util.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       18 2024-04-02 23:40:16.000000 latex-rubber-1.6.2/rubber/version.py
+-rw-r--r--   0 sping     (1000) sping     (1000)       22 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/version.py.in
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/setup.cfg
+-rw-r--r--   0 sping     (1000) sping     (1000)    10152 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/setup.py
```

### Comparing `latex-rubber-1.6.1/COPYING` & `latex-rubber-1.6.2/COPYING`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/NEWS` & `latex-rubber-1.6.2/NEWS`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Upcoming Version
 
   Nothing so far…
 
+Version 1.6.2 (2024-03-30)
+
+  - Require Python >=3.8 (!29 by Sebastian Pipping)
+  - Fix crash with source path that uses special characters
+    (#10, !25 by Pietro Battiston)
+  - Announce "--into DIR" at runtime more consistently (!27 by Florian Fischer)
+  - setup.py: Fix version going into call setup(..) and file rubber/version.py
+    (!29 by Sebastian Pipping)
+  - setup.py: Migrate off of distutils (!29 by Sebastian Pipping)
+  - setup.py: Hide virtualenvs from command "clean" (!29 by Sebastian Pipping)
+
 Version 1.6.1 (2022-06-08)
 
   - Available on PyPI as `latex-rubber`
 
 Version 1.6.0 (2021-06-16)
 
   - Add support for LuaTeX via the lualatex module
```

### Comparing `latex-rubber-1.6.1/PKG-INFO` & `latex-rubber-1.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: latex-rubber
-Version: 1.6.1
+Version: 1.6.2
 Summary: an automated system for building LaTeX documents
 Home-page: https://gitlab.com/latex-rubber/rubber
 Author: Sebastian Kapfer
 Author-email: sebastian.kapfer@fau.de
 Maintainer: Florian Schmaus
 Maintainer-email: flo@geekplace.eu
 License: GPL
+Requires-Python: >=3.8
 License-File: COPYING
 
 This is a building system for LaTeX documents. It is based on a routine that
 runs just as many compilations as necessary. The module system provides a
 great flexibility that virtually allows support for any package with no user
 intervention, as well as pre- and post-processing of the document. The
 standard modules currently provide support for bibtex, dvips, dvipdfm, pdftex,
```

### Comparing `latex-rubber-1.6.1/README` & `latex-rubber-1.6.2/README`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 automatic conversion between various graphics formats and Metapost
 compilation. The associated tool "rubber-info" extracts information, such as
 dependency relations or post-compilation diagnostics.
 
 
 * Installation
 
-Running Rubber just requires Python 3.5.  Of course it won't
+Running Rubber just requires Python 3.8.  Of course it won't
 be of much use without a working LaTeX environment (Rubber is known to work on
 TeXLive and VTeX on various flavors of Unix including Darwin and Cygwin, any
 feedback is welcome about other systems).
 
 For compilation, you will need the Python Distutils, which are usually included
 in development packages (in Debian, this is the python3-dev package).
```

### Comparing `latex-rubber-1.6.1/bin/rubber` & `latex-rubber-1.6.2/bin/rubber`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/bin/rubber-info` & `latex-rubber-1.6.2/bin/rubber-info`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/bin/rubber-lsmod` & `latex-rubber-1.6.2/bin/rubber-lsmod`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/bin/rubber-pipe` & `latex-rubber-1.6.2/bin/rubber-pipe`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/doc/man-en/rubber-info.1.in` & `latex-rubber-1.6.2/doc/man-en/rubber-info.1.in`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/doc/man-en/rubber.1.in` & `latex-rubber-1.6.2/doc/man-en/rubber.1.in`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/doc/man-fr/rubber-info.1.in` & `latex-rubber-1.6.2/doc/man-fr/rubber-info.1.in`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/doc/man-fr/rubber.1.in` & `latex-rubber-1.6.2/doc/man-fr/rubber.1.in`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/doc/rubber.texi.in` & `latex-rubber-1.6.2/doc/rubber.texi.in`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/latex_rubber.egg-info/PKG-INFO` & `latex-rubber-1.6.2/latex_rubber.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: latex-rubber
-Version: 1.6.1
+Version: 1.6.2
 Summary: an automated system for building LaTeX documents
 Home-page: https://gitlab.com/latex-rubber/rubber
 Author: Sebastian Kapfer
 Author-email: sebastian.kapfer@fau.de
 Maintainer: Florian Schmaus
 Maintainer-email: flo@geekplace.eu
 License: GPL
+Requires-Python: >=3.8
 License-File: COPYING
 
 This is a building system for LaTeX documents. It is based on a routine that
 runs just as many compilations as necessary. The module system provides a
 great flexibility that virtually allows support for any package with no user
 intervention, as well as pre- and post-processing of the document. The
 standard modules currently provide support for bibtex, dvips, dvipdfm, pdftex,
```

### Comparing `latex-rubber-1.6.1/latex_rubber.egg-info/SOURCES.txt` & `latex-rubber-1.6.2/latex_rubber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/biblio.py` & `latex-rubber-1.6.2/rubber/biblio.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/cmdline.py` & `latex-rubber-1.6.2/rubber/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         else:
             args = options.source
 
         if options.place is None:  # --inplace
             # Compute all absolute paths before the first chdir.
             args = map(os.path.abspath, args)
         elif options.place != '.':  # non default --into
-            print("                       into", options.place)
+            msg.info(_("changing to %s from --into option") % options.place)
             # Make arguments relative to the new directory,
             # go there then proceed normally.
             args = map(lambda p: os.path.relpath(p, options.place), args)
             try:
                 os.chdir(options.place)
             except OSError as e:
                 raise rubber.GenericError \
```

### Comparing `latex-rubber-1.6.1/rubber/contents.py` & `latex-rubber-1.6.2/rubber/contents.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/convert.py` & `latex-rubber-1.6.2/rubber/convert.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/compressor.py` & `latex-rubber-1.6.2/rubber/converters/compressor.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/eps_gz.py` & `latex-rubber-1.6.2/rubber/converters/eps_gz.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/fig2dev.py` & `latex-rubber-1.6.2/rubber/converters/fig2dev.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/latex.py` & `latex-rubber-1.6.2/rubber/converters/latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,15 @@
         self.failed_module = None
 
         assert os.path.exists(path)
         assert len(self.sources) == 0
         self.vars['source'] = path
         (src_path, name) = os.path.split(path)
         # derive jobname, which latex uses as the basename for all output
-        (job, _) = os.path.splitext(name)
+        (job, ext) = os.path.splitext(name)
         if jobname is None:
             self.set_job = 0
         else:
             self.set_job = 1
             job = jobname
         self.vars['job'] = job
         if src_path == "":
```

### Comparing `latex-rubber-1.6.1/rubber/converters/literate.py` & `latex-rubber-1.6.2/rubber/converters/literate.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/mpost.py` & `latex-rubber-1.6.2/rubber/converters/mpost.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/converters/shell.py` & `latex-rubber-1.6.2/rubber/converters/shell.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/depend.py` & `latex-rubber-1.6.2/rubber/depend.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/dvip_tool.py` & `latex-rubber-1.6.2/rubber/dvip_tool.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/environment.py` & `latex-rubber-1.6.2/rubber/environment.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/index.py` & `latex-rubber-1.6.2/rubber/index.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/asymptote.py` & `latex-rubber-1.6.2/rubber/latex_modules/asymptote.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/beamer.py` & `latex-rubber-1.6.2/rubber/latex_modules/beamer.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/biblatex.py` & `latex-rubber-1.6.2/rubber/latex_modules/biblatex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/bibtex.py` & `latex-rubber-1.6.2/rubber/latex_modules/bibtex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/bibtopic.py` & `latex-rubber-1.6.2/rubber/latex_modules/bibtopic.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/combine.py` & `latex-rubber-1.6.2/rubber/latex_modules/combine.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/epsfig.py` & `latex-rubber-1.6.2/rubber/latex_modules/epsfig.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/glossaries.py` & `latex-rubber-1.6.2/rubber/latex_modules/glossaries.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/graphics.py` & `latex-rubber-1.6.2/rubber/latex_modules/graphics.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/graphicx.py` & `latex-rubber-1.6.2/rubber/latex_modules/graphicx.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/index.py` & `latex-rubber-1.6.2/rubber/latex_modules/index.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/listings.py` & `latex-rubber-1.6.2/rubber/latex_modules/listings.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/ltxtable.py` & `latex-rubber-1.6.2/rubber/latex_modules/ltxtable.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/minitoc-hyper.py` & `latex-rubber-1.6.2/rubber/latex_modules/minitoc-hyper.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/minitoc.py` & `latex-rubber-1.6.2/rubber/latex_modules/minitoc.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/moreverb.py` & `latex-rubber-1.6.2/rubber/latex_modules/moreverb.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/multibib.py` & `latex-rubber-1.6.2/rubber/latex_modules/multibib.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/pdftex.py` & `latex-rubber-1.6.2/rubber/latex_modules/pdftex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/ps2pdf.py` & `latex-rubber-1.6.2/rubber/latex_modules/ps2pdf.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/pythontex.py` & `latex-rubber-1.6.2/rubber/latex_modules/pythontex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/verbatim.py` & `latex-rubber-1.6.2/rubber/latex_modules/verbatim.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/vtex.py` & `latex-rubber-1.6.2/rubber/latex_modules/vtex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/latex_modules/xr.py` & `latex-rubber-1.6.2/rubber/latex_modules/xr.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/module_interface.py` & `latex-rubber-1.6.2/rubber/module_interface.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/rules.ini` & `latex-rubber-1.6.2/rubber/rules.ini`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/tex.py` & `latex-rubber-1.6.2/rubber/tex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/rubber/util.py` & `latex-rubber-1.6.2/rubber/util.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.1/setup.py` & `latex-rubber-1.6.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 # This is the setup script for Rubber. It acts both as a part of the
 # configuration script a la autoconf and as a setup script a la Distutils.
 #
 # Copyright 2002-2006 Emmanuel Beffara
 # Copyright 2015-2015 Sebastian Kapfer
 # Copyright 2015-2015 Nicolas Boulenguez
 
-import distutils.cmd
-import distutils.command.build
-import distutils.command.clean
-import distutils.command.install
-import distutils.core
-import distutils.dir_util
-import distutils.log
-import distutils.util
+import logging
 import os.path
 import re
-import subprocess
-import sys
+import shutil
+from setuptools import Command, setup
+from setuptools.command.build import build as BuildCommand
+from setuptools.command.install import install as InstallCommand
 
 project_root_dir = os.path.dirname(__file__)
 
 # A file f is generated from f.in by replacing @author@, @version@ by
 # sensible values (as ./configure does in the autoconf world).
 files_with_substitutions = (
     os.path.join("doc", "man-en", "rubber.1"),
@@ -39,34 +34,50 @@
     ("html", ("makeinfo", "--html", "--no-split")),
     ("info", ("makeinfo", "--info")),
     ("pdf", ("texi2dvi", "--pdf", "--quiet", "--tidy")),
     ("txt", ("makeinfo", "--plaintext")),
 )
 
 
-class build(distutils.command.build.build):
+class build(BuildCommand):
     man = False
     info = False
     html = False
     pdf = False
     txt = False
-    user_options = distutils.command.build.build.user_options + [
+    user_options = BuildCommand.user_options + [
         ("man=", None, "build Manpages [{default}]".format(default=man)),
         ("info=", None, "build Info documentation [{default}]".format(default=info)),
         ("html=", None, "format HTML documentation [{default}]".format(default=html)),
         ("pdf=", None, "format PDF documentation [{default}]".format(default=pdf)),
         ("txt=", None, "format plain text documentation [{default}]".format(default=txt)),
     ]
 
+    @staticmethod
+    def _distutils_util_strtobool(val):
+        """Convert a string representation of truth to true (1) or false (0).
+
+        True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+        are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+        'val' is anything else.
+        """
+        val = val.lower()
+        if val in ('y', 'yes', 't', 'true', 'on', '1'):
+            return 1
+        elif val in ('n', 'no', 'f', 'false', 'off', '0'):
+            return 0
+        else:
+            raise ValueError("invalid truth value {!r}".format(val))
+
     def finalize_options(self):
-        distutils.command.build.build.finalize_options(self)
+        super().finalize_options()
         for fmt in ['man'] + [fmt for fmt, recipe in doc_recipes]:
             value = getattr(self, fmt)
             if type(value) is str:
-                value = distutils.util.strtobool(value)
+                value = self._distutils_util_strtobool(value)
                 setattr(self, fmt, value)
 
     def generate_files_with_substitutions(self, subs):
         pattern = "|".join(subs.keys())
         pattern = "@(" + pattern + ")@"
         pattern = re.compile(pattern)
 
@@ -97,35 +108,35 @@
 
     def run(self):
         subs = {}
         for v in ("author", "author_email", "maintainer", "maintainer_email", "url", "version"):
             subs[v] = getattr(self.distribution.metadata, "get_" + v)()
         self.generate_files_with_substitutions(subs)
 
-        distutils.command.build.build.run(self)
+        super().run()
 
         self.generate_documentation()
 
 
-class install(distutils.command.install.install):
+class install(InstallCommand):
 
     mandir = "$base/man"
     infodir = "$base/info"
     docdir = "$base/share/doc/rubber"
-    user_options = distutils.command.install.install.user_options + [
+    user_options = InstallCommand.user_options + [
         ("mandir=", None,
          "installation directory for manual pages [{default}]".format(default=mandir)),
         ("infodir=", None,
          "installation directory for info manuals [{default}]".format(default=infodir)),
         ("docdir=", None,
          "installation directory for other documentation [{default}]".format(default=docdir)),
     ]
 
     def finalize_options(self):
-        distutils.command.install.install.finalize_options(self)
+        super().finalize_options()
         self._expand_attrs(("mandir", "infodir", "docdir"))
 
     def run(self):
         build = self.get_finalized_command("build")
         assert self.distribution.data_files is None
         self.distribution.data_files = []
         if build.man:
@@ -141,52 +152,76 @@
                                             ))]
         if build.info:
             infodocs = (manual_basename + "info",)
             self.distribution.data_files.append((self.infodir, infodocs))
         otherdocs = [manual_basename + f for f in ("html", "pdf", "txt") if getattr(build, f)]
         if len(otherdocs) > 0:
             self.distribution.data_files.append((self.docdir, otherdocs))
-        distutils.command.install.install.run(self)
+        super().run()
 
 
-class clean(distutils.command.clean.clean):
+class clean(Command):
+    description = "clean up temporary files from 'build' command"
+    user_options = [
+        ('build-base=', 'b', "base build directory (default: 'build')"),
+        ('all', 'a', "remove all build output, not just temporary by-products"),
+    ]
+
+    def initialize_options(self):
+        self.build_base = None
+        self.all = None
+
+    def finalize_options(self):
+        self.set_undefined_options(
+            'build',
+            ('build_base', 'build_base'),
+        )
 
     def remove_tree(self, path):
         if os.path.exists(path):
-            distutils.dir_util.remove_tree(path, dry_run=self.dry_run)
+            logging.info("removing '%s'", path)
+            if not self.dry_run:
+                shutil.rmtree(path)
         else:
-            distutils.log.debug("'%s' does not exist -- can't clean it", path)
+            logging.debug("'%s' does not exist -- can't clean it", path)
 
     def remove_file(self, path):
         if os.path.exists(path):
-            distutils.log.info("removing '%s'", path)
+            logging.info("removing '%s'", path)
             if not self.dry_run:
                 os.remove(path)
 
     def run(self):
-        distutils.command.clean.clean.run(self)
+        try:
+            self.remove_tree(self.build_base)
+        except OSError:
+            pass
 
         if self.all:
             for f in files_with_substitutions:
                 self.remove_file(f)
 
         for fmt, _ in doc_recipes:
             self.remove_file(manual_basename + fmt)
         self.remove_tree("rubber.t2d")
 
         for dirpath, dirnames, filenames in os.walk(os.curdir):
+            for venv in ('.venv', 'venv'):
+                if venv in dirnames:
+                    dirnames.remove(venv)
+
             for filename in filenames:
                 ew = filename.endswith
                 if ew("~") or ew(".pyc") or ew(".pyo"):
                     self.remove_file(os.path.join(dirpath, filename))
 
         self.remove_tree(os.path.join("tests", "tmp"))
 
 
-class tar(distutils.cmd.Command):
+class tar(Command):
     description = "wrapper for git archive"
     user_options = [
         ("revision=", None, "git tree-ish [HEAD]"),
         ("extension=", None, "archive extension [tar.gz]"),
     ]
     revision = "HEAD"
     extension = "tar.gz"
@@ -208,32 +243,18 @@
         while True:
             line = f.readline()
             if line.startswith("Version"):
                 break
     match = re.match(r'^Version ([0-9.]+) ', line)
     version = match.group(1)
 
-    git_dir = os.path.join(project_root_dir, '.git')
-    if os.path.exists(git_dir):
-        try:
-            result = subprocess.Popen(['git', '--git-dir', git_dir, 'describe'],
-                                      stdout=subprocess.PIPE,
-                                      stderr=subprocess.DEVNULL)
-            result.wait()
-            git_describe_output = result.stdout.read().decode('utf-8').strip()
-            if git_describe_output != version:
-                version += " (" + git_describe_output + ")"
-        except Exception:
-            # We warn about, but otherwise ignore exceptions here.
-            print(f"Exception during 'git' invocation {sys.exc_info()[0]}", file=sys.stderr)
-
     return version
 
 
-distutils.core.setup(
+setup(
     name="latex-rubber",
     version=extract_version(),
     description="an automated system for building LaTeX documents",
     long_description="""\
 This is a building system for LaTeX documents. It is based on a routine that
 runs just as many compilations as necessary. The module system provides a
 great flexibility that virtually allows support for any package with no user
@@ -245,14 +266,15 @@
 """,
     author='Sebastian Kapfer',
     author_email='sebastian.kapfer@fau.de',
     maintainer='Florian Schmaus',
     maintainer_email='flo@geekplace.eu',
     url='https://gitlab.com/latex-rubber/rubber',
     license="GPL",
+    python_requires='>=3.8',
     packages=(
         "rubber",
         "rubber.converters",
         "rubber.latex_modules",
     ),
     package_dir={
         "rubber": "rubber",
```

