# Comparing `tmp/shells_cae-0.0.8.tar.gz` & `tmp/shells_cae-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shells_cae-0.0.8.tar", last modified: Wed Nov 16 00:02:12 2022, max compression
+gzip compressed data, was "shells_cae-0.0.9.tar", last modified: Fri Nov 18 13:23:20 2022, max compression
```

## Comparing `shells_cae-0.0.8.tar` & `shells_cae-0.0.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      177 2022-11-16 00:02:12.971860 shells_cae-0.0.8/PKG-INFO
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)       32 2022-11-09 20:52:29.000000 shells_cae-0.0.8/README.md
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)       38 2022-11-16 00:02:12.971860 shells_cae-0.0.8/setup.cfg
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1341 2022-11-16 00:00:10.000000 shells_cae-0.0.8/setup.py
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1000 2022-11-15 22:02:15.000000 shells_cae-0.0.8/shells_cae/__init__.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5002 2022-11-15 22:02:15.000000 shells_cae-0.0.8/shells_cae/al_tate_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2755 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/apfsd_fl_stable_solver.py
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae/compiled/
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae/compiled/al_tate_model/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1004 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/al_tate_model/CMakeLists.txt
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae/compiled/al_tate_model/src/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    10761 2022-11-15 23:57:51.000000 shells_cae-0.0.8/shells_cae/compiled/al_tate_model/src/penetration.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      629 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/al_tate_model/src/test.f90
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae/compiled/build/
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/build/bin/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   126290 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/ballistics.exe
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/
--rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    22296 2022-11-15 23:54:33.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libmcdrag.so
--rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    19288 2022-11-15 23:58:05.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libpenetrationlib.so
--rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    26816 2022-11-15 23:54:34.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libsextbal.so
--rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    60600 2022-11-15 23:54:34.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libsintbal.so
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   129010 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/libmcdrag.dll
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   136663 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/libpenetrationlib.dll
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   117084 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/libsextbal.dll
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   790530 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/libsintbal.dll
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)   126229 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/build/bin/mcdrag_lib.exe
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/external_ballistics/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      758 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/external_ballistics/CMakeLists.txt
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/external_ballistics/src/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5440 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/external_ballistics/src/solve_eb.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7139 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/external_ballistics/src/solve_ebh.f90
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      786 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/CMakeLists.txt
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4618 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/ibstructs.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1727 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/preproc.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    12023 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/solve_ib.f90
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/kontur/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1511 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/CMakeLists.txt
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4518 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/csv_header.txt
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/kontur/include/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4563 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/include/csv.h
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      967 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/include/kontur.h
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4806 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/include/structs.h
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/kontur/src/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     6809 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/csv.c
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5926 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/csvstep.c
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      972 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/dcel.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1832 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/disco.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4109 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/geom.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1844 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/ggr.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5354 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/hybrid.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      616 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/inter5.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      311 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/interp.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5032 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/kontur.c
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    12171 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/kontur.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      665 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/nave.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1379 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/newt.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4468 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/normfo.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      528 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/popin.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      653 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/prebr.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      412 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/prod.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      913 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/s4.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1472 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/schape.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      567 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/simp.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2755 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/skbarb.for
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1089 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/structs.c
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2844 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/kontur/src/trans.for
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/mcdrag/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      825 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/mcdrag/CMakeLists.txt
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/compiled/mcdrag/src/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     9625 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/mcdrag/src/mcdrag.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      603 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/compiled/mcdrag/src/test.f90
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     9085 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/eb_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    11816 2022-11-15 22:02:15.000000 shells_cae-0.0.8/shells_cae/geometry_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7677 2022-11-15 22:02:15.000000 shells_cae-0.0.8/shells_cae/ib_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7769 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/kontur_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    22209 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/mcc_solver.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5306 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/mcdrag_solver.py
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.971860 shells_cae-0.0.8/shells_cae/optimizers/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)       25 2022-11-09 20:54:49.000000 shells_cae-0.0.8/shells_cae/optimizers/__init__.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    27148 2022-11-15 22:25:32.000000 shells_cae-0.0.8/shells_cae/optimizers/optimizers.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    23295 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/penetration.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      293 2022-11-09 20:52:29.000000 shells_cae-0.0.8/shells_cae/solvers_abc.py
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)    60217 2022-11-15 22:02:15.000000 shells_cae-0.0.8/shells_cae/strength_solver.py
-drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-16 00:02:12.967860 shells_cae-0.0.8/shells_cae.egg-info/
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)      177 2022-11-16 00:02:12.000000 shells_cae-0.0.8/shells_cae.egg-info/PKG-INFO
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2922 2022-11-16 00:02:12.000000 shells_cae-0.0.8/shells_cae.egg-info/SOURCES.txt
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)        1 2022-11-16 00:02:12.000000 shells_cae-0.0.8/shells_cae.egg-info/dependency_links.txt
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)        1 2022-11-09 20:58:58.000000 shells_cae-0.0.8/shells_cae.egg-info/not-zip-safe
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)       27 2022-11-16 00:02:12.000000 shells_cae-0.0.8/shells_cae.egg-info/requires.txt
--rw-r--r--   0 vadimm    (1000) vadimm    (1000)       11 2022-11-16 00:02:12.000000 shells_cae-0.0.8/shells_cae.egg-info/top_level.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.767745 shells_cae-0.0.9/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      177 2022-11-18 13:23:20.767745 shells_cae-0.0.9/PKG-INFO
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)       32 2022-11-09 20:52:29.000000 shells_cae-0.0.9/README.md
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)       38 2022-11-18 13:23:20.767745 shells_cae-0.0.9/setup.cfg
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1341 2022-11-18 13:23:05.000000 shells_cae-0.0.9/setup.py
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.759745 shells_cae-0.0.9/shells_cae/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1000 2022-11-15 22:02:15.000000 shells_cae-0.0.9/shells_cae/__init__.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5002 2022-11-15 22:02:15.000000 shells_cae-0.0.9/shells_cae/al_tate_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2755 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/apfsd_fl_stable_solver.py
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.759745 shells_cae-0.0.9/shells_cae/compiled/
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/al_tate_model/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1004 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/al_tate_model/CMakeLists.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/al_tate_model/src/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    10761 2022-11-15 23:57:51.000000 shells_cae-0.0.9/shells_cae/compiled/al_tate_model/src/penetration.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      629 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/al_tate_model/src/test.f90
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.759745 shells_cae-0.0.9/shells_cae/compiled/build/
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/build/bin/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   126290 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/ballistics.exe
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/
+-rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    22296 2022-11-15 23:54:33.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libmcdrag.so
+-rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    19288 2022-11-15 23:58:05.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libpenetrationlib.so
+-rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    26816 2022-11-15 23:54:34.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libsextbal.so
+-rwxr-xr-x   0 vadimm    (1000) vadimm    (1000)    60600 2022-11-15 23:54:34.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libsintbal.so
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   129010 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/libmcdrag.dll
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   136663 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/libpenetrationlib.dll
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   117084 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/libsextbal.dll
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   790530 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/libsintbal.dll
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)   126229 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/build/bin/mcdrag_lib.exe
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/external_ballistics/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      758 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/external_ballistics/CMakeLists.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/external_ballistics/src/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5440 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/external_ballistics/src/solve_eb.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7139 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/external_ballistics/src/solve_ebh.f90
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      786 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/CMakeLists.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4618 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/ibstructs.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1727 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/preproc.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    12023 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/solve_ib.f90
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/kontur/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1511 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/CMakeLists.txt
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4518 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/csv_header.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae/compiled/kontur/include/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4563 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/include/csv.h
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      967 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/include/kontur.h
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4806 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/include/structs.h
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.767745 shells_cae-0.0.9/shells_cae/compiled/kontur/src/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     6809 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/csv.c
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5926 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/csvstep.c
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      972 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/dcel.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1832 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/disco.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4109 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/geom.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1844 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/ggr.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5354 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/hybrid.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      616 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/inter5.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      311 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/interp.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5032 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/kontur.c
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    12171 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/kontur.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      665 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/nave.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1379 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/newt.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     4468 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/normfo.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      528 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/popin.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      653 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/prebr.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      412 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/prod.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      913 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/s4.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1472 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/schape.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      567 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/simp.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2755 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/skbarb.for
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     1089 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/structs.c
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2844 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/kontur/src/trans.for
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.767745 shells_cae-0.0.9/shells_cae/compiled/mcdrag/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      825 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/mcdrag/CMakeLists.txt
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.767745 shells_cae-0.0.9/shells_cae/compiled/mcdrag/src/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     9625 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/mcdrag/src/mcdrag.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      603 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/compiled/mcdrag/src/test.f90
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     9085 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/eb_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    11816 2022-11-15 22:02:15.000000 shells_cae-0.0.9/shells_cae/geometry_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7677 2022-11-15 22:02:15.000000 shells_cae-0.0.9/shells_cae/ib_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     7769 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/kontur_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    22209 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/mcc_solver.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     5306 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/mcdrag_solver.py
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.767745 shells_cae-0.0.9/shells_cae/optimizers/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)       25 2022-11-09 20:54:49.000000 shells_cae-0.0.9/shells_cae/optimizers/__init__.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    27148 2022-11-15 22:25:32.000000 shells_cae-0.0.9/shells_cae/optimizers/optimizers.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    23295 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/penetration.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      293 2022-11-09 20:52:29.000000 shells_cae-0.0.9/shells_cae/solvers_abc.py
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)    60219 2022-11-18 13:22:10.000000 shells_cae-0.0.9/shells_cae/strength_solver.py
+drwxr-xr-x   0 vadimm    (1000) vadimm    (1000)        0 2022-11-18 13:23:20.763745 shells_cae-0.0.9/shells_cae.egg-info/
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)      177 2022-11-18 13:23:20.000000 shells_cae-0.0.9/shells_cae.egg-info/PKG-INFO
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)     2922 2022-11-18 13:23:20.000000 shells_cae-0.0.9/shells_cae.egg-info/SOURCES.txt
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)        1 2022-11-18 13:23:20.000000 shells_cae-0.0.9/shells_cae.egg-info/dependency_links.txt
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)        1 2022-11-09 20:58:58.000000 shells_cae-0.0.9/shells_cae.egg-info/not-zip-safe
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)       27 2022-11-18 13:23:20.000000 shells_cae-0.0.9/shells_cae.egg-info/requires.txt
+-rw-r--r--   0 vadimm    (1000) vadimm    (1000)       11 2022-11-18 13:23:20.000000 shells_cae-0.0.9/shells_cae.egg-info/top_level.txt
```

### Comparing `shells_cae-0.0.8/setup.py` & `shells_cae-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='shells_cae',
-      version='0.0.8',
+      version='0.0.9',
       description='Special CAЕ Library by sabbraxcaddabra&denchina',
       packages=['shells_cae', 'shells_cae.optimizers'],
       package_data={'shells_cae':[
             'compiled/al_tate_model/src/*.f90',
             'compiled/al_tate_model/CMakeLists.txt',
             'compiled/external_ballistics/src/*.f90',
             'compiled/external_ballistics/CMakeLists.txt',
```

### Comparing `shells_cae-0.0.8/shells_cae/__init__.py` & `shells_cae-0.0.9/shells_cae/__init__.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/al_tate_solver.py` & `shells_cae-0.0.9/shells_cae/al_tate_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/apfsd_fl_stable_solver.py` & `shells_cae-0.0.9/shells_cae/apfsd_fl_stable_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/al_tate_model/CMakeLists.txt` & `shells_cae-0.0.9/shells_cae/compiled/al_tate_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/al_tate_model/src/penetration.f90` & `shells_cae-0.0.9/shells_cae/compiled/al_tate_model/src/penetration.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/al_tate_model/src/test.f90` & `shells_cae-0.0.9/shells_cae/compiled/al_tate_model/src/test.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/ballistics.exe` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/ballistics.exe`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libmcdrag.so` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libmcdrag.so`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libpenetrationlib.so` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libpenetrationlib.so`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libsextbal.so` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libsextbal.so`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/lib/libsintbal.so` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/lib/libsintbal.so`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/libmcdrag.dll` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/libmcdrag.dll`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/libpenetrationlib.dll` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/libpenetrationlib.dll`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/libsextbal.dll` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/libsextbal.dll`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/libsintbal.dll` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/libsintbal.dll`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/build/bin/mcdrag_lib.exe` & `shells_cae-0.0.9/shells_cae/compiled/build/bin/mcdrag_lib.exe`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/external_ballistics/CMakeLists.txt` & `shells_cae-0.0.9/shells_cae/compiled/external_ballistics/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/external_ballistics/src/solve_eb.f90` & `shells_cae-0.0.9/shells_cae/compiled/external_ballistics/src/solve_eb.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/external_ballistics/src/solve_ebh.f90` & `shells_cae-0.0.9/shells_cae/compiled/external_ballistics/src/solve_ebh.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/CMakeLists.txt` & `shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/ibstructs.f90` & `shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/ibstructs.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/preproc.f90` & `shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/preproc.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/internal_ballistics/src/solve_ib.f90` & `shells_cae-0.0.9/shells_cae/compiled/internal_ballistics/src/solve_ib.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/CMakeLists.txt` & `shells_cae-0.0.9/shells_cae/compiled/kontur/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/csv_header.txt` & `shells_cae-0.0.9/shells_cae/compiled/kontur/csv_header.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/include/csv.h` & `shells_cae-0.0.9/shells_cae/compiled/kontur/include/csv.h`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/include/kontur.h` & `shells_cae-0.0.9/shells_cae/compiled/kontur/include/kontur.h`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/include/structs.h` & `shells_cae-0.0.9/shells_cae/compiled/kontur/include/structs.h`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/csv.c` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/csv.c`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/csvstep.c` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/csvstep.c`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/dcel.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/dcel.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/disco.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/disco.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/geom.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/geom.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/ggr.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/ggr.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/hybrid.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/hybrid.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/inter5.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/inter5.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/kontur.c` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/kontur.c`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/kontur.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/kontur.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/nave.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/nave.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/newt.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/newt.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/normfo.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/normfo.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/popin.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/popin.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/prebr.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/prebr.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/s4.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/s4.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/schape.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/schape.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/simp.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/simp.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/skbarb.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/skbarb.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/structs.c` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/structs.c`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/kontur/src/trans.for` & `shells_cae-0.0.9/shells_cae/compiled/kontur/src/trans.for`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/mcdrag/CMakeLists.txt` & `shells_cae-0.0.9/shells_cae/compiled/mcdrag/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/mcdrag/src/mcdrag.f90` & `shells_cae-0.0.9/shells_cae/compiled/mcdrag/src/mcdrag.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/compiled/mcdrag/src/test.f90` & `shells_cae-0.0.9/shells_cae/compiled/mcdrag/src/test.f90`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/eb_solver.py` & `shells_cae-0.0.9/shells_cae/eb_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/geometry_solver.py` & `shells_cae-0.0.9/shells_cae/geometry_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/ib_solver.py` & `shells_cae-0.0.9/shells_cae/ib_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/kontur_solver.py` & `shells_cae-0.0.9/shells_cae/kontur_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/mcc_solver.py` & `shells_cae-0.0.9/shells_cae/mcc_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/mcdrag_solver.py` & `shells_cae-0.0.9/shells_cae/mcdrag_solver.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/optimizers/optimizers.py` & `shells_cae-0.0.9/shells_cae/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/penetration.py` & `shells_cae-0.0.9/shells_cae/penetration.py`

 * *Files identical despite different names*

### Comparing `shells_cae-0.0.8/shells_cae/strength_solver.py` & `shells_cae-0.0.9/shells_cae/strength_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1447,15 +1447,15 @@
         return 0.
 
     @np.vectorize
     def get_sigma_r(self, x):
         p_data = self.preprocessed_data
         x_db_n = p_data['x_db_n']
         p_max = p_data['p_max']
-        if 0. < x < x_db_n:
+        if 0. <= x <= x_db_n:
             return p_max
         return 0.
 
     def run(self, data: dict, global_state: dict):
         n_points = data['settings'][APFSDStrengthSolver.name]['n_points']
         x = np.linspace(0., self.preprocessed_data['la'], n_points)
```

### Comparing `shells_cae-0.0.8/shells_cae.egg-info/SOURCES.txt` & `shells_cae-0.0.9/shells_cae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

