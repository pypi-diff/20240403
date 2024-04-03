# Comparing `tmp/rarfile-4.1.tar.gz` & `tmp/rarfile-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rarfile-4.1.tar", last modified: Sun Sep 17 19:39:59 2023, max compression
+gzip compressed data, was "rarfile-4.2.tar", last modified: Wed Apr  3 17:10:18 2024, max compression
```

## Comparing `rarfile-4.1.tar` & `rarfile-4.2.tar`

### file list

```diff
@@ -1,149 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.397534 rarfile-4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-09-17 19:39:49.000000 rarfile-4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.381534 rarfile-4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.381534 rarfile-4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-09-17 19:39:49.000000 rarfile-4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-09-17 19:39:49.000000 rarfile-4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15502 2023-09-17 19:39:49.000000 rarfile-4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-09-17 19:39:49.000000 rarfile-4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-09-17 19:39:49.000000 rarfile-4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-09-17 19:39:49.000000 rarfile-4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-09-17 19:39:59.397534 rarfile-4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-09-17 19:39:49.000000 rarfile-4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.385534 rarfile-4.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-09-17 19:39:49.000000 rarfile-4.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-09-17 19:39:49.000000 rarfile-4.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2023-09-17 19:39:49.000000 rarfile-4.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2023-09-17 19:39:49.000000 rarfile-4.1/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-09-17 19:39:49.000000 rarfile-4.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-09-17 19:39:49.000000 rarfile-4.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2023-09-17 19:39:49.000000 rarfile-4.1/doc/news.rst
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-09-17 19:39:49.000000 rarfile-4.1/doc/note.awk
--rwxr-xr-x   0 runner    (1001) docker     (127)    18522 2023-09-17 19:39:49.000000 rarfile-4.1/dumprar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.385534 rarfile-4.1/etc/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-09-17 19:39:49.000000 rarfile-4.1/etc/requirements.build.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.385534 rarfile-4.1/rarfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-09-17 19:39:59.000000 rarfile-4.1/rarfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2023-09-17 19:39:59.000000 rarfile-4.1/rarfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 19:39:59.000000 rarfile-4.1/rarfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-17 19:39:59.000000 rarfile-4.1/rarfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   104442 2023-09-17 19:39:49.000000 rarfile-4.1/rarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-09-17 19:39:59.397534 rarfile-4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-09-17 19:39:49.000000 rarfile-4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.385534 rarfile-4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 19:39:49.000000 rarfile-4.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 19:39:59.397534 rarfile-4.1/test/files/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime0.rar
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime0.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime1.rar
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime1.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime2.rar
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime2.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime3.rar
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime3.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime4.rar
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime4.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime5.rar
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/ctime5.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar15-comment-lock.rar
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar15-comment-lock.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar15-comment.rar
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar15-comment.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar202-comment-nopsw.rar
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar202-comment-nopsw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar202-comment-psw.rar
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar202-comment-psw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-hpsw.rar
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-hpsw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-plain.rar
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-plain.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-psw.rar
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-comment-psw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-old.r00
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-old.r01
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-old.rar
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-old.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-owner.rar
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-owner.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-readonly-unix.rar
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-readonly-unix.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-readonly-win.rar
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-readonly-win.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   730253 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-seektest.sfx
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-subdirs.rar
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-subdirs.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-symlink-unix.rar
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-symlink-unix.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-versions.rar
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-versions.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part1.rar
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part1.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part2.rar
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part2.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part3.rar
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar3-vols.part3.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-blake.rar
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-blake.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-crc.rar
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-crc.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   130269 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-crc.sfx
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-dups.rar
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-dups.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-hlink.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-hlink.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-hpsw.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-hpsw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-owner.rar
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-owner.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-psw-blake.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-psw-blake.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-psw.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-psw.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-quick-open.rar
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-quick-open.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-readonly-unix.rar
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-readonly-unix.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-readonly-win.rar
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-readonly-win.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-solid-qo.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-solid-qo.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-solid.rar
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-solid.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-subdirs.rar
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-subdirs.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-symlink-unix.rar
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-symlink-unix.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-symlink-win.rar
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-symlink-win.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-times.rar
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-times.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-times2.rar
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-times2.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-versions.rar
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-versions.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part1.rar
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part1.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part2.rar
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part2.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part3.rar
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/rar5-vols.part3.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/seektest.rar
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/seektest.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/unicode.rar
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/unicode.rar.exp
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/unicode2.rar
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-09-17 19:39:49.000000 rarfile-4.1/test/files/unicode2.rar.exp
--rwxr-xr-x   0 runner    (1001) docker     (127)      979 2023-09-17 19:39:49.000000 rarfile-4.1/test/run_dump.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2023-09-17 19:39:49.000000 rarfile-4.1/test/run_dump_all.sh
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_korrupt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_reading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-09-17 19:39:49.000000 rarfile-4.1/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-09-17 19:39:49.000000 rarfile-4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.862236 rarfile-4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 17:10:11.000000 rarfile-4.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.838236 rarfile-4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.842236 rarfile-4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-03 17:10:11.000000 rarfile-4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-03 17:10:11.000000 rarfile-4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-04-03 17:10:11.000000 rarfile-4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 17:10:11.000000 rarfile-4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 17:10:11.000000 rarfile-4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-03 17:10:11.000000 rarfile-4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-03 17:10:18.862236 rarfile-4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-03 17:10:11.000000 rarfile-4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.842236 rarfile-4.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-03 17:10:11.000000 rarfile-4.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-03 17:10:11.000000 rarfile-4.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-03 17:10:11.000000 rarfile-4.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-03 17:10:11.000000 rarfile-4.2/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 17:10:11.000000 rarfile-4.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-03 17:10:11.000000 rarfile-4.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    16669 2024-04-03 17:10:11.000000 rarfile-4.2/doc/news.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-03 17:10:11.000000 rarfile-4.2/doc/note.awk
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18522 2024-04-03 17:10:11.000000 rarfile-4.2/dumprar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.842236 rarfile-4.2/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 17:10:11.000000 rarfile-4.2/etc/requirements.build.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.862236 rarfile-4.2/rarfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-03 17:10:18.000000 rarfile-4.2/rarfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-03 17:10:18.000000 rarfile-4.2/rarfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:18.000000 rarfile-4.2/rarfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:10:18.000000 rarfile-4.2/rarfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   105004 2024-04-03 17:10:11.000000 rarfile-4.2/rarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 17:10:18.862236 rarfile-4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 17:10:11.000000 rarfile-4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.846236 rarfile-4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:11.000000 rarfile-4.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:18.862236 rarfile-4.2/test/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime0.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime0.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime1.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime1.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime2.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime2.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime3.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime3.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime4.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime4.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime5.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/ctime5.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar15-comment-lock.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar15-comment-lock.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar15-comment.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar15-comment.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar202-comment-nopsw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar202-comment-nopsw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar202-comment-psw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar202-comment-psw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-hpsw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-hpsw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-plain.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-plain.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-psw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-comment-psw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-old.r00
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-old.r01
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-old.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-old.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-owner.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-owner.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-readonly-unix.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-readonly-unix.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-readonly-win.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-readonly-win.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   730253 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-seektest.sfx
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-solid.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-solid.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-subdirs.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-subdirs.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-symlink-unix.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-symlink-unix.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-versions.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-versions.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part1.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part1.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part2.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part2.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part3.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar3-vols.part3.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-blake.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-blake.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-crc.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-crc.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   130269 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-crc.sfx
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-dups.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-dups.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-hlink.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-hlink.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-hpsw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-hpsw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-owner.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-owner.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-psw-blake.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-psw-blake.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-psw.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-psw.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-quick-open.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-quick-open.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-readonly-unix.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-readonly-unix.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-readonly-win.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-readonly-win.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-solid-qo.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-solid-qo.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-solid.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-solid.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-subdirs.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-subdirs.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-symlink-unix.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-symlink-unix.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-symlink-win.rar
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-symlink-win.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-times.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-times.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-times2.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-times2.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-versions.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-versions.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part1.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part1.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part2.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part2.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part3.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/rar5-vols.part3.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/seektest.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/seektest.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/unicode.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/unicode.rar.exp
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/unicode2.rar
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 17:10:11.000000 rarfile-4.2/test/files/unicode2.rar.exp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      979 2024-04-03 17:10:11.000000 rarfile-4.2/test/run_dump.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-04-03 17:10:11.000000 rarfile-4.2/test/run_dump_all.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_korrupt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-03 17:10:11.000000 rarfile-4.2/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-03 17:10:11.000000 rarfile-4.2/tox.ini
```

### Comparing `rarfile-4.1/.github/workflows/ci.yml` & `rarfile-4.2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         pick:
           - {OS: "ubuntu-latest", PY: "3.10", TOXENV: "lint,docs"}
     steps:
       - name: "Checkout"
         uses: actions/checkout@v4
 
       - name: "Setup Python ${{matrix.pick.PY}}"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{matrix.pick.PY}}
 
       - name: "Install build tools"
         run: python -m pip install -r etc/requirements.build.txt --disable-pip-version-check
 
       - name: "Run tox - ${{matrix.pick.TOXENV}}"
