# Comparing `tmp/FORD-7.0.5.tar.gz` & `tmp/FORD-7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FORD-7.0.5.tar", last modified: Mon Jan  8 11:13:11 2024, max compression
+gzip compressed data, was "FORD-7.0.6.tar", last modified: Wed Apr  3 15:44:54 2024, max compression
```

## Comparing `FORD-7.0.5.tar` & `FORD-7.0.6.tar`

### file list

```diff
@@ -1,208 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-08 11:13:00.000000 FORD-7.0.5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.132678 FORD-7.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.152678 FORD-7.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-08 11:13:00.000000 FORD-7.0.5/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-08 11:13:00.000000 FORD-7.0.5/.github/workflows/corpus_regressions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-08 11:13:00.000000 FORD-7.0.5/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-08 11:13:00.000000 FORD-7.0.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-01-08 11:13:00.000000 FORD-7.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-08 11:13:00.000000 FORD-7.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)  4225846 2024-01-08 11:13:00.000000 FORD-7.0.5/2003standard.pdf
--rw-r--r--   0 runner    (1001) docker     (127)  8053119 2024-01-08 11:13:00.000000 FORD-7.0.5/2008standard.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    47702 2024-01-08 11:13:00.000000 FORD-7.0.5/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/FORD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-08 11:13:11.000000 FORD-7.0.5/FORD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-01-08 11:13:00.000000 FORD-7.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-08 11:13:00.000000 FORD-7.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-01-08 11:13:11.180678 FORD-7.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-01-08 11:13:00.000000 FORD-7.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.152678 FORD-7.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.152678 FORD-7.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/_static/ford_docs_custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.156678 FORD-7.0.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.external_project.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.fixed2free2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.fortran_project.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.intrinsics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.md_admonition.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.md_environ.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.md_striped_table.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.output.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.pagetree.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.sourceform.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.tipue_search.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/ford.version.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.156678 FORD-7.0.5/docs/developers_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/developers_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/callgraph.png
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/command_line_options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/documentation_meta_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/limitation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/note_box.png
--rw-r--r--   0 runner    (1001) docker     (127)    72521 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/output-example.png
--rw-r--r--   0 runner    (1001) docker     (127)   132134 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/pages-example.png
--rw-r--r--   0 runner    (1001) docker     (127)    31751 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/project_file_options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/running_ford.rst
--rw-r--r--   0 runner    (1001) docker     (127)    40179 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/say_hello_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/writing_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-01-08 11:13:00.000000 FORD-7.0.5/docs/user_guide/writing_pages.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 11:13:00.000000 FORD-7.0.5/example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-08 11:13:00.000000 FORD-7.0.5/example/example-project-file.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-08 11:13:00.000000 FORD-7.0.5/example/images/Fortran_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/pages/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/subdir/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/subdir/subsubpage.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/subpage1.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/subpage2.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-08 11:13:00.000000 FORD-7.0.5/example/pages/subpage3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.160678 FORD-7.0.5/example/src/excluded_directory/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/excluded_directory/this_file_will_not_be_included.f90
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/excluded_file.f90
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/ford_example_type.f90
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/ford_f77_example.f
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/ford_interfaces.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/ford_test_module.fpp
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-01-08 11:13:00.000000 FORD-7.0.5/example/src/ford_test_program.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.168678 FORD-7.0.5/ford/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16385 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-08 11:13:10.000000 FORD-7.0.5/ford/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.168678 FORD-7.0.5/ford/css/
--rw-r--r--   0 runner    (1001) docker     (127)    26651 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (127)    21984 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/css/local.css
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/css/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/external_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fixed2free2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.168678 FORD-7.0.5/ford/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    85908 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)    56006 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   287007 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   112160 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    65452 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)    62926 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41280 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17575 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/fortran_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    49140 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/intrinsics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.168678 FORD-7.0.5/ford/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.168678 FORD-7.0.5/ford/js/MathJax-config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/js/MathJax-config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    28810 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/js/svg-pan-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/md_admonition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/md_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/md_striped_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/pagetree.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16076 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)   119409 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/sourceform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.172678 FORD-7.0.5/ford/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/absint_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/block_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/block_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/file_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/file_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/genint_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/info_page.html
--rw-r--r--   0 runner    (1001) docker     (127)    28913 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/mod_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/mod_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/namelist_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/namelist_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/nongenint_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/proc_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/proc_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/prog_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/prog_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/type_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/templates/types_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipue_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.176678 FORD-7.0.5/ford/tipuesearch/
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.176678 FORD-7.0.5/ford/tipuesearch/img/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/img/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/img/loader.gif
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/img/search.png
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/tipuesearch.css
--rw-r--r--   0 runner    (1001) docker     (127)    22505 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/tipuesearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/tipuesearch.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/tipuesearch/tipuesearch_set.js
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-08 11:13:00.000000 FORD-7.0.5/ford/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      138 2024-01-08 11:13:00.000000 FORD-7.0.5/ford.py
--rw-r--r--   0 runner    (1001) docker     (127)    72521 2024-01-08 11:13:00.000000 FORD-7.0.5/output-example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-01-08 11:13:00.000000 FORD-7.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-08 11:13:00.000000 FORD-7.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 11:13:11.180678 FORD-7.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-08 11:13:00.000000 FORD-7.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.176678 FORD-7.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-01-08 11:13:00.000000 FORD-7.0.5/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_md_admonition.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_md_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_md_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_md_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_pagetree.py
--rw-r--r--   0 runner    (1001) docker     (127)    34018 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.176678 FORD-7.0.5/test/test_projects/
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_projects/test_external_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    61473 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_sourceform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-08 11:13:00.000000 FORD-7.0.5/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.132678 FORD-7.0.5/test_data/external_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/test_data/external_project/external_project/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/external_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/external_project/doc.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/test_data/external_project/external_project/src/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/external_project/src/external.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/test_data/external_project/top_level_project/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/top_level_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/top_level_project/doc.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 11:13:11.180678 FORD-7.0.5/test_data/external_project/top_level_project/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/external_project/top_level_project/src/top_level.f90
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/ford_issues_bad.f90
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/ford_issues_ok.f90
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/ford_issues_ok_expected.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/ford_test_program.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-08 11:13:00.000000 FORD-7.0.5/test_data/ford_test_program_expected.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.609510 FORD-7.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 15:44:49.000000 FORD-7.0.6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.557509 FORD-7.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.581509 FORD-7.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 15:44:49.000000 FORD-7.0.6/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 15:44:49.000000 FORD-7.0.6/.github/workflows/corpus_regressions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-03 15:44:49.000000 FORD-7.0.6/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-03 15:44:49.000000 FORD-7.0.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-03 15:44:49.000000 FORD-7.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 15:44:49.000000 FORD-7.0.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)  4225846 2024-04-03 15:44:49.000000 FORD-7.0.6/2003standard.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  8053119 2024-04-03 15:44:49.000000 FORD-7.0.6/2008standard.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    47702 2024-04-03 15:44:49.000000 FORD-7.0.6/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/FORD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 15:44:54.000000 FORD-7.0.6/FORD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-04-03 15:44:49.000000 FORD-7.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 15:44:49.000000 FORD-7.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-03 15:44:54.609510 FORD-7.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-03 15:44:49.000000 FORD-7.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.581509 FORD-7.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.581509 FORD-7.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/_static/ford_docs_custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.585509 FORD-7.0.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford._markdown.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.external_project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.fixed2free2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.fortran_project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.intrinsics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.md_admonition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.md_environ.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.md_striped_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.pagetree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.sourceform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.tipue_search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/ford.version.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.585509 FORD-7.0.6/docs/developers_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/developers_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.585509 FORD-7.0.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/callgraph.png
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/command_line_options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/documentation_meta_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/limitation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/note_box.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72521 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/output-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132134 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/pages-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31748 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/project_file_options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/running_ford.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    40179 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/say_hello_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/writing_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 15:44:49.000000 FORD-7.0.6/docs/user_guide/writing_pages.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:44:49.000000 FORD-7.0.6/example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-03 15:44:49.000000 FORD-7.0.6/example/example-project-file.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 15:44:49.000000 FORD-7.0.6/example/images/Fortran_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/pages/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/subdir/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/subdir/subsubpage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/subpage1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/subpage2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 15:44:49.000000 FORD-7.0.6/example/pages/subpage3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.589509 FORD-7.0.6/example/src/excluded_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/excluded_directory/this_file_will_not_be_included.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/excluded_file.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/ford_example_type.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/ford_f77_example.f
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/ford_interfaces.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/ford_test_module.fpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 15:44:49.000000 FORD-7.0.6/example/src/ford_test_program.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.593510 FORD-7.0.6/ford/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16385 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 15:44:54.000000 FORD-7.0.6/ford/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.593510 FORD-7.0.6/ford/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    26651 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21984 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/css/local.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/css/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/external_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fixed2free2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.597509 FORD-7.0.6/ford/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    85908 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    56006 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   287007 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   112160 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    65452 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    62926 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41280 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17684 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/fortran_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49246 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/intrinsics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.597509 FORD-7.0.6/ford/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.597509 FORD-7.0.6/ford/js/MathJax-config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/js/MathJax-config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    28810 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/js/svg-pan-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/md_admonition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/md_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/md_striped_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/pagetree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16076 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119748 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/sourceform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.601509 FORD-7.0.6/ford/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/absint_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/block_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/block_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/file_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/file_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/genint_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/info_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28936 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/mod_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/mod_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/namelist_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/namelist_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/nongenint_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/proc_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/proc_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/prog_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/prog_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/type_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/templates/types_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipue_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.601509 FORD-7.0.6/ford/tipuesearch/
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.601509 FORD-7.0.6/ford/tipuesearch/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/img/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/img/loader.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/img/search.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/tipuesearch.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22505 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/tipuesearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/tipuesearch.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/tipuesearch/tipuesearch_set.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 15:44:49.000000 FORD-7.0.6/ford/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      138 2024-04-03 15:44:49.000000 FORD-7.0.6/ford.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72521 2024-04-03 15:44:49.000000 FORD-7.0.6/output-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 15:44:49.000000 FORD-7.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 15:44:49.000000 FORD-7.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:44:54.609510 FORD-7.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 15:44:49.000000 FORD-7.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 15:44:49.000000 FORD-7.0.6/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_md_admonition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_md_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_md_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_md_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_pagetree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35952 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test/test_projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_projects/test_external_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62075 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_sourceform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-03 15:44:49.000000 FORD-7.0.6/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.561509 FORD-7.0.6/test_data/external_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test_data/external_project/external_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/external_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/external_project/doc.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test_data/external_project/external_project/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/external_project/src/external.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test_data/external_project/top_level_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/top_level_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/top_level_project/doc.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:44:54.605509 FORD-7.0.6/test_data/external_project/top_level_project/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/external_project/top_level_project/src/top_level.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/ford_issues_bad.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/ford_issues_ok.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/ford_issues_ok_expected.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/ford_test_program.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-03 15:44:49.000000 FORD-7.0.6/test_data/ford_test_program_expected.f90
```

### Comparing `FORD-7.0.5/.github/workflows/black.yml` & `FORD-7.0.6/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/.github/workflows/corpus_regressions.yml` & `FORD-7.0.6/.github/workflows/corpus_regressions.yml`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/.github/workflows/python_publish.yml` & `FORD-7.0.6/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/.github/workflows/test.yml` & `FORD-7.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/.gitignore` & `FORD-7.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/.readthedocs.yaml` & `FORD-7.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/2003standard.pdf` & `FORD-7.0.6/2003standard.pdf`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/2008standard.pdf` & `FORD-7.0.6/2008standard.pdf`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/CHANGELOG.md` & `FORD-7.0.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/FORD.egg-info/PKG-INFO` & `FORD-7.0.6/FORD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FORD
-Version: 7.0.5
+Version: 7.0.6
 Summary: FORD (FORtran Documenter) is an automatic documentation generator for modern Fortran programs.
 Author-email: Chris MacMackin <cmacmackin@gmail.com>, Peter Hill <peter.hill@york.ac.uk>
 License: GPLv3
 Project-URL: Source, https://github.com/Fortran-FOSS-Programmers/ford
 Project-URL: Tracker, https://github.com/Fortran-FOSS-Programmers/ford/issues
 Project-URL: Documentation, https://forddocs.readthedocs.io/en/latest/
 Keywords: Markdown,Fortran,documentation,comments
```

### Comparing `FORD-7.0.5/FORD.egg-info/SOURCES.txt` & `FORD-7.0.6/FORD.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 FORD.egg-info/requires.txt
 FORD.egg-info/top_level.txt
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/_static/ford_docs_custom.css
+docs/api/ford._markdown.rst
 docs/api/ford.external_project.rst
 docs/api/ford.fixed2free2.rst
 docs/api/ford.fortran_project.rst
 docs/api/ford.graphs.rst
 docs/api/ford.intrinsics.rst
 docs/api/ford.md_admonition.rst
 docs/api/ford.md_environ.rst
```

### Comparing `FORD-7.0.5/LICENSE` & `FORD-7.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/PKG-INFO` & `FORD-7.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FORD
-Version: 7.0.5
+Version: 7.0.6
 Summary: FORD (FORtran Documenter) is an automatic documentation generator for modern Fortran programs.
 Author-email: Chris MacMackin <cmacmackin@gmail.com>, Peter Hill <peter.hill@york.ac.uk>
 License: GPLv3
 Project-URL: Source, https://github.com/Fortran-FOSS-Programmers/ford
 Project-URL: Tracker, https://github.com/Fortran-FOSS-Programmers/ford/issues
 Project-URL: Documentation, https://forddocs.readthedocs.io/en/latest/
 Keywords: Markdown,Fortran,documentation,comments
```

### Comparing `FORD-7.0.5/README.md` & `FORD-7.0.6/README.md`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/Makefile` & `FORD-7.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/conf.py` & `FORD-7.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/developers_guide/index.rst` & `FORD-7.0.6/docs/developers_guide/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,27 @@
    At the end of parsing a particular entity, its ``_cleanup`` method
    will be called, which will do things like, for example, collating
    all the public entities in a module.
 
 #. After each file has been parsed, the lists of entities are added to
    the `Project`'s lists of all the entities in the whole project.
 
-#. After all the files have been parsed, the documentation comments are
-   converted from Markdown to HTML, recursively down from the source
-   files. At this point, metadata in the comments is also parsed.
-
 #. Entities defined in other files are now "correlated" with their
    concrete objects. This is done recursively from
    `Project.correlate`, first by finding which modules are ``use``\ d
    by each entity, and then looking up names in the corresponding
    `FortranModule`.
 
-#. Another recursive pass is done of the project to convert internal
-   `links <writing-links>` to actual HTML links using `sub_links`.
+#. After all the files have been parsed, the documentation comments
+   are converted from Markdown to HTML, recursively down from the
+   source files. At this point, metadata in the comments is also
+   parsed. Several markdown extensions, `AliasPreprocessor`,
+   `FordLinkProcessor`, `RelativeLinksTreeProcessor`, handle aliases,
+   links, and absolute to relative link conversion respectively. The
+   `MetaMarkdown` class just wraps constructing the markdown object.
 
 #. The static pages are processed with `get_page_tree`.
 
 #. `Documentation` then processes the `Jinja2
    <https://jinja.palletsprojects.com/en/3.0.x/>`_ templates to create
    the actual HTML files.
```

### Comparing `FORD-7.0.5/docs/index.rst` & `FORD-7.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/make.bat` & `FORD-7.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/callgraph.png` & `FORD-7.0.6/docs/user_guide/callgraph.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/command_line_options.rst` & `FORD-7.0.6/docs/user_guide/command_line_options.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/documentation_meta_data.rst` & `FORD-7.0.6/docs/user_guide/documentation_meta_data.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/getting_started.rst` & `FORD-7.0.6/docs/user_guide/getting_started.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/limitation.rst` & `FORD-7.0.6/docs/user_guide/limitation.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/note_box.png` & `FORD-7.0.6/docs/user_guide/note_box.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/output-example.png` & `FORD-7.0.6/docs/user_guide/output-example.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/pages-example.png` & `FORD-7.0.6/docs/user_guide/pages-example.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/project_file_options.rst` & `FORD-7.0.6/docs/user_guide/project_file_options.rst`

 * *Files 0% similar despite different names*

```diff
@@ -672,28 +672,28 @@
 
 .. _option-docmark:
 
 docmark
 ^^^^^^^
 
 The symbol(s) following an exclaimation mark which designates that a
-comment contains documentation. For excample, if the docmark was ``!``,
+comment contains documentation. For example, if the docmark was ``!``,
 comments would then be designated by ``!!``. It should not be the same
 as any other docmark. (*default:* ``!``)
 
 .. _option-docmark_alt:
 
 docmark_alt
 ^^^^^^^^^^^
 
 The symbol(s) following an exclaimation mark which designate that the
 following set of comments, until the end of the block, are all
 documentation. This mark needs only to be used at the beginning of the
 block, after which all regular comments will be treated as
-documentation. For excample, if the docmark was ``*``, comments would
+documentation. For example, if the docmark was ``*``, comments would
 then be designated by ``!*``. An example of such a block of
 documentation is provided.
 
 .. code:: fortran
 
    !* This is an example.
    !  Here is another line of comments.
@@ -712,15 +712,15 @@
 .. _option-predocmark:
 
 predocmark
 ^^^^^^^^^^
 
 The symbol(s) following an exclaimation mark which designates that a
 comment contains documentation preceding the code which it is
-documenting. For excample, if the docmark was ``>``, comments would then
+documenting. For example, if the docmark was ``>``, comments would then
 be designated by ``!>``. It should not be the same as any other docmark.
 (*default:* ``>``)
 
 .. _option-predocmark_alt:
 
 predocmark_alt
 ^^^^^^^^^^^^^^
