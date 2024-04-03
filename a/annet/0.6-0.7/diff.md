# Comparing `tmp/annet-0.6.tar.gz` & `tmp/annet-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annet-0.6.tar", last modified: Tue Mar  5 11:08:16 2024, max compression
+gzip compressed data, was "annet-0.7.tar", last modified: Wed Apr  3 09:27:19 2024, max compression
```

## Comparing `annet-0.6.tar` & `annet-0.7.tar`

### file list

```diff
@@ -1,146 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.452397 annet-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-05 11:08:12.000000 annet-0.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-05 11:08:12.000000 annet-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-05 11:08:12.000000 annet-0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-05 11:08:16.452397 annet-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-05 11:08:12.000000 annet-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.436397 annet-0.6/annet/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-05 11:08:12.000000 annet-0.6/annet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-03-05 11:08:12.000000 annet-0.6/annet/annet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/filter_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/jsontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/netdev/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/netdev/devdb/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/devdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/netdev/devdb/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/devdb/data/devdb.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/netdev/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/views/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/netdev/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/rbparser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/deploying.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rbparser/syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/annlib/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rulebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-05 11:08:12.000000 annet-0.6/annet/annlib/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/api/
--rw-r--r--   0 runner    (1001) docker     (127)    33212 2024-03-05 11:08:12.000000 annet-0.6/annet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-03-05 11:08:12.000000 annet-0.6/annet/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-03-05 11:08:12.000000 annet-0.6/annet/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-03-05 11:08:12.000000 annet-0.6/annet/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.440397 annet-0.6/annet/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-05 11:08:12.000000 annet-0.6/annet/configs/context.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-05 11:08:12.000000 annet-0.6/annet/configs/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-05 11:08:12.000000 annet-0.6/annet/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-03-05 11:08:12.000000 annet-0.6/annet/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-05 11:08:12.000000 annet-0.6/annet/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-03-05 11:08:12.000000 annet-0.6/annet/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-05 11:08:12.000000 annet-0.6/annet/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    31246 2024-03-05 11:08:12.000000 annet-0.6/annet/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/generators/
--rw-r--r--   0 runner    (1001) docker     (127)    34049 2024-03-05 11:08:12.000000 annet-0.6/annet/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/generators/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/generators/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-05 11:08:12.000000 annet-0.6/annet/generators/common/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-05 11:08:12.000000 annet-0.6/annet/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-05 11:08:12.000000 annet-0.6/annet/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-05 11:08:12.000000 annet-0.6/annet/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-03-05 11:08:12.000000 annet-0.6/annet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-03-05 11:08:12.000000 annet-0.6/annet/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-05 11:08:12.000000 annet-0.6/annet/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-05 11:08:12.000000 annet-0.6/annet/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/arista/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/arista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/arista/iface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/aruba/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/aruba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/aruba/ap_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/aruba/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/cisco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/cisco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/cisco/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/cisco/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/cisco/vlandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/deploying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/huawei/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/aaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/huawei/vlandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/juniper/
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.444397 annet-0.6/annet/rulebook/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/nexus/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.448397 annet-0.6/annet/rulebook/ribbon/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/ribbon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.448397 annet-0.6/annet/rulebook/texts/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/arista.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/arista.order
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/arista.rul
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/aruba.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/aruba.order
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/aruba.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/cisco.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/cisco.order
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/cisco.rul
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/huawei.deploy
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/huawei.order
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/huawei.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/juniper.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/nexus.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/nexus.order
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/nexus.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/nokia.rul
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/pc.order
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/pc.rul
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/ribbon.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/ribbon.rul
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/routeros.order
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-05 11:08:12.000000 annet-0.6/annet/rulebook/texts/routeros.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-05 11:08:12.000000 annet-0.6/annet/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-05 11:08:12.000000 annet-0.6/annet/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-05 11:08:12.000000 annet-0.6/annet/text_term_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-05 11:08:12.000000 annet-0.6/annet/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-03-05 11:08:12.000000 annet-0.6/annet/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.452397 annet-0.6/annet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:08:16.000000 annet-0.6/annet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.448397 annet-0.6/annet_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:12.000000 annet-0.6/annet_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.452397 annet-0.6/annet_generators/example/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-05 11:08:12.000000 annet-0.6/annet_generators/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-05 11:08:12.000000 annet-0.6/annet_generators/example/lldp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:08:16.452397 annet-0.6/annet_nbexport/
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-03-05 11:08:12.000000 annet-0.6/annet_nbexport/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1216 2024-03-05 11:08:12.000000 annet-0.6/annet_nbexport/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-05 11:08:12.000000 annet-0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:08:16.452397 annet-0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1393 2024-03-05 11:08:12.000000 annet-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 09:27:12.000000 annet-0.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 09:27:12.000000 annet-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 09:27:12.000000 annet-0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 09:27:19.053083 annet-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 09:27:12.000000 annet-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-03 09:27:12.000000 annet-0.7/annet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/adapters/netbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/status_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/storage_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/v24/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/v37/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-03 09:27:12.000000 annet-0.7/annet/annet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/annlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/filter_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/jsontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/devdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/devdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/devdb/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/devdb/data/devdb.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/rbparser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/deploying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rulebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    33752 2024-04-03 09:27:12.000000 annet-0.7/annet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-03 09:27:12.000000 annet-0.7/annet/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-03 09:27:12.000000 annet-0.7/annet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-03 09:27:12.000000 annet-0.7/annet/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 09:27:12.000000 annet-0.7/annet/configs/context.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 09:27:12.000000 annet-0.7/annet/configs/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-03 09:27:12.000000 annet-0.7/annet/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-04-03 09:27:12.000000 annet-0.7/annet/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-03 09:27:12.000000 annet-0.7/annet/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-03 09:27:12.000000 annet-0.7/annet/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 09:27:12.000000 annet-0.7/annet/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31426 2024-04-03 09:27:12.000000 annet-0.7/annet/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)    33829 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/generators/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/common/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 09:27:12.000000 annet-0.7/annet/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-03 09:27:12.000000 annet-0.7/annet/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-03 09:27:12.000000 annet-0.7/annet/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-03 09:27:12.000000 annet-0.7/annet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-03 09:27:12.000000 annet-0.7/annet/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-03 09:27:12.000000 annet-0.7/annet/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-03 09:27:12.000000 annet-0.7/annet/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/arista/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/arista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/arista/iface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/aruba/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/ap_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/cisco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/vlandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/deploying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/huawei/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/vlandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/juniper/
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/nexus/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/ribbon/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/ribbon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet/rulebook/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.order
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.rul
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.order
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/juniper.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nokia.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/pc.order
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/pc.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/ribbon.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/ribbon.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/routeros.order
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/routeros.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 09:27:12.000000 annet-0.7/annet/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-03 09:27:12.000000 annet-0.7/annet/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-03 09:27:12.000000 annet-0.7/annet/text_term_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 09:27:12.000000 annet-0.7/annet/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-03 09:27:12.000000 annet-0.7/annet/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet_generators/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/example/lldp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 09:27:12.000000 annet-0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:27:19.053083 annet-0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-03 09:27:12.000000 annet-0.7/setup.py
```

### Comparing `annet-0.6/AUTHORS` & `annet-0.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `annet-0.6/LICENSE` & `annet-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `annet-0.6/PKG-INFO` & `annet-0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.6
+Version: 0.7
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
@@ -17,7 +17,9 @@
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: contextlog>=1.1
 Requires-Dist: valkit>=0.1.4
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: yarl>=1.8.2
+Requires-Dist: adaptix==3.0.0b2
+Requires-Dist: dataclass-rest==0.4
```

### Comparing `annet-0.6/README.md` & `annet-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 - ```annet diff``` - first does gen and then builds diff with current config version
 - ```annet patch``` - first does diff and then generates a list of commands to apply diff on the device
 
 Usage help can be obtained by calling ```annet -h``` or for a specific command, such as ```annet gen -h```.
 
 ## Overview
 