@@ -41,31 +41,31 @@
 
   test:
     name: "Test - ${{matrix.pick.OS}} / ${{matrix.pick.PYNAME}}"
     runs-on: ${{matrix.pick.OS}}
     strategy:
       matrix:
         pick:
-          - {OS: "ubuntu-20.04", PY: "3.7", PYNAME: "Python 3.7", TOXENV: "py37-cryptography"}
           - {OS: "ubuntu-latest", PY: "3.8", PYNAME: "Python 3.8", TOXENV: "py38"}
           - {OS: "ubuntu-latest", PY: "3.9", PYNAME: "Python 3.9", TOXENV: "py39-pycryptodome"}
           - {OS: "ubuntu-latest", PY: "3.10", PYNAME: "Python 3.10", TOXENV: "py310-cryptography"}
           - {OS: "ubuntu-latest", PY: "3.11", PYNAME: "Python 3.11", TOXENV: "py311-cryptography"}
+          - {OS: "ubuntu-latest", PY: "3.12", PYNAME: "Python 3.12", TOXENV: "py312-cryptography"}
           - {OS: "ubuntu-latest", PY: "pypy3.9", PYNAME: "PyPy3.9", TOXENV: "pypy39-cryptography"}
           - {OS: "ubuntu-latest", PY: "pypy3.10", PYNAME: "PyPy3.10", TOXENV: "pypy310-cryptography"}
           - {OS: "macos-latest", PY: "3.9", PYNAME: "Python 3.9", TOXENV: "py39-pycryptodome"}
           - {OS: "macos-latest", PY: "3.10", PYNAME: "Python 3.10", TOXENV: "py310-cryptography"}
           - {OS: "windows-latest", PY: "3.9", PYNAME: "Python 3.9", TOXENV: "py39-cryptography" }
           - {OS: "windows-latest", PY: "3.10", PYNAME: "Python 3.10", TOXENV: "py310-cryptography" }
     steps:
       - name: "Checkout"
         uses: actions/checkout@v4
 
       - name: "Setup ${{matrix.pick.PYNAME}}"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{matrix.pick.PY}}
 
       - name: "Install archivers (linux)"
         if: ${{runner.os == 'Linux'}}
         run: |
           sudo -nH apt-get -qqy install unrar unar libarchive-tools p7zip-rar