```

### Comparing `FORD-7.0.5/docs/user_guide/running_ford.rst` & `FORD-7.0.6/docs/user_guide/running_ford.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/say_hello_example.png` & `FORD-7.0.6/docs/user_guide/say_hello_example.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/docs/user_guide/writing_documentation.rst` & `FORD-7.0.6/docs/user_guide/writing_documentation.rst`

 * *Files 17% similar despite different names*

```diff
@@ -41,15 +41,15 @@
            !! The number of cats to keep track of.
        integer, intent(in)  :: dogs
            !! The number of dogs to keep track of.
        real, intent(inout)  :: food
            !! The ammount of pet food (in kilograms) which you have on hand.
        integer, intent(out) :: angry
            !! The number of pets angry because they weren't fed.
-           
+
        !...
        return
    end subroutine feed_pets
 
 looks better/more readable than::
 
    !! Feeds your cats and dogs, if enough food is available. If not enough
@@ -61,15 +61,15 @@
        integer, intent(in)  :: cats
        !! The number of dogs to keep track of.
        integer, intent(in)  :: dogs
        !! The ammount of pet food (in kilograms) which you have on hand.
        real, intent(inout)  :: food
        !! The number of pets angry because they weren't fed.
        integer, intent(out) :: angry
-           
+
        !...
        return
    end subroutine feed_pets
 
 in the opinion of this author, especially with regards to the list of
 arguments. Since version 1.0.0 it is now possible to place
 documentation before the code which it is documenting. To do so, use
@@ -276,43 +276,81 @@
    module, or anything else with its own page of documentation. This is
    the only item which is mandatory.
 -  ``type`` (optional) is ``component``\ ’s type of Fortran construct.
    This is necessary if you have multiple items with the same name (such
    as a type and its public constructor). If multiple items with the
    same name exist and ``type`` is not specified then FORD’s behaviour
    is undefined; it will link to the first of those items which it
-   finds. The available options are “procedure”, “subroutine”,
-   “function”, “proc” (all of which are interchangeable and specify a
-   procedure), “interface”, “absinterface” (both of which are for
-   abstract interfaces), “block” (for the legacy ``block data`` program
-   unit), and “type”, “file”, “module”, and “program” (which are
-   self-explanatory).
+   finds. The available options are:
+
+   - "procedure", "proc", "subroutine", "function" for any kind of
+     procedure defined within the project
+   - "interface", "absinterface" for abstract interfaces
+   - "block" for the legacy ``block data`` construct
+   - "type"
+   - "file"
+   - "module"
+   - "submodule"
+   - "program"
+   - "namelist"
+
+   The majority of these can also be prefixed with "ext" to refer to
+   entities defined in `external projects <option-external>`
 -  ``item`` (optional) specifies an item within ``component`` which is
    to be linked to. The link’s target will be ``item``\ ’s location on
    ``component``\ ’s page. If ``item`` is not present then the colon in
    the link must be omitted.
 -  ``type`` (optional, but ``item`` must also be present) is
    ``item``\ ’s type of Fortran construct. It can be used in the same
-   manner as the component ``type``, but has different options. These
-   are “variable”, “type”, “constructor”, “interface”, “absinterface”
-   (abstract interface), “subroutine”, “function”, “final” (finalization
-   procedure), “bound” (type-bound procedure), “modproc” (module
-   procedure in a generic interface block), and “common”. None of these
-   options are interchangeable. If no description is given then its
-   meaning should be self-explanatory. If you specify an option that can
-   not exist within ``component`` (for example, if ``component`` is a
-   module and ``item`` is “bound”) then a warning message is issued and
-   the link is not generated.
+   manner as the component ``type``, but has different options:
+
+   - "absinterface" for abstract interfaces
+   - "bound" for type-bound procedures
+   - "common" for ``common`` blocks
+   - "constructor" for structure constructor procedures
+   - "final" for finalization procedures
+   - "function"
+   - "interface"
+   - "modproc" for module procedures in generic interfaces
+   - "subroutine"
+   - "type"
+   - "variable"
+
+   None of these options are interchangeable. If you specify an option
+   that can not exist within ``component`` (for example, if
+   ``component`` is a module and ``item`` is “bound”) then a warning
+   message is issued and the link is not generated.
+
+For example, to link to a module called ``my_mod`` you could
+use ``[[my_mod]]`` or ``[[my_mod(module)]]``, while if you wanted to
+refer to a function called ``my_function`` in that module you could
+use any of (from least to most specific):
+
+- ``[[my_function]]``
+- ``[[my_function(function)]]``
+- ``[[my_function(proc)]]``
+- ``[[my_mod:my_function]]``
+- ``[[my_mod(module):my_function]]``
+- ``[[my_mod:my_function(function)]]``
+- ``[[my_mod(module):my_function(function)]]``
 
 If you have an overridden constructor a derived type, then it is
 strongly recommended that you specify ``item`` should you wish to link
 to either of them. Otherwise FORD will not know whether you are
 referring to the derived type itself or the interface for its
 constructor.
 
+.. versionchanged:: 7.0.0
+   Previously, links inside code blocks (with backticks) were
+   resolved, now they are left verbatim, as with all other
+   markup. That is, pre-v7, ```call [[my_subroutine]]``` would be
+   rendered as ``call my_subroutine`` with a link to
+   ``my_subroutine``, while now it will be left as: ``call
+   [[my_subroutine]]``.
+
 .. _non-fortran-source-files:
 
 Non-Fortran Source Files
 ------------------------
 
 As of version 4.5.0, FORD now offers limited support for non-Fortran
 source files. While it will not analyze the code within such files, it
```

### Comparing `FORD-7.0.5/docs/user_guide/writing_pages.rst` & `FORD-7.0.6/docs/user_guide/writing_pages.rst`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/example-project-file.md` & `FORD-7.0.6/example/example-project-file.md`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/images/Fortran_logo.svg` & `FORD-7.0.6/example/images/Fortran_logo.svg`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/pages/index.md` & `FORD-7.0.6/example/pages/index.md`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/src/ford_example_type.f90` & `FORD-7.0.6/example/src/ford_example_type.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/src/ford_f77_example.f` & `FORD-7.0.6/example/src/ford_f77_example.f`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/src/ford_interfaces.f90` & `FORD-7.0.6/example/src/ford_interfaces.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/src/ford_test_module.fpp` & `FORD-7.0.6/example/src/ford_test_module.fpp`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/example/src/ford_test_program.f90` & `FORD-7.0.6/example/src/ford_test_program.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/__init__.py` & `FORD-7.0.6/ford/__init__.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/_markdown.py` & `FORD-7.0.6/ford/_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         md_base: PathLike = ".",
         base_url: PathLike = ".",
         extensions: Optional[List[Union[str, Extension]]] = None,
         extension_configs: Optional[Dict[str, Dict]] = None,
         aliases: Optional[Dict[str, str]] = None,
         project: Optional[Project] = None,
     ):
-        """make thing"""
 
         default_extensions: List[Union[str, Extension]] = [
             "markdown_include.include",
             "markdown.extensions.codehilite",
             "markdown.extensions.extra",
             "mdx_math",
             EnvironExtension(),
```

### Comparing `FORD-7.0.5/ford/config.json` & `FORD-7.0.6/ford/config.json`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/css/font-awesome.css` & `FORD-7.0.6/ford/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/css/font-awesome.min.css` & `FORD-7.0.6/ford/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/css/local.css` & `FORD-7.0.6/ford/css/local.css`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/css/pygments.css` & `FORD-7.0.6/ford/css/pygments.css`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/external_project.py` & `FORD-7.0.6/ford/external_project.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/favicon.png` & `FORD-7.0.6/ford/favicon.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fixed2free2.py` & `FORD-7.0.6/ford/fixed2free2.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/FontAwesome.otf` & `FORD-7.0.6/ford/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/fontawesome-webfont.eot` & `FORD-7.0.6/ford/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/fontawesome-webfont.svg` & `FORD-7.0.6/ford/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/fontawesome-webfont.ttf` & `FORD-7.0.6/ford/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/fontawesome-webfont.woff` & `FORD-7.0.6/ford/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.eot` & `FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.svg` & `FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.ttf` & `FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fonts/glyphicons-halflings-regular.woff` & `FORD-7.0.6/ford/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/fortran_project.py` & `FORD-7.0.6/ford/fortran_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 )
 from ford.settings import ProjectSettings
 from ford._typing import PathLike
 
 
 LINK_TYPES = {
     "module": "modules",
+    "submodule": "submodules",
     "extmodule": "extModules",
     "type": "types",
     "exttype": "extTypes",
     "procedure": "procedures",
     "extprocedure": "extProcedures",
     "subroutine": "procedures",
     "extsubroutine": "extProcedures",
@@ -178,15 +179,17 @@
                     self._fortran_file(extension, filename, settings)
                 elif extension in self.extra_filetypes:
                     self.extra_files.append(GenericSource(filename, settings))
             except Exception as e:
                 if not settings.dbg:
                     raise e
 
-                warn(f"Error parsing {relative_path}.\n\t{e.args[0]}")
+                warn(
+                    f"Error parsing {relative_path}.\n\t{e.args if len(e.args) == 0 else e.args[0]}"
+                )
                 continue
 
     def _fortran_file(
         self, extension: str, filename: PathLike, settings: ProjectSettings
     ):
         if extension in settings.fpp_extensions:
             preprocessor = settings.preprocessor.split()
@@ -422,15 +425,15 @@
 
         """
 
         item = None
 
         if entity is not None:
             try:
-                collection = getattr(self, LINK_TYPES[entity])
+                collection = getattr(self, LINK_TYPES[entity.lower()])
             except KeyError:
                 raise ValueError(f"Unknown class of entity {entity!r}")
         else:
             collection = chain(
                 *(getattr(self, collection) for collection in LINK_TYPES.values())
             )
```

### Comparing `FORD-7.0.5/ford/graphs.py` & `FORD-7.0.6/ford/graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,16 +332,15 @@
                 ExternalFunction,
                 ExternalInterface,
                 ExternalSubroutine,
                 ExternalProgram,
                 ExternalSourceFile,
             ),
         ):
-            self.fromstr = True
-            obj = obj.name
+            obj = str(obj)
 
         self.url = None
         if isinstance(obj, str):
             self.fromstr = True
             if m := HYPERLINK_RE.match(obj):
                 self.url = m.group(1)[1:-1]
                 self.name = m.group(2)
@@ -468,15 +467,15 @@
         "boundproc": "#A7506F",
     }
 
     @property
     def colour(self):
         return ProcNode.COLOURS.get(self.proctype, super().colour)
 
-    def __init__(self, obj, gd, hist=None):
+    def __init__(self, obj, gd: GraphData, hist=None):
         # ToDo: Figure out appropriate way to handle interfaces to routines in submodules.
         self.proctype = getattr(obj, "proctype", "").lower()
         if self.proctype == "" and isinstance(obj, FortranBoundProcedure):
             self.proctype = "boundproc"
         super().__init__(obj, gd)
 
         if isinstance(obj, FortranBoundProcedure):
@@ -484,15 +483,15 @@
             parent = getattr(binder, "parent", None)
         else:
             parent = getattr(obj, "parent", None)
             binder = getattr(getattr(obj, "binding", None), "parent", None)
 
         parent_label = ""
         binding_label = ""
-        if parent:
+        if parent and gd.show_proc_parent:
             parent_label = f"{parent.name}::"
         if binder:
             binding_label = f"{binder.name}%"
 
         self.attribs["label"] = f"{parent_label}{binding_label}{self.name}"
 
         self.uses = set()
@@ -882,22 +881,25 @@
         graph_as_table = len(self.hop_nodes) > 0 and len(self.root) == 1
 
         # Do not render empty graphs
         if len(self.added) <= 1 and not graph_as_table:
             return ""
 
         # Do not render overly large graphs.
-        if len(self.added) > self.max_nodes and self.warn:
-            warn(
-                f"Not showing graph {self.ident} as it would exceed the maximal number of {self.max_nodes} nodes"
-            )
+        if len(self.added) > self.max_nodes:
+            if self.warn:
+                warn(
+                    f"Not showing graph {self.ident} as it would exceed the maximal number of {self.max_nodes} nodes"
+                )
             return ""
+
         # Do not render incomplete graphs.
-        if len(self.added) < len(self.root) and self.warn:
-            warn(f"Not showing graph {self.ident} as it would be incomplete")
+        if len(self.added) < len(self.root):
+            if self.warn:
+                warn(f"Not showing graph {self.ident} as it would be incomplete")
             return ""
 
         if self.truncated > 0 and self.warn:
             warn(f"Graph {self.ident} is truncated after {self.truncated} hops")
 
         if graph_as_table:
             rettext = self._make_graph_as_table()
@@ -1017,15 +1019,15 @@
 
         total_len = len(nodes)
 
         def rainbowcolour(depth, maxd):
             if not self.data.coloured_edges:
                 return "#000000"
             (r, g, b) = colorsys.hsv_to_rgb(float(depth) / maxd, 1.0, 1.0)
-            return f"#{int(255 * r)}{int(255 * g)}{int(255 * b)}"
+            return f"#{int(255 * r):02X}{int(255 * g):02X}{int(255 * b):02X}"
 
         for i, node in enumerate(sorted(nodes)):
             colour = rainbowcolour(i, total_len)
 
             self._add_node(hop_nodes, hop_edges, node, colour)
 
         if not self.add_to_graph(hop_nodes, hop_edges, nesting):
@@ -1385,17 +1387,19 @@
             elif is_proc(obj):
                 obj.callsgraph = CallsGraph(obj, self.data)
                 obj.calledbygraph = CalledByGraph(obj, self.data)
                 obj.usesgraph = UsesGraph(obj, self.data)
                 self.procedures.add(obj)
                 # regester internal procedures
                 for p in traverse(obj, ["subroutines", "functions"]):
-                    self.internal_procedures.add(p) if getattr(
-                        p, "visible", False
-                    ) else None
+                    (
+                        self.internal_procedures.add(p)
+                        if getattr(p, "visible", False)
+                        else None
+                    )
             elif is_program(obj):
                 obj.usesgraph = UsesGraph(obj, self.data)
                 obj.callsgraph = CallsGraph(obj, self.data)
                 self.programs.add(obj)
             elif is_sourcefile(obj):
                 obj.afferentgraph = AfferentGraph(obj, self.data)
                 obj.efferentgraph = EfferentGraph(obj, self.data)
```

### Comparing `FORD-7.0.5/ford/intrinsics.py` & `FORD-7.0.6/ford/intrinsics.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/js/svg-pan-zoom.min.js` & `FORD-7.0.6/ford/js/svg-pan-zoom.min.js`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/md_admonition.py` & `FORD-7.0.6/ford/md_admonition.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/md_environ.py` & `FORD-7.0.6/ford/md_environ.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/md_striped_table.py` & `FORD-7.0.6/ford/md_striped_table.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/output.py` & `FORD-7.0.6/ford/output.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/pagetree.py` & `FORD-7.0.6/ford/pagetree.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/reader.py` & `FORD-7.0.6/ford/reader.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/settings.py` & `FORD-7.0.6/ford/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
     """Convert the cargs dict's value's types to be consistent with a given dataclass
     if set and override them in settings.
     """
 
     field_types = get_type_hints(type(settings))
 
     for key, value in cargs.items():
-        if value != None:
+        if value is not None:
             if key in field_types:
                 setattr(settings, key, convert_setting(field_types[key], key, value))
             else:
                 setattr(settings, key, value)
 
     return settings
```

### Comparing `FORD-7.0.5/ford/sourceform.py` & `FORD-7.0.6/ford/sourceform.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from pygments import highlight
 from pygments.lexers import FortranLexer, FortranFixedLexer, guess_lexer_for_filename
 from pygments.formatters import HtmlFormatter
 
 from ford.console import warn
 from ford.reader import FortranReader
 import ford.utils
+from ford.utils import paren_split, strip_paren
 from ford.intrinsics import INTRINSICS
 from ford._markdown import MetaMarkdown
 from ford.settings import ProjectSettings, EntitySettings
 from ford._typing import PathLike
 
 if TYPE_CHECKING:
     from ford.fortran_project import Project
@@ -105,15 +106,15 @@
 
 def _find_in_list(collection: Iterable, name: str) -> Optional[FortranBase]:
     for item in collection:
         # `item` might still be a string if we've not managed to
         # correlate it for whatever reason, if so skip it
         if not isinstance(item, FortranBase):
             continue
-        if name == item.name.lower():
+        if name.lower() == item.name.lower():
             return item
     return None
 
 
 def read_docstring(source: FortranReader, docmark: str) -> List[str]:
     """Read a contiguous docstring"""
     docstring = []
@@ -337,14 +338,15 @@
             return str(self.base_url / url)
 
         return None
 
     def lines_description(self, total, total_all=0, obj=None):
         if not obj:
             obj = self.obj
+        total = total or self.num_lines
         description = f"{float(self.num_lines) / total * 100:4.1f}% of total for {self.pretty_obj[obj]}."
         if total_all:
             description = (
                 f"<p>{description}</p>Including implementation: {self.num_lines_all} statements, "
                 f"{float(self.num_lines_all) / total_all * 100:4.1f}% of total for {self.pretty_obj[obj]}."
             )
         return description