+## Configuration
+
+Provide `NETBOX_URL` and `NETBOX_TOKEN` environment variable to setup data source.
+
+```shell
+export NETBOX_URL="https://demo.netbox.dev"
+export NETBOX_TOKEN="1234567890abcdef01234567890abcdef0123456"
+```
+
 ### annet gen
 
 The annet_generators directory contains many files called generators.
 A generator takes information about the switch as input and returns the configuration.
 The part of the config that the generator is responsible for is specified in the generator's acl function. If a generator returns a configuration that does not fall under acl, an exception will be thrown.
 
 Example generator:
```

### Comparing `annet-0.6/annet/__init__.py` & `annet-0.7/annet/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annet.py` & `annet-0.7/annet/annet.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/command.py` & `annet-0.7/annet/annlib/command.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/diff.py` & `annet-0.7/annet/annlib/diff.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/filter_acl.py` & `annet-0.7/annet/annlib/filter_acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/jsontools.py` & `annet-0.7/annet/annlib/jsontools.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/lib.py` & `annet-0.7/annet/annlib/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/netdev/db.py` & `annet-0.7/annet/annlib/netdev/db.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/netdev/devdb/__init__.py` & `annet-0.7/annet/annlib/netdev/devdb/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/netdev/devdb/data/devdb.json` & `annet-0.7/annet/annlib/netdev/devdb/data/devdb.json`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/netdev/views/dump.py` & `annet-0.7/annet/annlib/netdev/views/dump.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/netdev/views/hardware.py` & `annet-0.7/annet/annlib/netdev/views/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/output.py` & `annet-0.7/annet/annlib/output.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/patching.py` & `annet-0.7/annet/annlib/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rbparser/acl.py` & `annet-0.7/annet/annlib/rbparser/acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rbparser/deploying.py` & `annet-0.7/annet/annlib/rbparser/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rbparser/ordering.py` & `annet-0.7/annet/annlib/rbparser/ordering.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rbparser/platform.py` & `annet-0.7/annet/annlib/rbparser/platform.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rbparser/syntax.py` & `annet-0.7/annet/annlib/rbparser/syntax.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/rulebook/common.py` & `annet-0.7/annet/annlib/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/tabparser.py` & `annet-0.7/annet/annlib/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/annlib/types.py` & `annet-0.7/annet/annlib/types.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/api/__init__.py` & `annet-0.7/annet/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,15 +184,17 @@
                         _print_pre_as_diff(item["children"], show_rules, indent, file, _level + 1)
                         rule_printed = False
 
 
 def log_host_progress_cb(pool: Parallel, task_result: TaskResult):
     progress_logger = get_logger("progress")
     args = cast(cli_args.QueryOptions, pool.args[0])
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         hosts = storage.resolve_fdnds_by_query(args.query)
     perc = int(pool.tasks_done / len(hosts) * 100)
     fqdn = hosts[task_result.device_id]
     elapsed_time = "%dsec" % int(time.monotonic() - task_result.extra["start_time"])
     if task_result.extra.get("regression", False):
         status = task_result.extra["status"]
         status_color = task_result.extra["status_color"]
@@ -206,15 +208,17 @@
                          worker=task_result.worker_name, task_time=elapsed_time)
     return task_result
 
 
 # =====
 def gen(args: cli_args.ShowGenOptions):
     """ Сгенерировать конфиг для устройств """
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         loader = ann_gen.Loader(storage, args)
         stdin = args.stdin(storage=storage, filter_acl=args.filter_acl, config=None)
 
     filterer = filtering.filterer_connector.get()
     pool = Parallel(ann_gen.worker, args, stdin, loader, filterer).tune_args(args)
     if args.show_hosts_progress:
         pool.add_callback(log_host_progress_cb)
@@ -239,15 +243,17 @@
         ret[path] = (diff_lines, reload_data, is_new)
     return ret
 
 
 def patch(args: cli_args.ShowPatchOptions):
     """ Сгенерировать патч для устройств """
     global live_configs  # pylint: disable=global-statement
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         loader = ann_gen.Loader(storage, args)
         if args.config == "running":
             fetcher = annet.deploy.fetcher_connector.get()
             live_configs = fetcher.fetch(loader.devices, processes=args.parallel)
         stdin = args.stdin(storage=storage, filter_acl=args.filter_acl, config=args.config)
 
     filterer = filtering.filterer_connector.get()
@@ -282,15 +288,17 @@
                 False,
             )
 
 
 # =====
 def res_diff_patch(device_id, args: cli_args.ShowPatchOptions, stdin, loader: ann_gen.Loader, filterer: filtering.Filterer) -> Iterable[
     Tuple[OldNewResult, Dict, Dict]]:
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         for res in ann_gen.old_new(
             args,
             storage,
             config=args.config,
             loader=loader,
             filterer=filterer,
             stdin=stdin,
@@ -310,15 +318,17 @@
                 (diff_tree, patch_tree) = _diff_and_patch(device, old, new, acl_rules, res.filter_acl_rules,
                                                           args.add_comments)
                 yield res, diff_tree, patch_tree
 
 
 def diff(args: cli_args.DiffOptions, loader: ann_gen.Loader, filterer: filtering.Filterer) -> Mapping[Device, Union[Diff, PCDiff]]:
     ret = {}
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         for res in ann_gen.old_new(
             args,
             storage,
             config=args.config,
             loader=loader,
             no_new=args.clear,
             do_files_download=True,
@@ -620,15 +630,17 @@
                     _print_pre_as_diff(patching.make_pre(diff_obj), diff_args.show_rules, diff_args.indent)
 
 
 def deploy(args: cli_args.DeployOptions) -> ExitCode:
     """ Сгенерировать конфиг для устройств и задеплоить его """
     ret: ExitCode = 0
     deployer = Deployer(args)
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         global live_configs  # pylint: disable=global-statement
         loader = ann_gen.Loader(storage, args)
         filterer = filtering.filterer_connector.get()
         fetcher = annet.deploy.fetcher_connector.get()
         deploy_driver = annet.deploy.driver_connector.get()
         live_configs = fetcher.fetch(devices=loader.devices, processes=args.parallel)
         pool = ann_gen.OldNewParallel(storage, args, loader, filterer)
```

