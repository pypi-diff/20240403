# Comparing `tmp/mkdoxy-1.1.7.tar.gz` & `tmp/mkdoxy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.7.tar", last modified: Thu Nov  9 12:22:20 2023, max compression
+gzip compressed data, was "mkdoxy-1.2.0.tar", last modified: Tue Apr  2 23:48:25 2024, max compression
```

## Comparing `mkdoxy-1.1.7.tar` & `mkdoxy-1.2.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-11-09 12:22:20.167018 mkdoxy-1.1.7/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.7/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5905 2023-11-09 12:22:20.166659 mkdoxy-1.1.7/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.7/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-11-09 12:22:20.160951 mkdoxy-1.1.7/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2935 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.7/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      303 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     3585 2023-11-09 12:15:43.000000 mkdoxy-1.1.7/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     5619 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     5432 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     2414 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    13298 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    19374 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    14411 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     5270 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    26601 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     8940 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)    11715 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-11-09 12:22:20.165808 mkdoxy-1.1.7/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.7/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.7/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.7/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      614 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      165 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      582 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      408 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      499 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      438 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.7/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.7/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4633 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.7/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      414 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.7/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      457 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      233 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3534 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     9918 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-11-09 12:22:20.162104 mkdoxy-1.1.7/mkdoxy.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     5905 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1087 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      124 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-11-09 12:22:20.000000 mkdoxy-1.1.7/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       62 2023-10-10 12:59:26.000000 mkdoxy-1.1.7/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-11-09 12:22:20.167065 mkdoxy-1.1.7/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1807 2023-11-09 12:16:18.000000 mkdoxy-1.1.7/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.912005 mkdoxy-1.2.0/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.0/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5999 2024-04-02 23:48:25.911688 mkdoxy-1.2.0/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.2.0/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.903595 mkdoxy-1.2.0/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2935 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.0/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      303 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3585 2023-11-09 12:15:43.000000 mkdoxy-1.2.0/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-02 23:45:50.000000 mkdoxy-1.2.0/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9922 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-02 23:45:50.000000 mkdoxy-1.2.0/mkdoxy/filters.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2414 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-02-14 21:55:15.000000 mkdoxy-1.2.0/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    19728 2024-04-02 23:45:52.000000 mkdoxy-1.2.0/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    15034 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-02 23:45:55.000000 mkdoxy-1.2.0/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9076 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11685 2024-04-02 23:45:56.000000 mkdoxy-1.2.0/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910061 mkdoxy-1.2.0/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.2.0/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      614 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      582 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      408 2023-12-27 13:57:12.000000 mkdoxy-1.2.0/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      499 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      438 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      791 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.2.0/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      414 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      233 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3534 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-02 23:45:59.000000 mkdoxy-1.2.0/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910717 mkdoxy-1.2.0/mkdoxy.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5999 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      156 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       62 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-04-02 23:48:25.912063 mkdoxy-1.2.0/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1869 2024-04-02 23:43:44.000000 mkdoxy-1.2.0/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910318 mkdoxy-1.2.0/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/tests/test_doxyrun.py
```

### Comparing `mkdoxy-1.1.7/LICENSE` & `mkdoxy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/PKG-INFO` & `mkdoxy-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.7
+Version: 1.2.0
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
@@ -17,20 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs
 Provides-Extra: dev
-Requires-Dist: mkdocs-material==9.1.18; extra == "dev"
+Requires-Dist: mkdocs-material~=9.1.18; extra == "dev"
 Requires-Dist: Jinja2~=3.1.2; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev"
 Requires-Dist: pathlib~=1.0.1; extra == "dev"
 Requires-Dist: path~=16.7.1; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
+Requires-Dist: pytest~=6.2.5; extra == "dev"
+Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.7 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.0 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: mkdocs Provides-Extra: dev Requires-Dist: mkdocs-
-material==9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+material~=9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev" Requires-Dist:
 pathlib~=1.0.1; extra == "dev" Requires-Dist: path~=16.7.1; extra == "dev"