@@ -86,16 +86,16 @@
 
       - name: "Install archivers (windows)"
         if: ${{runner.os == 'Windows'}}
         shell: cmd
         run: |
           set "PATH=c:\msys64\usr\bin;%PATH%"
           pacman -S --noconfirm --needed bsdtar p7zip
-          curl -sS -o unrarw32.exe https://www.rarlab.com/rar/unrarw32.exe
-          7z x unrarw32.exe
+          curl -sS -o unrarw64.exe https://www.rarlab.com/rar/unrarw64.exe
+          7z x unrarw64.exe
           unrar
           bsdtar -h
           7z i
 
       - name: "Install tools"
         run: python -m pip install -r etc/requirements.build.txt --disable-pip-version-check
```

### Comparing `rarfile-4.1/.github/workflows/release.yml` & `rarfile-4.2/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 jobs:
   sdist:
     name: "Build source package"
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with: {python-version: "3.11"}
       - run: python3 -m pip install -r etc/requirements.build.txt --disable-pip-version-check
       - run: python3 setup.py sdist
       - run: python3 setup.py bdist_wheel
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with: {name: "dist", path: "dist"}
 
   publish:
     name: "Publish"
     runs-on: ubuntu-latest
     needs: [sdist]
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with: {python-version: "3.11"}
 
       - run: python3 -m pip install -r etc/requirements.build.txt --disable-pip-version-check
 
       - name: "Get files"
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with: {name: "dist", path: "dist"}
 
       - name: "Install pandoc"
         run: |
           sudo -nH apt-get -u -y install pandoc
           pandoc --version