@@ -585,15 +587,15 @@
         Optional[FortranBase]
             Child if found, `None` if not
 
         """
 
         if entity is not None:
             try:
-                collection_name = SUBLINK_TYPES[entity]
+                collection_name = SUBLINK_TYPES[entity.lower()]
             except KeyError:
                 raise ValueError(f"Unknown class of entity {entity!r}")
             if not hasattr(self, collection_name):
                 raise ValueError(f"{self.obj!r} cannot have child {entity!r}")
             # Ensure this is a list, as constructors are single items
             collection = list(getattr(self, collection_name))
         else:
@@ -854,15 +856,15 @@
                         describe_object=False,
                     )
                 endtype = match.group(1)
                 if endtype and endtype.lower() == "block":
                     blocklevel -= 1
                 elif endtype and endtype.lower() == "associate":
                     associations.remove_last_batch()
-                else:
+                elif blocklevel == 0:
                     self._cleanup()
                     return
 
             elif (match := self.MODPROC_RE.match(line)) and (
                 match["module"] or isinstance(self, FortranInterface)
             ):
                 if isinstance(self, FortranInterface):
@@ -888,17 +890,15 @@
             elif self.BLOCK_RE.match(line):
                 blocklevel += 1
             elif match := self.ASSOCIATE_RE.match(line):
                 # Associations 'call' the rhs of the => operator
                 self._add_procedure_calls(line, associations)
 
                 # Register the associations
-                assoc_batch = ford.utils.strip_paren(match["associations"])[0].split(
-                    ","
-                )
+                assoc_batch = paren_split(",", strip_paren(match["associations"])[0])
                 associations.add_batch(assoc_batch)
 
             elif match := self.MODULE_RE.match(line):
                 if hasattr(self, "modules"):
                     self.modules.append(FortranModule(source, match, self))
                     self.num_lines += self.modules[-1].num_lines - 1
                 else:
@@ -1384,14 +1384,22 @@
                 "interfaces",
                 "absinterfaces",
                 "variables",
             )
             if item.permission == "public"
         ] + [item for item, attr in self.attr_dict.items() if "public" in attr]
 
+        if self.settings.warn:
+            for item, values in self.attr_dict.items():
+                for value in values:
+                    warn(
+                        f"Unknown entity '{item}' with attribute '{value}' in {self.obj} "
+                        f"'{self.name}' ('{self.filename}')"
+                    )
+
         del self.attr_dict
 
     def prune(self):
         """
         Remove anything which shouldn't be displayed.
         """
 
@@ -1599,16 +1607,14 @@
 
     def _initialize(self, line: re.Match) -> None:
         self.name = line["name"]
         self._common_initialize()
         del self.calls
         self.descendants: List[FortranSubmodule] = []
         self.modprocedures: List[FortranModuleProcedureImplementation] = []
-        self.private_list: List[str] = []
-        self.protected_list: List[str] = []
         self.visible = True
         self.deplist: List[FortranModule] = []
 
     def _cleanup(self):
         """Create list of all local procedures. Ones coming from other modules
         will be added later, during correlation."""
         super()._cleanup()
@@ -1673,16 +1679,14 @@
     def _initialize(self, line: re.Match) -> None:
         super()._initialize(line)
         self.parent_submodule: Union[str, None, FortranSubmodule] = line[
             "parent_submod"
         ]
         self.ancestor_module: Union[str, FortranModule] = line["ancestor_module"]
         del self.public_list
-        del self.private_list
-        del self.protected_list
 
     def get_dir(self):
         return "module"
 
 
 def _list_of_procedure_attributes(
     attribute_string: Optional[str],
@@ -1958,28 +1962,28 @@
     components and type-bound procedures. It also contains information on the
     type's inheritance.
     """
 
     def _initialize(self, line: re.Match) -> None:
         self.name = line.group(2)
         self.extends = None
-        self.attributes = []
+        self.attribs = []
         if line.group(1):
             attribstr = line.group(1)[1:].strip()
             attriblist = self.SPLIT_RE.split(attribstr.strip())
             for attrib in attriblist:
                 attrib_lower = attrib.strip().lower()
                 if extends := EXTENDS_RE.search(attrib):
                     self.extends = extends["base"]
                 elif attrib_lower in ["public", "private"]:
                     self.permission = attrib_lower
                 elif attrib_lower == "external":
-                    self.attributes.append("external")
+                    self.attribs.append("external")
                 else:
-                    self.attributes.append(attrib.strip())
+                    self.attribs.append(attrib.strip())
         if line.group(3):
             paramstr = line.group(3).strip()
             self.parameters = self.SPLIT_RE.split(paramstr)
         else:
             self.parameters = []
         self.sequence = False
         self.variables: List[FortranVariable] = []
@@ -3264,27 +3268,30 @@
 class ExternalSubmodule(FortranSubmodule):
     def __init__(self, name: str):
         self.name = name
         self.url = ""
         self.uses = []
         self.parent_submodule = None
         self.ancestor_module = ExternalModule("Parent module")
+        self.external_url = ""
 
 
 class ExternalProgram(FortranProgram):
     def __init__(self, name: str):
         self.name = name
         self.url = ""
         self.uses = []
         self.calls = []
+        self.external_url = ""
 
 
 class ExternalSourceFile(FortranSourceFile):
     def __init__(self, name: str):
         self.name = name
         self.url = ""
         self.modules = []
         self.submodules = []
         self.functions = []
         self.subroutines = []
         self.programs = []
         self.blockdata = []
+        self.external_url = ""
```

### Comparing `FORD-7.0.5/ford/templates/absint_list.html` & `FORD-7.0.6/ford/templates/absint_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/base.html` & `FORD-7.0.6/ford/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,30 @@
               {% if incl_src %}
                 {% if (project.files|length + project.extra_files|length) is more_than_one %}
                   <li class="nav-item">
                     <a class="nav-link" href="{{ project_url }}/lists/files.html">Source Files</a>
                   </li>
                 {% else %}
                   <li class="nav-item">
-                    <a class="nav-link" href="{{project.files[0].get_url()}}">Source File</a>
+                    <a class="nav-link" href="{{ project_url }}/{{project.files[0].get_url()}}">Source File</a>
                   </li>
                 {% endif %}
               {% endif %}
               {% if project.modules %}
                 <li class="nav-item">
                   <a class="nav-link" href="{{ project_url }}/lists/modules.html">Modules</a>
                 </li>
               {% endif %}
               {% if project.blockdata|length is more_than_one %}
                 <li class="nav-item">
                   <a class="nav-link" href="{{ project_url }}/lists/blockdata.html">Block Data</a>
                 </li>
               {% elif project.blockdata|length == 1 %}
                 <li class="nav-item">
-                  <a class="nav-link" href="{{ project.blockdata[0].get_url() }}">Block Data</a>
+                  <a class="nav-link" href="{{ project_url }}/{{ project.blockdata[0].get_url() }}">Block Data</a>
                 </li>
               {% endif %}
               {% if project.procedures %}
                 <li class="nav-item">
                   <a class="nav-link" href="{{ project_url }}/lists/procedures.html">Procedures</a>
                 </li>
               {% endif %}
@@ -128,15 +128,19 @@
       {% block body %}
       {% endblock body %}
       <hr>
     </div> <!-- /container -->
     <footer>
       <div class="container">
         <div class="row justify-content-between">
-          <div class="col"><p>{{ project }} was developed by {{ author }}<br>&copy; {{ year }} {{ license }}
+          <div class="col">
+            <p>
+              {{ project }}
+              {% if author %} was developed by {{ author }}<br>{% endif %}
+              &copy; {{ year }} {{ license }}
               {% if revision %}<br /><small>{{ revision }}</small>{% endif %}</p>
           </div>
           <div class="col">
             <p class="text-end">
               Documentation generated by
               <a href="https://github.com/Fortran-FOSS-Programmers/ford">FORD</a>
               {% if print_creation_date %} on {{ creation_date }} {% endif %}
```

#### html2text {}

```diff
@@ -36,16 +36,16 @@
     * _T_e_r_m_s_ _O_f_ _S_e_r_v_i_c_e
     * {% endif %}
 {% if search %}
 [q                   ]
 {% endif %}
 {% block body %} {% endblock body %}
 ===============================================================================
-{{ project }} was developed by {{ author }}
-© {{ year }} {{ license }} {% if revision %}
+{{ project }} {% if author %} was developed by {{ author }}
+{% endif %} © {{ year }} {{ license }} {% if revision %}
 {{ revision }}{% endif %}
 Documentation generated by _F_O_R_D {% if print_creation_date %} on {
 { creation_date }} {% endif %} {% if doc_license %}
 © {{ doc_license }} {% endif %}
 
 {% if mathjax_config %}
 {% endif %}
```

### Comparing `FORD-7.0.5/ford/templates/block_list.html` & `FORD-7.0.6/ford/templates/block_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/block_page.html` & `FORD-7.0.6/ford/templates/block_page.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,38 +18,38 @@
     </div>
     
     <div class="col-md-9" id='text'>
     {{ macros.use_list(blockdat) }}
     {{ blockdat.doc }}
     <br>
 
-    {% if blockdat.common|length > 0 %}
+    {% if blockdat.common %}
     <section>
       <h2>Common Blocks</h2>
       {% for com in blockdat.common %}
       {{ macros.common_block(com) }}
       {% endfor %}
     </section>
     <br>
     <script>
       $(function () {
       $('[data-bs-toggle="popover"]').popover()
       })
     </script>
     {% endif %}
 
-    {% if blockdat.variables|length > 0 %}
+    {% if blockdat.variables %}
     <section>
     <h2>Variables</h2>
     {{ macros.variable_list(blockdat.variables) }}
     </section>
     <br>
     {% endif %}
     
-    {% if blockdat.types|length > 0 %}
+    {% if blockdat.types %}
     <section>
      <h2>Derived Types</h2>
    {% for type in blockdat.types %}
      {{ macros.type_summary(type) }}
      {% endfor %}
     </section>
   <br>