-Requires-Dist: isort~=5.12.0; extra == "dev" # MkDoxy **[MkDoxy](https://
-mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)**
-generates API documentation based on **[Doxygen](https://www.doxygen.nl)**
-comments and **[code snippets](/intro)** in your markdown files.
+Requires-Dist: isort~=5.12.0; extra == "dev" Requires-Dist: pytest~=6.2.5;
+extra == "dev" Requires-Dist: pre-commit~=3.7.0; extra == "dev" # MkDoxy **
+[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://
+www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://
+www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown
+files.
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_J_a_k_u_b_A_n_d_r_y_s_e_k_%_2_F_M_k_D_o_x_y_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_t_r_u_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
```

### Comparing `mkdoxy-1.1.7/README.md` & `mkdoxy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.2.0/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/constants.py` & `mkdoxy-1.2.0/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/doxygen.py` & `mkdoxy-1.2.0/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/finder.py` & `mkdoxy-1.2.0/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/generatorAuto.py` & `mkdoxy-1.2.0/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/generatorBase.py` & `mkdoxy-1.2.0/mkdoxy/generatorBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import os
 import string
 from typing import Dict
 
-from jinja2 import Template
+from jinja2 import BaseLoader, Environment, Template
 from jinja2.exceptions import TemplateError
 from mkdocs import exceptions
 
 import mkdoxy
 from mkdoxy.constants import Kind
+from mkdoxy.filters import use_code_language
 from mkdoxy.node import DummyNode, Node
 from mkdoxy.utils import (
     merge_two_dicts,
     parseTemplateFile,
     recursive_find,
     recursive_find_with_parent,
 )
@@ -34,23 +35,25 @@
         @param debug (bool): If True, debug messages will be printed (default: False)
         """
 
         self.debug: bool = debug  # if True, debug messages will be printed
         self.templates: Dict[str, Template] = {}
         self.metaData: Dict[str, list[str]] = {}
 
+        environment = Environment(loader=BaseLoader())
+        environment.filters["use_code_language"] = use_code_language
         # code from https://github.com/daizutabi/mkapi/blob/master/mkapi/core/renderer.py#L29-L38
         path = os.path.join(os.path.dirname(mkdoxy.__file__), "templates")
         for fileName in os.listdir(path):
             filePath = os.path.join(path, fileName)
             if fileName.endswith(".jinja2"):
                 with open(filePath, "r") as file:
                     name = os.path.splitext(fileName)[0]
                     fileTemplate, metaData = parseTemplateFile(file.read())
-                    self.templates[name] = Template(fileTemplate)
+                    self.templates[name] = environment.from_string(fileTemplate)
                     self.metaData[name] = metaData
             else:
                 log.error(f"Trying to load unsupported file '{filePath}'. Supported file ends with '.jinja2'.")
 
         # test if templateDir is existing
         if templateDir:
             if not os.path.exists(templateDir):
@@ -110,18 +113,21 @@
         code_header: str = "",
         code: str = "",
         code_language: str = "",
         snippet_code: str = "",
     ):
         """! Render an error page.
         @details
-        @param title (str): Title of the error page (default: "")
-        @param message (str): Message of the error page (default: "")
-        @param language (str): Programming language of the error page (default: "")
-        @return (str): Rendered error page.
+        @param config (dict): Config for the template.
+        @param title (str): Title of the error.
+        @param description (str): Description of the error.
+        @param code_header (str): Header of the code (default: "")
+        @param code (str): Code (default: "")
+        @param code_language (str): Language of the code (default: "")
+        @param snippet_code (str): Snippet code (default: "")
         """
         if config is None:
             config = {}
         template, metaConfig = self.loadConfigAndTemplate("error")
 
         data = {
             "title": title,
```

### Comparing `mkdoxy-1.1.7/mkdoxy/generatorSnippets.py` & `mkdoxy-1.2.0/mkdoxy/generatorSnippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,17 @@
         )
 
     def doxyCode(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, ["file"])
         if errorMsg:
             return errorMsg
         node = self.finder.doxyCode(project, config.get("file"))
+        if node is None:
+            return self.doxyNodeIsNone(project, config, snippet)
+
         if isinstance(node, Node):
             progCode = self.codeStrip(
                 node.programlisting,
                 node.code_language,
                 config.get("start", 1),
                 config.get("end", 0),
             )
@@ -264,14 +267,17 @@
 
     def doxyFunction(self, snippet, project: str, config: dict):
         errorMsg = self.checkConfig(snippet, project, config, ["name"])
         if errorMsg:
             return errorMsg
 
         node = self.finder.doxyFunction(project, config.get("name"))
+        if node is None:
+            return self.doxyNodeIsNone(project, config, snippet)
+
         if isinstance(node, Node):
             self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].function(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect function configuration",
@@ -284,14 +290,17 @@
 
     def doxyClass(self, snippet, project: str, config: dict):
         errorMsg = self.checkConfig(snippet, project, config, ["name"])
         if errorMsg:
             return errorMsg
 
         node = self.finder.doxyClass(project, config.get("name"))
+        if node is None:
+            return self.doxyNodeIsNone(project, config, snippet)
+
         if isinstance(node, Node):
             self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].member(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect class configuration",
@@ -304,14 +313,17 @@
 
     def doxyClassMethod(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, ["name", "method"])
         if errorMsg:
             return errorMsg
 
         node = self.finder.doxyClassMethod(project, config.get("name"), config.get("method"))
+        if node is None:
+            return self.doxyNodeIsNone(project, config, snippet)
+
         if isinstance(node, Node):
             self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].function(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect class method configuration",
@@ -358,14 +370,24 @@
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].files.children
         self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].fileindex(nodes, config)
 
+    def doxyNodeIsNone(self, project: str, config: dict, snippet: str) -> str:
+        return self.doxyError(
+            project,
+            config,
+            "Node is None",
+            "Node is None",
+            "yaml",
+            snippet,
+        )
+
 
 ### Create documentation generator callbacks END
 
 
 class SnippetClass:
     def __init__(self, config):
         self.config = config
```

### Comparing `mkdoxy-1.1.7/mkdoxy/markdown.py` & `mkdoxy-1.2.0/mkdoxy/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,19 @@
     def __init__(self, lines: List[str]):
         self.lines = lines
 
     def append(self, line: str):
         self.lines.append(line)
 
     def render(self, f: MdRenderer, indent: str):
+        f.write("```\n")
         for line in self.lines:
             f.write(line)
             f.write("\n")
+        f.write("```\n")
 
 
 class MdBlockQuote(Md):
     def __init__(self, children: List[Md]):
         Md.__init__(self, children)
 
     def render(self, f: MdRenderer, indent: str):
```

### Comparing `mkdoxy-1.1.7/mkdoxy/node.py` & `mkdoxy-1.2.0/mkdoxy/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -683,15 +683,15 @@
                         code.append(f"    {param},")
                 code.append(f") {self._initializer.plain()}")
             else:
                 code.append(f"#define {self.name_full_unescaped} {self._initializer.plain()}")
 
         else:
             code.append(self._definition.plain())
-        return "\n".join(code)
+        return "\n".join(["```", *code, "```"])
 
     @property
     def has_base_classes(self) -> bool:
         return len(self._xml.findall("basecompoundref")) > 0
 
     @property
     def has_derived_classes(self) -> bool:
```

### Comparing `mkdoxy-1.1.7/mkdoxy/plugin.py` & `mkdoxy-1.2.0/mkdoxy/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     # Config options for each project
     config_project = (
         ("src-dirs", config_options.Type(str)),
         ("full-doc", config_options.Type(bool, default=True)),
         ("debug", config_options.Type(bool, default=False)),
         # ('ignore-errors', config_options.Type(bool, default=False)),
         ("doxy-cfg", config_options.Type(dict, default={}, required=False)),
+        ("doxy-cfg-file", config_options.Type(str, default="", required=False)),
         ("template-dir", config_options.Type(str, default="", required=False)),
     )
 
     def is_enabled(self) -> bool:
         """! Checks if the plugin is enabled
         @details
         @return: (bool) True if the plugin is enabled.
@@ -115,14 +116,15 @@
             # Check src changes -> run Doxygen
             runPath = os.path.dirname(config.config_file_path) if config.config_file_path else None
             doxygenRun = DoxygenRun(
                 self.config["doxygen-bin-path"],
                 project_data.get("src-dirs"),
                 tempDirApi,
                 project_data.get("doxy-cfg", {}),
+                project_data.get("doxy-cfg-file", ""),
                 runPath,
             )
             if doxygenRun.checkAndRun():
                 log.info("  -> generating Doxygen files")
             else:
                 log.info("  -> skip generating Doxygen files (nothing changes)")
```

### Comparing `mkdoxy-1.1.7/mkdoxy/property.py` & `mkdoxy-1.2.0/mkdoxy/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,20 +184,19 @@
                     if notype:
                         declname = param.find("declname")
                         if declname is None:
                             declname = param.find("type")
                         ret.append(self.parser.paras_as_str(declname, plain=plain))
                     else:
                         type = param.find("type")
+                        declaration = self.parser.paras_as_str(type, plain=plain)
                         declname = param.find("declname")
-                        if declname is None:
-                            declname = param.find("type")
-                        ret.append(
-                            f"{self.parser.paras_as_str(type, plain=plain)} {self.parser.paras_as_str(declname, plain=plain)}"  # noqa: E501
-                        )
+                        if declname is not None:
+                            declaration += f" {self.parser.paras_as_str(declname, plain=plain)}"
+                        ret.append(declaration)
             return ret
 
         def has(self) -> bool:
             return self.xml.find("templateparamlist") is not None
 
     class CodeBlock:
         def __init__(self, xml: Element, parser: XmlParser, kind: Kind):
```

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/code.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/error.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/templates/member.jinja2` & `mkdoxy-1.2.0/mkdoxy/templates/member.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 {%- endfor -%}
 
 {{ templateMemTab.render({'config': {"":""}, 'node': node, 'parent': None, 'title': 'Macros', 'visibility': 'public', 'kinds': ['define'], 'static': False}) }}
 
 {%- if node.has_details %}
 # Detailed Description
 
-{{node.details}}
+{{node.details | use_code_language(node.code_language)}}
 {%- endif %}
 
 {%- for visibility in ['public', 'protected'] -%}
 {%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['properties', ['property']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {%- if node.has(visibility, query[1], static[1]) %}
 ## {{visibility|title}} {{static[0]|title}}{{query[0]|title}} Documentation
```

### Comparing `mkdoxy-1.1.7/mkdoxy/utils.py` & `mkdoxy-1.2.0/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.7/mkdoxy/xml_parser.py` & `mkdoxy-1.2.0/mkdoxy/xml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     MdTable,
     MdTableCell,
     MdTableRow,
     Text,
 )
 from mkdoxy.utils import lookahead
 
+# https://www.doxygen.nl/manual/commands.html
 SIMPLE_SECTIONS = {
     "see": "See also:",
     "note": "Note:",
     "bug": "Bug:",
     "warning": "Warning:",
     "return": "Returns:",
     "returns": "Returns:",
@@ -41,24 +42,25 @@
     "post": "Postcondition:",
     "rcs": "Rcs:",
     "attention": "Attention:",
     "invariant": "Invariant:",
     "exception": "Exception:",
     "date": "Date:",
     "version": "Version:",
+    "par": "\r\n",
 }
 
 
 class XmlParser:
     def __init__(self, cache: Cache, debug: bool = False):
         self.cache = cache
         self.debug = debug
 
     def anchor(self, name: str) -> str:
-        return '<a name="' + name + '"></a>'
+        return f'<a name="{name}"></a>'
 
     def paras_as_str(self, p: Element, italic: bool = False, plain: bool = False) -> str:
         if plain:
             return self.plain_as_str(p)
         renderer = MdRenderer()
         for m in self.paras(p, italic=italic):
             m.render(renderer, "")
@@ -229,15 +231,15 @@
             elif item.tag == "parameterlist":
                 parameteritems = item.findall("parameteritem")
                 lst = MdList([])
                 for parameteritem in parameteritems:
                     name = parameteritem.find("parameternamelist").find("parametername")
                     description = parameteritem.find("parameterdescription").findall("para")
                     par = MdParagraph([])
-                    if len(name) > 0:
+                    if name is not None and len(name) > 0:
                         par.extend(self.paras(name))
                     else:
                         par.append(Code(name.text))
                     par.append(Text(" "))
                     for ip in description:
                         par.extend(self.paras(ip))
                     lst.append(par)
```

### Comparing `mkdoxy-1.1.7/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.2.0/mkdoxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.7
+Version: 1.2.0
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
@@ -17,20 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs
 Provides-Extra: dev
-Requires-Dist: mkdocs-material==9.1.18; extra == "dev"
+Requires-Dist: mkdocs-material~=9.1.18; extra == "dev"
 Requires-Dist: Jinja2~=3.1.2; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev"
 Requires-Dist: pathlib~=1.0.1; extra == "dev"
 Requires-Dist: path~=16.7.1; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
+Requires-Dist: pytest~=6.2.5; extra == "dev"
+Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.7 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.0 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: mkdocs Provides-Extra: dev Requires-Dist: mkdocs-
-material==9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+material~=9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev" Requires-Dist:
 pathlib~=1.0.1; extra == "dev" Requires-Dist: path~=16.7.1; extra == "dev"
-Requires-Dist: isort~=5.12.0; extra == "dev" # MkDoxy **[MkDoxy](https://
-mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)**
-generates API documentation based on **[Doxygen](https://www.doxygen.nl)**
-comments and **[code snippets](/intro)** in your markdown files.
+Requires-Dist: isort~=5.12.0; extra == "dev" Requires-Dist: pytest~=6.2.5;
+extra == "dev" Requires-Dist: pre-commit~=3.7.0; extra == "dev" # MkDoxy **
+[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://
+www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://
+www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown
+files.
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_J_a_k_u_b_A_n_d_r_y_s_e_k_%_2_F_M_k_D_o_x_y_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_t_r_u_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
```

### Comparing `mkdoxy-1.1.7/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.2.0/mkdoxy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 mkdoxy/DoxyTagParser.py
 mkdoxy/__init__.py
 mkdoxy/cache.py
 mkdoxy/constants.py
 mkdoxy/doxygen.py
 mkdoxy/doxyrun.py
+mkdoxy/filters.py
 mkdoxy/finder.py
 mkdoxy/generatorAuto.py
 mkdoxy/generatorBase.py
 mkdoxy/generatorSnippets.py
 mkdoxy/markdown.py
 mkdoxy/node.py
 mkdoxy/plugin.py
@@ -36,8 +37,9 @@
 mkdoxy/templates/memDef.jinja2
 mkdoxy/templates/memTab.jinja2
 mkdoxy/templates/member.jinja2
 mkdoxy/templates/modules.jinja2
 mkdoxy/templates/namespaces.jinja2
 mkdoxy/templates/page.jinja2
 mkdoxy/templates/programlisting.jinja2
-mkdoxy/templates/relatedPages.jinja2
+mkdoxy/templates/relatedPages.jinja2
+tests/test_doxyrun.py
```

### Comparing `mkdoxy-1.1.7/setup.py` & `mkdoxy-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name="mkdoxy",
-    version="1.1.7",
+    version="1.2.0",
     description="MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator",  # noqa: E501
     url="https://github.com/JakubAndrysek/MkDoxy",
     author="Jakub Andrýsek",
     author_email="email@kubaandrysek.cz",
@@ -29,20 +29,22 @@
         "Documentation": "https://mkdoxy.kubaandrysek.cz/",
         "Tracker": "https://github.com/JakubAndrysek/MkDoxy/issues",
         "Funding": "https://github.com/sponsors/jakubandrysek",
     },
     install_requires=["mkdocs"],
     extras_require={
         "dev": [
-            "mkdocs-material==9.1.18",
+            "mkdocs-material~=9.1.18",
             "Jinja2~=3.1.2",
             "mkdocs-open-in-new-tab~=1.0.2",
             "pathlib~=1.0.1",
             "path~=16.7.1",
             "isort~=5.12.0",
+            "pytest~=6.2.5",
+            "pre-commit~=3.7.0",
         ],
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