```

### Comparing `rarfile-4.1/.pylintrc` & `rarfile-4.2/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 	protected-access,
 	ungrouped-imports,
 	chained-comparison,
 	len-as-condition,
 	redefined-builtin,
 	import-outside-toplevel,
 	duplicate-code,
+        consider-using-min-builtin,
 	unnecessary-pass
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=c-extension-no-member
```

### Comparing `rarfile-4.1/LICENSE` & `rarfile-4.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Copyright (c) 2005-2020 Marko Kreen <markokr@gmail.com>
+Copyright (c) 2005-2024 Marko Kreen <markokr@gmail.com>
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
```

### Comparing `rarfile-4.1/Makefile` & `rarfile-4.2/Makefile`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/PKG-INFO` & `rarfile-4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rarfile
-Version: 4.1
+Version: 4.2
 Summary: RAR archive reader for Python
 Home-page: https://github.com/markokr/rarfile
 Author: Marko Kreen
 Author-email: markokr@gmail.com
 License: ISC
 Keywords: rar,unrar,archive
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,17 +64,17 @@
 +-------------+----------------------+-----------------------------------------------------+
 | bsdtar_     | Supported            | * Not recommended: limited RAR format support.      |
 |             |                      | * Does not support multi-volume archives.           |
 |             |                      | * Does not support solid archives.                  |
 |             |                      | * Does not support password-protected archives.     |
 |             |                      | * Does not support RARVM-based compression filters. |
 +-------------+----------------------+-----------------------------------------------------+
-| unrar-free_ | Not supported        | * Unusable: Does not support output to stdout.      |
+| unrar-free_ | Supported            | * Supports output to stdout (v0.2.0).               |
 |             |                      | * Based on libarchive so similar format support     |
-|             |                      |   as ``bsdtar``.                                    |
+|             |                      |   as ``bsdtar`` but supports multi-volume (v0.3.0). |
 +-------------+----------------------+-----------------------------------------------------+
 
 .. _p7zip: https://sourceforge.net/projects/p7zip/
 .. _unrar-free: https://gitlab.com/bgermann/unrar-free
 
 Links:
```

### Comparing `rarfile-4.1/README.rst` & `rarfile-4.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 +-------------+----------------------+-----------------------------------------------------+
 | bsdtar_     | Supported            | * Not recommended: limited RAR format support.      |
 |             |                      | * Does not support multi-volume archives.           |
 |             |                      | * Does not support solid archives.                  |
 |             |                      | * Does not support password-protected archives.     |
 |             |                      | * Does not support RARVM-based compression filters. |
 +-------------+----------------------+-----------------------------------------------------+
-| unrar-free_ | Not supported        | * Unusable: Does not support output to stdout.      |
+| unrar-free_ | Supported            | * Supports output to stdout (v0.2.0).               |
 |             |                      | * Based on libarchive so similar format support     |
-|             |                      |   as ``bsdtar``.                                    |
+|             |                      |   as ``bsdtar`` but supports multi-volume (v0.3.0). |
 +-------------+----------------------+-----------------------------------------------------+
 
 .. _p7zip: https://sourceforge.net/projects/p7zip/
 .. _unrar-free: https://gitlab.com/bgermann/unrar-free
 
 Links:
```

### Comparing `rarfile-4.1/doc/Makefile` & `rarfile-4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/doc/api.rst` & `rarfile-4.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/doc/conf.py` & `rarfile-4.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/doc/faq.rst` & `rarfile-4.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/doc/make.bat` & `rarfile-4.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/doc/news.rst` & `rarfile-4.2/doc/news.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 
 rarfile history
 ===============
 
 .. py:currentmodule:: rarfile
 
+Version 4.2 (2024-04-03)
+------------------------
+
+Features:
+
+* Support ``unrar-free`` >= 0.2.0.
+  [`#103 <https://github.com/markokr/rarfile/pull/103>`_]
+* Add :meth:`RarFile.is_solid` to check if archive uses
+  solid compression.
+  [`#101 <https://github.com/markokr/rarfile/issues/101>`_]
+
+Fixes:
+
+* Support old multi-volume archives better where ENDARC
+  does not contain NEXTVOL.
+  [`#97 <https://github.com/markokr/rarfile/issues/97>`_]
+
+Cleanups:
+
+* ci: Drop Python 3.7, add 3.12
+* ci: upgrade actions
+
 Version 4.1 (2023-09-17)
 ------------------------
 
 Features:
 
 * Support 7zip/p7zip as decompression backend.
   [`#71 <https://github.com/markokr/rarfile/issues/71>`_]