```

### Comparing `FORD-7.0.5/ford/templates/file_list.html` & `FORD-7.0.6/ford/templates/file_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/file_page.html` & `FORD-7.0.6/ford/templates/file_page.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/genint_page.html` & `FORD-7.0.6/ford/templates/genint_page.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/index.html` & `FORD-7.0.6/ford/templates/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,428 +1,380 @@
-00000000: 7b25 2065 7874 656e 6473 2022 6261 7365  {% extends "base
-00000010: 2e68 746d 6c22 2025 7d0a 7b25 2062 6c6f  .html" %}.{% blo
-00000020: 636b 2062 6f64 7920 257d 0a20 2020 2020  ck body %}.     
-00000030: 203c 212d 2d20 4d61 696e 2063 6f6d 706f   <!-- Main compo
-00000040: 6e65 6e74 2066 6f72 2061 2070 7269 6d61  nent for a prima
-00000050: 7279 206d 6172 6b65 7469 6e67 206d 6573  ry marketing mes
-00000060: 7361 6765 206f 7220 6361 6c6c 2074 6f20  sage or call to 
-00000070: 6163 7469 6f6e 202d 2d3e 0a20 2020 2020  action -->.     
-00000080: 203c 6469 7620 636c 6173 733d 2270 2d35   <div class="p-5
-00000090: 206d 622d 3420 6267 2d6c 6967 6874 2062   mb-4 bg-light b
-000000a0: 6f72 6465 7220 726f 756e 6465 642d 3322  order rounded-3"
-000000b0: 2069 643d 226a 756d 626f 7472 6f6e 223e   id="jumbotron">
-000000c0: 0a20 2020 2020 2020 207b 7b20 7375 6d6d  .        {{ summ
-000000d0: 6172 7920 7d7d 0a20 2020 2020 2020 2009  ary }}.        .
-000000e0: 207b 2520 6966 2070 726f 6a65 6374 5f67   {% if project_g
-000000f0: 6974 6875 6220 6f72 2070 726f 6a65 6374  ithub or project
-00000100: 5f62 6974 6275 636b 6574 206f 7220 7072  _bitbucket or pr
-00000110: 6f6a 6563 745f 6769 746c 6162 206f 7220  oject_gitlab or 
-00000120: 7072 6f6a 6563 745f 736f 7572 6365 666f  project_sourcefo
-00000130: 7267 6520 6f72 2070 726f 6a65 6374 5f77  rge or project_w
-00000140: 6562 7369 7465 2025 7d0a 093c 703e 2046  ebsite %}..<p> F
-00000150: 696e 6420 7573 206f 6e26 6865 6c6c 6970  ind us on&hellip
-00000160: 3b3c 2f70 3e0a 2020 2020 2020 2020 3c70  ;</p>.        <p
-00000170: 3e0a 0909 0920 7b25 2069 6620 7072 6f6a  >.... {% if proj
-00000180: 6563 745f 6769 7468 7562 2025 7d0a 2020  ect_github %}.  
-00000190: 2020 2020 2020 2020 3c61 2063 6c61 7373          <a class
-000001a0: 3d22 6274 6e20 6274 6e2d 6c67 2062 746e  ="btn btn-lg btn
-000001b0: 2d70 7269 6d61 7279 2220 6872 6566 3d22  -primary" href="
-000001c0: 7b7b 2070 726f 6a65 6374 5f67 6974 6875  {{ project_githu
-000001d0: 6220 7d7d 2220 726f 6c65 3d22 6275 7474  b }}" role="butt
-000001e0: 6f6e 223e 4769 7448 7562 3c2f 613e 0a09  on">GitHub</a>..
-000001f0: 0909 207b 2520 656e 6469 6620 257d 0a09  .. {% endif %}..
-00000200: 0909 207b 2520 6966 2070 726f 6a65 6374  .. {% if project
-00000210: 5f67 6974 6c61 6220 257d 0a20 2020 2020  _gitlab %}.     
-00000220: 2020 2020 203c 6120 636c 6173 733d 2262       <a class="b
-00000230: 746e 2062 746e 2d6c 6720 6274 6e2d 7072  tn btn-lg btn-pr
-00000240: 696d 6172 7922 2068 7265 663d 227b 7b20  imary" href="{{ 
-00000250: 7072 6f6a 6563 745f 6769 746c 6162 207d  project_gitlab }
-00000260: 7d22 2072 6f6c 653d 2262 7574 746f 6e22  }" role="button"
-00000270: 3e54 6865 2057 6562 3c2f 613e 0a09 0909  >The Web</a>....
-00000280: 207b 2520 656e 6469 6620 257d 0a09 0909   {% endif %}....
-00000290: 207b 2520 6966 2070 726f 6a65 6374 5f62   {% if project_b
-000002a0: 6974 6275 636b 6574 2025 7d0a 2020 2020  itbucket %}.    
-000002b0: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
-000002c0: 6274 6e20 6274 6e2d 6c67 2062 746e 2d70  btn btn-lg btn-p
-000002d0: 7269 6d61 7279 2220 6872 6566 3d22 7b7b  rimary" href="{{
-000002e0: 2070 726f 6a65 6374 5f62 6974 6275 636b   project_bitbuck
-000002f0: 6574 207d 7d22 2072 6f6c 653d 2262 7574  et }}" role="but
-00000300: 746f 6e22 3e42 6974 6275 636b 6574 3c2f  ton">Bitbucket</
-00000310: 613e 0a09 0909 207b 2520 656e 6469 6620  a>.... {% endif 
-00000320: 257d 0a09 0909 207b 2520 6966 2070 726f  %}.... {% if pro
-00000330: 6a65 6374 5f73 6f75 7263 6566 6f72 6765  ject_sourceforge
-00000340: 2025 7d0a 2020 2020 2020 2020 2020 3c61   %}.          <a
-00000350: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
-00000360: 6c67 2062 746e 2d70 7269 6d61 7279 2220  lg btn-primary" 
-00000370: 6872 6566 3d22 7b7b 2070 726f 6a65 6374  href="{{ project
-00000380: 5f73 6f75 7263 6566 6f72 6765 207d 7d22  _sourceforge }}"
-00000390: 2072 6f6c 653d 2262 7574 746f 6e22 3e53   role="button">S
-000003a0: 6f75 7263 6566 6f72 6765 3c2f 613e 0a09  ourceforge</a>..
-000003b0: 0909 207b 2520 656e 6469 6620 257d 0a09  .. {% endif %}..
-000003c0: 0909 207b 2520 6966 2070 726f 6a65 6374  .. {% if project
-000003d0: 5f77 6562 7369 7465 2025 7d0a 2020 2020  _website %}.    
-000003e0: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
-000003f0: 6274 6e20 6274 6e2d 6c67 2062 746e 2d70  btn btn-lg btn-p
-00000400: 7269 6d61 7279 2220 6872 6566 3d22 7b7b  rimary" href="{{
-00000410: 2070 726f 6a65 6374 5f77 6562 7369 7465   project_website
-00000420: 207d 7d22 2072 6f6c 653d 2262 7574 746f   }}" role="butto
-00000430: 6e22 3e54 6865 2057 6562 3c2f 613e 0a09  n">The Web</a>..
-00000440: 0909 207b 2520 656e 6469 6620 257d 0a09  .. {% endif %}..
-00000450: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-00000460: 6620 257d 0a09 0909 207b 2520 6966 2070  f %}.... {% if p
-00000470: 726f 6a65 6374 5f64 6f77 6e6c 6f61 6420  roject_download 
-00000480: 257d 0a20 2020 2020 2020 2020 203c 6120  %}.          <a 
-00000490: 636c 6173 733d 2262 746e 2062 746e 2d6c  class="btn btn-l
-000004a0: 6720 6274 6e2d 6461 6e67 6572 2220 7374  g btn-danger" st
-000004b0: 796c 653d 2266 6c6f 6174 3a72 6967 6874  yle="float:right
-000004c0: 2220 6872 6566 3d22 7b7b 2070 726f 6a65  " href="{{ proje
-000004d0: 6374 5f64 6f77 6e6c 6f61 6420 7d7d 2220  ct_download }}" 
-000004e0: 726f 6c65 3d22 6275 7474 6f6e 223e 446f  role="button">Do
-000004f0: 776e 6c6f 6164 2074 6865 2053 6f75 7263  wnload the Sourc
-00000500: 653c 2f61 3e0a 0909 0920 7b25 2065 6e64  e</a>.... {% end
-00000510: 6966 2025 7d0a 2020 2020 2020 2020 3c2f  if %}.        </
-00000520: 703e 0a20 2020 2020 203c 2f64 6976 3e0a  p>.      </div>.
-00000530: 0a20 2020 2020 203c 6469 7620 636c 6173  .      <div clas
-00000540: 733d 2272 6f77 2220 6964 3d27 7465 7874  s="row" id='text
-00000550: 273e 0a09 097b 2520 7365 7420 636f 6c20  '>...{% set col 
-00000560: 3d20 2263 6f6c 2d6d 642d 3822 2069 6620  = "col-md-8" if 
-00000570: 6175 7468 6f72 2065 6c73 6520 2263 6f6c  author else "col
-00000580: 2d6d 642d 3132 2225 7d0a 2020 2020 2020  -md-12"%}.      
-00000590: 2020 3c64 6976 2063 6c61 7373 3d7b 7b20    <div class={{ 
-000005a0: 636f 6c20 7d7d 3e0a 2020 2020 2020 2020  col }}>.        
-000005b0: 2020 3c68 313e 7b7b 2070 726f 6a65 6374    <h1>{{ project
-000005c0: 207d 7d3c 2f68 313e 0a20 2020 2020 2020   }}</h1>.       
-000005d0: 2020 207b 7b20 7072 6f6a 5f64 6f63 7320     {{ proj_docs 
-000005e0: 7d7d 0a20 2020 2020 2020 203c 2f64 6976  }}.        </div
-000005f0: 3e0a 0909 7b25 2069 6620 6175 7468 6f72  >...{% if author
-00000600: 2025 7d0a 2020 2020 2020 2020 2020 3c64   %}.          <d
-00000610: 6976 2063 6c61 7373 3d22 636f 6c2d 6d64  iv class="col-md
-00000620: 2d34 223e 0a09 2020 2020 2020 2020 3c64  -4">..        <d
-00000630: 6976 2063 6c61 7373 3d22 6361 7264 2063  iv class="card c
-00000640: 6172 642d 626f 6479 2062 672d 6c69 6768  ard-body bg-ligh
-00000650: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00000660: 2020 7b25 2069 6620 6175 7468 6f72 5f70    {% if author_p
-00000670: 6963 2025 7d0a 2020 2020 2009 0920 2020  ic %}.     ..   
-00000680: 203c 696d 6720 7372 633d 227b 7b20 6175   <img src="{{ au
-00000690: 7468 6f72 5f70 6963 207d 7d22 2061 6c74  thor_pic }}" alt
-000006a0: 3d22 4465 7665 6c6f 7065 7220 7069 6374  ="Developer pict
-000006b0: 7572 6522 2063 6c61 7373 3d22 6361 7264  ure" class="card
-000006c0: 2d69 6d67 2d74 6f70 223e 0a20 2020 2009  -img-top">.    .
-000006d0: 0920 207b 2520 656e 6469 6620 257d 0a20  .  {% endif %}. 
-000006e0: 2020 2020 2020 2020 2020 2020 203c 6832               <h2
-000006f0: 2063 6c61 7373 3d22 6361 7264 2d74 6974   class="card-tit
-00000700: 6c65 223e 4465 7665 6c6f 7065 7220 496e  le">Developer In
-00000710: 666f 3c2f 6832 3e0a 2020 2020 2020 2020  fo</h2>.        
-00000720: 2020 2020 2020 3c68 3420 636c 6173 733d        <h4 class=
-00000730: 2263 6172 642d 7465 7874 223e 7b7b 2061  "card-text">{{ a
-00000740: 7574 686f 7220 7d7d 3c2f 6834 3e0a 2020  uthor }}</h4>.  
-00000750: 2020 2020 2020 2020 2020 2020 3c70 2063              <p c
-00000760: 6c61 7373 3d22 6361 7264 2d74 6578 7422  lass="card-text"
-00000770: 3e7b 7b20 6175 7468 6f72 5f64 6573 6372  >{{ author_descr
-00000780: 6970 7469 6f6e 207d 7d3c 2f70 3e0a 0909  iption }}</p>...
-00000790: 0920 207b 2520 6966 2067 6974 6875 6220  .  {% if github 
-000007a0: 6f72 2062 6974 6275 636b 6574 206f 7220  or bitbucket or 
-000007b0: 6661 6365 626f 6f6b 206f 7220 7477 6974  facebook or twit
-000007c0: 7465 7220 6f72 2067 6f6f 676c 655f 706c  ter or google_pl
-000007d0: 7573 206f 7220 6c69 6e6b 6564 696e 206f  us or linkedin o
-000007e0: 7220 656d 6169 6c20 6f72 2077 6562 7369  r email or websi
-000007f0: 7465 2025 7d0a 2020 2020 2020 2020 2020  te %}.          
-00000800: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000810: 3d22 7465 7874 2d63 656e 7465 7222 3e3c  ="text-center"><
-00000820: 6469 7620 636c 6173 733d 2262 746e 2d67  div class="btn-g
-00000830: 726f 7570 2220 726f 6c65 3d22 6772 6f75  roup" role="grou
-00000840: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00000850: 2020 2020 2020 2020 7b25 2069 6620 656d          {% if em
-00000860: 6169 6c20 257d 0a20 2020 2020 2020 2020  ail %}.         
-00000870: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00000880: 636c 6173 733d 2262 746e 2062 746e 2d6c  class="btn btn-l
-00000890: 6720 6274 6e2d 7072 696d 6172 7922 2068  g btn-primary" h
-000008a0: 7265 663d 226d 6169 6c74 6f3a 7b7b 2065  ref="mailto:{{ e
-000008b0: 6d61 696c 207d 7d22 3e3c 6920 636c 6173  mail }}"><i clas
-000008c0: 733d 2266 6120 6661 2d65 6e76 656c 6f70  s="fa fa-envelop
-000008d0: 6520 6661 2d6c 6722 3e3c 2f69 3e3c 2f61  e fa-lg"></i></a
-000008e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000008f0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00000900: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000910: 2020 2020 2020 7b25 2069 6620 7765 6273        {% if webs
-00000920: 6974 6520 257d 0a20 2020 2020 2020 2020  ite %}.         
-00000930: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00000940: 636c 6173 733d 2262 746e 2062 746e 2d6c  class="btn btn-l
-00000950: 6720 6274 6e2d 7072 696d 6172 7922 2068  g btn-primary" h
-00000960: 7265 663d 227b 7b20 7765 6273 6974 6520  ref="{{ website 
-00000970: 7d7d 223e 3c69 2063 6c61 7373 3d22 6661  }}"><i class="fa
-00000980: 2066 612d 676c 6f62 6520 6661 2d6c 6722   fa-globe fa-lg"
-00000990: 3e3c 2f69 3e3c 2f61 3e0a 2020 2020 2020  ></i></a>.      
-000009a0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000009b0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-000009c0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000009d0: 2069 6620 6769 7468 7562 2025 7d0a 2020   if github %}.  
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 3c61 2063 6c61 7373 3d22 6274      <a class="bt
-00000a00: 6e20 6274 6e2d 6c67 2062 746e 2d70 7269  n btn-lg btn-pri
-00000a10: 6d61 7279 2220 6872 6566 3d22 7b7b 2067  mary" href="{{ g
-00000a20: 6974 6875 6220 7d7d 223e 3c69 2063 6c61  ithub }}"><i cla
-00000a30: 7373 3d22 6661 2066 612d 6769 7468 7562  ss="fa fa-github
-00000a40: 2066 612d 6c67 223e 3c2f 693e 3c2f 613e   fa-lg"></i></a>
+00000000: 7b25 206d 6163 726f 2070 726f 6a65 6374  {% macro project
+00000010: 5f6c 696e 6b5f 6275 7474 6f6e 2861 6464  _link_button(add
+00000020: 7265 7373 2c20 6e61 6d65 2920 257d 0a20  ress, name) %}. 
+00000030: 207b 2320 4f70 7469 6f6e 616c 2062 7574   {# Optional but
+00000040: 746f 6e20 696e 206a 756d 6274 726f 6e20  ton in jumbtron 
+00000050: 666f 7220 7072 6f6a 6563 7420 6c69 6e6b  for project link
+00000060: 2023 7d0a 2020 7b25 2d20 6966 2061 6464   #}.  {%- if add
+00000070: 7265 7373 202d 257d 0a20 2020 203c 6120  ress -%}.    <a 
+00000080: 636c 6173 733d 2262 746e 2062 746e 2d6c  class="btn btn-l
+00000090: 6720 6274 6e2d 7072 696d 6172 7922 2068  g btn-primary" h
+000000a0: 7265 663d 227b 7b20 6164 6472 6573 7320  ref="{{ address 
+000000b0: 7d7d 2220 726f 6c65 3d22 6275 7474 6f6e  }}" role="button
+000000c0: 223e 7b7b 206e 616d 6520 7d7d 3c2f 613e  ">{{ name }}</a>
+000000d0: 0a20 207b 252d 2065 6e64 6966 202d 257d  .  {%- endif -%}
+000000e0: 0a7b 2520 656e 646d 6163 726f 2025 7d0a  .{% endmacro %}.
+000000f0: 0a7b 2520 6d61 6372 6f20 6465 765f 6c69  .{% macro dev_li
+00000100: 6e6b 5f62 7574 746f 6e28 6164 6472 6573  nk_button(addres
+00000110: 732c 2069 636f 6e29 2025 7d0a 2020 7b23  s, icon) %}.  {#
+00000120: 204f 7074 696f 6e61 6c20 6275 7474 6f6e   Optional button
+00000130: 2069 6e20 7369 6465 6261 7220 666f 7220   in sidebar for 
+00000140: 6465 7665 6c6f 7065 7220 6c69 6e6b 2023  developer link #
+00000150: 7d0a 2020 7b25 2d20 6966 2061 6464 7265  }.  {%- if addre
+00000160: 7373 202d 257d 0a20 2020 203c 6120 636c  ss -%}.    <a cl
+00000170: 6173 733d 2262 746e 2062 746e 2d6c 6720  ass="btn btn-lg 
+00000180: 6274 6e2d 7072 696d 6172 7922 2068 7265  btn-primary" hre
+00000190: 663d 227b 7b20 6164 6472 6573 7320 7d7d  f="{{ address }}
+000001a0: 223e 3c69 2063 6c61 7373 3d22 6661 207b  "><i class="fa {
+000001b0: 7b20 6963 6f6e 207d 7d20 6661 2d6c 6722  { icon }} fa-lg"
+000001c0: 3e3c 2f69 3e3c 2f61 3e0a 2020 7b25 2d20  ></i></a>.  {%- 
+000001d0: 656e 6469 6620 2d25 7d0a 7b25 2065 6e64  endif -%}.{% end
+000001e0: 6d61 6372 6f20 257d 0a0a 7b25 2065 7874  macro %}..{% ext
+000001f0: 656e 6473 2022 6261 7365 2e68 746d 6c22  ends "base.html"
+00000200: 2025 7d0a 7b25 2062 6c6f 636b 2062 6f64   %}.{% block bod
+00000210: 7920 257d 0a20 203c 212d 2d20 4d61 696e  y %}.  <!-- Main
+00000220: 2063 6f6d 706f 6e65 6e74 2066 6f72 2061   component for a
+00000230: 2070 7269 6d61 7279 206d 6172 6b65 7469   primary marketi
+00000240: 6e67 206d 6573 7361 6765 206f 7220 6361  ng message or ca
+00000250: 6c6c 2074 6f20 6163 7469 6f6e 202d 2d3e  ll to action -->
+00000260: 0a20 207b 2520 7365 7420 7072 6f6a 6563  .  {% set projec
+00000270: 745f 6c69 6e6b 7320 3d20 7072 6f6a 6563  t_links = projec
+00000280: 745f 6769 7468 7562 206f 7220 7072 6f6a  t_github or proj
+00000290: 6563 745f 6269 7462 7563 6b65 7420 6f72  ect_bitbucket or
+000002a0: 2070 726f 6a65 6374 5f67 6974 6c61 6220   project_gitlab 
+000002b0: 6f72 2070 726f 6a65 6374 5f73 6f75 7263  or project_sourc
+000002c0: 6566 6f72 6765 206f 7220 7072 6f6a 6563  eforge or projec
+000002d0: 745f 7765 6273 6974 6520 257d 0a20 207b  t_website %}.  {
+000002e0: 2520 6966 2073 756d 6d61 7279 206f 7220  % if summary or 
+000002f0: 7072 6f6a 6563 745f 6c69 6e6b 7320 6f72  project_links or
+00000300: 2070 726f 6a65 6374 5f64 6f77 6e6c 6f61   project_downloa
+00000310: 6420 257d 0a20 2020 203c 6469 7620 636c  d %}.    <div cl
+00000320: 6173 733d 2270 2d35 206d 622d 3420 6267  ass="p-5 mb-4 bg
+00000330: 2d6c 6967 6874 2062 6f72 6465 7220 726f  -light border ro
+00000340: 756e 6465 642d 3322 2069 643d 226a 756d  unded-3" id="jum
+00000350: 626f 7472 6f6e 223e 0a20 2020 2020 207b  botron">.      {
+00000360: 7b20 7375 6d6d 6172 7920 7d7d 0a20 2020  { summary }}.   
+00000370: 2020 207b 2520 6966 2070 726f 6a65 6374     {% if project
+00000380: 5f6c 696e 6b73 2025 7d0a 2020 2020 2020  _links %}.      
+00000390: 2020 3c70 3e20 4669 6e64 2075 7320 6f6e    <p> Find us on
+000003a0: 2668 656c 6c69 703b 3c2f 703e 0a20 2020  &hellip;</p>.   
+000003b0: 2020 203c 703e 0a20 2020 2020 2020 207b     <p>.        {
+000003c0: 7b20 7072 6f6a 6563 745f 6c69 6e6b 5f62  { project_link_b
+000003d0: 7574 746f 6e28 7072 6f6a 6563 745f 6769  utton(project_gi
+000003e0: 7468 7562 2c20 2247 6974 4875 6222 2920  thub, "GitHub") 
+000003f0: 7d7d 0a20 2020 2020 2020 207b 7b20 7072  }}.        {{ pr
+00000400: 6f6a 6563 745f 6c69 6e6b 5f62 7574 746f  oject_link_butto
+00000410: 6e28 7072 6f6a 6563 745f 6769 746c 6162  n(project_gitlab
+00000420: 2c20 2247 6974 6c61 6222 2920 7d7d 0a20  , "Gitlab") }}. 
+00000430: 2020 2020 2020 207b 7b20 7072 6f6a 6563         {{ projec
+00000440: 745f 6c69 6e6b 5f62 7574 746f 6e28 7072  t_link_button(pr
+00000450: 6f6a 6563 745f 6269 7462 7563 6b65 742c  oject_bitbucket,
+00000460: 2022 4269 7462 7563 6b65 7422 2920 7d7d   "Bitbucket") }}
+00000470: 0a20 2020 2020 2020 207b 7b20 7072 6f6a  .        {{ proj
+00000480: 6563 745f 6c69 6e6b 5f62 7574 746f 6e28  ect_link_button(
+00000490: 7072 6f6a 6563 745f 736f 7572 6365 666f  project_sourcefo
+000004a0: 7267 652c 2022 536f 7572 6365 666f 7267  rge, "Sourceforg
+000004b0: 6522 2920 7d7d 0a20 2020 2020 2020 207b  e") }}.        {
+000004c0: 7b20 7072 6f6a 6563 745f 6c69 6e6b 5f62  { project_link_b
+000004d0: 7574 746f 6e28 7072 6f6a 6563 745f 7765  utton(project_we
+000004e0: 6273 6974 652c 2022 5468 6520 5765 6222  bsite, "The Web"
+000004f0: 2920 7d7d 0a20 2020 2020 207b 2520 656e  ) }}.      {% en
+00000500: 6469 6620 257d 0a20 2020 2020 207b 2520  dif %}.      {% 
+00000510: 6966 2070 726f 6a65 6374 5f64 6f77 6e6c  if project_downl
+00000520: 6f61 6420 257d 0a20 2020 2020 2020 203c  oad %}.        <
+00000530: 6120 636c 6173 733d 2262 746e 2062 746e  a class="btn btn
+00000540: 2d6c 6720 6274 6e2d 6461 6e67 6572 2220  -lg btn-danger" 
+00000550: 7374 796c 653d 2266 6c6f 6174 3a72 6967  style="float:rig
+00000560: 6874 2220 6872 6566 3d22 7b7b 2070 726f  ht" href="{{ pro
+00000570: 6a65 6374 5f64 6f77 6e6c 6f61 6420 7d7d  ject_download }}
+00000580: 2220 726f 6c65 3d22 6275 7474 6f6e 223e  " role="button">
+00000590: 446f 776e 6c6f 6164 2074 6865 2053 6f75  Download the Sou
+000005a0: 7263 653c 2f61 3e0a 2020 2020 2020 7b25  rce</a>.      {%
+000005b0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+000005c0: 3c2f 703e 0a20 2020 203c 2f64 6976 3e0a  </p>.    </div>.
+000005d0: 2020 7b25 2065 6e64 6966 2025 7d0a 0a20    {% endif %}.. 
+000005e0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000005f0: 2272 6f77 2220 6964 3d27 7465 7874 273e  "row" id='text'>
+00000600: 0a20 2020 2020 2020 207b 2520 7365 7420  .        {% set 
+00000610: 636f 6c20 3d20 2263 6f6c 2d6d 642d 3822  col = "col-md-8"
+00000620: 2069 6620 6175 7468 6f72 2065 6c73 6520   if author else 
+00000630: 2263 6f6c 2d6d 642d 3132 2225 7d0a 2020  "col-md-12"%}.  
+00000640: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000650: 3d7b 7b20 636f 6c20 7d7d 3e0a 2020 2020  ={{ col }}>.    
+00000660: 2020 2020 2020 3c68 313e 7b7b 2070 726f        <h1>{{ pro
+00000670: 6a65 6374 207d 7d3c 2f68 313e 0a20 2020  ject }}</h1>.   
+00000680: 2020 2020 2020 207b 7b20 7072 6f6a 5f64         {{ proj_d
+00000690: 6f63 7320 7d7d 0a20 2020 2020 2020 203c  ocs }}.        <
+000006a0: 2f64 6976 3e0a 2020 2020 2020 2020 7b25  /div>.        {%
+000006b0: 2069 6620 6175 7468 6f72 2025 7d0a 2020   if author %}.  
+000006c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000006d0: 7373 3d22 636f 6c2d 6d64 2d34 223e 0a20  ss="col-md-4">. 
+000006e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000006f0: 636c 6173 733d 2263 6172 6420 6361 7264  class="card card
+00000700: 2d62 6f64 7920 6267 2d6c 6967 6874 223e  -body bg-light">
+00000710: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00000720: 2520 6966 2061 7574 686f 725f 7069 6320  % if author_pic 
+00000730: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000740: 2020 203c 696d 6720 7372 633d 227b 7b20     <img src="{{ 
+00000750: 6175 7468 6f72 5f70 6963 207d 7d22 2061  author_pic }}" a
+00000760: 6c74 3d22 4465 7665 6c6f 7065 7220 7069  lt="Developer pi
+00000770: 6374 7572 6522 2063 6c61 7373 3d22 6361  cture" class="ca
+00000780: 7264 2d69 6d67 2d74 6f70 223e 0a20 2020  rd-img-top">.   
+00000790: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+000007a0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+000007b0: 2020 2020 203c 6832 2063 6c61 7373 3d22       <h2 class="
+000007c0: 6361 7264 2d74 6974 6c65 223e 4465 7665  card-title">Deve
+000007d0: 6c6f 7065 7220 496e 666f 3c2f 6832 3e0a  loper Info</h2>.
+000007e0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+000007f0: 3420 636c 6173 733d 2263 6172 642d 7465  4 class="card-te
+00000800: 7874 223e 7b7b 2061 7574 686f 7220 7d7d  xt">{{ author }}
+00000810: 3c2f 6834 3e0a 2020 2020 2020 2020 2020  </h4>.          
+00000820: 2020 2020 3c70 2063 6c61 7373 3d22 6361      <p class="ca
+00000830: 7264 2d74 6578 7422 3e7b 7b20 6175 7468  rd-text">{{ auth
+00000840: 6f72 5f64 6573 6372 6970 7469 6f6e 207d  or_description }
+00000850: 7d3c 2f70 3e0a 2020 2020 2020 2020 2020  }</p>.          
+00000860: 2020 2020 7b25 2069 6620 6769 7468 7562      {% if github
+00000870: 206f 7220 6269 7462 7563 6b65 7420 6f72   or bitbucket or
+00000880: 2066 6163 6562 6f6f 6b20 6f72 2074 7769   facebook or twi
+00000890: 7474 6572 206f 7220 676f 6f67 6c65 5f70  tter or google_p
+000008a0: 6c75 7320 6f72 206c 696e 6b65 6469 6e20  lus or linkedin 
+000008b0: 6f72 2065 6d61 696c 206f 7220 7765 6273  or email or webs
+000008c0: 6974 6520 257d 0a20 2020 2020 2020 2020  ite %}.         
+000008d0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000008e0: 733d 2274 6578 742d 6365 6e74 6572 223e  s="text-center">
+000008f0: 3c64 6976 2063 6c61 7373 3d22 6274 6e2d  <div class="btn-
+00000900: 6772 6f75 7022 2072 6f6c 653d 2267 726f  group" role="gro
+00000910: 7570 223e 0a20 2020 2020 2020 2020 2020  up">.           
+00000920: 2020 2020 2020 2020 207b 2520 6966 2065           {% if e
+00000930: 6d61 696c 2025 7d0a 2020 2020 2020 2020  mail %}.        
+00000940: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
+00000950: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+00000960: 6c67 2062 746e 2d70 7269 6d61 7279 2220  lg btn-primary" 
+00000970: 6872 6566 3d22 6d61 696c 746f 3a7b 7b20  href="mailto:{{ 
+00000980: 656d 6169 6c20 7d7d 223e 3c69 2063 6c61  email }}"><i cla
+00000990: 7373 3d22 6661 2066 612d 656e 7665 6c6f  ss="fa fa-envelo
+000009a0: 7065 2066 612d 6c67 223e 3c2f 693e 3c2f  pe fa-lg"></i></
+000009b0: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
+000009c0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000009d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000009e0: 2020 2020 2020 207b 7b20 6465 765f 6c69         {{ dev_li
+000009f0: 6e6b 5f62 7574 746f 6e28 7765 6273 6974  nk_button(websit
+00000a00: 652c 2022 6661 2d67 6c6f 6265 2229 207d  e, "fa-globe") }
+00000a10: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000a20: 2020 2020 2020 7b7b 2064 6576 5f6c 696e        {{ dev_lin
+00000a30: 6b5f 6275 7474 6f6e 2867 6974 6875 622c  k_button(github,
+00000a40: 2022 6661 2d67 6974 6875 6222 2920 7d7d   "fa-github") }}
 00000a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a60: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a80: 2020 2020 207b 2520 6966 2067 6974 6c61       {% if gitla
-00000a90: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
-00000aa0: 2020 2020 2020 2020 2020 203c 6120 636c             <a cl
-00000ab0: 6173 733d 2262 746e 2062 746e 2d6c 6720  ass="btn btn-lg 
-00000ac0: 6274 6e2d 7072 696d 6172 7922 2068 7265  btn-primary" hre
-00000ad0: 663d 227b 7b20 6769 746c 6162 207d 7d22  f="{{ gitlab }}"
-00000ae0: 3e3c 6920 636c 6173 733d 2266 6120 6661  ><i class="fa fa
-00000af0: 2d67 6974 6c61 6220 6661 2d6c 6722 3e3c  -gitlab fa-lg"><
-00000b00: 2f69 3e3c 2f61 3e0a 0909 0909 2020 2020  /i></a>.....    
-00000b10: 7b25 2065 6e64 6966 2025 7d0a 0909 0909  {% endif %}.....
-00000b20: 2020 2020 7b25 2069 6620 6269 7462 7563      {% if bitbuc
-00000b30: 6b65 7420 257d 0a20 2020 2020 2020 2020  ket %}.         
-00000b40: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00000b50: 636c 6173 733d 2262 746e 2062 746e 2d6c  class="btn btn-l
-00000b60: 6720 6274 6e2d 7072 696d 6172 7922 2068  g btn-primary" h
-00000b70: 7265 663d 227b 7b20 6269 7462 7563 6b65  ref="{{ bitbucke
-00000b80: 7420 7d7d 223e 3c69 2063 6c61 7373 3d22  t }}"><i class="
-00000b90: 6661 2066 612d 6269 7462 7563 6b65 7420  fa fa-bitbucket 
-00000ba0: 6661 2d6c 6722 3e3c 2f69 3e3c 2f61 3e0a  fa-lg"></i></a>.
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2020 7b25 2069 6620 6661 6365 626f      {% if facebo
-00000bf0: 6f6b 2025 7d0a 2020 2020 2020 2020 2020  ok %}.          
-00000c00: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-00000c10: 6c61 7373 3d22 6274 6e20 6274 6e2d 6c67  lass="btn btn-lg
-00000c20: 2062 746e 2d70 7269 6d61 7279 2220 6872   btn-primary" hr
-00000c30: 6566 3d22 7b7b 2066 6163 6562 6f6f 6b20  ef="{{ facebook 
-00000c40: 7d7d 223e 3c69 2063 6c61 7373 3d22 6661  }}"><i class="fa
-00000c50: 2066 612d 6661 6365 626f 6f6b 2066 612d   fa-facebook fa-
-00000c60: 6c67 223e 3c2f 693e 3c2f 613e 0a09 0909  lg"></i></a>....
-00000c70: 0920 2020 207b 2520 656e 6469 6620 257d  .    {% endif %}
-00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c90: 2020 2020 207b 2520 6966 2067 6f6f 676c       {% if googl
-00000ca0: 655f 706c 7573 2025 7d0a 2020 2020 2020  e_plus %}.      
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 3c61 2063 6c61 7373 3d22 6274 6e20 6274  <a class="btn bt
-00000cd0: 6e2d 6c67 2062 746e 2d70 7269 6d61 7279  n-lg btn-primary
-00000ce0: 2220 6872 6566 3d22 7b7b 2067 6f6f 676c  " href="{{ googl
-00000cf0: 655f 706c 7573 207d 7d22 3e3c 6920 636c  e_plus }}"><i cl
-00000d00: 6173 733d 2266 6120 6661 2d67 6f6f 676c  ass="fa fa-googl
-00000d10: 652d 706c 7573 2066 612d 6c67 223e 3c2f  e-plus fa-lg"></
-00000d20: 693e 3c2f 613e 0a09 0909 0920 2020 207b  i></a>.....    {
-00000d30: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00000d40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000d50: 2520 6966 206c 696e 6b65 6469 6e20 257d  % if linkedin %}
-00000d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d70: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
-00000d80: 2262 746e 2062 746e 2d6c 6720 6274 6e2d  "btn btn-lg btn-
-00000d90: 7072 696d 6172 7922 2068 7265 663d 227b  primary" href="{
-00000da0: 7b20 6c69 6e6b 6564 696e 207d 7d22 3e3c  { linkedin }}"><
-00000db0: 6920 636c 6173 733d 2266 6120 6661 2d6c  i class="fa fa-l
-00000dc0: 696e 6b65 6469 6e20 6661 2d6c 6722 3e3c  inkedin fa-lg"><
-00000dd0: 2f69 3e3c 2f61 3e0a 0909 0909 2020 2020  /i></a>.....    
-00000de0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 7b25 2069 6620 7477 6974 7465 7220 257d  {% if twitter %}
-00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e20: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
-00000e30: 2262 746e 2062 746e 2d6c 6720 6274 6e2d  "btn btn-lg btn-
-00000e40: 7072 696d 6172 7922 2068 7265 663d 227b  primary" href="{
-00000e50: 7b20 7477 6974 7465 7220 7d7d 223e 3c69  { twitter }}"><i
-00000e60: 2063 6c61 7373 3d22 6661 2066 612d 7477   class="fa fa-tw
-00000e70: 6974 7465 7220 6661 2d6c 6722 3e3c 2f69  itter fa-lg"></i
-00000e80: 3e3c 2f61 3e0a 0909 0909 2020 2020 7b25  ></a>.....    {%
-00000e90: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000ea0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000eb0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000ec0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000ed0: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-00000ee0: 6976 3e0a 2020 2020 2020 2020 2020 3c2f  iv>.          </
-00000ef0: 6469 763e 0a20 2020 2020 2020 207b 2520  div>.        {% 
-00000f00: 656e 6469 6620 257d 0a20 2020 2020 203c  endif %}.      <
-00000f10: 2f64 6976 3e0a 2020 2020 2020 7b25 2073  /div>.      {% s
-00000f20: 6574 2063 6f75 6e74 3d30 2025 7d0a 2020  et count=0 %}.  
-00000f30: 2020 2020 7b25 2069 6620 696e 636c 5f73      {% if incl_s
-00000f40: 7263 2025 7d7b 2520 7365 7420 636f 756e  rc %}{% set coun
-00000f50: 7420 3d20 636f 756e 7420 2b20 3120 257d  t = count + 1 %}
-00000f60: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000f70: 2020 7b25 2069 6620 7072 6f6a 6563 742e    {% if project.
-00000f80: 6d6f 6475 6c65 737c 6c65 6e67 7468 203e  modules|length >
-00000f90: 2030 2025 7d7b 2520 7365 7420 636f 756e   0 %}{% set coun
-00000fa0: 7420 3d20 636f 756e 7420 2b20 3120 257d  t = count + 1 %}
-00000fb0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000fc0: 2020 7b25 2069 6620 7072 6f6a 6563 742e    {% if project.
-00000fd0: 7072 6f63 6564 7572 6573 7c6c 656e 6774  procedures|lengt
-00000fe0: 6820 3e20 3020 257d 7b25 2073 6574 2063  h > 0 %}{% set c
-00000ff0: 6f75 6e74 203d 2063 6f75 6e74 202b 2031  ount = count + 1
-00001000: 2025 7d7b 2520 656e 6469 6620 257d 0a20   %}{% endif %}. 
-00001010: 2020 2020 207b 2520 6966 2070 726f 6a65       {% if proje
-00001020: 6374 2e74 7970 6573 7c6c 656e 6774 6820  ct.types|length 
-00001030: 3e20 3020 257d 7b25 2073 6574 2063 6f75  > 0 %}{% set cou
-00001040: 6e74 203d 2063 6f75 6e74 202b 2031 2025  nt = count + 1 %
-00001050: 7d7b 2520 656e 6469 6620 257d 0a20 2020  }{% endif %}.   
-00001060: 2020 207b 2520 7365 7420 6d61 785f 6c65     {% set max_le
-00001070: 6e67 7468 203d 206d 6178 5f66 726f 6e74  ngth = max_front
-00001080: 7061 6765 5f69 7465 6d73 7c69 6e74 2025  page_items|int %
-00001090: 7d0a 2020 2020 2020 7b25 2069 6620 636f  }.      {% if co
-000010a0: 756e 7420 616e 6420 6d61 785f 6c65 6e67  unt and max_leng
-000010b0: 7468 2025 7d0a 2020 2020 2020 2020 7b25  th %}.        {%
-000010c0: 2073 6574 2077 6964 7468 203d 2028 3132   set width = (12
-000010d0: 2f63 6f75 6e74 297c 696e 7420 257d 0a20  /count)|int %}. 
-000010e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000010f0: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
-00001100: 2020 203c 6872 3e0a 2020 2020 2020 2020     <hr>.        
-00001110: 2020 7b25 2069 6620 696e 636c 5f73 7263    {% if incl_src
-00001120: 2025 7d0a 2020 2020 2020 2020 2020 3c64   %}.          <d
-00001130: 6976 2063 6c61 7373 3d22 636f 6c2d 7873  iv class="col-xs
-00001140: 2d36 2063 6f6c 2d73 6d2d 7b7b 2077 6964  -6 col-sm-{{ wid
-00001150: 7468 207d 7d22 3e0a 2020 2020 2020 2020  th }}">.        
-00001160: 2020 2020 3c64 6976 3e0a 2020 2020 2020      <div>.      
-00001170: 2020 2020 2020 2020 3c68 333e 536f 7572          <h3>Sour
-00001180: 6365 2046 696c 6573 3c2f 6833 3e0a 2020  ce Files</h3>.  
-00001190: 2020 2020 2020 2020 2020 2020 3c75 6c3e              <ul>
-000011a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011b0: 207b 252d 2066 6f72 2073 7263 2069 6e20   {%- for src in 
-000011c0: 2870 726f 6a65 6374 2e61 6c6c 6669 6c65  (project.allfile
-000011d0: 737c 736f 7274 2861 7474 7269 6275 7465  s|sort(attribute
-000011e0: 3d27 6e61 6d65 2729 295b 3a6d 6178 5f6c  ='name'))[:max_l
-000011f0: 656e 6774 685d 202d 257d 0a20 2020 2020  ength] -%}.     
-00001200: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-00001210: 3e7b 7b20 7372 6320 7c20 7265 6c75 726c  >{{ src | relurl
-00001220: 2870 6167 655f 7572 6c29 207d 7d3c 2f6c  (page_url) }}</l
-00001230: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-00001240: 2020 207b 252d 2065 6e64 666f 7220 2d25     {%- endfor -%
-00001250: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001260: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
-00001270: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001280: 2020 2020 203c 6469 763e 0a20 2020 2020       <div>.     
-00001290: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-000012b0: 693e 3c61 2068 7265 663d 227b 7b20 7072  i><a href="{{ pr
-000012c0: 6f6a 6563 745f 7572 6c20 7d7d 2f6c 6973  oject_url }}/lis
-000012d0: 7473 2f66 696c 6573 2e68 746d 6c22 3e3c  ts/files.html"><
-000012e0: 656d 3e41 6c6c 2073 6f75 7263 6520 6669  em>All source fi
-000012f0: 6c65 7326 6865 6c6c 6970 3b3c 2f65 6d3e  les&hellip;</em>
-00001300: 3c2f 613e 3c2f 6c69 3e0a 2020 2020 2020  </a></li>.      
-00001310: 2020 2020 2020 2020 3c2f 756c 3e0a 2020          </ul>.  
-00001320: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00001330: 0a20 2020 2020 2020 2020 203c 2f64 6976  .          </div
-00001340: 3e0a 2020 2020 2020 2020 2020 7b25 2065  >.          {% e
-00001350: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-00001360: 2020 7b25 2069 6620 7072 6f6a 6563 742e    {% if project.
-00001370: 6d6f 6475 6c65 737c 6c65 6e67 7468 203e  modules|length >
-00001380: 2030 2025 7d0a 2020 2020 2020 2020 2020   0 %}.          
-00001390: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-000013a0: 7873 2d36 2063 6f6c 2d73 6d2d 7b7b 2077  xs-6 col-sm-{{ w
-000013b0: 6964 7468 207d 7d22 3e0a 2020 2020 2020  idth }}">.      
-000013c0: 2020 2020 2020 3c64 6976 3e0a 2020 2020        <div>.    
-000013d0: 2020 2020 2020 2020 2020 3c68 333e 4d6f            <h3>Mo
-000013e0: 6475 6c65 733c 2f68 333e 0a20 2020 2020  dules</h3>.     
-000013f0: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
-00001400: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00001410: 2d20 666f 7220 6d6f 6420 696e 2028 7072  - for mod in (pr
-00001420: 6f6a 6563 742e 6d6f 6475 6c65 737c 736f  oject.modules|so
-00001430: 7274 2861 7474 7269 6275 7465 3d27 6e61  rt(attribute='na
-00001440: 6d65 2729 295b 3a6d 6178 5f6c 656e 6774  me'))[:max_lengt
-00001450: 685d 202d 257d 0a20 2020 2020 2020 2020  h] -%}.         
-00001460: 2020 2020 2020 2020 203c 6c69 3e7b 7b20           <li>{{ 
-00001470: 6d6f 6420 7c20 7265 6c75 726c 2870 6167  mod | relurl(pag
-00001480: 655f 7572 6c29 207d 7d3c 2f6c 693e 0a20  e_url) }}</li>. 
-00001490: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000014a0: 252d 2065 6e64 666f 7220 2d25 7d0a 2020  %- endfor -%}.  
-000014b0: 2020 2020 2020 2020 2020 2020 3c2f 756c              </ul
-000014c0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-000014d0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000014e0: 203c 6469 763e 0a20 2020 2020 2020 2020   <div>.         
-000014f0: 2020 2020 203c 756c 3e0a 2020 2020 2020       <ul>.      
-00001500: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
-00001510: 2068 7265 663d 227b 7b20 7072 6f6a 6563   href="{{ projec
-00001520: 745f 7572 6c20 7d7d 2f6c 6973 7473 2f6d  t_url }}/lists/m
-00001530: 6f64 756c 6573 2e68 746d 6c22 3e3c 656d  odules.html"><em
-00001540: 3e41 6c6c 206d 6f64 756c 6573 2668 656c  >All modules&hel
-00001550: 6c69 703b 3c2f 656d 3e3c 2f61 3e3c 2f6c  lip;</em></a></l
-00001560: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-00001570: 203c 2f75 6c3e 0a20 2020 2020 2020 2020   </ul>.         
-00001580: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001590: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000015a0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000015b0: 0a20 2020 2020 2020 2020 207b 2520 6966  .          {% if
-000015c0: 2070 726f 6a65 6374 2e70 726f 6365 6475   project.procedu
-000015d0: 7265 737c 6c65 6e67 7468 203e 2030 2025  res|length > 0 %
-000015e0: 7d0a 2020 2020 2020 2020 2020 3c64 6976  }.          <div
-000015f0: 2063 6c61 7373 3d22 636f 6c2d 7873 2d36   class="col-xs-6
-00001600: 2063 6f6c 2d73 6d2d 7b7b 2077 6964 7468   col-sm-{{ width
-00001610: 207d 7d22 3e0a 2020 2020 2020 2020 2020   }}">.          
-00001620: 2020 3c64 6976 3e0a 2020 2020 2020 2020    <div>.        
-00001630: 2020 2020 2020 3c68 333e 5072 6f63 6564        <h3>Proced
-00001640: 7572 6573 3c2f 6833 3e0a 2020 2020 2020  ures</h3>.      
-00001650: 2020 2020 2020 2020 3c75 6c3e 0a20 2020          <ul>.   
-00001660: 2020 2020 2020 2020 2020 2020 207b 252d               {%-
-00001670: 2066 6f72 2070 726f 6320 696e 2028 7072   for proc in (pr
-00001680: 6f6a 6563 742e 7072 6f63 6564 7572 6573  oject.procedures
-00001690: 7c73 6f72 7428 6174 7472 6962 7574 653d  |sort(attribute=
-000016a0: 276e 616d 6527 2929 5b3a 6d61 785f 6c65  'name'))[:max_le
-000016b0: 6e67 7468 5d20 2d25 7d0a 2020 2020 2020  ngth] -%}.      
-000016c0: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
-000016d0: 7b7b 2070 726f 6320 7c20 7265 6c75 726c  {{ proc | relurl
-000016e0: 2870 6167 655f 7572 6c29 207d 7d3c 2f6c  (page_url) }}</l
-000016f0: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-00001700: 2020 207b 252d 2065 6e64 666f 7220 2d25     {%- endfor -%
-00001710: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001720: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
-00001730: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001740: 2020 2020 203c 6469 763e 0a20 2020 2020       <div>.     
-00001750: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
-00001760: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-00001770: 693e 3c61 2068 7265 663d 227b 7b20 7072  i><a href="{{ pr
-00001780: 6f6a 6563 745f 7572 6c20 7d7d 2f6c 6973  oject_url }}/lis
-00001790: 7473 2f70 726f 6365 6475 7265 732e 6874  ts/procedures.ht
-000017a0: 6d6c 223e 3c65 6d3e 416c 6c20 7072 6f63  ml"><em>All proc
-000017b0: 6564 7572 6573 2668 656c 6c69 703b 3c2f  edures&hellip;</
-000017c0: 656d 3e3c 2f61 3e3c 2f6c 693e 0a20 2020  em></a></li>.   
-000017d0: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
-000017e0: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-000017f0: 6976 3e0a 2020 2020 2020 2020 2020 3c2f  iv>.          </
-00001800: 6469 763e 0a20 2020 2020 2020 2020 207b  div>.          {
-00001810: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00001820: 2020 2020 207b 2520 6966 2070 726f 6a65       {% if proje
-00001830: 6374 2e74 7970 6573 7c6c 656e 6774 6820  ct.types|length 
-00001840: 3e20 3020 257d 0a20 2020 2020 2020 2020  > 0 %}.         
-00001850: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00001860: 2d78 732d 3620 636f 6c2d 736d 2d7b 7b20  -xs-6 col-sm-{{ 
-00001870: 7769 6474 6820 7d7d 223e 0a20 2020 2020  width }}">.     
-00001880: 2020 2020 2020 203c 6469 763e 0a20 2020         <div>.   
-00001890: 2020 2020 2020 2020 2020 203c 6833 3e44             <h3>D
-000018a0: 6572 6976 6564 2054 7970 6573 3c2f 6833  erived Types</h3
-000018b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000018c0: 3c75 6c3e 0a20 2020 2020 2020 2020 2020  <ul>.           
-000018d0: 2020 2020 207b 252d 2066 6f72 2064 7479       {%- for dty
-000018e0: 7065 2069 6e20 2870 726f 6a65 6374 2e74  pe in (project.t
-000018f0: 7970 6573 7c73 6f72 7428 6174 7472 6962  ypes|sort(attrib
-00001900: 7574 653d 276e 616d 6527 2929 5b3a 6d61  ute='name'))[:ma
-00001910: 785f 6c65 6e67 7468 5d20 2d25 7d0a 2020  x_length] -%}.  
-00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 3c6c 693e 7b7b 2064 7479 7065 207c 2072  <li>{{ dtype | r
-00001940: 656c 7572 6c28 7061 6765 5f75 726c 2920  elurl(page_url) 
-00001950: 7d7d 3c2f 6c69 3e0a 2020 2020 2020 2020  }}</li>.        
-00001960: 2020 2020 2020 2020 7b25 2d20 656e 6466          {%- endf
-00001970: 6f72 202d 257d 0a20 2020 2020 2020 2020  or -%}.         
-00001980: 2020 2020 203c 2f75 6c3e 0a20 2020 2020       </ul>.     
-00001990: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000019a0: 2020 2020 2020 2020 2020 3c64 6976 3e0a            <div>.
-000019b0: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
-000019c0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-000019d0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000019e0: 7b7b 2070 726f 6a65 6374 5f75 726c 207d  {{ project_url }
-000019f0: 7d2f 6c69 7374 732f 7479 7065 732e 6874  }/lists/types.ht
-00001a00: 6d6c 223e 3c65 6d3e 416c 6c20 6465 7269  ml"><em>All deri
-00001a10: 7665 6420 7479 7065 7326 6865 6c6c 6970  ved types&hellip
-00001a20: 3b3c 2f65 6d3e 3c2f 613e 3c2f 6c69 3e0a  ;</em></a></li>.
-00001a30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001a40: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
-00001a50: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00001a60: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001a70: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
-00001a80: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00001a90: 2020 207b 2520 656e 6469 6620 257d 0a7b     {% endif %}.{
-00001aa0: 2520 656e 6462 6c6f 636b 2062 6f64 7920  % endblock body 
-00001ab0: 257d 0a0a                                %}..
+00000a60: 2020 2020 207b 7b20 6465 765f 6c69 6e6b       {{ dev_link
+00000a70: 5f62 7574 746f 6e28 6769 746c 6162 2c20  _button(gitlab, 
+00000a80: 2266 612d 6769 746c 6162 2229 207d 7d0a  "fa-gitlab") }}.
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 7b7b 2064 6576 5f6c 696e 6b5f      {{ dev_link_
+00000ab0: 6275 7474 6f6e 2862 6974 6275 636b 6574  button(bitbucket
+00000ac0: 2c20 2266 612d 6269 7462 7563 6b65 7422  , "fa-bitbucket"
+00000ad0: 2920 7d7d 0a20 2020 2020 2020 2020 2020  ) }}.           
+00000ae0: 2020 2020 2020 2020 207b 7b20 6465 765f           {{ dev_
+00000af0: 6c69 6e6b 5f62 7574 746f 6e28 6661 6365  link_button(face
+00000b00: 626f 6f6b 2c20 2266 612d 6661 6365 626f  book, "fa-facebo
+00000b10: 6f6b 2229 207d 7d0a 2020 2020 2020 2020  ok") }}.        
+00000b20: 2020 2020 2020 2020 2020 2020 7b7b 2064              {{ d
+00000b30: 6576 5f6c 696e 6b5f 6275 7474 6f6e 2867  ev_link_button(g
+00000b40: 6f6f 676c 655f 706c 7573 2c20 2266 612d  oogle_plus, "fa-
+00000b50: 676f 6f67 6c65 2d70 6c75 7322 2920 7d7d  google-plus") }}
+00000b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b70: 2020 2020 207b 7b20 6465 765f 6c69 6e6b       {{ dev_link
+00000b80: 5f62 7574 746f 6e28 6c69 6e6b 6564 696e  _button(linkedin
+00000b90: 2c20 2266 612d 6c69 6e6b 6564 696e 2229  , "fa-linkedin")
+00000ba0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+00000bb0: 2020 2020 2020 2020 7b7b 2064 6576 5f6c          {{ dev_l
+00000bc0: 696e 6b5f 6275 7474 6f6e 2874 7769 7474  ink_button(twitt
+00000bd0: 6572 2c20 2266 612d 7477 6974 7465 7222  er, "fa-twitter"
+00000be0: 2920 7d7d 0a20 2020 2020 2020 2020 2020  ) }}.           
+00000bf0: 2020 2020 203c 2f64 6976 3e3c 2f64 6976       </div></div
+00000c00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000c10: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000c20: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000c30: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000c40: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00000c50: 2025 7d0a 2020 2020 2020 3c2f 6469 763e   %}.      </div>
+00000c60: 0a20 2020 2020 207b 2520 7365 7420 636f  .      {% set co
+00000c70: 756e 743d 3020 257d 0a20 2020 2020 207b  unt=0 %}.      {
+00000c80: 2520 6966 2069 6e63 6c5f 7372 6320 257d  % if incl_src %}
+00000c90: 7b25 2073 6574 2063 6f75 6e74 203d 2063  {% set count = c
+00000ca0: 6f75 6e74 202b 2031 2025 7d7b 2520 656e  ount + 1 %}{% en
+00000cb0: 6469 6620 257d 0a20 2020 2020 207b 2520  dif %}.      {% 
+00000cc0: 6966 2070 726f 6a65 6374 2e6d 6f64 756c  if project.modul
+00000cd0: 6573 2025 7d7b 2520 7365 7420 636f 756e  es %}{% set coun
+00000ce0: 7420 3d20 636f 756e 7420 2b20 3120 257d  t = count + 1 %}
+00000cf0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000d00: 2020 7b25 2069 6620 7072 6f6a 6563 742e    {% if project.
+00000d10: 7072 6f63 6564 7572 6573 2025 7d7b 2520  procedures %}{% 
+00000d20: 7365 7420 636f 756e 7420 3d20 636f 756e  set count = coun
+00000d30: 7420 2b20 3120 257d 7b25 2065 6e64 6966  t + 1 %}{% endif
+00000d40: 2025 7d0a 2020 2020 2020 7b25 2069 6620   %}.      {% if 
+00000d50: 7072 6f6a 6563 742e 7479 7065 7320 257d  project.types %}
+00000d60: 7b25 2073 6574 2063 6f75 6e74 203d 2063  {% set count = c
+00000d70: 6f75 6e74 202b 2031 2025 7d7b 2520 656e  ount + 1 %}{% en
+00000d80: 6469 6620 257d 0a20 2020 2020 207b 2520  dif %}.      {% 
+00000d90: 7365 7420 6d61 785f 6c65 6e67 7468 203d  set max_length =
+00000da0: 206d 6178 5f66 726f 6e74 7061 6765 5f69   max_frontpage_i
+00000db0: 7465 6d73 7c69 6e74 2025 7d0a 2020 2020  tems|int %}.    
+00000dc0: 2020 7b25 2069 6620 636f 756e 7420 616e    {% if count an
+00000dd0: 6420 6d61 785f 6c65 6e67 7468 2025 7d0a  d max_length %}.
+00000de0: 2020 2020 2020 2020 7b25 2073 6574 2077          {% set w
+00000df0: 6964 7468 203d 2028 3132 2f63 6f75 6e74  idth = (12/count
+00000e00: 297c 696e 7420 257d 0a20 2020 2020 2020  )|int %}.       
+00000e10: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
+00000e20: 223e 0a20 2020 2020 2020 2020 203c 6872  ">.          <hr
+00000e30: 3e0a 2020 2020 2020 2020 2020 7b25 2069  >.          {% i
+00000e40: 6620 696e 636c 5f73 7263 2025 7d0a 2020  f incl_src %}.  
+00000e50: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000e60: 7373 3d22 636f 6c2d 7873 2d36 2063 6f6c  ss="col-xs-6 col
+00000e70: 2d73 6d2d 7b7b 2077 6964 7468 207d 7d22  -sm-{{ width }}"
+00000e80: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00000e90: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000ea0: 2020 3c68 333e 536f 7572 6365 2046 696c    <h3>Source Fil
+00000eb0: 6573 3c2f 6833 3e0a 2020 2020 2020 2020  es</h3>.        
+00000ec0: 2020 2020 2020 3c75 6c3e 0a20 2020 2020        <ul>.     
+00000ed0: 2020 2020 2020 2020 2020 207b 252d 2066             {%- f
+00000ee0: 6f72 2073 7263 2069 6e20 2870 726f 6a65  or src in (proje
+00000ef0: 6374 2e61 6c6c 6669 6c65 737c 736f 7274  ct.allfiles|sort
+00000f00: 2861 7474 7269 6275 7465 3d27 6e61 6d65  (attribute='name
+00000f10: 2729 295b 3a6d 6178 5f6c 656e 6774 685d  '))[:max_length]
+00000f20: 202d 257d 0a20 2020 2020 2020 2020 2020   -%}.           
+00000f30: 2020 2020 2020 203c 6c69 3e7b 7b20 7372         <li>{{ sr
+00000f40: 6320 7c20 7265 6c75 726c 2870 6167 655f  c | relurl(page_
+00000f50: 7572 6c29 207d 7d3c 2f6c 693e 0a20 2020  url) }}</li>.   
+00000f60: 2020 2020 2020 2020 2020 2020 207b 252d               {%-
+00000f70: 2065 6e64 666f 7220 2d25 7d0a 2020 2020   endfor -%}.    
+00000f80: 2020 2020 2020 2020 2020 3c2f 756c 3e0a            </ul>.
+00000f90: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000fa0: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
+00000fb0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000fc0: 2020 203c 756c 3e0a 2020 2020 2020 2020     <ul>.        
+00000fd0: 2020 2020 2020 2020 3c6c 693e 3c61 2068          <li><a h
+00000fe0: 7265 663d 227b 7b20 7072 6f6a 6563 745f  ref="{{ project_
+00000ff0: 7572 6c20 7d7d 2f6c 6973 7473 2f66 696c  url }}/lists/fil
+00001000: 6573 2e68 746d 6c22 3e3c 656d 3e41 6c6c  es.html"><em>All
+00001010: 2073 6f75 7263 6520 6669 6c65 7326 6865   source files&he
+00001020: 6c6c 6970 3b3c 2f65 6d3e 3c2f 613e 3c2f  llip;</em></a></
+00001030: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00001040: 2020 3c2f 756c 3e0a 2020 2020 2020 2020    </ul>.        
+00001050: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00001060: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00001070: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001080: 7d0a 2020 2020 2020 2020 2020 7b25 2069  }.          {% i
+00001090: 6620 7072 6f6a 6563 742e 6d6f 6475 6c65  f project.module
+000010a0: 7320 257d 0a20 2020 2020 2020 2020 203c  s %}.          <
+000010b0: 6469 7620 636c 6173 733d 2263 6f6c 2d78  div class="col-x
+000010c0: 732d 3620 636f 6c2d 736d 2d7b 7b20 7769  s-6 col-sm-{{ wi
+000010d0: 6474 6820 7d7d 223e 0a20 2020 2020 2020  dth }}">.       
+000010e0: 2020 2020 203c 6469 763e 0a20 2020 2020       <div>.     
+000010f0: 2020 2020 2020 2020 203c 6833 3e4d 6f64           <h3>Mod
+00001100: 756c 6573 3c2f 6833 3e0a 2020 2020 2020  ules</h3>.      
+00001110: 2020 2020 2020 2020 3c75 6c3e 0a20 2020          <ul>.   
+00001120: 2020 2020 2020 2020 2020 2020 207b 252d               {%-
+00001130: 2066 6f72 206d 6f64 2069 6e20 2870 726f   for mod in (pro
+00001140: 6a65 6374 2e6d 6f64 756c 6573 7c73 6f72  ject.modules|sor
+00001150: 7428 6174 7472 6962 7574 653d 276e 616d  t(attribute='nam
+00001160: 6527 2929 5b3a 6d61 785f 6c65 6e67 7468  e'))[:max_length
+00001170: 5d20 2d25 7d0a 2020 2020 2020 2020 2020  ] -%}.          
+00001180: 2020 2020 2020 2020 3c6c 693e 7b7b 206d          <li>{{ m
+00001190: 6f64 207c 2072 656c 7572 6c28 7061 6765  od | relurl(page
+000011a0: 5f75 726c 2920 7d7d 3c2f 6c69 3e0a 2020  _url) }}</li>.  
+000011b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000011c0: 2d20 656e 6466 6f72 202d 257d 0a20 2020  - endfor -%}.   
+000011d0: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
+000011e0: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
+000011f0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00001200: 3c64 6976 3e0a 2020 2020 2020 2020 2020  <div>.          
+00001210: 2020 2020 3c75 6c3e 0a20 2020 2020 2020      <ul>.       
+00001220: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
+00001230: 6872 6566 3d22 7b7b 2070 726f 6a65 6374  href="{{ project
+00001240: 5f75 726c 207d 7d2f 6c69 7374 732f 6d6f  _url }}/lists/mo
+00001250: 6475 6c65 732e 6874 6d6c 223e 3c65 6d3e  dules.html"><em>
+00001260: 416c 6c20 6d6f 6475 6c65 7326 6865 6c6c  All modules&hell
+00001270: 6970 3b3c 2f65 6d3e 3c2f 613e 3c2f 6c69  ip;</em></a></li
+00001280: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001290: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
+000012a0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+000012b0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000012c0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+000012d0: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+000012e0: 7072 6f6a 6563 742e 7072 6f63 6564 7572  project.procedur
+000012f0: 6573 2025 7d0a 2020 2020 2020 2020 2020  es %}.          
+00001300: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00001310: 7873 2d36 2063 6f6c 2d73 6d2d 7b7b 2077  xs-6 col-sm-{{ w
+00001320: 6964 7468 207d 7d22 3e0a 2020 2020 2020  idth }}">.      
+00001330: 2020 2020 2020 3c64 6976 3e0a 2020 2020        <div>.    
+00001340: 2020 2020 2020 2020 2020 3c68 333e 5072            <h3>Pr
+00001350: 6f63 6564 7572 6573 3c2f 6833 3e0a 2020  ocedures</h3>.  
+00001360: 2020 2020 2020 2020 2020 2020 3c75 6c3e              <ul>
+00001370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001380: 207b 252d 2066 6f72 2070 726f 6320 696e   {%- for proc in
+00001390: 2028 7072 6f6a 6563 742e 7072 6f63 6564   (project.proced
+000013a0: 7572 6573 7c73 6f72 7428 6174 7472 6962  ures|sort(attrib
+000013b0: 7574 653d 276e 616d 6527 2929 5b3a 6d61  ute='name'))[:ma
+000013c0: 785f 6c65 6e67 7468 5d20 2d25 7d0a 2020  x_length] -%}.  
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 3c6c 693e 7b7b 2070 726f 6320 7c20 7265  <li>{{ proc | re
+000013f0: 6c75 726c 2870 6167 655f 7572 6c29 207d  lurl(page_url) }
+00001400: 7d3c 2f6c 693e 0a20 2020 2020 2020 2020  }</li>.         
+00001410: 2020 2020 2020 207b 252d 2065 6e64 666f         {%- endfo
+00001420: 7220 2d25 7d0a 2020 2020 2020 2020 2020  r -%}.          
+00001430: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
+00001440: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00001450: 2020 2020 2020 2020 203c 6469 763e 0a20           <div>. 
+00001460: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
+00001470: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001480: 2020 3c6c 693e 3c61 2068 7265 663d 227b    <li><a href="{
+00001490: 7b20 7072 6f6a 6563 745f 7572 6c20 7d7d  { project_url }}
+000014a0: 2f6c 6973 7473 2f70 726f 6365 6475 7265  /lists/procedure
+000014b0: 732e 6874 6d6c 223e 3c65 6d3e 416c 6c20  s.html"><em>All 
+000014c0: 7072 6f63 6564 7572 6573 2668 656c 6c69  procedures&helli
+000014d0: 703b 3c2f 656d 3e3c 2f61 3e3c 2f6c 693e  p;</em></a></li>
+000014e0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000014f0: 2f75 6c3e 0a20 2020 2020 2020 2020 2020  /ul>.           
+00001500: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00001510: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00001520: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00001530: 2020 2020 2020 2020 207b 2520 6966 2070           {% if p
+00001540: 726f 6a65 6374 2e74 7970 6573 2025 7d0a  roject.types %}.
+00001550: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001560: 6c61 7373 3d22 636f 6c2d 7873 2d36 2063  lass="col-xs-6 c
+00001570: 6f6c 2d73 6d2d 7b7b 2077 6964 7468 207d  ol-sm-{{ width }
+00001580: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+00001590: 3c64 6976 3e0a 2020 2020 2020 2020 2020  <div>.          
+000015a0: 2020 2020 3c68 333e 4465 7269 7665 6420      <h3>Derived 
+000015b0: 5479 7065 733c 2f68 333e 0a20 2020 2020  Types</h3>.     
+000015c0: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
+000015d0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000015e0: 2d20 666f 7220 6474 7970 6520 696e 2028  - for dtype in (
+000015f0: 7072 6f6a 6563 742e 7479 7065 737c 736f  project.types|so
+00001600: 7274 2861 7474 7269 6275 7465 3d27 6e61  rt(attribute='na
+00001610: 6d65 2729 295b 3a6d 6178 5f6c 656e 6774  me'))[:max_lengt
+00001620: 685d 202d 257d 0a20 2020 2020 2020 2020  h] -%}.         
+00001630: 2020 2020 2020 2020 203c 6c69 3e7b 7b20           <li>{{ 
+00001640: 6474 7970 6520 7c20 7265 6c75 726c 2870  dtype | relurl(p
+00001650: 6167 655f 7572 6c29 207d 7d3c 2f6c 693e  age_url) }}</li>
+00001660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001670: 207b 252d 2065 6e64 666f 7220 2d25 7d0a   {%- endfor -%}.
+00001680: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001690: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
+000016a0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000016b0: 2020 203c 6469 763e 0a20 2020 2020 2020     <div>.       
+000016c0: 2020 2020 2020 203c 756c 3e0a 2020 2020         <ul>.    
+000016d0: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+000016e0: 3c61 2068 7265 663d 227b 7b20 7072 6f6a  <a href="{{ proj
+000016f0: 6563 745f 7572 6c20 7d7d 2f6c 6973 7473  ect_url }}/lists
+00001700: 2f74 7970 6573 2e68 746d 6c22 3e3c 656d  /types.html"><em
+00001710: 3e41 6c6c 2064 6572 6976 6564 2074 7970  >All derived typ
+00001720: 6573 2668 656c 6c69 703b 3c2f 656d 3e3c  es&hellip;</em><
+00001730: 2f61 3e3c 2f6c 693e 0a20 2020 2020 2020  /a></li>.       
+00001740: 2020 2020 2020 203c 2f75 6c3e 0a20 2020         </ul>.   
+00001750: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001760: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00001770: 0a20 2020 2020 2020 2020 207b 2520 656e  .          {% en
+00001780: 6469 6620 257d 0a20 2020 2020 2020 203c  dif %}.        <
+00001790: 2f64 6976 3e0a 2020 2020 2020 7b25 2065  /div>.      {% e
+000017a0: 6e64 6966 2025 7d0a 7b25 2065 6e64 626c  ndif %}.{% endbl
+000017b0: 6f63 6b20 626f 6479 2025 7d0a            ock body %}.
```

### Comparing `FORD-7.0.5/ford/templates/info_page.html` & `FORD-7.0.6/ford/templates/info_page.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/macros.html` & `FORD-7.0.6/ford/templates/macros.html`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
           {% endif %}
           {% if entity | meta('category') %}
             <li class="list-inline-item" id="meta-category"><i class="fa fa-folder-open"></i> {{ entity | meta('category') }}</li>
           {% endif %}
 
           {% if line_info %}
             <li class="list-inline-item" id="statements"><i class="fa fa-list-ol"></i>
-              <a data-bs-toggle="tooltip"
-                 data-bs-placement="bottom" data-html="true"
+              <a data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-html="true"
                  title="{{ line_info }}">{{ entity | meta('num_lines') }} statements</a>
             </li>
           {% endif %}
 
           {% if incl_src %}
             <li class="list-inline-item" id="source-file">
               <i class="fa fa-code"></i>
@@ -497,15 +496,15 @@
   <div class="card">
     <div class="card-header codesum">
       <span class="anchor" id="{{ dtype.anchor }}"></span>
       <h3>
         type
         {%- if dtype.parobj == 'module' %}, {{ dtype.permission }}{% endif -%}
         {%- if dtype.sequence %}, sequence {% endif -%}
-        {{ dtype.attribs | join(", ") }}
+        {%- if dtype.attribs %}, {{ dtype.attribs | join(", ") }}{% endif -%}
         {%- if dtype.extends %}, extends({{ dtype.extends | relurl(page_url) }}){% endif -%}&nbsp;::&nbsp;
         {{ dtype | relurl(page_url) }}
         {{ deprecated(dtype) }}
       </h3>
     </div>
     <div class="card-body">
       {% if not dtype.visible %}
```

### Comparing `FORD-7.0.5/ford/templates/mod_list.html` & `FORD-7.0.6/ford/templates/mod_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/mod_page.html` & `FORD-7.0.6/ford/templates/mod_page.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/namelist_list.html` & `FORD-7.0.6/ford/templates/namelist_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/namelist_page.html` & `FORD-7.0.6/ford/templates/namelist_page.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/nongenint_page.html` & `FORD-7.0.6/ford/templates/nongenint_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,26 @@
       <h2>{% if interface.abstract %}abstract {% endif %}interface <br>
       {{ macros.proc_line(procedure,False) }}</h2>    
     {% endif %}
 
     {{ macros.use_list(interface) }}
 
     <h3>Arguments</h3>
-    {% if procedure.args|length > 0 %}
+    {% if procedure.args %}
       {{ macros.variable_list(procedure.args, intent=True) }}
     {% else %}
       <em>None</em>
     {% endif %}
     {% if procedure.retvar %}
     {% set var = procedure.retvar %}
     {% set args = 0 %}
     {% if var.kind %}{% set args = args + 1 %}{% endif %}
     {% if var.strlen %}{% set args = args + 1 %}{% endif %}
     {% if var.proto %}{% set args = args + 1 %}{% endif %}
-      <h3>Return Value <span class="anchor" id="{{ var.anchor }}"></span><small>{{ var.vartype }}{% if args > 0 -%}({% if var.kind -%}kind={{ var.kind }}{%- endif %}{% if args > 1 -%},{%- endif %}{% if var.strlen -%}len={{ var.strlen }}{%- endif %}{% if var.proto -%}{% if not var.proto[0].permission or var.proto[0].visible -%}{{ var.proto[0] }}{% else %}{{ var.proto[0].name }}{%- endif %}{{ var.proto[1] }}{%- endif %}){%- endif %}{% if var.attribs|length > 0 -%},{%- endif %}
+      <h3>Return Value <span class="anchor" id="{{ var.anchor }}"></span><small>{{ var.vartype }}{% if args > 0 -%}({% if var.kind -%}kind={{ var.kind }}{%- endif %}{% if args > 1 -%},{%- endif %}{% if var.strlen -%}len={{ var.strlen }}{%- endif %}{% if var.proto -%}{% if not var.proto[0].permission or var.proto[0].visible -%}{{ var.proto[0] }}{% else %}{{ var.proto[0].name }}{%- endif %}{{ var.proto[1] }}{%- endif %}){%- endif %}{% if var.attribs -%},{%- endif %}
   {% for attrib in var.attribs -%}{{ attrib }}{% if not loop.last or var.dimension -%}, {%- endif %}{%- endfor %}{{ var.dimension }}</small></h3>
     {{ var.doc }}
     {% endif %}
     {% if procedure.doc %}
     <h3>Description</h3>
     {{ procedure.doc }}
     {% endif %}
```

### Comparing `FORD-7.0.5/ford/templates/proc_list.html` & `FORD-7.0.6/ford/templates/proc_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/proc_page.html` & `FORD-7.0.6/ford/templates/proc_page.html`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     {% if procedure.binding %}
     <h3>Type Bound</h3>
     <p>{{ procedure.binding.parent | relurl(page_url) }}</p>
     {% endif %}
 
     <h3>Arguments</h3>
-    {% if procedure.args|length > 0 %}
+    {% if procedure.args %}
       {{ macros.variable_list(procedure.args, intent=True) }}
     {% else %}
     <em>None</em>
     <br>
     {% endif %}
     {% if procedure.retvar %}
       <h3>Return Value
@@ -68,89 +68,89 @@
       <div class="card-body">
   {{ procedure.calledbygraph }}
       </div>
     </div>
      {% endif %}
     <br>
 
-    {% if procedure.common|length > 0 %}
+    {% if procedure.common %}
     <section>
       <h2>Common Blocks</h2>
       {% for com in procedure.common %}
       {{ macros.common_block(com) }}
       {% endfor %}
     </section>
     <br>
     <script>
       $(function () {
       $('[data-bs-toggle="popover"]').popover()
       })
     </script>
     {% endif %}
 
-    {% if procedure.variables|length > 0 %}
+    {% if procedure.variables %}
     <section>    
       <h2>Variables</h2>
     {{ macros.variable_list(procedure.variables, permission=True) }}
     </section>
     <br>
     {% endif %}
     
-    {% if procedure.enums|length > 0 %}
+    {% if procedure.enums %}
     <section>
     <h2>Enumerations</h2>
     {% for enum in procedure.enums %}
       {{ macros.enum_entry(enum) }}
     {% endfor %}
     </section>
     <br>
     {% endif %}
     
-    {% if procedure.interfaces|length > 0 %}
+    {% if procedure.interfaces %}
   <section> 
      <h2>Interfaces</h2>
    {% for intr in procedure.interfaces %}
      {{ macros.interface(intr) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
 
-    {% if procedure.absinterfaces|length > 0 %}
+    {% if procedure.absinterfaces %}
     <section>
    <h2>Abstract Interfaces</h2>
    {% for intr in procedure.absinterfaces %}
      {{ macros.absinterface(intr) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
     
-    {% if procedure.types|length > 0 %}
+    {% if procedure.types %}
     <section>
    <h2>Derived Types</h2>
    {% for type in procedure.types %}
      {{ macros.type_summary(type) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
     
-    {% if procedure.functions|length > 0 %} 
+    {% if procedure.functions %} 
     <section>
     <h2>Functions</h2>
     {% for proc in procedure.functions %}
     {{ macros.proc_entry(proc) }}
     {% endfor %}
     </section>
     <br>
     {% endif %}
 
 
-    {% if procedure.subroutines|length > 0 %}
+    {% if procedure.subroutines %}
     <section>
     <h2>Subroutines</h2>
     {% for proc in procedure.subroutines %}
     {{ macros.proc_entry(proc) }}
     {% endfor %}
     </section>    
     {% endif %}
```

### Comparing `FORD-7.0.5/ford/templates/prog_list.html` & `FORD-7.0.6/ford/templates/prog_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/prog_page.html` & `FORD-7.0.6/ford/templates/prog_page.html`

 * *Files 16% similar despite different names*

```diff
@@ -29,89 +29,89 @@
       <div class="card-body">
   {{ program.callsgraph }}
       </div>
     </div>
      {% endif %}
     {% if program.doc or program.callsgraph %}<br>{% endif %}
 
-     {% if program.common|length > 0 %}
+     {% if program.common %}
      <section>
        <h2>Common Blocks</h2>
        {% for com in program.common %}
        {{ macros.common_block(com) }}
        {% endfor %}
      </section>
      <br>
      <script>
        $(function () {
        $('[data-bs-toggle="popover"]').popover()
        })
      </script>
      {% endif %}
 
-    {% if program.variables|length > 0 %}
+    {% if program.variables %}
     <section>
     <h2>Variables</h2>
     {{ macros.variable_list(program.variables) }}
     </section>
     <br>
     {% endif %}
     
-    {% if program.enums|length > 0 %}
+    {% if program.enums %}
     <section>
     <h2>Enumerations</h2>
     {% for enum in program.enums %}
       {{ macros.enum_entry(enum) }}
     {% endfor %}
     </section>
     <br>
     {% endif %}
     
-    {% if program.interfaces|length > 0 %}
+    {% if program.interfaces %}
     <section>
    <h2>Interfaces</h2>
    {% for intr in program.interfaces %}
      {{ macros.interface(intr) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
     
-    {% if program.absinterfaces|length > 0 %}
+    {% if program.absinterfaces %}
     <section>
    <h2>Abstract Interfaces</h2>
    {% for intr in program.absinterfaces %}
      {{ macros.absinterface(intr) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
 
-    {% if program.types|length > 0 %}
+    {% if program.types %}
     <section>
    <h2>Derived Types</h2>
    {% for type in program.types %}
      {{ macros.type_summary(type) }}
     {% endfor %}
     </section>
    <br>
     {% endif %}
     
-    {% if program.functions|length > 0 %} 
+    {% if program.functions %} 
     <section>
     <h2>Functions</h2>
     {% for proc in program.functions %}
     {{ macros.proc_entry(proc) }}
     {% endfor %}
     </section>
     <br>
     {% endif %}
 
 
-    {% if program.subroutines|length > 0 %}
+    {% if program.subroutines %}
     <section>
     <h2>Subroutines</h2>
     {% for proc in program.subroutines %}
     {{ macros.proc_entry(proc) }}
     {% endfor %}
     </section>    
     {% endif %}
```

### Comparing `FORD-7.0.5/ford/templates/search.html` & `FORD-7.0.6/ford/templates/search.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/templates/type_page.html` & `FORD-7.0.6/ford/templates/type_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
   
   <div class="row">
     <div class="col-md-3 hidden-xs hidden-sm visible-md visible-lg">
     {{ macros.sidebar(project,dtype) }}
     </div>
     
     <div class="col-md-9" id='text'>
-      <h2>
+      <h2 id="type-def-statement">
         type
         {%- if dtype.parobj == 'module' %}, {{ dtype.permission }}{% endif -%}
-        {{ dtype.attribs | join(", ") }}
+        {%- if dtype.attribs %}, {{ dtype.attribs | join(", ") }}{% endif -%}
         {%- if dtype.extends %}, extends({{ dtype.extends | relurl(page_url) }}){% endif %} :: {{ dtype.name }}
         {%- if dtype.sequence%}<br>sequence{% endif -%}
       </h2>
     {{ dtype.doc }}
     {% if dtype.inherbygraph or dtype.inhergraph %}<br>{% endif %}
     {% if dtype.inhergraph %}
       <div class="card">
@@ -45,15 +45,15 @@
         <div class="card-body">
           {{ dtype.inherbygraph }}
         </div>
       </div>
     {% endif %}
     <br>
 
-    {% if dtype.variables|length > 0 %}
+    {% if dtype.variables %}
     <section>
     <h2>Components</h2>
     {{ macros.variable_list(dtype.variables, permission=True) }}
     </section>
     <br>
     {% endif %}
```

### Comparing `FORD-7.0.5/ford/templates/types_list.html` & `FORD-7.0.6/ford/templates/types_list.html`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipue_search.py` & `FORD-7.0.6/ford/tipue_search.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/.DS_Store` & `FORD-7.0.6/ford/tipuesearch/.DS_Store`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/img/.DS_Store` & `FORD-7.0.6/ford/tipuesearch/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/img/loader.gif` & `FORD-7.0.6/ford/tipuesearch/img/loader.gif`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/tipuesearch.css` & `FORD-7.0.6/ford/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/tipuesearch.js` & `FORD-7.0.6/ford/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/tipuesearch.min.js` & `FORD-7.0.6/ford/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/tipuesearch/tipuesearch_set.js` & `FORD-7.0.6/ford/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/ford/utils.py` & `FORD-7.0.6/ford/utils.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/output-example.png` & `FORD-7.0.6/output-example.png`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/pyproject.toml` & `FORD-7.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,8 @@
 
 [tool.pytest.ini_options]
 addopts = "-m 'not slow'"
 markers = ["slow"]
 
 [tool.ruff]
 line-length = 88
-ignore = ["E501"]
+lint.ignore = ["E501"]
```

### Comparing `FORD-7.0.5/test/conftest.py` & `FORD-7.0.6/test/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import ford
 import pathlib
 import pytest
 from textwrap import dedent
 import subprocess
 
 # Ford default src folder
```

### Comparing `FORD-7.0.5/test/test_corpus.py` & `FORD-7.0.6/test/test_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,20 @@
         (
             "https://github.com/cibinjoseph/naturalFRUIT",
             "naturalFRUIT/ford_input.md",
             "",
         ),
         ("https://github.com/fortran-lang/fftpack", "fftpack/API-doc-FORD-file.md", ""),
         ("https://github.com/fortran-lang/fpm", "fpm/docs.md", ""),
-        ("https://github.com/fortran-lang/stdlib", "stdlib/API-doc-FORD-file.md", ""),
+        (
+            "https://github.com/fortran-lang/stdlib",
+            "stdlib/API-doc-FORD-file.md",
+            # The linear algebra files cause massive slowdown, although I'm not sure why yet
+            '--config=exclude=["**/*linalg**"]',
+        ),
         (
             "https://github.com/jacobwilliams/Fortran-Astrodynamics-Toolkit",
             "Fortran-Astrodynamics-Toolkit/ford.md",
             "",
         ),
         (
             "https://github.com/jacobwilliams/bspline-fortran",
```

### Comparing `FORD-7.0.5/test/test_example.py` & `FORD-7.0.6/test/test_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,7 +517,15 @@
 
 def test_linking_to_page_alias_from_nested_page(example_project):
     path, _ = example_project
     subsubpage = read_html(path / "page/subdir/subsubpage.html")
 
     link = subsubpage.find("a", string=re.compile("such as"))
     assert link["href"] == "../subpage1.html"
+
+
+def test_type_attributes(example_project):
+    path, _ = example_project
+    type_page = read_html(path / "type/say_type_base.html")
+
+    def_statement = type_page.find(id="type-def-statement")
+    assert def_statement.text.strip() == "type, public, abstract :: say_type_base"
```

### Comparing `FORD-7.0.5/test/test_graphs.py` & `FORD-7.0.6/test/test_graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ford.fortran_project import Project
 from ford import ProjectSettings
 from ford.graphs import graphviz_installed, GraphManager
 import ford.sourceform
 from ford._markdown import MetaMarkdown
+from ford.settings import INTRINSIC_MODS
 
 from textwrap import dedent
 from typing import Dict
 
 
 import pytest
 from bs4 import BeautifulSoup
@@ -157,15 +158,18 @@
 
     settings = ProjectSettings(
         src_dir=src_dir, graph=True, proc_internals=proc_internals
     )
     project = create_project(settings)
 
     graphs = GraphManager(
-        graphdir="", parentdir="..", coloured_edges=True, show_proc_parent=True
+        graphdir="",
+        parentdir="..",
+        coloured_edges=True,
+        show_proc_parent=proc_internals,
     )
     for entity_list in [
         project.types,
         project.procedures,
         project.submodprocedures,
         project.modules,
         project.submodules,
@@ -216,15 +220,15 @@
                 "a",
                 "b",
                 "c",
                 "c_submod",
                 "c_subsubmod",
                 "iso_fortran_env",
                 "external_mod",
-                "foo::three",
+                "three",
                 "foo",
             ],
             [
                 "module~b->module~a",
                 "module~c->module~b",
                 "module~c->iso_fortran_env",
                 "module~c->external_mod",
@@ -235,30 +239,30 @@
             ],
             MOD_GRAPH_KEY,
         ),
         (
             {"proc_internals": False},
             ["callgraph"],
             [
-                "c::defined_elsewhere",
-                "c::submod_proc",
-                "c_subsubmod::submod_proc",
-                "c::one",
-                "foo::three",
-                "c::two",
-                "foo::four",
+                "defined_elsewhere",
+                "submod_proc",
+                "submod_proc",
+                "one",
+                "three",
+                "two",
+                "four",
                 "other_sub",
                 "foo",
-                "c::alpha%five",
-                "c::alpha%six",
-                "c::seven",
-                "c::alpha%eight",
-                "c::alpha%nine",
-                "c::alpha%eight_nine",
-                "c::alpha%ten",
+                "alpha%five",
+                "alpha%six",
+                "seven",
+                "alpha%eight",
+                "alpha%nine",
+                "alpha%eight_nine",
+                "alpha%ten",
             ],
             [
                 "proc~three->proc~one",
                 "proc~three->proc~two",
                 "proc~two->proc~one",
                 "proc~three->other_sub",
                 "program~foo->proc~three",
@@ -364,15 +368,15 @@
             ["derived", "leaf", "thing"],
             ["type~leaf->type~derived", "type~thing->type~derived"],
             TYPE_GRAPH_KEY,
         ),
         (
             {"proc_internals": False},
             ["procedures", "two", "callsgraph"],
-            ["c::one", "c::two"],
+            ["one", "two"],
             ["proc~two->proc~one"],
             PROC_GRAPH_KEY,
         ),
         (
             {"proc_internals": True},
             ["procedures", "seven", "callsgraph"],
             ["c::seven", "c::one", "seven::seven_one", "seven::seven_two"],
@@ -383,22 +387,22 @@
                 "none~seven_two->proc~one",
             ],
             PROC_GRAPH_KEY,
         ),
         (
             {"proc_internals": False},
             ["procedures", "two", "calledbygraph"],
-            ["foo::three", "c::two", "foo"],
+            ["three", "two", "foo"],
             ["proc~three->proc~two", "program~foo->proc~three"],
             PROC_GRAPH_KEY,
         ),
         (
             {"proc_internals": False},
             ["procedures", "three", "usesgraph"],
-            ["external_mod", "foo::three"],
+            ["external_mod", "three"],
             ["proc~three->external_mod"],
             MOD_GRAPH_KEY,
         ),
         (
             {"proc_internals": True},
             [
                 "procedures",
@@ -456,14 +460,23 @@
 
     legend = svgs[1]
     legend_nodes = [s.title.text for s in legend.find_all("g", class_="node")]
     assert legend_nodes == expected_legend_nodes + ["This Page's Entity"]
     assert legend.find_all("g", class_="edge") == []
 
 
+def test_external_module_links(make_project_graphs):
+    graphs = make_project_graphs
+
+    soup = BeautifulSoup(str(graphs.usegraph), features="html.parser")
+    iso_fortran_env_node = soup.find(string="iso_fortran_env").parent.parent
+    link = iso_fortran_env_node.a["xlink:href"]
+    assert link == INTRINSIC_MODS["iso_fortran_env"]
+
+
 def test_graphs_as_table(tmp_path):
     data = """\
     program foo
     contains
       subroutine one
       end subroutine one
```

### Comparing `FORD-7.0.5/test/test_initialisation.py` & `FORD-7.0.6/test/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_markdown.py` & `FORD-7.0.6/test/test_markdown.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_md_admonition.py` & `FORD-7.0.6/test/test_md_admonition.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_md_inputs.py` & `FORD-7.0.6/test/test_md_inputs.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_md_table.py` & `FORD-7.0.6/test/test_md_table.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_pagetree.py` & `FORD-7.0.6/test/test_pagetree.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_project.py` & `FORD-7.0.6/test/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     FortranModule,
     NameSelector,
 )
 from ford._markdown import MetaMarkdown
 import ford.sourceform
 
 from itertools import chain
-from os.path import relpath
-import pathlib
 
 import pytest
 from bs4 import BeautifulSoup
 
 
 @pytest.fixture
 def copy_fortran_file(tmp_path):
@@ -1041,15 +1039,15 @@
     assert mod_c.ancestor_module == mod_a
 
     assert mod_d.parent_submodule == mod_c
     assert mod_d.ancestor_module == mod_a
 
 
 def test_make_links(copy_fortran_file):
-    links = "[[a]] [[b(type)]] [[b:c]] [[a:d]] [[b:e]] [[f(proc)]] [[a:g]] [[h]]"
+    links = "[[a]] [[b(type)]] [[b:c]] [[a:d]] [[b:e]] [[F(proc)]] [[A:G]] [[H]] [[I]]"
 
     data = f"""\
     module a !! {links}
       type b !! {links}
         integer :: c !! {links}
       contains
         final :: d !! {links}
@@ -1071,14 +1069,85 @@
       function f() !! {links}
         type(b) :: f !! {links}
       end function f
     end module a
 
     program h !! {links}
     end program h
+
+    submodule (a) i !! {links}
+    end submodule i
+    """
+    settings = copy_fortran_file(data)
+    project = create_project(settings)
+    md = MetaMarkdown(project=project)
+    project.markdown(md)
+
+    expected_links = {
+        "a": "../module/a.html",
+        "b": "../type/b.html",
+        "c": "../type/b.html#variable-c",
+        "d": "../proc/d.html",
+        "e": "../type/b.html#boundprocedure-e",
+        "f": "../proc/f.html",
+        "g": "../module/a.html#variable-g",
+        "h": "../program/h.html",
+        "i": "../module/i.html",
+    }
+
+    for item in chain(
+        project.files[0].children,
+        project.types[0].children,
+        project.procedures[0].children,
+        project.procedures[2].children,
+    ):
+        docstring = BeautifulSoup(item.doc, features="html.parser")
+        link_locations = {a.string: a.get("href", None) for a in docstring("a")}
+
+        assert link_locations == expected_links, (item, item.name)
+
+
+def test_make_links_with_entity_spec(copy_fortran_file):
+    links = (
+        "[[a(module)]] [[b(type)]] [[b(type):c(variable)]] "
+        "[[A(MODULE):D(SUBROUTINE)]] [[B(TYPE):E]] [[F(PROC)]] "
+        "[[A(module):G(variable)]] [[H(program)]] [[I(SUBMODULE)]]"
+    )
+
+    data = f"""\
+    module a !! {links}
+      type b !! {links}
+        integer :: c !! {links}
+      contains
+        final :: d !! {links}
+        procedure :: e !! {links}
+      end type b
+
+      interface b !! {links}
+        module procedure f
+      end interface b
+
+      type(b) :: g !! {links}
+    contains
+      subroutine d(self) !! {links}
+        type(b) :: self !! {links}
+      end subroutine d
+      subroutine e(self) !! {links}
+        class(b) :: self !! {links}
+      end subroutine e
+      function f() !! {links}
+        type(b) :: f !! {links}
+      end function f
+    end module a
+
+    program h !! {links}
+    end program h
+
+    submodule (a) i !! {links}
+    end submodule i
     """
     settings = copy_fortran_file(data)
     project = create_project(settings)
     md = MetaMarkdown(project=project)
     project.markdown(md)
 
     expected_links = {
@@ -1086,40 +1155,41 @@
         "b": "../type/b.html",
         "c": "../type/b.html#variable-c",
         "d": "../proc/d.html",
         "e": "../type/b.html#boundprocedure-e",
         "f": "../proc/f.html",
         "g": "../module/a.html#variable-g",
         "h": "../program/h.html",
+        "i": "../module/i.html",
     }
 
     for item in chain(
         project.files[0].children,
         project.types[0].children,
         project.procedures[0].children,
         project.procedures[2].children,
     ):
         docstring = BeautifulSoup(item.doc, features="html.parser")
         link_locations = {a.string: a.get("href", None) for a in docstring("a")}
 
         assert link_locations == expected_links, (item, item.name)
 
 
-def test_link_with_context(copy_fortran_file):
+def test_make_links_with_context(copy_fortran_file):
     data = """\
     module a !! [[g]]
       type b !! [[c]] [[e]] [[g]]
         integer :: c
       contains
         procedure :: e
       end type b
 
       type(b) :: g
     contains
-      subroutine d(i) !! [[i]] [[f]] [[f:x]]
+      subroutine d(i) !! [[I]] [[F]] [[F:X]]
         type(b) :: i
         contains
           integer function f(x)
             integer :: x
           end function f
       end subroutine d
     end module a
```

### Comparing `FORD-7.0.5/test/test_projects/test_external_project.py` & `FORD-7.0.6/test/test_projects/test_external_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import shutil
 import sys
 import os
 import pathlib
-import copy
 from urllib.parse import urlparse
 import json
 from typing import Dict, Any
 
 import ford
 
 from bs4 import BeautifulSoup
```

### Comparing `FORD-7.0.5/test/test_reader.py` & `FORD-7.0.6/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_settings.py` & `FORD-7.0.6/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test/test_sourceform.py` & `FORD-7.0.6/test/test_sourceform.py`

 * *Files 1% similar despite different names*

```diff
@@ -2223,7 +2223,36 @@
     project = FakeProject()
     module = parse_fortran_file(data).modules[0]
     module.correlate(project)
 
     example_type = module.types[0]
     assert example_type.num_lines == 8
     assert example_type.num_lines_all == 8 + 9
+
+
+def test_associate_array(parse_fortran_file):
+    data = """\
+    subroutine test()
+      associate(phi => [1,2], theta => (/ 3, 4 /))
+      end associate
+    end subroutine test"""
+
+    # Just check we can parse ok
+    parse_fortran_file(data)
+
+
+def test_blocks_with_type(parse_fortran_file):
+    data = """\
+    module foo
+    contains
+      subroutine sub1()
+        block
+          type :: t1
+          end type t1
+        end block
+      end subroutine sub1
+    end module foo
+    """
+
+    source = parse_fortran_file(data)
+    module = source.modules[0]
+    assert len(module.subroutines) == 1
```

### Comparing `FORD-7.0.5/test/test_utils.py` & `FORD-7.0.6/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/external_project/external_project/src/external.f90` & `FORD-7.0.6/test_data/external_project/external_project/src/external.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/external_project/top_level_project/src/top_level.f90` & `FORD-7.0.6/test_data/external_project/top_level_project/src/top_level.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/ford_issues_bad.f90` & `FORD-7.0.6/test_data/ford_issues_bad.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/ford_issues_ok.f90` & `FORD-7.0.6/test_data/ford_issues_ok.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/ford_issues_ok_expected.f90` & `FORD-7.0.6/test_data/ford_issues_ok_expected.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/ford_test_program.f90` & `FORD-7.0.6/test_data/ford_test_program.f90`

 * *Files identical despite different names*

### Comparing `FORD-7.0.5/test_data/ford_test_program_expected.f90` & `FORD-7.0.6/test_data/ford_test_program_expected.f90`

 * *Files identical despite different names*