### Comparing `annet-0.6/annet/argparse.py` & `annet-0.7/annet/argparse.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/cli.py` & `annet-0.7/annet/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,17 @@
                 yield (destname, result, False)
             else:
                 for entire_path, entire_data in sorted(result.items(), key=operator.itemgetter(0)):
                     if entire_data is None:
                         entire_data = ""
                     yield (output_driver.entire_config_dest_path(device, entire_path), entire_data, False)
 
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         ids = storage.resolve_object_ids_by_query(args.query)
         if not ids:
             get_logger().error("No devices found for %s", args.query)
         output_driver_connector.get().write_output(arg_out, _gen_items(storage), len(ids))
 
 
 @subcommand(cli_args.ShowGenOptions)
@@ -76,15 +78,17 @@
         get_logger().error("No devices found for %s", args.query)
     output_driver.write_output(args, out, total)
 
 
 @subcommand(cli_args.ShowDiffOptions)
 def diff(args: cli_args.ShowDiffOptions):
     """ Сгенерировать конфиг для устройств и показать дифф по рулбуку с текущим """
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         filterer = filtering.filterer_connector.get()
         loader = Loader(storage, args)
         output_driver_connector.get().write_output(
             args,
             gen_sort_diff(api.diff(args, loader, filterer), args),
             len(loader.device_ids)
         )