@@ -120,14 +142,19 @@
 * Add the .sfx test files to MANIFEST.in for inclusion in pypi tarball.
   [`#60 <https://github.com/markokr/rarfile/issues/60>`_]
 * Add all files in git to tarball.
 
 Version 3.2 (2020-07-19)
 ------------------------
 
+Breaking change:
+
+* Top-level function ``custom_check()`` is removed as part
+  of tool discovery refactor.
+
 New features:
 
 * Support ``unar`` as decompression backend.  It has much better
   support for RAR features than ``bsdtar``.
   [`#36 <https://github.com/markokr/rarfile/issues/36>`_]
 
 * Support SFX archives - archive header is searched in first
```

### Comparing `rarfile-4.1/dumprar.py` & `rarfile-4.2/dumprar.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/rarfile.egg-info/PKG-INFO` & `rarfile-4.2/rarfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rarfile
-Version: 4.1
+Version: 4.2
 Summary: RAR archive reader for Python
 Home-page: https://github.com/markokr/rarfile
 Author: Marko Kreen
 Author-email: markokr@gmail.com
 License: ISC
 Keywords: rar,unrar,archive
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,17 +64,17 @@
 +-------------+----------------------+-----------------------------------------------------+
 | bsdtar_     | Supported            | * Not recommended: limited RAR format support.      |
 |             |                      | * Does not support multi-volume archives.           |
 |             |                      | * Does not support solid archives.                  |
 |             |                      | * Does not support password-protected archives.     |
 |             |                      | * Does not support RARVM-based compression filters. |
 +-------------+----------------------+-----------------------------------------------------+
-| unrar-free_ | Not supported        | * Unusable: Does not support output to stdout.      |
+| unrar-free_ | Supported            | * Supports output to stdout (v0.2.0).               |
 |             |                      | * Based on libarchive so similar format support     |
-|             |                      |   as ``bsdtar``.                                    |
+|             |                      |   as ``bsdtar`` but supports multi-volume (v0.3.0). |
 +-------------+----------------------+-----------------------------------------------------+
 
 .. _p7zip: https://sourceforge.net/projects/p7zip/
 .. _unrar-free: https://gitlab.com/bgermann/unrar-free
 
 Links:
```

### Comparing `rarfile-4.1/rarfile.egg-info/SOURCES.txt` & `rarfile-4.2/rarfile.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 test/files/rar3-owner.rar
 test/files/rar3-owner.rar.exp
 test/files/rar3-readonly-unix.rar
 test/files/rar3-readonly-unix.rar.exp
 test/files/rar3-readonly-win.rar
 test/files/rar3-readonly-win.rar.exp
 test/files/rar3-seektest.sfx
+test/files/rar3-solid.rar
+test/files/rar3-solid.rar.exp
 test/files/rar3-subdirs.rar
 test/files/rar3-subdirs.rar.exp
 test/files/rar3-symlink-unix.rar
 test/files/rar3-symlink-unix.rar.exp
 test/files/rar3-versions.rar
 test/files/rar3-versions.rar.exp
 test/files/rar3-vols.part1.rar
```

### Comparing `rarfile-4.1/rarfile.py` & `rarfile-4.2/rarfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # rarfile.py
 #
-# Copyright (c) 2005-2020  Marko Kreen <markokr@gmail.com>
+# Copyright (c) 2005-2024  Marko Kreen <markokr@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
@@ -88,15 +88,15 @@
         if _have_crypto == 2:
             self.decrypt = AES.new(key, AES.MODE_CBC, iv).decrypt
         else:
             ciph = Cipher(algorithms.AES(key), modes.CBC(iv), default_backend())
             self.decrypt = ciph.decryptor().update
 
 
-__version__ = "4.1"
+__version__ = "4.2"
 
 # export only interesting items
 __all__ = ["get_rar_version", "is_rarfile", "is_rarfile_sfx", "RarInfo", "RarFile", "RarExtFile"]
 
 ##
 ## Module configuration.  Can be tuned after importing.
 ##
@@ -667,14 +667,16 @@
             set to False to disable CRC checks
         errors
             Either "stop" to quietly stop parsing on errors,
             or "strict" to raise errors.  Default is "stop".
         part_only
             If True, read only single file and allow it to be middle-part
             of multi-volume archive.
+
+            .. versionadded:: 4.0
     """
 
     #: File name, if available.  Unicode string or None.
     filename = None
 
     #: Archive comment.  Unicode string or None.
     comment = None
@@ -733,14 +735,21 @@
             self._file_parser.setpassword(self._password)
 
     def needs_password(self):
         """Returns True if any archive entries require password for extraction.
         """
         return self._file_parser.needs_password()
 
+    def is_solid(self):
+        """Returns True if archive uses solid compression.
+
+        .. versionadded:: 4.2
+        """
+        return self._file_parser.is_solid()
+
     def namelist(self):
         """Return list of filenames in archive.
         """
         return [f.filename for f in self.infolist()]
 
     def infolist(self):
         """Return RarInfo objects for all files/directories in archive.
@@ -761,14 +770,16 @@
         return self._file_parser.getinfo(name)
 
     def getinfo_orig(self, name):
         """Return RarInfo for file source.
 
         RAR5: if name is hard-linked or copied file,
         returns original entry with original filename.
+
+        .. versionadded:: 4.1
         """
         return self._file_parser.getinfo_orig(name)
 
     def open(self, name, mode="r", pwd=None):
         """Returns file-like object (:class:`RarExtFile`) from where the data can be read.
 
         The object implements :class:`io.RawIOBase` interface, so it can
@@ -1022,14 +1033,22 @@
         self._info_callback = info_cb
         self._info_list = []
         self._info_map = {}
         self._vol_list = []
         self._sfx_offset = sfx_offset
         self._part_only = part_only
 
+    def is_solid(self):
+        """Returns True if archive uses solid compression.
+        """
+        if self._main:
+            if self._main.flags & RAR_MAIN_SOLID:
+                return True
+        return False
+
     def has_header_encryption(self):
         """Returns True if headers are encrypted
         """
         if self._hdrenc_main:
             return True
         if self._main:
             if self._main.flags & RAR_MAIN_PASSWORD:
@@ -1159,15 +1178,17 @@
                         # delay raise until we have volnr from ENDARC
                         raise_need_first_vol = True
                 if h.flags & RAR_MAIN_PASSWORD:
                     self._needs_password = True
                     if not self._password:
                         break
             elif h.type == RAR_BLOCK_ENDARC:
-                more_vols = (h.flags & RAR_ENDARC_NEXT_VOLUME) > 0
+                # use flag, but also allow RAR 2.x logic below to trigger
+                if h.flags & RAR_ENDARC_NEXT_VOLUME:
+                    more_vols = True
                 endarc = True
                 if raise_need_first_vol and (h.flags & RAR_ENDARC_VOLNR) > 0:
                     raise NeedFirstVolume(
                         "Need to start from first volume (current: %r)"
                         % (h.endarc_volnr,),
                         h.endarc_volnr
                     )
@@ -2333,16 +2354,16 @@
         """Return current reading position in uncompressed data."""
         return self._inf.file_size - self._remain
 
     def seek(self, offset, whence=0):
         """Seek in data.
 
         On uncompressed files, the seeking works by actual
-        seeks so it's fast.  On compresses files its slow
-        - forward seeking happends by reading ahead,
+        seeks so it's fast.  On compressed files its slow
+        - forward seeking happens by reading ahead,
         backwards by re-opening and decompressing from the start.
         """
 
         # disable crc check when seeking
         if not self._seeking:
             self._md_context = NoHashContext()
             self._seeking = True
@@ -3106,15 +3127,15 @@
         return p.communicate()[0]
     finally:
         tmpf.close()
         os.unlink(tmpname)
 
 
 def sanitize_filename(fname, pathsep, is_win32):
-    """Simulate unrar sanitization.
+    """Make filename safe for write access.
     """
     if is_win32:
         if len(fname) > 1 and fname[1] == ":":
             fname = fname[2:]
         rc = RC_BAD_CHARS_WIN32
     else:
         rc = RC_BAD_CHARS_UNIX
@@ -3178,20 +3199,20 @@
     return (yr, mon, day, hr, mn, sec * 2)
 
 
 # pylint: disable=arguments-differ,signature-differs
 class nsdatetime(datetime):
     """Datetime that carries nanoseconds.
 
-    Arithmetic not supported, will lose nanoseconds.
+    Arithmetic operations will lose nanoseconds.
 
     .. versionadded:: 4.0
     """
     __slots__ = ("nanosecond",)