```

### Comparing `annet-0.6/annet/cli_args.py` & `annet-0.7/annet/cli_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -429,14 +429,19 @@
 
 class FileOutOptions(ArgGroup):
     dest = opt_dest
     expand_path = opt_expand_path
     no_label = opt_no_label
     no_color = opt_no_color
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self.dest:
+            self.no_color = True
+
 
 class DiffOptions(GenOptions, ComocutorOptions):
     clear = opt_clear
     config = opt_config
 
 
 class FileInputOptions(ArgGroup):
@@ -463,14 +468,19 @@
 
 
 class ShowDiffOptions(DiffOptions, FileOutOptions):
     indent = opt_indent
     show_rules = opt_show_rules
     no_collapse = opt_no_collapse
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self.dest:
+            self.no_collapse = True
+
 
 class ShowPatchOptions(PatchOptions, FileOutOptions):
     indent = opt_indent
     show_hosts_progress = opt_show_hosts_progress
 
 
 class FileDiffOptions(FileInputOptions, FileOutOptions, ParallelOptions):
```

### Comparing `annet-0.6/annet/configs/logging.yaml` & `annet-0.7/annet/configs/logging.yaml`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/connectors.py` & `annet-0.7/annet/connectors.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/deploy.py` & `annet-0.7/annet/deploy.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/diff.py` & `annet-0.7/annet/diff.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     diffs: Mapping[Device, Union[Diff, PCDiff]], args: ShowDiffOptions
 ) -> Generator[Tuple[str, Generator[str, None, None], bool], None, None]:
     """
     Возвращает осортированный дифф, совместимый с write_output
     :param diffs: Маппинг устройства в дифф
     :param args: Параметры коммандной строки
     """
-    # NOCDEV-2201 non-null --dest implies --no-collapse
-    if args.no_collapse or args.dest:
+    if args.no_collapse:
         devices_to_diff = {(dev,): diff for dev, diff in diffs.items()}
     else:
         non_pc_diffs = {dev: diff for dev, diff in diffs.items() if not isinstance(diff, PCDiff)}
         devices_to_diff = collapse_diffs(non_pc_diffs)
         devices_to_diff.update({(dev,): diff for dev, diff in diffs.items() if isinstance(diff, PCDiff)})
     for devices, diff_obj in devices_to_diff.items():
         if not diff_obj:
```