-    nanosecond: int     #: Number of nanoseconds, 0 <= nanosecond < 999999999
+    nanosecond: int     #: Number of nanoseconds, 0 <= nanosecond <= 999999999
 
     def __new__(cls, year, month=None, day=None, hour=0, minute=0, second=0,
                 microsecond=0, tzinfo=None, *, fold=0, nanosecond=0):
         usec, mod = divmod(nanosecond, 1000) if nanosecond else (microsecond, 0)
         if mod == 0:
             return datetime(year, month, day, hour, minute, second, usec, tzinfo, fold=fold)
         self = super().__new__(cls, year, month, day, hour, minute, second, usec, tzinfo, fold=fold)
@@ -3385,15 +3406,15 @@
                 cmdline.append(pwd)
         else:
             cmdline.extend(self.setup["no_password"])
 
 
 UNRAR_CONFIG = {
     "open_cmd": ("UNRAR_TOOL", "p", "-inul"),
-    "check_cmd": ("UNRAR_TOOL", "-inul"),
+    "check_cmd": ("UNRAR_TOOL", "-inul", "-?"),
     "password": "-p",
     "no_password": ("-p-",),
     # map return code to exception class, codes from rar.txt
     "errmap": [None,
                RarWarning, RarFatalError, RarCRCError, RarLockedArchiveError,    # 1..4
                RarWriteError, RarOpenError, RarUserError, RarMemoryError,        # 5..8
                RarCreateError, RarNoFilesError, RarWrongPassword]                # 9..11
```

### Comparing `rarfile-4.1/setup.py` & `rarfile-4.2/setup.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar15-comment-lock.rar.exp` & `rarfile-4.2/test/files/rar15-comment-lock.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar15-comment.rar.exp` & `rarfile-4.2/test/files/rar15-comment.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar202-comment-nopsw.rar.exp` & `rarfile-4.2/test/files/rar202-comment-nopsw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar202-comment-psw.rar.exp` & `rarfile-4.2/test/files/rar202-comment-psw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-comment-hpsw.rar.exp` & `rarfile-4.2/test/files/rar3-comment-hpsw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-comment-plain.rar.exp` & `rarfile-4.2/test/files/rar3-comment-plain.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-comment-psw.rar.exp` & `rarfile-4.2/test/files/rar3-comment-psw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-old.r00` & `rarfile-4.2/test/files/rar3-old.r00`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-old.r01` & `rarfile-4.2/test/files/rar3-old.r01`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-old.rar` & `rarfile-4.2/test/files/rar3-old.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-old.rar.exp` & `rarfile-4.2/test/files/rar3-old.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-owner.rar.exp` & `rarfile-4.2/test/files/rar3-owner.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-readonly-unix.rar.exp` & `rarfile-4.2/test/files/rar3-readonly-unix.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-readonly-win.rar.exp` & `rarfile-4.2/test/files/rar3-readonly-win.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-seektest.sfx` & `rarfile-4.2/test/files/rar3-seektest.sfx`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-subdirs.rar` & `rarfile-4.2/test/files/rar3-subdirs.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-subdirs.rar.exp` & `rarfile-4.2/test/files/rar3-subdirs.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-symlink-unix.rar.exp` & `rarfile-4.2/test/files/rar3-symlink-unix.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-vols.part1.rar` & `rarfile-4.2/test/files/rar3-vols.part1.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-vols.part1.rar.exp` & `rarfile-4.2/test/files/rar3-vols.part1.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-vols.part2.rar` & `rarfile-4.2/test/files/rar3-vols.part2.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar3-vols.part3.rar` & `rarfile-4.2/test/files/rar3-vols.part3.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-blake.rar` & `rarfile-4.2/test/files/rar5-blake.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-blake.rar.exp` & `rarfile-4.2/test/files/rar5-blake.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-crc.rar` & `rarfile-4.2/test/files/rar5-crc.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-crc.rar.exp` & `rarfile-4.2/test/files/rar5-crc.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-crc.sfx` & `rarfile-4.2/test/files/rar5-crc.sfx`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-dups.rar` & `rarfile-4.2/test/files/rar5-dups.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-dups.rar.exp` & `rarfile-4.2/test/files/rar5-dups.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-hlink.rar.exp` & `rarfile-4.2/test/files/rar5-hlink.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-hpsw.rar` & `rarfile-4.2/test/files/rar5-hpsw.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-hpsw.rar.exp` & `rarfile-4.2/test/files/rar5-hpsw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-owner.rar.exp` & `rarfile-4.2/test/files/rar5-owner.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-psw-blake.rar` & `rarfile-4.2/test/files/rar5-psw-blake.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-psw-blake.rar.exp` & `rarfile-4.2/test/files/rar5-psw-blake.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-psw.rar` & `rarfile-4.2/test/files/rar5-psw.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-psw.rar.exp` & `rarfile-4.2/test/files/rar5-psw.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-quick-open.rar.exp` & `rarfile-4.2/test/files/rar5-quick-open.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-readonly-unix.rar.exp` & `rarfile-4.2/test/files/rar5-readonly-unix.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-readonly-win.rar.exp` & `rarfile-4.2/test/files/rar5-readonly-win.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-solid-qo.rar.exp` & `rarfile-4.2/test/files/rar5-solid-qo.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-solid.rar.exp` & `rarfile-4.2/test/files/rar5-solid.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-subdirs.rar` & `rarfile-4.2/test/files/rar5-subdirs.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-subdirs.rar.exp` & `rarfile-4.2/test/files/rar5-subdirs.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-symlink-unix.rar.exp` & `rarfile-4.2/test/files/rar5-symlink-unix.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-symlink-win.rar` & `rarfile-4.2/test/files/rar5-symlink-win.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-symlink-win.rar.exp` & `rarfile-4.2/test/files/rar5-symlink-win.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-vols.part1.rar` & `rarfile-4.2/test/files/rar5-vols.part1.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-vols.part1.rar.exp` & `rarfile-4.2/test/files/rar5-vols.part1.rar.exp`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-vols.part2.rar` & `rarfile-4.2/test/files/rar5-vols.part2.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/rar5-vols.part3.rar` & `rarfile-4.2/test/files/rar5-vols.part3.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/files/seektest.rar` & `rarfile-4.2/test/files/seektest.rar`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/run_dump.sh` & `rarfile-4.2/test/run_dump.sh`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_api.py` & `rarfile-4.2/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,7 +379,18 @@
         info_list.append(info)
     with rarfile.RarFile("test/files/rar3-vols.part1.rar", info_callback=info_cb) as rf:
         assert len(info_list) == 10
     info_list = []
     with rarfile.RarFile("test/files/rar5-vols.part1.rar", info_callback=info_cb) as rf:
         assert len(info_list) == 16
 
+
+def test_is_solid():
+    with rarfile.RarFile("test/files/rar3-comment-plain.rar") as rf:
+        assert not rf.is_solid()
+    with rarfile.RarFile("test/files/rar3-solid.rar") as rf:
+        assert rf.is_solid()
+    with rarfile.RarFile("test/files/rar5-crc.rar") as rf:
+        assert not rf.is_solid()
+    with rarfile.RarFile("test/files/rar5-solid.rar") as rf:
+        assert rf.is_solid()
+
```

### Comparing `rarfile-4.1/test/test_compat.py` & `rarfile-4.2/test/test_compat.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_crypto.py` & `rarfile-4.2/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_extract.py` & `rarfile-4.2/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_format.py` & `rarfile-4.2/test/test_format.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_hashing.py` & `rarfile-4.2/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_korrupt.py` & `rarfile-4.2/test/test_korrupt.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_reading.py` & `rarfile-4.2/test/test_reading.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_seek.py` & `rarfile-4.2/test/test_seek.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_tool.py` & `rarfile-4.2/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/test/test_util.py` & `rarfile-4.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `rarfile-4.1/tox.ini` & `rarfile-4.2/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 [tox]
 envlist = lint,docs,py3-pycryptodome,py3-cryptography,py3
 
 [package]
 name = rarfile
 deps =
-    pycryptodome: pycryptodome==3.15.0
-    cryptography: cryptography==41.0.3
+    pycryptodome: pycryptodome==3.20.0
+    cryptography: cryptography==42.0.5
 test_deps =
     #coverage==7.3.1
-    coverage==7.2.7
-    pytest==7.4.2
-    pytest-cov==4.1.0
-    pytest-xdist==3.3.1
+    coverage==7.4.4
+    pytest==8.1.1
+    pytest-cov==5.0.0
+    pytest-xdist==3.5.0
 doc_deps =
     sphinx==7.2.6
     docutils==0.20.1
 lint_deps =
-    pylint==2.17.5
+    pylint==3.1.0
 
 [testenv]
 deps =
     {[package]deps}
     {[package]test_deps}
 commands =
     pytest --cov=rarfile --cov-report=term --cov-report=html:{toxinidir}/cover/{envname} {posargs}
```