### Comparing `annet-0.6/annet/executor.py` & `annet-0.7/annet/executor.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/filtering.py` & `annet-0.7/annet/filtering.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/gen.py` & `annet-0.7/annet/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,17 @@
 
 @tracing.function
 def worker(device_id, args: ShowGenOptions, stdin, loader: "Loader", filterer: Filterer) -> Generator[Tuple[str, str, bool], None, None]:
     span = tracing_connector.get().get_current_span()
     if span:
         span.set_attribute("device.id", device_id)
 
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         for res in old_new(
             args,
             storage,
             config="/dev/null",
             loader=loader,
             filterer=filterer,
             add_implicit=False,
@@ -461,15 +463,17 @@
                            device.hw,
                            args.indent
                        ),
                        False)
 
 
 def old_new_worker(device_id, args: DeployOptions, config, stdin, loader: "Loader", filterer: Filterer):
-    with storage_connector.get().storage()(args) as storage:
+    connector = storage_connector.get()
+    storage_opts = connector.opts().from_cli_opts(args)
+    with connector.storage()(storage_opts) as storage:
         yield from old_new(
             args,
             storage,
             config=config,
             loader=loader,
             filterer=filterer,
             stdin=stdin,
```

### Comparing `annet-0.6/annet/generators/__init__.py` & `annet-0.7/annet/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,23 +534,15 @@
                             seen.add(module)
             module_paths = modules or module_paths.get("default")
     res_generators = []
     for module_path in module_paths:
         module = importlib.import_module(module_path)
         if hasattr(module, "get_generators"):
             generators: List[BaseGenerator] = module.get_generators(storage)
-            if device is None:
-                res_generators += generators
-            else:
-                logger = get_logger()
-                for gen in generators:
-                    if gen.supports_vendor(device.hw.vendor):
-                        res_generators.append(gen)
-                    else:
-                        logger.info("generator %s does not support device vendor %s, skipping", gen, device.hw.vendor)
+            res_generators += generators
     return res_generators
 
 
 def _get_ref_generators(module_paths: List[str], storage):
     if isinstance(module_paths, dict):
         module_paths = module_paths.get("default")
     res_generators = []
@@ -702,14 +694,20 @@
     def acl_safe(self, device):
         if hasattr(self, "acl_safe_" + device.hw.vendor):
             return getattr(self, "acl_safe_" + device.hw.vendor)(device)
 
     def run(self, device) -> Iterable[Union[str, tuple]]:
         if hasattr(self, "run_" + device.hw.vendor):
             return getattr(self, "run_" + device.hw.vendor)(device)
+        logger = get_logger()
+        logger.info(
+            "generator %s is not supported for vendor %s",
+            self,
+            device.hw.vendor,
+        )
         return iter(())
 
     def get_user_runner(self, device):
         if self.__class__.run is not PartialGenerator.run:
             return self.run
         elif hasattr(self, "run_" + device.hw.vendor):
             return getattr(self, "run_" + device.hw.vendor)
```

### Comparing `annet-0.6/annet/generators/common/initial.py` & `annet-0.7/annet/generators/common/initial.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/hardware.py` & `annet-0.7/annet/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/implicit.py` & `annet-0.7/annet/implicit.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/lib.py` & `annet-0.7/annet/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/output.py` & `annet-0.7/annet/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,17 @@
                 with open(dest, "w") as file:
                     writer.write(file)
 
     def format_fails(self, fail, args: Optional[QueryOptions] = None):
         ret = []
         fqdns = {}
         if args:
-            with storage_connector.get().storage()(args) as storage:
+            connector = storage_connector.get()
+            storage_opts = connector.opts().from_cli_opts(args)
+            with connector.storage()(storage_opts) as storage:
                 fqdns = storage.resolve_fdnds_by_query(args.query)
         for (assignment, exc) in fail.items():
             label = assignment
             if assignment in fqdns:
                 label = fqdns[assignment]
             elif isinstance(assignment, tuple):
                 label = assignment[0]
```

### Comparing `annet-0.6/annet/parallel.py` & `annet-0.7/annet/parallel.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/patching.py` & `annet-0.7/annet/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/reference.py` & `annet-0.7/annet/reference.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/__init__.py` & `annet-0.7/annet/rulebook/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/arista/iface.py` & `annet-0.7/annet/rulebook/arista/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/aruba/ap_env.py` & `annet-0.7/annet/rulebook/aruba/ap_env.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/cisco/iface.py` & `annet-0.7/annet/rulebook/cisco/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/cisco/misc.py` & `annet-0.7/annet/rulebook/cisco/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/cisco/vlandb.py` & `annet-0.7/annet/rulebook/cisco/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/common.py` & `annet-0.7/annet/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/deploying.py` & `annet-0.7/annet/rulebook/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/huawei/aaa.py` & `annet-0.7/annet/rulebook/huawei/aaa.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/huawei/bgp.py` & `annet-0.7/annet/rulebook/huawei/bgp.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/huawei/iface.py` & `annet-0.7/annet/rulebook/huawei/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/huawei/misc.py` & `annet-0.7/annet/rulebook/huawei/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/huawei/vlandb.py` & `annet-0.7/annet/rulebook/huawei/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/juniper/__init__.py` & `annet-0.7/annet/rulebook/juniper/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/nexus/iface.py` & `annet-0.7/annet/rulebook/nexus/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/patching.py` & `annet-0.7/annet/rulebook/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/arista.deploy` & `annet-0.7/annet/rulebook/texts/arista.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/arista.order` & `annet-0.7/annet/rulebook/texts/arista.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/arista.rul` & `annet-0.7/annet/rulebook/texts/arista.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/aruba.deploy` & `annet-0.7/annet/rulebook/texts/aruba.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/aruba.order` & `annet-0.7/annet/rulebook/texts/aruba.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/aruba.rul` & `annet-0.7/annet/rulebook/texts/aruba.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/cisco.deploy` & `annet-0.7/annet/rulebook/texts/cisco.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/cisco.order` & `annet-0.7/annet/rulebook/texts/cisco.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/cisco.rul` & `annet-0.7/annet/rulebook/texts/cisco.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/huawei.deploy` & `annet-0.7/annet/rulebook/texts/huawei.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/huawei.order` & `annet-0.7/annet/rulebook/texts/huawei.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/huawei.rul` & `annet-0.7/annet/rulebook/texts/huawei.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/juniper.rul` & `annet-0.7/annet/rulebook/texts/juniper.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/nexus.deploy` & `annet-0.7/annet/rulebook/texts/nexus.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/nexus.order` & `annet-0.7/annet/rulebook/texts/nexus.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/nexus.rul` & `annet-0.7/annet/rulebook/texts/nexus.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/nokia.rul` & `annet-0.7/annet/rulebook/texts/nokia.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/ribbon.deploy` & `annet-0.7/annet/rulebook/texts/ribbon.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/ribbon.rul` & `annet-0.7/annet/rulebook/texts/ribbon.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/routeros.order` & `annet-0.7/annet/rulebook/texts/routeros.order`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/rulebook/texts/routeros.rul` & `annet-0.7/annet/rulebook/texts/routeros.rul`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/storage.py` & `annet-0.7/annet/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/tabparser.py` & `annet-0.7/annet/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/text_term_format.py` & `annet-0.7/annet/text_term_format.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/tracing.py` & `annet-0.7/annet/tracing.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet/types.py` & `annet-0.7/annet/types.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/annet.egg-info/PKG-INFO` & `annet-0.7/annet.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.6
+Version: 0.7
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
@@ -17,7 +17,9 @@
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: contextlog>=1.1
 Requires-Dist: valkit>=0.1.4
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: yarl>=1.8.2
+Requires-Dist: adaptix==3.0.0b2
+Requires-Dist: dataclass-rest==0.4
```

### Comparing `annet-0.6/annet_generators/example/lldp.py` & `annet-0.7/annet_generators/example/lldp.py`

 * *Files identical despite different names*

### Comparing `annet-0.6/setup.py` & `annet-0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,28 +22,25 @@
         license="MIT",
         url="https://github.com/annetutil/annet",
         packages=setuptools.find_packages(include=[
             "annet",
             "annet.*",
             "annet_generators",
             "annet_generators.*",
-            "annet_nbexport",
-            "annet_nbexport.*"
         ]),
         package_data={
             "annet": ["configs/*"],
             "annet.rulebook": ["texts/*.rul", "texts/*.order", "texts/*.deploy"],
             "annet.annlib.netdev.devdb": ["data/*.json"],
         },
         entry_points={
           "console_scripts": [
               "annet = annet.annet:main",
-              "annet_nbexport = annet_nbexport.main:main",
           ],
           "annet.connectors": [
-            "storage = annet_nbexport:AnnetNbExportProvder",
+            "storage = annet.adapters.netbox.provider:NetboxProvider",
           ],
         },
         python_requires=">=3.8",
         install_requires=requirements(),
         include_package_data=True,
     )
```

